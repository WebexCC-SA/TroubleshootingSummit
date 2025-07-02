---
#icon: material/folder-open-outline
icon: material/bullseye-arrow
---
<script>
    // Function to initialize and handle form submission
    function setupAttendeeForm() {
        const form = document.getElementById('attendee-form');
        const displayAttendee = document.getElementById('display-attendee');
        const attendeeInput = document.getElementById('attendee');

        // Load stored Attendee ID on page load
        const storedAttendeeID = localStorage.getItem('attendeeID');
        if (storedAttendeeID) {
            attendeeInput.value = storedAttendeeID;
            displayAttendee.textContent = storedAttendeeID;
        }

        // Restrict input to only allow three digits
        attendeeInput.addEventListener('input', function() {
            this.value = this.value.replace(/\D/g, '').slice(0, 3);
        });

        // Handle form submission
        form.addEventListener('submit', function(event) {
            event.preventDefault();
            const attendeeIDInput = attendeeInput.value;

            if (attendeeIDInput && attendeeIDInput.length === 3) {
                // Store the Attendee ID in local storage
                localStorage.setItem('attendeeID', attendeeIDInput);

                // Update the displayed Attendee ID
                displayAttendee.textContent = attendeeIDInput;
            } else {
                alert('Please enter exactly 3 digits.');
            }
        });
    }

    // Wait for the DOM content to be fully loaded
    document.addEventListener('DOMContentLoaded', setupAttendeeForm);
    
    document.addEventListener('DOMContentLoaded', function() {
        const attendeeID = localStorage.getItem('attendeeID') || 'Not Set';
        const attendeePlaceholder = document.getElementById('attendee-id-placeholder');

        if (attendeePlaceholder) {
            attendeePlaceholder.textContent = attendeeID;
        }
    });
</script>

<style>
    /* Style for the button */
    button {
        background-color: black;
        color: white;
        border: none;
        padding: 10px 20px;
        cursor: pointer;
    }

    /* Style for the input element */
    input[type="text"] {
        border: 2px solid black;
        padding: 5px;
    }
</style>

<!-- Markdown content with embedded HTML -->
<div>
    <h2>Please select Attendee ID as any 3-digit number.</h2> 
    <h3>All configuration entries in the lab guide will be renamed to include your Attendee ID.</h3>
    <form id="attendee-form">
        <label for="attendee">Attendee ID:</label>
        <input type="text" id="attendee" name="attendee" placeholder="Enter 3 digits" required>
        <button type="submit">Save</button>
    </form>

    <br>

    <p>Your stored Attendee ID is: <b><span id="display-attendee">No ID stored</span></b></p>
</div>

# Overview

## Use Case 

## Webex AI Agent Design for Flower Shop

Designing a **Webex AI Agent** for a flower shop to assist customers via **voice and digital channels**.

### AI Agent Capabilities

- **Recommending flowers** based on customer preferences or occasions  
- **Collecting order details** for both **standard and custom bouquets**  
- **Calculating total price** in real time  
- **Gathering delivery information**, including **address** and **delivery date**  
- **order confirmations via SMS**  
- **Providing order status updates** upon request  
- **Sharing store hours** and relevant **business information**  
- **Transferring to a human agent** when needed for complex inquiries  

### Human Agent Support

- **Human agents** are equipped with **AI-powered tools** to ensure:
  - **Fast issue resolution**  
  - **Personalized service**  
  - **Exceptional customer experience** across all interactions


## Disclaimer
The lab design and configuration examples provided are for educational purposes. For production design queries, please consult your Cisco representative or an authorized Cisco partner.
Let’s get started and discover how **Webex Contact Center Flow Designer** takes customer experiences from good to great!


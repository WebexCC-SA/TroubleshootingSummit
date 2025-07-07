---
#icon: material/folder-open-outline
icon: material/medal
---



# Mission 1: Create AI Autonomous Agent.


## Mission overview
Your mission is to:

Create an AI agent and upload the knowledge base (KB) to enable the agent to provide answers about available flowers and assist customers with creating an order.

---

## Build

### Task 1. Creating new AI Agent with Knowladge Base.

1. <span style="color: red;">[IMPORTANT]</span> Download .xlsx the file [Flowrs_Catalog](https://docs.google.com/spreadsheets/d/1QjbL58okbEfl-ODgyv_ohIIPUiPBP34n/edit?usp=sharing&ouid=100862210011127627593&rtpof=true&sd=true){:target="_blank"}.
    ![Profiles](../graphics/Lab1_AI_Agent/2.74.png)
    
    > 
    > **Flower_Catalog.xlsx** - file contains information on the available single flowers and bouquets, including the price of the flowers or bouquets and occasions that suit the flowers.
    >

2. Open up and review the file. 
    ![Profiles](../graphics/Lab1_AI_Agent/2.56.png)


3. Go to Contact Center from the left side navigation panel, and under Quick Links, click on **Webex AI Agent**

    ![Profiles](../graphics/Lab1/L1M6_OpenWebexAI.gif)  

4. In AI Agent Builder navigate to **Knowledge** from left hand side menu panel. 

5. Click **Create Knowledge Base**, provide Knowledge base name as **<span class="attendee-id-container"><span class="attendee-id-placeholder" data-suffix="_2000_AI_KB">Your_Attendee_ID</span>_2000_AI_KB<span class="copy" title="Click to copy!"></span></span>**, then click **Create**.

    ![Profiles](../graphics/Lab1_AI_Agent/2.1.gif)

6. Click **Add File** or drag and drop file **Flower_Catalog.xlsx** you downloaded from external drive on **Step 1**. Then click **Process Files**. Wait until the file is processed. It could take 1-2 mins.

    ![Profiles](../graphics/Lab1_AI_Agent/2.2.gif)

    Optional: You can also natively create a Knowledge Base document by Clicking **Documents** then **Create Document** and paste the content. **Save** it. 
    ![Profiles](../graphics/Lab1_AI_Agent/2.75KBDocument.gif)
    
7. Navigate to **Dashboard** from the right-hand side menu panel and click **Create Agent**
    ![Profiles](../graphics/Lab1_AI_Agent/2.58.gif)
8. Select **Start from Scratch** and click **Next**
9. On **Create an AI agent** page select the following select the type of agent: **Autonomous**

10. New section **Add the essential details** will appear. Provide the following information, then click **Create**:

    > Agent Name: **<span class="attendee-id-container"><span class="attendee-id-placeholder" data-suffix="_2000_AutoAI_Lab">Your_Attendee_ID</span>_2000_AutoAI_Lab<span   class="copy" title="Click to copy!"></span></span>**
    >
    > System ID is created automatically
    >
    > AI engine: **Webex AI Pro 1.0**
    > 
    > Agent's goal: ***This is Flower Shop. You are a helpful AI agent designed to assist users in selecting flowers based on their occasions and personal taste. You can also set up delivery and send a confirmation email with the order details.***<span class="copy-static" title="Click to copy!" data-copy-text="This is Flower Shop. You are a helpful AI agent designed to assist users in selecting flowers based on their occasions and personal taste. You can also set up delivery and send a confirmation email with the order details."><span class="copy"></span></span>


    ![Profiles](../graphics/Lab1_AI_Agent/2.3.gif)

11. Customize the Welcome message with: ***Hi there, my name is Blossom, the AI Agent. How can I assist you?***<span class="copy-static" title="Click to copy!" data-copy-text="Hi there, my name is Blossom, the AI Agent. How can I assist you?"><span class="copy"></span></span>


    ![Profiles](../graphics/Lab1_AI_Agent/2.16.png)


12. In the instructions add additional specific guidlines that you would like the AI Agent to follow. Just **copy the text below and paste it to the Instractions section**: <br>


    >Always first check what is the event for the flowers so you can provide the best option. 

    >Always print the total at the end of the conversation at any stage.

    >Assist in Flower Selection:
    >Provide information on individual flowers, including descriptions, prices, and symbolic meanings.
    >Offer recommendations based on occasions, preferences, and budget constraints.

    >Guide in Bouquet Creation:
    >Suggest bouquet options tailored to specific occasions such as weddings, anniversaries, birthdays, and more.
    >Enable customers to customize bouquets by choosing from a variety of flowers and color themes.

    >Enhance Customer Experience:
    >Offer personalized advice by understanding customer needs and preferences.
    >Ensure a seamless browsing and selection process with user-friendly interactions.

    >Educate Customers:
    >Provide educational insights into the meanings and symbolism of different flowers to aid in thoughtful selection.
    >Share care tips for maintaining flower freshness and longevity.

    >Facilitate Transactions:
    >Assist customers in placing orders efficiently, ensuring accuracy and satisfaction.
    >Provide support for payment processing and order confirmations.

    >Ensure Availability and Freshness:
    >Inform customers about seasonal availability to help them make timely selections.
    >Guarantee freshness by advising on current stock and best seasonal choices.

    >Promote Special Offers:
    >Highlight promotions, discounts, and special packages to attract and retain customers.
    >Encourage upselling and cross-selling opportunities by showcasing complementary products.

    >Ask if the customer needs the deliver. Collect the address and add price of the delivery to the Total. 

    >Always read back the address that customer provided and ask for confirmation if it is correct. If it is not correct, ask to provide the address again.

    >Always ask if the customer needs to confirmation email before completing the order.</br></br>
    ![Profiles](../graphics/Lab1_AI_Agent/2.4.gif)




13.  Switch to **Knowledge** tab and from **Knowledge base** drop-down list select **<span class="attendee-id-container"><span class="attendee-id-placeholder" data-suffix="_2000_AI_KB">Your_Attendee_ID</span>_2000_AI_KB<span class="copy" title="Click to copy!"></span></span>**. Click **Save Changes**.
    ![Profiles](../graphics/Lab1_AI_Agent/2.5.gif)

14.  Click **Publish**. Provide any version name in popped up window (ex. "1.0").<br>
    ![Profiles](../graphics/Lab1_AI_Agent/2.6.gif)


### Task 2. Test your AI Agent

1. Click on **Preview** and testing the AI Agent to understnad how it behaives using Chat channel. You can start the conversation with: **"I need flower for my friend"**<span class="copy-static" title="Click to copy!" data-copy-text="I need flower for my friend"><span class="copy"></span></span> and try to customize you order.<br> Note: <i>Please be aware that you still haven't configured the order creation and email confirmation functionalities. For now, just test the flower selection and price calculation.</i>
![Profiles](../graphics/Lab1_AI_Agent/2.59.gif)

2. Click on **Preview** and testing the AI Agent to understnad how it behaives using Voice channel. You can start the conversation with: **"I need flower for my friend"**<span class="copy-static" title="Click to copy!" data-copy-text="I need flower for my friend"><span class="copy"></span></span> and try to customize you order. 


![Profiles](../graphics/Lab1_AI_Agent/2.60.gif)

<p style="text-align:center"><strong>Congratulations, you have officially completed this mission! 🎉🎉 </strong></p>
---
#icon: material/folder-open-outline
icon: material/bullseye-arrow
---

## Learning Objectives
1. Ensure that you have **LTRCCT-2000_LAB_Credential** file on your desktop with instructions and credentials to access your lab. If you do not, please ask your lab proctor now.
2. Understand your configuration instructions


### Know before you start

1. We will be using a shared lab tenant for simulations, meaning all attendees will work within the same Webex Contact Center environment. To avoid conflicts, ensure that any entities you configure are tagged with the Attendee ID assigned to you.
    
    <details><summary>WxCC Schema</summary>![Profiles](../graphics/overview/WxCC_Schema.png)</details>

2. The majority of the configuration in Control Hub is already set up, allowing you to focus primarily on configuration Webex AI Virtual Agent and other AI features. Of course, there may still be some elements to adjust, but these should be minimal, letting you concentrate on building and refining the flow logic rather than spending time on initial setup.
3. The Human Agent have been configured for you. You will be performing the rest of the configurations for AI Agent and integartion with channels.
4. All your configurations should contain your attendee ID so the lab users don't step over each other's configurations.
5. Each of you has been provided with the phone number to dial (Entry point DN), 1 agent and 1 admin.
6. Please ask for help when you need it. You can do so by:
   * Dropping your question in the LAB Space **LTRCCT-2000: In Room Lab Support** from Webex App in your Lab PC. 
   * Raising your hand and calling the proctor.
       ![Profiles](../graphics/Lab1_AI_Agent/GS8.gif)
---

### Predefined configuration

> Entry Point/Channels:  **<span class="attendee-id-container"><span class="attendee-id-placeholder" data-suffix="_2000_Channel">Your_Attendee_ID</span>_2000_Channel<span class="copy"></span></span>**

> Queue:  **<span class="attendee-id-container"><span class="attendee-id-placeholder" data-suffix="_2000_Voice_Queue">Your_Attendee_ID</span>_2000_Voice_Queue<span class="copy"></span></span>**

> Team:  **<span class="attendee-id-container"><span class="attendee-id-placeholder" data-suffix="_2000_Team">Your_Attendee_ID</span>_2000_Team<span class="copy"></span></span>**

> Admin:   **<span class="attendee-id-container">wxcclabs+admin_ID<span class="attendee-id-placeholder" data-prefix="wxcclabs+admin_ID" data-suffix="@gmail.com">Your_Attendee_ID</span>@gmail.com<span class="copy"></span></span>**

> Webex App has been pre-installed on your Lab PC

> Assigned Inbound Channel Number: **Provided by Lab Instructor**

More pre-configured entities will be mentioned during the lab missions if they have any.

---

### Testing

#### Login to Webex Control. 

1. Open up Google Chrome Web browser and start login to [Control Hub](https://admin.webex.com){:target="_blank"}.
   ![Profiles](../graphics/Lab1_AI_Agent/GS1.png)

2. Login using your Admin user name and password. 
   ![Profiles](../graphics/Lab1_AI_Agent/GS2.gif)

#### Login to Agent Desktop

1. Click on **Contact Center** Service. 
   ![Profiles](../graphics/Lab1_AI_Agent/GS.3.png)

2. From **Quick Links** click on **Desktop**.
   ![Profiles](../graphics/Lab1_AI_Agent/GS4.png)

3. Allo notification for the Aget Desktop. Select login option as **Desktop**, select your Team and click on **Submit**.
   ![Profiles](../graphics/Lab1_AI_Agent/GS5.png)

4. Click Continue on the Emergency Serice Notification. 
   ![Profiles](../graphics/Lab1_AI_Agent/GS6.png)

5. Allow use of microphones.
   ![Profiles](../graphics/Lab1_AI_Agent/GS7.png)

#### Calling to Contact Center
You can make test calls from your mobile phone or by using Webex Calling phones. Please find the Webex App and log in with the admin credentials that were shared with you.
   ![Profiles](../graphics/Lab1_AI_Agent/GS8.gif)

Place test call to the test number  +15206603129 to confirm that you Webex Phone is configured to place calls

!!! Note
    International dialing is not allowed so you won't be able to dial your cell phones unless you have a US number.

---


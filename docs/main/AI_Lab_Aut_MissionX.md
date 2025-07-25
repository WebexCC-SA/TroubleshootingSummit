---
#icon: material/folder-open-outline
icon: material/medal
---


# Mission  Integrating the AI Agent with Flow for Voice Calls

## Mission overview
Your mission is to:

Integrate the AI Agent with the Voice Flow. 

### Task 1. Build WxCC voice flow with AI Agent.

1. In Control Hub navigate to **Flows**, click on **Manage Flows** dropdown list and select **Create Flows**. Select **Start Fresh**.
   ![Profiles](../graphics/Lab1_AI_Agent/2.47.gif)

2.  Name the new flow **<span class="attendee-id-container">AutonomousAI_Flow_2000_<span class="attendee-id-placeholder" data-prefix="AutonomousAI_Flow_2000_">Your_Attendee_ID</span><span class="copy" title="Click to copy!"></span></span>** and click **Create Flow**.
   ![Profiles](../graphics/Lab1_AI_Agent/2.48.png)

3. Make sure the **Edit** mode at the top is set to **ON**. Then, drag and drop the **Virtual Agent V2** and **DisconnectContact** activities from the left panel onto the canvas.

    !!! Note
        Please make sure to use **VirtualAgentV2** activity and <span style="color: red;">**NOT**</span> **VirtualAgent** also present on the Activity Library for Backward Compatability.

    > Connect the **New Phone Contact** output node edge to this **VirtualAgentV2** node
    >
    > Connect the Handled outputs to **DisconnectContact** 
    >
    > Connect the Errored outputs to **DisconnectContact** 
    >
    > Click on **VirtulaAgentV2** block and select **Static Contact Center AI Config**
    >
    > Select Contact Center AI Config as **Webex AI Agent (Autonomous)**
    >
    > Virtual Agent: **<span class="attendee-id-container"><span class="attendee-id-placeholder" data-suffix="_2000_AutoAI_Lab">Your_Attendee_ID</span>_2000_AutoAI_Lab<span   class="copy" title="Click to copy!"></span></span>**
    ![Profiles](../graphics/Lab1_AI_Agent/2.49.gif)  

4. Drag and drop **Queue Contact** and **Play Music** nodes. Configure them as the following:

    - **Queue Contact** activity onto the Flow from the left side panel

      >
      > Connect the **Escalated** path from the **Virtual Agent V2** activity to the **Queue Contact** activity.
      >
      > Connect the **Queue Contact** activity to the **Play Music** activity
      >
      > Connect the **Failure** path from the **Queue Contact** activity to the **Disconnect Contact** activity.
      > 
      > Click on **Queue Contact** node and select **Static Queue**.
      > 
      > Queue name: **<span class="attendee-id-container"><span class="attendee-id-placeholder" data-suffix="_2000_Voice_Queue">Your_Attendee_ID</span>_2000_Voice_Queue<span class="copy" title="Click to copy!"></span></span>**
      > 

    - **Play Music**

      >
      > Create a loop by connecting the Play Music activity back to itself - to create a music loop, following the diagram provided.
      >
      > Connect the **Undefined Error** path from the **Play Music** activity to the **Disconnect Contact** activity.
      > 
      > Music File: **defaultmusic_on_hold.wav**
      >
    ![Profiles](../graphics/Lab1_AI_Agent/2.50.gif)  

5. **Validate** and **Publish** Flow. In popped up window click on dropdown menu to select **Latest** label, then click **Publish**.
    ![Profiles](../graphics/Lab1_AI_Agent/2.51.gif)  

6. Assign the Flow to your **Channel (Entry Point)** - Do this by first going to **Channel** > Search for your channel **<span class="attendee-id-placeholder">Your_Attendee_ID</span>_2000_Channel**.
7. Click on **<span class="attendee-id-placeholder">Your_Attendee_ID</span>_2000_Channel**
    ![Profiles](../graphics/Lab1_AI_Agent/2.52.png)  
8. In **Entry Point** Settings section change the following:

    > Routing Flow: **<span class="attendee-id-container">AutonomousAI_Flow_2000_<span class="attendee-id-placeholder" data-prefix="AutonomousAI_Flow_2000_">Your_Attendee_ID</span><span class="copy" title="Click to copy!"></span></span>**

    > Version Label: **Latest**

    > Music on Hold: **defaultmusic_on_hold.wav**

    ![Profiles](../graphics/Lab1_AI_Agent/2.53.gif)

9. Dial Support Number assigned to your **<span class="attendee-id-placeholder">Your_Attendee_ID</span>_2000_Channel** to test the Autonomous AI Agent over a voice call.


### Task 2. Test Agent Handoff Configurations.

1. Login to [Agent Desktop](https://desktop.wxcc-us1.cisco.com){:target="_blank"}.
2. Select **Desktop** endpoint option and choose the team. **<span class="attendee-id-container"><span class="attendee-id-placeholder" data-suffix="__2000_Team">Your_Attendee_ID</span>_2000_Team<span class="copy" title="Click to copy!"></span></span>**. Click **Submit**. Allow browser to access Microphone by clicking **Allow** on every visit.
3. Make your agent ***Available*** and you're ready to receive a call.

    ![profiles](../graphics/Lab1/5-Agent_Login.gif)

4. Dial the support number assigned to your **<span class="attendee-id-placeholder">Your_Attendee_ID</span>_2000_Channel** channel, and during the conversation with the AI agent, ask to talk to a representetive or live agent. 

5. By default, the **Conversation Transcripts** setting is enabled in VirtualAgentV2 block.
    ![Profiles](../graphics/Lab1_AI_Agent/2.54.png)

6. With this setting enabled, the live agent can see the conversation details between the caller and the AI agent. Please check if you can view the IVR transcripts during your test calls with Agent Handoff. 
    ![Profiles](../graphics/Lab1_AI_Agent/2.55.png)


<p style="text-align:center"><strong>Congratulations, you have officially completed the Autonomous AI Agent lab! 🎉🎉 </strong></p>

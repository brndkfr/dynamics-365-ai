---
title: "Use Microsoft Flow with your virtual agent"
description: "Learn how to use Microsoft Flow in your virtual agent."
keywords: ""
ms\.date: 1/14/2019
ms.service:
  - "dynamics-365-ai"
ms.topic: article
ms.assetid: 
author: stevesaunders1952
ms.author: stevesaunders1952
manager: shellyha
---

# Use Microsoft Flow with your virtual agent

You can use flows created using Microsoft Flow in your virtual agent as long as the flows and virtual agent share the same CDS environment. First, create Microsoft PowerApps and Microsoft Flow environments, and then create your flow. You can then create a virtual agent that invokes your flow.

## To create a new Microsoft PowerApps environment

1. Enter [https://tip1.admin.powerapps.com/environments](https://tip1.admin.powerapps.com/environments) in your browser to open the PowerApps Admin center.

2. Click **New Environment** to open the New environment screen.

    Specify a unique name for the environment, *Preview (United States) (default)* as the region, *Trial* as the environment type. Select the **Join Preview** checkbox, and click **Create Enviroment**.

   > [!div class="mx-imgBorder"]
   > ![Create environment](media/how-to-flow-1-1.PNG)

    PowerApps creates the environment and displays a prompt asking if you want to create a database.

3. Click **Create database** to display the Create a database for this environment screen.

   > [!div class="mx-imgBorder"]
   > ![Create database screen](media/how-to-flow-1-2.PNG)

4. Select your currency type and language, and then click **Create Database**.

   > [!div class="mx-imgBorder"]
   > ![Create database](media/how-to-flow-1-3.PNG)

    **Note:**  Creating a database and environment can take several hours.

## To create a Microsoft Flow environment

1. If you do not already have a Microsoft Flow environment, log in to the Flow admin portal to create one. Enter [https://us.tip1.flow.microsoft.com/en-us/]( https://us.tip1.flow.microsoft.com/en-us/) in your browser to open the Flow portal.

2. Click on your User icon in the upper right corner of the screen, then select the PowerApps environment you created from the list.

   > [!div class="mx-imgBorder"]
   > ![Select environment](media/how-to-flow-1-4.PNG)

3. Verify that the PowerApps environment database was created correctly. Click **Solutions** in the navigation pane to display the Solutions page, and then verify that the Solutions list includes *Common Data Services Default Solution*.

   > [!div class="mx-imgBorder"]
   > ![Verify database](media/how-to-flow-1-5.PNG)

    **Note:**  Since creating a new environment can take some time, the new solution may not immediately appear in the list. Log out and check again in 30-60 minutes.

Once you have created your environment, return to the Flow portal and switch to the newly created environment to create your flow.

## To create a flow

1. Click on **Common Data Services Default Solution** to open the solution.

2. On the Common Data Services Default Solution page, click **+New**, and then select **Flow** from the list.

   > [!div class="mx-imgBorder"]
   > ![New flow](media/how-to-flow-1-6.PNG)

    You can create a variety of flows for your solution. For example, you could create a simple flow that takes an email address as input parameter, sends an email message to that address, and returns a message that the email was successfully sent to a virtual agent as output.

3. Select a trigger for your flow. A Virtual Agent Designer virtual agent can only invoke flows that have HTTP request interfaces. Enter *HTTP* in the Search box, and select **When HTTP request is received** to create a flow with an HTTP request trigger.

   > [!div class="mx-imgBorder"]
   > ![Select trigger](media/how-to-flow-8.PNG)

4. Add the following JSON code in the **Request Body JSON Schema** box. The code specifies that the flow expects an email address to receive one string input parameter.

    ``` JSON
        {  
        "type": "object",  
            "properties": {  
                "to": {  
                    "type": "string"  
                }  
            }  
        }
    ```

   > [!div class="mx-imgBorder"]
   > ![Add JSON code](media/how-to-flow-9.PNG)

5. Specify that an email message should be sent to the email address specified in the input. Enter *Outlook* in the Search box and select **Send an email** to create a connection to Microsoft Outlook using your Outlook credentials to send the message.

   > [!div class="mx-imgBorder"]
   > ![Send email](media/how-to-flow-10.PNG)

6. Specify an email address for the message, and fill in the Subject and Body fields.

    You can specify a Flow input variable (“to”) as the recipient address using Dynamic Content. Click **See more** to see all dynamic variables.

   > [!div class="mx-imgBorder"]
   > ![Create message](media/how-to-flow-11.PNG)

7. If you specify the “to” variable as the recipient address, click **New step** to return a message to the flow.

   > [!div class="mx-imgBorder"]
   > ![Return message](media/how-to-flow-12.PNG)

8. Use an HTTP Response to return a variable to the virtual agent. Enter *Response* in the search box and select the **Response** action in the search results list.

   > [!div class="mx-imgBorder"]
   > ![HTTP response](media/how-to-flow-12-1.PNG)

9. Specify the following information for the Response action, and then save your flow.

   > [!div class="mx-imgBorder"]
   > ![Response action](media/how-to-flow-13.PNG)

## To create a virtual agent that invokes a flow

1. Log in to the AI for Customer Service Virtual Agent portal [https://bots.ppe.customercareintelligence.net/#/](https://bots.ppe.customercareintelligence.net/#/) and create a new virtual agent in the same environment as your flow. To create a new virtual agent, click the **+** button on the Virtual Agent Designer title bar.

   > [!div class="mx-imgBorder"]
   > ![Create virtual agent](media/how-to-flow-14.PNG)

    For more information about creating a virtual agent, see [Creating a virtual agent](getting-started-create-bot.md).

2. On the **Create a new bot** screen, specify a template, a unique name for your virtual agent, and the environment where your flow was created.

   > [!div class="mx-imgBorder"]
   > ![Specify environment](media/how-to-flow-15.PNG)

    Then click **Create**.

3. Once you have created your virtual agent, create a topic that uses the flow. Click **Topics** in the navigation pane to open the Topics page, and then click **New topic**.

   > [!div class="mx-imgBorder"]
   > ![New topic](media/create-topic-2.png)

    For more information about creating a topic, see [Creating topics for your virtual agent](getting-started-create-topics.md).

4. Specify trigger phrases for the topic. For example, for a Daily Deals topic you could specify the following trigger phrases:

    - daily deals
    - deal of the day
    - current deals
    - today’s deals
    - current offers
    - today’s specials
    - current specials
    - special offers
    - today’s coupons
    - current coupons
    - today’s offers

    Then click **Save topic** save the topic.

   > [!div class="mx-imgBorder"]
   > ![Save topic](media/how-to-flow-16.png)

5. Once you have created the topic, you can create a conversation path that uses your flow. Click **Edit** to open the conversation editor, enter a virtual agent response in the **Bot says** box, and then click **User says** to display the **User response** node.

   > [!div class="mx-imgBorder"]
   > ![Create conversation](media/how-to-flow-17.png)

    In the user response, click **Add Variable** to add a variable to save a customer's email address. In the Properties pane, click **Create variable** to display the **Create new variable** screen.

   > [!div class="mx-imgBorder"]
   > ![Create variable](media/how-to-flow-18.png)

    For more information on creating variables, see [Work with variables](how0to-variables.md).

6. Specify a variable name and type. For example, you could create a text variable named *User_Email*.  Click **Done** to save the variable.

   > [!div class="mx-imgBorder"]
   > ![Save variable](media/how-to-flow-19.png)

    The Virtual Agent Designer creates an **Expression** node that can be deleted if you do not want to do any validation.

   > [!div class="mx-imgBorder"]
   > ![Delete expression](media/how-to-flow-20.png)

7. Add another **Bot says** node with text confirming that the email will be sent. You can choose to display the email address that the User has specified by clicking on the rightmost icon and selecting the variable you created.

   > [!div class="mx-imgBorder"]
   > ![Select variable](media/how-to-flow-21.png)

8. To send an email message to the address specified by the customer, select **Action** to display the list of available actions, and then select the flow action you created.

   > [!div class="mx-imgBorder"]
   > ![Select variable](media/how-to-flow-22.png)

    **Note:**  The Flows and virtual agent must be created in the same envioenment. Otherwise, the flow action does not appear in the list of available actions.

    The Virtual Agent Designer creates an **Action** node indicating that the action has one required input and one output. Select the variable you created from the list to pass it as input.

   > [!div class="mx-imgBorder"]
   > ![Create action](media/how-to-flow-23.png)

9. Add another **Bot says** node to display the message from the flow to the customer, end your conversation with at survey, and then click **Save** to save the topic.

   > [!div class="mx-imgBorder"]
   > ![Display flow message](media/how-to-flow-24.png)

## To test the flow

1. In the Test Bot, click **Start over with latest conversation**. Then specify a trigger phrase for the topic that contains the flow.

2. Enter your email address at the prompt.

   > [!div class="mx-imgBorder"]
   > ![Test flow](media/how-to-flow-25.png)

    After you specify the email address, the flow sends an email message and returns the message to the virtual agent. The Virtual Agent Designer stores the message in the *(x) message* variable and displays it to the customer.

   > [!div class="mx-imgBorder"]
   > ![Complete test](media/how-to-flow-26.png)
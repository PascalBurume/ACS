<!-- markdownlint-disable MD041 -->

In this excercice, you will incorporate the **ACS email**composite into a **Power Platform** application, which will allow you to send email requests from a personalized app to **Power Apps** using **Power Automate**.

**Power Platform** is a suite of apps, services, connectors, and data platform that provides a rapid application development environment to build custom apps for your business needs. 

You can use **Power Apps** to create apps that run on mobile devices, tablets, and the web without writing any code. You can also use **Power Platform**to automate workflows and processes using **Microsoft Power Automate**, analyze data for insights using **Microsoft Power BI**, rapidly design, configure, and publish modern websites using **Microsoft Power Pages**, and build intelligent bots with a no-code interface using **Microsoft Power Virtual Agents**.

:::image type="content" source="../media/16.Power-Platform.png" alt-text="Power Platform":::

- If you do not have access to Power Platforme access, you can setup your [Microsoft 365 developer tenant.](https://developer.microsoft.com/microsoft-365/dev-program)

Learn the business value and product capabilities of Microsoft Power Platform. Create simple Power Apps, connect data with Microsoft Dataverse, build a Power BI Dashboard, automate a process with Power Automate, and build a chatbot with Power Virtual Agents in  [Power Platform fundamental](https://learn.microsoft.com/en-us/certifications/power-platform-fundamentals/)

### Create a flow using Microsoft Power Automate

 **Power Automate** is a service that allows you to create automated workflows and processes using low-code, drag-and-drop tools. You can use Power Automate to connect to hundreds of data sources, automate tasks, enhance your workflows with AI, and run your flows on desktop, web, and mobile devices.

:::image type="content" source="../media/7.Power-Automate-Home-page.png" alt-text="Power Automate":::

1. In **Create**, we'll create an instant that can be triggered manually through an action from a Power Apps button.

:::image type="content" source="../media/8.Creating-an-instant-flow-with-Power-Apps-button.png" alt-text="Creation of a cloud flow":::

2. Next, we can set up a **Power Apps button** flow that utilizes **Azure Communication Services to send emails**. This will enable you to send emails directly from your application without the need for a separate email client. 

3. We'll walk you through the necessary steps to create this flow, which will leverage the email functionality of **Azure Communication Services**.

::image type="content" source="../media/9.creating-flow.png" alt-text="Creation of a cloud flow":::

### Create the app using Microsoft Power Apps

1. To streamline the process of managing partnerships between companies, we will use **Power Apps** to create a custom app. This will save time and effort by providing a central platform for all necessary information and tasks. Additionally, using **Copilot**, an AI-powered coding assistant, will further expedite the development process by suggesting code and providing helpful insights. 


:::image type="content" source="../media/10.Power-Apps-Home-page.png" alt-text="Creation of a cloud flow":::

2. After typing our instructions and the model of our application we can now **create app**.

:::image type="content" source="../media/11.Power-Apps-create-with-copilote.png" alt-text="Power Apps create with copilote":::

3. To enable users to send emails to a designated recipient, we can incorporate a **Send Mail button** into the app's functionality. To do this, we can create a button function that includes the following code:

    `PowerAppsMail.Run(TextInput2.Text, TextInput2_1.Text, TextInput2_2.Text)`

This code will allow users to input the recipient's **email address** in **TextInput2**, the email **subject** in **TextInput2_1**, and the **email message** in **TextInput2_2**. 
In addition, we can include a reset function to clear the input fields after the email is sent. This can be done using the Reset function for each input field: 

4. In addition, we can include a reset function to clear the input fields after the email is sent. This can be done using the **Reset function** for each input field:
   
   ` Reset(TextInput2); Reset(TextInput2_1); Reset(TextInput2_2)`

 By incorporating these functions, users can easily send emails from within the app and keep all communication centralized.

:::image type="content" source="../media/12.Overview-of-the-app-with-the bouton-sending-mail.png" alt-text="Overview of the app with the bouton sending mail":::

5. Once all configurations have been completed, the app is ready to be launched and used.

:::image type="content" source="../media/13.sending-mail.png" alt-text="sending mail":::

6. When an email is sent using the app, the recipient should receive the email in their inbox. They can then open and read the email as they normally would through their email service provider.

:::image type="content" source="../media/14.mail-receive.png" alt-text="mail-receive":::

7. Once you've completed all the necessary steps, you can **Publish** your application with the integrated **Azure Communication Services** features. This will enable you to provide your users with seamless communication and email capabilities directly from within your application. 

9. To ublish an app, save the app if you’ve made any changes, and then select Publish from the File menu in **Power Apps Studio**. In the **Publish dialog**, you can select settings such as the name of the app, an icon for the app, and a description.

:::image type="content" source="../media/15.Publish-the-app.png" alt-text="Publish the app":::

10. To install an app in the environment view, sign in to the **Power Platform admin center**, select **Environments**, and then select an environment. Under **Resources**, select **Dynamics 365 apps**, and then select Install app. Agree to the terms of service, and then select **Install**.

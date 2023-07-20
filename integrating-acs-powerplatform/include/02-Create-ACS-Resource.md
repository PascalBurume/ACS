<!-- markdownlint-disable MD041 -->

In this exercise you'll create an **Azure Communication Services (ACS)** resource in the
**Azure Portal**.

To get started, perform the following tasks:

1. Visit the [Azure Portal](https://portal.azure.com) in your browser and sign in.

1. Type *communication services* in the **search bar** at the top of the page and select **Communication Services** from the options that appear.

    :::image type="content" source="../media/1.email-communication-create.png" alt-text="ACS in the Azure Portal":::

1. Select **Create** in the toolbar.

1. Perform the following tasks:
    - Select your Azure subscription.
    - Select the resource group to use (create a new one if one doesn't exist).
    - Enter an ACS resource name. It must be a unique value.
    - Select a data location.

1. Select **Review + Create** followed by **Create**.

 :::image type="content" source="../media/2.email-communication-create-review.png" alt-text="email communication creation ":::

  - Wait for the validation to pass. **Click Create**.
  - Wait for the Deployment to complete. Click **Go to Resource** will land on Email
    Communication Service Overview Page.

:::image type="content" source="../media/3.email-communication-overview.png" alt-text="email communication overview ":::

  > [!TIP]
  > if you need to setup a custom domain or you are using an existing domain register like GoDaddy, you can follow this link : [How to add custom verified domains to Email Communication Service - An Azure Communication Services quick start guide | Microsoft Learn](https://learn.microsoft.com/en-us/azure/communication-services/quickstarts/email/add-custom-verified-domains)

1. Go to **Provision domain** to connect to your domain and adding email addresses.

:::image type="content" source="../media/4.Adding-domain-email-communication.png" alt-text="Adding domain email communication ":::


1. You need to verifier the status of your domain, if it **green** it means your domain is accessible,  in **configure** status it means we can’t verify your domain.

1. Go to the **green status**, to add email addresses 

:::image type="content" source="../media/5.Adding-mail-from.png" alt-text="Adding-mail-from ":::

1. Adding **mail from addresses**

:::image type="content" source="../media/6.Adding-mailfrom-creation.png" alt-text="Adding mailfrom creation ":::










# Module 03 - TEST SENSITIVITY LABEL IN SHAREPOINT

[< Previous Module](../modules.md/module02.md) - **[Home](../modules.md/module00.md)** - [Next Module >](../modules.md/module03.md)

## :loudspeaker: Introduction

After creating a Sensitivity Label and publishing a Label Policy, it's time to test the new label. It can take between 1 and 24 hours for the Sensitivity Label to appear throughout the services.  There are many external dependencies that each have their own timing cycles, so it's a good idea to wait this 24-hour time period before you spend time troubleshooting labels and label policies for recent changes.

However, there are some scenarios where label and label policy changes can take effect much faster or be longer than 24 hours. For example, for new and deleted sensitivity labels for Word, Excel, and PowerPoint on the web, you might see updates replicate within the hour. But for configurations that depend on populating a new group and group membership changes, or network replication latency and bandwidth restrictions, these changes might take 24-48 hours.

## :dart: Objectives

* Test Sensitivity Labels in SharePoint Online

## Create documents in a SPO doc library to test

1. Navigate to the engineering site collection in SharePoint Online in your tenant. This is typically https://domain.sharepoint.com/sites/Engineering where domain is the name of your lab tenant.

    ![image1](../images/module01/spo1.png)

2. Click **Documents**, **New**, and **Word Document** to create a new Word document in this doc library.

    ![image2](../images/module01/spo2.png)

3. In the new Word document, type =rand(5) to populate the document with sample text. Below the final paragraph enter a social security number, for example:  SSN 472-35-8912

4. Review the selected labels and to make any changes, select **Edit**. Otherwise, select **Next**.

5. Follow the prompts to configure the policy settings.
    The policy settings that you see match the scope of the labels that you selected. For example, if you selected labels that have just the **Items** scope, you don't see the policy settings **Apply this label by default to groups and sites** and **Require users to apply a label to their groups and sites**.

    For labels configured for **Microsoft Purview Data Map assets (preview)**: These labels don't have any associated policy settings.

    **For this lab we will accept the default values and not make any selections until we get to the Name your policy screen.**

6. On the Name your policy screen, give your new policy a name like HR Data policy and click next.  Completing the **Create policy** configuration automatically publishes the label policy. To make changes to a published policy, simply edit it. There's no specific publish or republish action for you to select.

## When to expect new labels and changes to take effect

For labels and label policy settings, allow 24 hours for the changes to propagate through the services. There are many external dependencies that each have their own timing cycles, so it's a good idea to wait this 24-hour time period before you spend time troubleshooting labels and label policies for recent changes.

However, there are some scenarios where label and label policy changes can take effect much faster or be longer than 24 hours. For example, for new and deleted sensitivity labels for Word, Excel, and PowerPoint on the web, you might see updates replicate within the hour. But for configurations that depend on populating a new group and group membership changes, or network replication latency and bandwidth restrictions, these changes might take 24-48 hours.

## :tada: CONGRATULATIONS!
You've just published your first Label Policy!  In the next module, you will test this sensitivity label using a SharePoint document library and Word online.


MODULE_SUMMARY

[Continue >](../modules/module00.md)

# Module 02 - PUBLISH SENSITIVITY LABELS

[< Previous Module](../modules/module00.md) - **[Home](../README.md)** - [Next Module >](../modules/module00.md)

## :loudspeaker: Introduction

You make your sensitivity labels available to users by publishing them in a sensitivity label policy that appears in a list on the Label policies page. Just like sensitivity labels, the order of the sensitivity label policies is important because it reflects their priority: The label policy with lowest priority is shown at the top of the list with the lowest order number, and the label policy with the highest priority is shown at the bottom of the list with the highest order number.

A label policy consists of:
* A set of labels.
* The users and groups that will be assigned the policy with labels.
* The scope of the policy and policy settings for that scope (such as default label for files and emails).

You can include a user in multiple label policies, and the user will get all the sensitivity labels and settings from those policies. If there is a conflict in settings from multiple policies, the settings from the policy with the highest priority (highest order number) is applied. In other words, the highest priority wins for each setting.

In this task, we will add our new Sensitivity Label to a new label policy.

<!--## :thinking: Prerequisites

* Microsoft 365 E5/A5/G5
* Microsoft 365 E5/A5/G5 Compliance
* Microsoft 365 E5/A5/G5 Information Protection, and Governance
* Office 365 E5, Enterprise Mobility + Security E5/A5/G5, and AIP Plan 2 -->

## :dart: Objectives

* Create and Publish a new Label Policy for our Sensitivity Label created in the previous lab module.

## 1. Publish Label Policy

1. From the [Microsoft Purivew Compliance Portal](https://compliance.microsoft.com), select Solutions > Information Protection > Label Policies

2. On the **Label policies** page, select **Publish label** to start the **Create policy** configuration:

    ![image1](../images/module01/image1.png)

    To enable sensitivity labels for Office files in SharePoint and OneDrive, click 'Turn on now' if the message appears below. This step has already been taken in our lab environement.

    ![image2](../images//module01/image2.png)

3. On the **Choose sensitivity labels to publish** page, select the **Choose sensitivity labels to publish** link. Select the labels that you want to make available in apps and to services, and then select **Add**.

4. Review the selected labels and to make any changes, select **Edit**. Otherwise, select **Next**.

5. Follow the prompts to configure the policy settings.

    ![image3](../images/module01/scope.png)

6. On the Choose protection settings for labeled items page, select Encrypt and click Next.

    ![image4](../images/module01/encrypt.png)

7. On the Encryption page, select Configure encryption settings, Assign permissions now, Never, and Always for the drop down choices, and then click Assign permissions under Assign permissions to specific users and groups.

    ![image5](../images/module01/encryptpage.png)

8. On the Assign permissions page, select Add all users and groups in your organization and Choose permissions as Co-Author, click Save, and then click Next.

    ![image6](../images/module01/assignpermissions2.png)

9. On the Auto-labeling for files and emails page, click to enable Auto-labeling for files and emails and define the condition below:
    - Click Add condition
    - Click Content contains
    - Click Add and select Sensitive info types
    - Search for social and checkbox select U.S. Social Security Number and click Add
    - Click Next

    ![image7](../images/module01/autolabel1.png)

10. On the Define protection settings for groups and sites page do not make any selections, select Next.

11. On the Auto-labeling for schematized data assests(preview) page click to enable, click Choose sensitive info types, search for social security number, select U.S. Social Security Number (SSN), click Add, and select Next.

    ![image8](../images/module01/autolabel2.png)

12. On the Review your settings and finish page, select Create label.  The label will be created and when complete a message will display: Your sensitivity label was created.  Select Dont create a policy yet and then select Done.

## :tada: CONGRATULATIONS!
You've just created your first Sensitivity Label.  In the next module, you will Publish this Sensitivity Label to make it available across your apps and services.




MODULE_SUMMARY

[Continue >](../modules/module00.md)

# Masking Sensitive Data with Data Safe

## Objectives

In this lab you'll:

- Mask sensitive data in your database by using the Data Masking feature
- Create a PDF of the Data Masking report
- Validate the masked data in your database

## Prerequisites

## Prerequisites

To complete this lab, you need to have the following:

- An Oracle Cloud account
- Access to an Oracle Database as the `SYS` user, sample data for Oracle Data Safe loaded into the database, and the Discovery and Masking features enabled on your database
- Access to an Oracle Data Safe service
- Privileges to use the Discovery and Masking features on your database

### **Step 1:** Mask sensitive data by using Data Masking

1. Return to the browser tab for the Oracle Cloud Infrastructure Console. If needed, sign in again.
2. From the navigation menu, select **Data Safe**. The **Overview** page for the Oracle Data Safe service is displayed.
3. Click **Service Console**. The **Home** page in the Oracle Data Safe Console is displayed.
4. To access the Data Discovery wizard, click the **Data Masking** tab.
5. On the **Select Target for Sensitive Data Discovery** page, select your target database, and then click **Continue**.

![Select masking target](images/select-masking-target.png)

6. On the Masking Policy page, move the Expand All slider to the right to view all of the sensitive columns. Scroll down the page and review the default masking format selected for each sensitive column.

![Select masking target](images/select-masking-target.png)

7. On the **Select Masking Policy** page:
 - Click the create button under **Masking Policy**
 - Under **Masking Policy Name** enter **Mask1**
 - Under **Sensitive Data Model** select the **Pick from Library** button. In the next page we will pick the sensitive data model that we created in the [**Discover Sensitive Data**](discovery.md) lab.
 - Pick the compartment that you would like to user then click **continue** at the bottom of the page.

![Select masking policy](images/select-masking-policy.png)

 8. On the **Select Sensitive Data Model** page select **SDM1**
 9. Click **Update the SDM with Target** then click **Continue**.

![Select masking policy](images/select-sd-model.png)

10. Click **Continue** once the **Sensitive Data Discovery** is complete

![Select masking policy](images/sdm-discovery-complete.png)

11. Notice that only newly discovered sensitive columns will be displayed on the  **Sensitive Data Model: SDM1** page

![SDM1 Discovery](images/sdm1-discovery.png)

12. Click **View all sensitive columns**. Notice All Sensitive Columns are now available.

![SDM1 Discovery](images/sdm1-discovery-all.png)

13. Click **Save and Continue**

14. On the **Masking Policy** page, move the **Expand All** slider to the right to view all of the sensitive columns. Scroll down the page and review the default masking format selected for each sensitive column.

![Masking Policy Page](images/masking-policy.png)

15. For the `HCM1.LOCATIONS.STREET_ADDRESS` column, click the arrow to the right of the masking format to view other masking formats.

![Masking formats dropdown](images/masking-formats.png)

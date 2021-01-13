# Create Private Endpoint

## Introduction

Oracle Data Safe can connect to an Oracle Cloud database that has a public or private IP address on a virtual cloud network (VCN) in Oracle Cloud Infrastructure (OCI). This workshop describes the difference between public and private endpoints and explains the network connection between Oracle Data Safe and the databases. It also walks you through the steps of creating a private endpoint and registering a Exadata Cloud DB system with Oracle Data Safe when the DB system has a private IP address.

## Step 1: Create a Private Endpoint

If your DB system has a private IP address, you need to create a private endpoint for it prior to registering it with Oracle Data Safe. You can create private endpoints on the Data Safe page in OCI. Be sure to create the private endpoint in the same tenancy and VCN as your database. The private IP address does not need to be on the same subnet as your database, although, it does need to be on a subnet that can communicate with the database. You can create a maximum of one private endpoint per VCN.

- From your database's Console in OCI, obtain the name of the virtual cloud network (VCN) on which your database resides. You can find the name on the DB System Information tab.

**IMAGE HERE**

- From the navigation menu in OCI, select DataSafe. The Data Safe page is displayed.

**IMAGE HERE**

- Click Create Private Endpoint. The Create Private Endpoint page is displayed.

**IMAGE HERE**

- In the Name field, enter the name of your private endpoint.
- Select the compartment in which you want to store the private endpoint.
- Scroll down to the Private Endpoint Information section.
- From the VIRTUAL CLOUD NETWORK drop-down list,select your database's VCN. If needed, click CHANGE COMPARTMENT and select the compartment that stores your VCN. You can select a different VCN than your database's VCN if VCN peering is set up between your database's VCN and the VCN that you select here.
- From the SUBNET drop-down list, select a subnet within the selected VCN. If needed, click CHANGE COMPARTMENT and select the compartment that stores the subnet that you want to use. The subnet can be in a different compartment than the VCN. The subnet that you select needs to have access to the database's subnet.
- (Optional) In the PRIVATE IP field, specify a private IP address. If you do not specify a private IP address, OCI automatically generates one for you in the selected subnet.
- (Optional)Select a network security group. The following screenshot shows you an example configuration for a private endpoint:

**IMAGE HERE**

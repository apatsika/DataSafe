# Connecting to OCI

There are various ways by which you can connect your on-premises location to Oracle Cloud Infrastructure OCI. These include FastConnect, IPSec VPN, and the Oracle Data Safe Connector.

## FastConnect

FastConnect is a way to create a private connection between customer on-prem and Oracle Cloud Infrastructure. FastConnect supports bandwidths from 1Gbps to 10Gbps. There are three FastConnect options to choose from Oracle Provider, Third-Party Provider, and Colocation. The purpose of this blog is to help/guide you to choose the best option taking in consideration important points in the design. This blog focuses on design, for configuration and enablement, refer to the public documentation for FastConnect where you will find detail instructions for each option.

[Learn more about FastConnect](https://www.ateam-oracle.com/fastconnect-design)

## IPSec VPN

VPN Connect in Oracle Cloud Infrastructure is a site-to-site IPSec virtual private network that securely connects your on-premises network to Oracle Cloud Infrastructure, using your existing internet connection. VPN Connect is the easiest and fastest way to connect your on-premises network and your Oracle virtual cloud network (VCN) using IPSec tunnels over the internet. It uses industry standard IPSec protocol suite that encrypts the entire IP traffic before the packets are transferred from the source to the destination.

[Learn more about IPSec VPN](https://www.ateam-oracle.com/vpn-connect-simpe-implementation-part-12)

## Data Safe Connector

Using Oracle Data Safe's on-premises connector is an easy and convenient way to connect Oracle Data Safe to your on-premises Oracle database without needing FastConnect or VPN Connect.

[Data Safe Connector Documentation](https://docs.oracle.com/en-us/iaas/data-safe/doc/register-onpremises-oracle-databases-using-oracle-data-safe-onpremises-connector.html#GUID-24F31744-23D7-45ED-8573-86AA5056A1D3)

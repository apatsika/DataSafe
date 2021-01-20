# Data Safe for On-premise Oracle Data Sources

## Introduction

Data Safe is a unified security control center for your Oracle Databases. Data Safe provides security automation to easily detect PII and other sensitive data elements in your autonomous databases, create masked clones for test/dev, assess and monitor user security, centralize audit data and generate security and compliance reports.

## Objectives

This workshop comprises various aspects of Data Security. So follow the given sequence to enhance your skills on utilizing Data Safe with on-premise databases. You can register an on-premises Oracle database with Oracle Data Safe by using an Oracle Data Safe private endpoint. Prior to registration, you need to create an Oracle Data Safe private endpoint in your Oracle Cloud Infrastructure (OCI) tenancy. FastConnect/IPSec VPN is required to connect your on-premise location to the Oracle Cloud. In this lab, you will learn how to setup an IPSec VPN connection to an on-premise data source.

## Assumptions

To successfully complete this workshop it is assumed you have the following

- IPSec VPN connectivity from on-premise data center to the Oracle Cloud
- OCI IAM  policies allowing the use of Data Safe and the creation of Private Endpoints
- The following Oracle Database Versions 11g, 12c, 18c, 19c ...

## Table of Contents

- [Connecting to OCI](networking.md)
- [Register a Target Database](target-registration.md)
- [Provision Auditing](auditing.md)
- [Assess Database Configuration and Users](assessments.md)
- [Discover and Mask Sensitive Data](discovery.md)

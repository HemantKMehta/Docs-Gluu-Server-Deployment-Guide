# Gluu Server Deployment Guide
   

This guide focuses on planning the efficient Gluu Server deployment strategy for your organization/ application. Gluu server supports single server/ VM/ container-based deployment, cluster manager based deployment, and up to the highly scalable solution relying on Kubernetes and Clouchbase.
The underlying innovative technologies have enabled the Gluu server in processing a billion authentication per day. Gluu server relies on the cloud-native technologies, hosted Kubernetes like Amazon Elastic Kubernetes Services (EKS)  and Couchbase database to process a billion authentication a day. It also uses cost-effective autoscaling to meet the sudden demand without any extra pre-provisioning. 

## Introduction of Gluu Server   

Gluu Server is a free open source software (FOSS) that enables its users to control access to their resources. In a nutshell, the Gluu Server is an efficient Identity and Access Management (IAM) solution. Any multi-user web/ mobile application that requires user authentication, identity management and resource access policies can leverage a Gluu server.  
**Open Source Gluu Server**
-Gluu Server is an open-source software consisting of software written by Gluu and incorporated by other open-source projects. Gluu also supports the open-source as:
The source code is a free open-source with several essential interception scripts written by Gluu to implement the custom business logic for authentication and authorization. 
Gluu server binaries are free for different distributions (packages, containers, K8, snap etc.).

-Gluu Server documentation is freely available. 

-Gluu offers free and VIP support. The Gluu support portal is open to browse, register and post questions. The support portal (https://support.gluu.org) serves as a knowledge 
base for the users. The VIP support comes under a paid contract with guaranteed response time and consultative support (more details: https://www.gluu.org/pricing/). 

**Open Standards behind Gluu Server**
Gluu Server uses several open standards. Subsequent paragraphs discuss a brief detail of these standards.
**OAuth:** OAuth is an open-standard authorization protocol for authorization. It describes the way of authenticated access among unrelated servers. OAuth 2.0 is an industry-standard authorization protocol that focuses on client developer simplicity and providing authentication flows for different applications.
**OpenID Connect:** OpenID connect (OIDC) is an identity layer on top of OAuth 2.0 protocol. OIDC enables the users to verify users’ identity, which was authenticated by an authorization server or identity provider (IDP). OpenID Connect specifies a RESTful HTTP API using JSON as a data format.
**SAML:** Security Assertion Markup Language (SAML) is a standard for Web-based single sign-on (SSO). SAML is an XML-based open-standard for exchanging authentication and authorization between the IDP and service provider (SP).
**UMA:** User-Managed Access (UMA) is an OAuth-based access management protocol standard. The purpose of UMA is to enable the resource owners to control the data sharing and protected resource access among the online services on the owner’s behalf.
**RADIUS:** RADIUS is an AAA (Authentication, Authorization, and Accounting) protocol to manage network access. RADIUS uses two packet types, namely Access-Request for authentication and authorization and Accounting-Request for third A, accounting. 
**SCIM:** System for Cross-Domain Identity Management (SCIM) is a standard to automate the user identity exchange on the web and in cross-domain applications such as enterprise to cloud service providers or inter-cloud services. 
**CAS:** Central Authentication Service is an SSO protocol for web-based applications. CAS protocol mainly involves a client (usually a web browser), a web application requesting the authentication, and a CAS Server.
**Gluu Server Design Goals**
The following are the underlying design goals behind Gluu server development. 
**High Concurrency:**  By design, Gluu Server supports applications with millions of authentication records and billions of authentications in a day.
**High Availability:**  Gluu Server supports the clustering of multiple instances to enable high availability with proper load balancing of the services. 
**Flexibility:**  This is another key design goal behind the Gluu Server is its capability to handle various requirements. The Gluu team has developed several interception scripts to enable the customization without forking the Gluu server code to achieve flexibility.
Low cost of operation: The selection of various components enables the lower operating cost of the Gluu Server deployment without compromising the performance and essential design goals (concurrency, availability and flexibility). 

## Making changes
Fork, clone, and make a pull request.

**Note: "Master" is the branch for editing this `README.md`.  You will not see documentation files until you check out the specific branch.**

## Check out the docs

`$ git checkout <branchname>`

## Update (for those who have privileges)

```
/path/to/repo/branchname (branchname)
$ ./update-site-local-sh
```


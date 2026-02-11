# Amazon QuickSight Embedding Sample
Thank you for using Amazon QuickSight. We have put together a sample for embedding dashboards in your apps running on a web browser. As the embedding API currently does not support CORS, we have provided an example of a lambda based setup, which enables you to invoke the embedding API from your web app.

## Disclaimers
Customers are responsible for making their own independent assessment of the information in this document.

This document:

(a) is for informational purposes only,

(b) references AWS product offerings and practices, which are subject to change without notice,

(c) does not create any commitments or assurances from AWS and its affiliates, suppliers or licensors. AWS products or services are provided "as is" without warranties, representations, or conditions of any kind, whether express or implied. The responsibilities and liabilities of AWS to its customers are controlled by AWS agreements, and this document is not part of, nor does it modify, any agreement between AWS and its customers, and

(d) is not to be considered a recommendation or viewpoint of AWS.

Additionally, you are solely responsible for testing, security and optimizing all code and assets on GitHub repo, and all such code and assets should be considered:

(a) as-is and without warranties or representations of any kind,

(b) not suitable for production environments, or on production or other critical data, and

(c) to include shortcuts in order to support rapid prototyping such as, but not limited to, relaxed authentication and authorization and a lack of strict adherence to security best practices.

All work produced is open source. More information can be found in the GitHub repo.

## Usage
Before you can embed an Amazon QuickSight dashboard, you need to publish it and ensure that users are granted necessary permissions. For more information, see  [Embedding Amazon QuickSight Dashboards](https://docs.aws.amazon.com/quicksight/latest/user/embedding-dashboards.html) in the Amazon QuickSight User Guide.

# Amazon QuickSight SSO
QuickSight Embedding SSO works by obtaining AWS Credentials from the users logged in credentials.

Amazon QuickSight provides the following options for implementing SSO.
1. OpenID Connect
2. SAML
3. QuickSight authenticated.

The sample application covers OpenID Connect based SSO integrating with Cognito - Refer to OpenIDAuthentication folder for more details.

QuickSight authenticated can be used for QuickSight enterprise account with AD integration, or can be used in cases. A sample application highlighting that is available in QuickSightAuthentication folder.
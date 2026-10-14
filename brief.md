Version: NAFATH-V1
Track: Software

## Overview

A national login service allows citizens to access different government services using one account through a mobile app or website. In software, OpenID Connect helps applications verify users' identities and sign them in securely. The service should use clear software design and reliable authentication methods to reduce login errors. The mobile app must be easy to use, accessible, and regularly updated because citizens depend on it to access important services. Networking and cybersecurity controls, such as encrypted connections and multi-factor authentication, can help protect users from data theft and unauthorized access. Artificial intelligence can help detect unusual login activity, but it can also produce false alerts and raise privacy concerns. Finally, the authority must protect citizens' personal data and follow Oman's applicable data protection laws. A secure and reliable service requires cooperation between software, mobile development, networking, cybersecurity, AI, and data management.

## Software

OAuth 2.0 and OpenID Connect have different purposes. OAuth 2.0 is an authorization framework that allows applications to access specific resources with permission. OpenID Connect is an identity layer built on top of OAuth 2.0. It adds authentication, allowing an application to verify who the user is through an ID token. For a national login service, OpenID Connect is suitable for verifying citizens' identities, while OAuth 2.0 supports authorized access to protected resources.

Resource: OpenID Connect Core 1.0 - https://openid.net/specs/openid-connect-core-1_0.html

## AI

The NIST AI Risk Management Framework (AI RMF) provides four functions: Govern, Map, Measure, and Manage. Before using an AI model to detect suspicious logins, the authority should identify risks such as false alerts, unfair bias, and privacy problems involving citizens' data. The model should be tested to measure its accuracy before deployment. Clear responsibility, regular monitoring, and human review of important decisions can help reduce risks and protect users.

Resource: NIST AI Risk Management Framework - https://www.nist.gov/itl/ai-risk-management-framework

## Mobile

Android runtime permissions help protect users' private data by allowing them to approve or deny access to sensitive features. For a national login app, permissions should be limited to what is necessary for each feature. The app should request permission when the user starts an action that needs it, such as scanning an identity document with the camera. If permission is denied, the app should offer another available login method when possible.

Resource: Permissions on Android - https://developer.android.com/guide/topics/permissions/overview

## Networking

DNS over HTTPS (DoH) sends DNS queries through encrypted HTTPS connections. This helps prevent other devices on the network from easily reading or changing DNS queries while they travel between the user and the DoH resolver. However, DoH does not provide complete privacy. The DoH provider may still see the queries, and the user's destination IP address may remain visible to the network. DoH also cannot prevent users from visiting phishing websites.

Resource: RFC 8484 - https://www.rfc-editor.org/rfc/rfc8484

## Cybersecurity

Phishing-resistant multi-factor authentication (MFA) helps stop attackers from using stolen login information on fake websites. FIDO2/WebAuthn and security keys provide strong protection because authentication is linked to the legitimate website. In contrast, SMS codes and app-generated one-time passwords can be stolen through phishing. Users may be tricked into entering these codes on a fake login page, allowing attackers to access their accounts.

Resource: Implementing Phishing-Resistant MFA - https://www.cisa.gov/sites/default/files/2023-01/fact-sheet-implementing-phishing-resistant-mfa-508c.pdf

## Data

Oman's Personal Data Protection Law, issued by Royal Decree 6/2022, defines a controller as the legal person responsible for processing personal data. Where the law applies, the controller must obtain explicit consent unless a legal exception applies, establish safeguards to manage risks, and erase data when its processing purpose ends, subject to legal exceptions. Article 3 excludes certain processing by government bodies when carrying out their legally assigned functions, so the law's applicability must be assessed carefully.

Resource: Royal Decree 6/2022 Issuing the Personal Data Protection Law (Consolidated) - https://decree.om/2022/l20220006/

## Misconception in My Track

## Open Question

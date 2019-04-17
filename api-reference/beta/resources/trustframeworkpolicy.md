---
title: "trustFrameworkPolicy"
description: "In the Azure AD B2C trust framework policy is referred to as custom policies. This describes the operations available on a trustFrameworkPolicy object for the tenant."
localization_priority: Normal
author: "valnav"
ms.prod: "microsoft-identity-platform"
---
# trustFrameworkPolicy resource type

> **Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change. Use of these APIs in production applications is not supported.

Represents a [TrustFramework](https://docs.microsoft.com/en-us/azure/active-directory-b2c/active-directory-b2c-reference-trustframeworks-defined-ief-custom) Policy (also called [custom policy](https://docs.microsoft.com/en-us/azure/active-directory-b2c/active-directory-b2c-overview-custom)) in [Azure Active Directory B2C](https://docs.microsoft.com/en-us/azure/active-directory-b2c/active-directory-b2c-overview). A trustFrameworkPolicy gives full control over the User Journeys.  Use the trustFrameworkPolicy to:

* Customize the sign-up and sign-in experiences fully.
* Federate to any SAML, Open ID Connect, or OAuth2 identity provider.
* Integrate with other systems or user data stores by calling REST endpoints.
* Transform claims and customize tokens issued to the relying party application.

For more information, see [https://docs.microsoft.com/en-us/azure/active-directory-b2c/active-directory-b2c-overview-custom](https://docs.microsoft.com/en-us/azure/active-directory-b2c/active-directory-b2c-overview-custom).

## Methods

| Method       | Return Type  |Description|
|:---------------|:--------|:----------|
|[Create trustFrameworkPolicy](../api/trustframework-post-trustframeworkpolicy.md)|trustFramework Policy|Create a new trustFrameworkPolicy.|
|[Get trustFrameworkPolicy](../api/trustframework-policies-get.md) |trustFrameworkPolicy|Read properties of an existing trustFrameworkPolicy.|
|[List trustFrameworkPolicies](../api/trustframework-policies-list.md)|trustFrameworkPolicy collection|List all trustFrameworkPolicies configured in a tenant.|
|[Update or create trustFrameworkPolicy](../api/trustframework-put-trustframeworkpolicy.md)|None|Update an existing trustFrameworkPolicy.|
|[Delete trustFrameworkPolicy](../api/trustframework-policies-delete.md)|None|Delete an existing trustFrameworkPolicy.|

## Properties

|Property|Type|Description|
|:---------------|:--------|:----------|
|id|String|The id of the policy.|

## JSON representation

The following is a JSON representation of the resource.

```json
{
   "id": "B2C_1A_Test"
}
```

## XML representation

The following is an XML representation of the policy.  For more information, refer to the [documentation](https://docs.microsoft.com/en-us/azure/active-directory-b2c/trustframeworkpolicy) here.  The complete XML schema, refer to the TrustFrameworkPolicy xsd file here: [https://github.com/Azure-Samples/active-directory-b2c-custom-policy-starterpack](https://github.com/Azure-Samples/active-directory-b2c-custom-policy-starterpack).

```xml
<TrustFrameworkPolicy xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns="http://schemas.microsoft.com/online/cpim/schemas/2013/06" PolicySchemaVersion="0.3.0.0" TenantId="tenantName.onmicrosoft.com" PolicyId="B2C_1A_SocialAndLocalAccounts_Base">
    <!---PolicyContent-->
</TrustFrameworkPolicy>
```
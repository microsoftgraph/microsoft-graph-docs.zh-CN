---
title: 更新 crossTenantAccessPolicyConfigurationPartner
description: 更新特定于合作伙伴的配置的属性。
author: jkdouglas
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
---

# <a name="update-crosstenantaccesspolicyconfigurationpartner"></a>更新 crossTenantAccessPolicyConfigurationPartner

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

更新特定于合作伙伴 [的配置的属性](../resources/crosstenantaccesspolicyconfigurationpartner.md) 。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|Policy.ReadWrite.CrossTenantAccess|
|委派（个人 Microsoft 帐户）|不适用|
|应用程序|Policy.ReadWrite.CrossTenantAccess|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->

``` http
PATCH /policies/crossTenantAccessPolicy/partners/{id}
```

## <a name="request-headers"></a>请求标头

|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文

[!INCLUDE [table-intro](../../includes/update-property-table-intro.md)]

|属性|类型|说明|
|:---|:---|:---|
| b2bCollaborationInbound | [crossTenantAccessPolicyB2BSetting](../resources/crosstenantaccesspolicyb2bsetting.md) | 为其他组织的用户定义合作伙伴特定的配置，这些用户通过 B2B 协作Azure AD你的资源。 |
| b2bCollaborationOutbound | [crossTenantAccessPolicyB2BSetting](../resources/crosstenantaccesspolicyb2bsetting.md) | 为贵组织的用户定义合作伙伴特定的配置，以便通过 B2B 协作出站访问Azure AD中的资源。 |
| b2bDirectConnectInbound | [crossTenantAccessPolicyB2BSetting](../resources/crosstenantaccesspolicyb2bsetting.md) | 为来自其他组织的用户定义合作伙伴特定的配置，这些用户通过 Azure AD B2B 直接连接访问你的资源。 |
| b2bDirectConnectOutbound | [crossTenantAccessPolicyB2BSetting](../resources/crosstenantaccesspolicyb2bsetting.md) | 为贵组织中出站以通过 B2B 直接连接访问另一Azure AD合作伙伴特定的配置。 |
| inboundTrust | [crossTenantAccessPolicyInboundTrust](../resources/crosstenantaccesspolicyinboundtrust.md) | 确定用于信任来自外部组织的其他条件访问声明的合作伙伴Azure Active Directory (Azure AD) 配置。 |

## <a name="response"></a>响应

如果成功，此方法返回 `204 No Content` 响应代码。

## <a name="examples"></a>示例

### <a name="request"></a>请求

<!-- {
  "blockType": "request",
  "name": "update_crosstenantaccesspolicyconfigurationpartner"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/policies/crossTenantAccessPolicy/partners/90e29127-71ad-49c7-9ce8-db3f41ea06f1
Content-Type: application/json

{
  "inboundTrust": 
  {
    "isMfaAccepted": true,
    "isCompliantDeviceAccepted": true,
    "isHybridAzureADJoinedDeviceAccepted" : true
  }
}
```

### <a name="response"></a>响应

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```

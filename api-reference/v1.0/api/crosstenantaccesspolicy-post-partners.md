---
title: 创建 crossTenantAccessPolicyConfigurationPartner
description: 在跨租户访问策略中创建新的合作伙伴配置。
author: jkdouglas
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 65d24e72ffbe80182641a3ba8a52500c0adfcb6e
ms.sourcegitcommit: a30eea2fa59087088f50e58706b91c0eb5b7a802
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/01/2022
ms.locfileid: "66604559"
---
# <a name="create-crosstenantaccesspolicyconfigurationpartner"></a>创建 crossTenantAccessPolicyConfigurationPartner

命名空间：microsoft.graph

在跨租户访问策略中创建新的合作伙伴配置。

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
POST /policies/crossTenantAccessPolicy/partners
```

## <a name="request-headers"></a>请求标头

|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文

在请求正文中，提供 [crossTenantAccessPolicyConfigurationPartner](../resources/crosstenantaccesspolicyconfigurationpartner.md) 对象的 JSON 表示形式。

下表显示了创建 [crossTenantAccessPolicyConfigurationPartner](../resources/crosstenantaccesspolicyconfigurationpartner.md) 时所需的属性。

|属性|类型|说明|
|:---|:---|:---|
| b2bCollaborationInbound | [crossTenantAccessPolicyB2BSetting](../resources/crosstenantaccesspolicyb2bsetting.md) | 为通过 Azure AD B2B 协作访问资源的其他组织的用户定义特定于合作伙伴的配置。 |
| b2bCollaborationOutbound | [crossTenantAccessPolicyB2BSetting](../resources/crosstenantaccesspolicyb2bsetting.md) | 为组织中通过 Azure AD B2B 协作出站访问其他组织中的资源的用户定义特定于合作伙伴的配置。 |
| b2bDirectConnectInbound | [crossTenantAccessPolicyB2BSetting](../resources/crosstenantaccesspolicyb2bsetting.md) | 为通过 Azure AD B2B 直接连接访问资源的其他组织的用户定义特定于合作伙伴的配置。 |
| b2bDirectConnectOutbound | [crossTenantAccessPolicyB2BSetting](../resources/crosstenantaccesspolicyb2bsetting.md) | 为组织中通过 Azure AD B2B 直接连接出站访问其他组织中的资源的用户定义特定于合作伙伴的配置。 |
| inboundTrust | [crossTenantAccessPolicyInboundTrust](../resources/crosstenantaccesspolicyinboundtrust.md) | 确定特定于合作伙伴的配置，以便信任来自外部 Azure AD 组织的其他条件访问声明。 |
| tenantId | String | 合作伙伴 Azure Active Directory (Azure AD) 组织的租户标识符。 |

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [crossTenantAccessPolicyConfigurationPartner](../resources/crosstenantaccesspolicyconfigurationpartner.md) 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求

<!-- {
  "blockType": "request",
  "name": "create_crosstenantaccesspolicyconfigurationpartner_from_"
}
-->

``` http
POST https://graph.microsoft.com/v1.0/policies/crossTenantAccessPolicy/partners
Content-Type: application/json

{
  "tenantId": "3d0f5dec-5d3d-455c-8016-e2af1ae4d31a",
  "b2bDirectConnectOutbound": 
  {
    "usersAndGroups": 
    {
      "accessType": "blocked",
      "targets": [
        {
            "target": "6f546279-4da5-4b53-a095-09ea0cef9971",
            "targetType": "group"
        }
      ]
    }
  },
  "b2bDirectConnectInbound": 
  {
    "applications":
    {
      "accessType": "allowed",
      "targets": [
        {
            "target": "Office365",
            "targetType": "application"
        }
      ]
    }
  }
}
```

### <a name="response"></a>响应

下面展示了示例响应。
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.crossTenantAccessPolicyConfigurationPartner"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "tenantId": "3d0f5dec-5d3d-455c-8016-e2af1ae4d31a",
  "inboundTrust": null,
  "b2bCollaborationInbound": null,
  "b2bCollaborationOutbound": null,
  "b2bDirectConnectOutbound": 
  {
    "usersAndGroups":
    {
      "accessType": "blocked",
      "targets": [
        {
          "target": "6f546279-4da5-4b53-a095-09ea0cef9971",
          "targetType": "group"
        }
      ]
    }
  },
  "b2bDirectConnectInbound":
  {
    "applications":
    {
      "accessType": "allowed",
      "targets": [
        {
          "target": "Office365",
          "targetType": "application"
        }
      ]
    }
  }
}
```

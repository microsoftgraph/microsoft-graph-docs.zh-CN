---
title: 创建 crossTenantAccessPolicyConfigurationPartner
description: 在跨租户访问策略中创建新的合作伙伴配置。
author: jkdouglas
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 0397a4d2d536c9b4fd11c4ba49721ede6ab596df
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63335813"
---
# <a name="create-crosstenantaccesspolicyconfigurationpartner"></a>创建 crossTenantAccessPolicyConfigurationPartner

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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

下表显示创建 [crossTenantAccessPolicyConfigurationPartner 时所需的属性](../resources/crosstenantaccesspolicyconfigurationpartner.md)。

|属性|类型|说明|
|:---|:---|:---|
| b2bCollaborationInbound | [crossTenantAccessPolicyB2BSetting](../resources/crosstenantaccesspolicyb2bsetting.md) | 为其他组织的用户定义合作伙伴特定的配置，这些用户通过 B2B 协作Azure AD你的资源。 |
| b2bCollaborationOutbound | [crossTenantAccessPolicyB2BSetting](../resources/crosstenantaccesspolicyb2bsetting.md) | 为贵组织的用户定义合作伙伴特定的配置，以便通过 B2B 协作出站访问另一Azure AD中的资源。 |
| b2bDirectConnectInbound | [crossTenantAccessPolicyB2BSetting](../resources/crosstenantaccesspolicyb2bsetting.md) | 为来自其他组织的用户定义合作伙伴特定的配置，这些用户通过 Azure AD B2B 直接连接访问你的资源。 |
| b2bDirectConnectOutbound | [crossTenantAccessPolicyB2BSetting](../resources/crosstenantaccesspolicyb2bsetting.md) | 为贵组织的用户定义合作伙伴特定的配置，以便通过 B2B 直接连接出站访问另一Azure AD中的资源。 |
| inboundTrust | [crossTenantAccessPolicyInboundTrust](../resources/crosstenantaccesspolicyinboundtrust.md) | 确定用于信任外部访问组织的其他条件访问声明的合作伙伴Azure AD配置。 |
| tenantId | String | 合作伙伴组织的租户Azure Active Directory (Azure AD) 标识符。 |

## <a name="response"></a>响应

如果成功，此方法在响应 `201 Created` 正文中返回 响应代码和 [crossTenantAccessPolicyConfigurationPartner](../resources/crosstenantaccesspolicyconfigurationpartner.md) 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_crosstenantaccesspolicyconfigurationpartner_from_"
}
-->

``` http
POST https://graph.microsoft.com/beta/policies/crossTenantAccessPolicy/partners
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
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-crosstenantaccesspolicyconfigurationpartner-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-crosstenantaccesspolicyconfigurationpartner-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-crosstenantaccesspolicyconfigurationpartner-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-crosstenantaccesspolicyconfigurationpartner-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-crosstenantaccesspolicyconfigurationpartner-from--go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/create-crosstenantaccesspolicyconfigurationpartner-from--powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


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

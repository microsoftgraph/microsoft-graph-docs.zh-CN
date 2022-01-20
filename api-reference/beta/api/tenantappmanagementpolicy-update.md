---
title: 更新 tenantAppManagementPolicy
description: 更新应用于应用程序和服务主体对象的默认租户策略。
ms.localizationpriority: medium
author: madansr7
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: c1d1e150d0eae6ed820b4ed0963a010b3bcfcea1
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62098491"
---
# <a name="update-tenantappmanagementpolicy"></a>更新 tenantAppManagementPolicy

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

更新 [tenantAppManagementPolicy 对象](../resources/tenantAppManagementPolicy.md) 的属性。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权）                                                |
| :------------------------------------- | :--------------------------------------------------------- |
| 委派（工作或学校帐户）     | Policy.ReadWrite.ApplicationConfiguration |
| 委派（个人 Microsoft 帐户） | 不支持。                                             |
| 应用程序                            | Policy.ReadWrite.ApplicationConfiguration |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
PATCH /policies/defaultAppManagementPolicy
```

## <a name="request-headers"></a>请求标头

| 名称          | 说明                 |
| :------------ | :-------------------------- |
| Authorization | Bearer {token}。必需。   |
| Content-Type  | application/json. Required. |

## <a name="request-body"></a>请求正文

在请求正文中，提供 [tenantAppManagementPolicy](../resources/tenantAppManagementPolicy.md) 中应更新的相关字段的值。 请求正文中未包含的现有属性将保留其以前的值。 为获得最佳性能，请勿在请求有效负载中包括未更改的值。

| 属性                | 类型                                                                        | 说明 |
|:------------------------|:----------------------------------------------------------------------------|:----------------------------------------------------|
| displayName                  | String                                                                   | 默认显示名称的默认值。 继承自 [policyBase](../resources/policybase.md)。                                |
| 说明                  | String                                                                   | 默认策略的说明。 继承自 [policyBase](../resources/policybase.md)。                                |
| isEnabled                    | Boolean                                                                  | 表示策略是否已启用。 默认值为 false。                                    |
| applicationRestrictions      | [appManagementConfiguration](../resources/appManagementConfiguration.md) | 应用于租户中所有应用程序对象的默认限制。               |
| servicePrincipalRestrictions | [appManagementConfiguration](../resources/appManagementConfiguration.md) | 应用于租户中所有服务主体对象的默认限制。 |

## <a name="response"></a>响应

如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。

## <a name="examples"></a>示例

### <a name="request"></a>请求

下面展示了示例请求。



# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_tenantAppManagementPolicy"
}-->

```msgraph-interactive
PATCH https://graph.microsoft.com/beta/policies/defaultAppManagementPolicy
Content-Type: application/json

{
    "isEnabled": true,
    "applicationRestrictions": {
        "passwordCredentials": [
            {
                "restrictionType": "passwordAddition",
                "maxLifetime": null,
                "restrictForAppsCreatedAfterDateTime": "2021-04-01T10:37:00Z"
            },
            {
                "restrictionType": "passwordLifetime",
                "maxLifetime": "P4DT12H30M5S",
                "restrictForAppsCreatedAfterDateTime": "2019-01-01T10:37:00Z"
            },
            {
                "restrictionType": "symmetricKeyAddition",
                "maxLifetime": null,
                "restrictForAppsCreatedAfterDateTime": "2021-04-01T10:37:00Z"
            },
            {
                "restrictionType": "symmetricKeyLifetime",
                "maxLifetime": "P40D",
                "restrictForAppsCreatedAfterDateTime": "2015-04-01T10:37:00Z"
            }
        ],
        "keyCredentials":[
            {
                "restrictionType": "asymmetricKeyLifetime",
                "maxLifetime": "P30D",
                "restrictForAppsCreatedAfterDateTime": "2015-01-01T10:37:00Z"
            },
        ]
    }
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-tenantappmanagementpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-tenantappmanagementpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-tenantappmanagementpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-tenantappmanagementpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-tenantappmanagementpolicy-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/update-tenantappmanagementpolicy-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应

下面展示了示例响应。

<!-- {
  "blockType": "response",
  "truncated": false
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update tenantAppManagementPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

---
title: 更新 tenantAppManagementPolicy
description: 更新应用于应用程序和服务主体对象的默认租户策略。
localization_priority: Normal
author: madansr7
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: eb7e7c6003f3b262c0745eb7ae5ca2b445e259be
ms.sourcegitcommit: b711aed8acc18512cf6591f4108ed5ddf05b649d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/29/2021
ms.locfileid: "53660375"
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
PATCH /policies/tenantAppManagementPolicy
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
| displayName                  | 字符串                                                                   | 默认显示名称的默认值。 继承自 [policyBase](../resources/policybase.md)。                                |
| 说明                  | 字符串                                                                   | 默认策略的说明。 继承自 [policyBase](../resources/policybase.md)。                                |
| isEnabled                    | Boolean                                                                  | 表示策略是否已启用。 默认值为 false。                                    |
| applicationRestrictions      | [appManagementConfiguration](../resources/appManagementConfiguration.md) | 应用于租户中所有应用程序对象的默认限制。               |
| servicePrincipalRestrictions | [appManagementConfiguration](../resources/appManagementConfiguration.md) | 应用于租户中所有服务主体对象的默认限制。 |

## <a name="response"></a>响应

如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。

## <a name="examples"></a>示例

### <a name="request"></a>请求

下面展示了示例请求。


<!-- {
  "blockType": "request",
  "name": "update_tenantAppManagementPolicy"
}-->

```msgraph-interactive
PATCH https://graph.microsoft.com/beta/policies/tenantAppManagementPolicy
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
            }
        ]
    }
}
```

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

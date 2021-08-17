---
title: 创建 appManagementPolicy
description: 创建应用程序管理策略。
localization_priority: Normal
author: madansr7
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 9553accf83925e1ab33c36f353a7ca74da6ad623
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58262388"
---
# <a name="create-appmanagementpolicy"></a>创建 appManagementPolicy

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

创建 [appManagementPolicy](../resources/appManagementPolicy.md) 对象。

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
POST /policies/appManagementPolicies
```

## <a name="request-headers"></a>请求标头

| 名称          | 说明                 |
| :------------ | :-------------------------- |
| Authorization | Bearer {token}。必需。   |
| Content-Type  | application/json. Required. |

## <a name="request-body"></a>请求正文

在请求正文中，提供 [appManagementPolicy](../resources/appManagementPolicy.md)的 JSON 表示形式。

## <a name="response"></a>响应

如果成功，此方法在响应有效负载中返回包含新 `201 Created` [appManagementPolicy ](../resources/appmanagementpolicy.md) 对象的 响应代码。

## <a name="examples"></a>示例

### <a name="request"></a>请求

下面展示了示例请求。 此请求创建了具有以下设置的应用管理策略：

- 启用策略。
- 阻止在 UTC 时间 2019 年 10 月 10-19 日上午 10：37 之后为应用和服务主体创建新密码。
- 将 UTC 时间 2019-10-19 日上午 10：37 创建的应用和服务主体的密码密码限制为少于 XX 天。


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_appManagementPolicy"
}-->

```http
POST https://graph.microsoft.com/beta/policies/appManagementPolicies

{
    "displayName": "Credential management policy",
    "description": "Cred policy sample",
    "isEnabled": true,
    "restrictions": {
        "passwordCredentials": [
            {
                "restrictionType": "passwordAddition",
                "maxLifetime": null,
                "restrictForAppsCreatedAfterDateTime": "2019-10-19T10:37:00Z"
            },
            {
                "restrictionType": "passwordLifetime",
                "maxLifetime": "P4DT12H30M5S",
                "restrictForAppsCreatedAfterDateTime": "2018-10-19T10:37:00Z"
            }
        ]
    }
}

```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-appmanagementpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-appmanagementpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-appmanagementpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-appmanagementpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应

下面展示了示例响应。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.appManagementPolicy"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#policies/appManagementPolicies/$entity",
    "id": "a4ab1ed9-46bb-4bef-88d4-86fd6398dd5d",
    "displayName": "credential management policy",
    "description": "Lorem ipsum",
    "isEnabled": true,
    "restrictions": {
        "passwordCredentials": [
            {
                "restrictionType": "passwordAddition",
                "maxLifetime": null,
                "restrictForAppsCreatedAfterDateTime": "2019-10-19T10:37:00Z"
            },
            {
                "restrictionType": "passwordLifetime",
                "maxLifetime": "P4DT12H30M5S",
                "restrictForAppsCreatedAfterDateTime": "2018-10-19T10:37:00Z"
            }
        ]
    }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "create appManagementPolicies",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

---
title: 分配给应用程序或服务主体的列表策略
description: 检索分配给应用程序或服务主体的策略对象。
localization_priority: Normal
ms.openlocfilehash: 417d59228aadd3c6a54c4634416fd577fce11f18
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29575959"
---
# <a name="list-policies-assigned-to-application-or-service-principal"></a>分配给应用程序或服务主体的列表策略

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

检索分配给应用程序或服务主体的[策略](../resources/policy.md)对象。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Directory.AccessAsUser.All    |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | 不支持。 |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
GET /applications/{id}/policies
```

> 注意： 请求中的"id"为应用程序或服务主体，不是"appid"属性"id"属性。

## <a name="request-headers"></a>请求标头
| 名称       | 类型 | 说明|
|:---------------|:--------|:----------|
| Authorization  | string  | Bearer {token}。必需。 |

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法返回`200 OK`响应正文中的响应代码和[策略](../resources/policy.md)对象。 如果不成功，`4xx`与特定的详细信息，则返回错误。

## <a name="example"></a>示例
以下示例检索分配给应用程序的策略。

##### <a name="request"></a>请求
下面是一个请求示例。

```http
GET https://graph.microsoft.com/beta/applications/{id}/policies
```

##### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。

```http
HTTP/1.1 200 OK
Cache-Control: private
Content-Type: application/json

{
    "value":[
        {
            "@odata.type":"#microsoft.graph.policy",
            "id":"id-value",
            "alternativeIdentifier":null,
            "definition":["policy-definition"],
            "displayName":"name-value",
            "isOrganizationDefault": true | false,
            "keyCredentials":[key-credentials],
            "type":"type-value"
        }
    ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/policy-list-assigned.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

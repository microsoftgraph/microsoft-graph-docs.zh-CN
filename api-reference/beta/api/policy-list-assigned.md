---
title: 为应用程序或服务主体分配的列表策略
description: 获取分配给应用程序或服务主体的策略对象。
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: dkershaw10
ms.openlocfilehash: 6aa20deefa63325bf369fc2c59db97add4732569
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2020
ms.locfileid: "44289705"
---
# <a name="list-policies-assigned-to-application-or-service-principal"></a>为应用程序或服务主体分配的列表策略

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

获取分配给应用程序或服务主体的[策略](../resources/policy.md)对象。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Directory.Read.All、Directory.AccessAsUser.All    |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | Directory.Read.All |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
GET /applications/{id}/policies
```

> 注意：请求中的 "id" 是应用程序或服务主体的 "id" 属性，而不是 "appid" 属性。

## <a name="request-headers"></a>请求标头
| 名称           | 说明                |
|:---------------|:---------------------------|
| Authorization  | Bearer {token}。必需。  |

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法 `200 OK` 在响应正文中返回响应代码和[policy](../resources/policy.md)对象。 如果失败，将返回 `4xx` 错误并显示具体详细信息。

## <a name="example"></a>示例
下面的示例检索分配给应用程序的策略。

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
            "isOrganizationDefault":boolean-value,
            "keyCredentials":[key-credentials],
            "type":"type-value"
        }
    ]
}
```

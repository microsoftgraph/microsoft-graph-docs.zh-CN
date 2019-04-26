---
title: 列表策略
description: 检索目录中的所有 policy 对象。
localization_priority: Normal
ms.openlocfilehash: 7f4b70391b68a47073866248c31395df4ebaaf45
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33337376"
---
# <a name="list-policies"></a>列表策略

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

检索目录中的所有[policy](../resources/policy.md)对象。

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
GET /policies
```
## <a name="request-headers"></a>请求标头
| 名称       | 类型 | 说明|
|:---------------|:--------|:----------|
| Authorization  | string  | Bearer {token}。必需。 |

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功, 此方法在`200 OK`响应正文中返回响应代码和[policy](../resources/policy.md)对象。 如果不成功 .。。

## <a name="example"></a>示例
下面的示例检索所有策略。

##### <a name="request"></a>请求
下面是一个请求示例。

```http
GET https://graph.microsoft.com/beta/policies
```

##### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。

```http
HTTP/1.1 200 OK
Content-type: application/json
{
    "value":[
        {
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

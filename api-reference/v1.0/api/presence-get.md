---
title: 获取状态
description: 获取用户的状态信息。
author: elvinyang-msft
localization_priority: Normal
doc_type: apiPageType
ms.prod: cloud-communications
ms.openlocfilehash: a82c03e9b63d83f8aab8b3556e75b17d926ff3e6
ms.sourcegitcommit: e68fdfb1124d16265deb8df268d4185d9deacac6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/05/2020
ms.locfileid: "49581197"
---
# <a name="get-presence"></a>获取状态

命名空间：microsoft.graph

获取用户的 [状态](../resources/presence.md) 信息。

## <a name="permissions"></a>权限
若要调用这些 Api，必须有以下权限之一。 若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型 | 权限（从最低特权到最高特权）                  |
| :-------------- | :----------------------------------------------------------- |
| 委派（工作或学校帐户）     | 状态.阅读，状态.阅读.全部      |
| 委派（个人 Microsoft 帐户） | 不支持。                        |
| 应用程序                            | 不支持。                        |

> **注意：** 此 API 的最大请求速率为每个租户在30秒内的每个应用程序的 1500 API 请求数。

## <a name="http-requests"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
GET /me/presence
GET /users/{id}/presence
GET /communications/presences
```

## <a name="request-headers"></a>请求标头
| 名称          | 说明               |
|:--------------|:--------------------------|
| Authorization | Bearer {token}。必需。 |


## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应
如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [状态](../resources/presence.md) 对象。

## <a name="examples"></a>示例

### <a name="example-1-get-your-own-presence-information"></a>示例1：获取自己的状态信息

下面的示例展示了如何获取自己的状态信息。 此操作需要状态为 "读取" 权限。

#### <a name="request"></a>请求


<!-- {
  "blockType": "request",
  "name": "get-your-presence"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/presence
```

---


#### <a name="response"></a>响应

<!-- {
  "blockType": "response",
  "name": "get-your-presence",
  "@odata.type": "microsoft.graph.presence",
  "truncated":"true"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1574

{  
    "id": "fa8bf3dc-eca7-46b7-bad1-db199b62afc3",
    "availability": "Available",
    "activity": "Available"
}
```

### <a name="example-2-get-the-presence-information-of-another-user"></a>示例2：获取其他用户的状态信息

下面的示例展示了如何获取其他用户的状态信息。 此操作需要已读。 All 权限。

#### <a name="request"></a>请求

<!-- {
  "blockType": "request",
  "name": "get-user-presence"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/66825e03-7ef5-42da-9069-724602c31f6b/presence
```

---


#### <a name="response"></a>响应

<!-- {
  "blockType": "response",
  "name": "get-user-presence",
  "@odata.type": "microsoft.graph.presence",
  "truncated":"true"
}-->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1574

{
    "id": "66825e03-7ef5-42da-9069-724602c31f6b",
    "availability": "DoNotDisturb",
    "activity": "Presenting"
}
```

### <a name="example-3-get-the-presence-information-of-another-user"></a>示例3：获取其他用户的状态信息

下面的示例展示了如何获取其他用户的状态信息。 此操作需要已读。 All 权限。

#### <a name="request"></a>请求

<!-- {
  "blockType": "request",
  "name": "get-user-presences"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/communications/presences/dc74d9bb-6afe-433d-8eaa-e39d80d3a647
```

---


#### <a name="response"></a>响应

<!-- {
  "blockType": "response",
  "name": "get-user-presences",
  "@odata.type": "microsoft.graph.presence",
  "truncated":"true"
}-->

```http
HTTP/1.1 200 OK

{
    "value": [
        {
            "id": "dc74d9bb-6afe-433d-8eaa-e39d80d3a647",
            "availability": "Away",
            "activity": "BeRightBack"
        }
    ]
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get Presence",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->



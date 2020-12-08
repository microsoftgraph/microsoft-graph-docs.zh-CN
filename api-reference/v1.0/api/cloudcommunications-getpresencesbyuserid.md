---
title: 'cloudCommunications: getPresencesByUserId'
description: 获取多个用户的状态信息。
author: elvinyang-msft
localization_priority: Normal
doc_type: apiPageType
ms.prod: cloud-communications
ms.openlocfilehash: e06c1403b1d96a42a670f4c6d53c3bf5251d3b8a
ms.sourcegitcommit: e68fdfb1124d16265deb8df268d4185d9deacac6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/05/2020
ms.locfileid: "49581190"
---
# <a name="cloudcommunications-getpresencesbyuserid"></a>cloudCommunications: getPresencesByUserId

命名空间：microsoft.graph

获取多个用户的 [状态](../resources/presence.md) 信息。

## <a name="permissions"></a>权限
若要调用这些 Api，必须有以下权限之一。 若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型 | 权限（从最低特权到最高特权）                  |
| :-------------- | :----------------------------------------------------------- |
| 委派（工作或学校帐户）     | Presence.Read.All                         |
| 委派（个人 Microsoft 帐户） | 不支持。                         |
| 应用程序                            | 不支持。                                  |

> **注意：**
> * 每个 API 请求最多支持650个用户 Id。
> * 此 API 的最大请求速率为每个租户在30秒内的每个应用程序的 1500 API 请求数。

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
POST /communications/getPresencesByUserId
```

## <a name="request-headers"></a>请求标头
| 名称          | 说明               |
|:--------------|:--------------------------|
| Authorization | Bearer {token}。必需。 |
|Content-type | application/json. Required. |


## <a name="request-body"></a>请求正文

在请求正文中，提供具有以下参数的 JSON 对象。

| 参数      | 类型    |说明|
|:---------------|:--------|:----------|
|ids|String collection|用户对象 Id。|

## <a name="response"></a>响应

如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [状态](../resources/presence.md) 对象集合。


## <a name="examples"></a>示例

### <a name="request"></a>请求
以下示例显示了一个请求。

<!-- {
  "blockType": "request",
  "name": "get-presence-multiple-users"
}-->

```http
POST https://graph.microsoft.com/v1.0/communications/getPresencesByUserId
Content-Type: application/json

{
    "ids": ["fa8bf3dc-eca7-46b7-bad1-db199b62afc3", "66825e03-7ef5-42da-9069-724602c31f6b"]
}
```

---

### <a name="response"></a>响应
以下示例显示了相应的响应。

> **注意：** 为了提高可读性，响应对象可能会缩短。 所有属性都将通过实际调用返回。

<!-- {
  "blockType": "response",
  "name": "get-presence-multiple-users",
  "truncated": "true",
  "@odata.type": "microsoft.graph.presence"
}-->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1574
```
```json
{
    "value": [{
            "id": "fa8bf3dc-eca7-46b7-bad1-db199b62afc3",
            "availability": "Busy",
            "activity": "InAMeeting"
        },
        {
            "id": "66825e03-7ef5-42da-9069-724602c31f6b",
            "availability": "Away",
            "activity": "Away"
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List Presence Information",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->



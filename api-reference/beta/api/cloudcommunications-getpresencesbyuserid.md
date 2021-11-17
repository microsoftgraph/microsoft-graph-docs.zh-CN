---
title: cloudCommunications：getPresencesByUserId
description: 获取多个用户状态信息。
author: ananmishr
ms.localizationpriority: medium
doc_type: apiPageType
ms.prod: cloud-communications
ms.openlocfilehash: a0da5262370e9b4b7f588b5ed58bc026647f8646
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61030511"
---
# <a name="cloudcommunications-getpresencesbyuserid"></a>cloudCommunications：getPresencesByUserId

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

获取 [多个](../resources/presence.md) 用户状态信息。

## <a name="permissions"></a>Permissions
调用这些 API 需要以下权限之一。 若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型 | 权限（从最低特权到最高特权）                  |
| :-------------- | :----------------------------------------------------------- |
| 委派（工作或学校帐户）     | Presence.Read.All                         |
| 委派（个人 Microsoft 帐户） | 不支持。                         |
| 应用程序                            | 不支持。                                  |

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
|ids|String collection|用户对象 ID。|

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [presence](../resources/presence.md) 对象集合。


## <a name="examples"></a>示例

### <a name="request"></a>请求
以下示例显示了一个请求。


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-presence-multiple-users"
}-->

```http
POST https://graph.microsoft.com/beta/communications/getPresencesByUserId
Content-Type: application/json

{
  "ids": ["fa8bf3dc-eca7-46b7-bad1-db199b62afc3", "66825e03-7ef5-42da-9069-724602c31f6b"]
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-presence-multiple-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-presence-multiple-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-presence-multiple-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-presence-multiple-users-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-presence-multiple-users-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a>响应
以下示例显示了相应的响应。

> **注意：** 为了可读性，可能会缩短响应对象。 所有属性都将通过实际调用返回。

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

{
   "value":[
      {
         "id":"fa8bf3dc-eca7-46b7-bad1-db199b62afc3",
         "availability":"Busy",
         "activity":"InAMeeting",
         "outOfOfficeSettings":{
            "message":null,
            "isOutOfOffice":false
         }
      },
      {
         "id":"66825e03-7ef5-42da-9069-724602c31f6b",
         "availability":"Away",
         "activity":"Away",
         "outOfOfficeSettings":{
            "message":null,
            "isOutOfOffice":true
         }
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



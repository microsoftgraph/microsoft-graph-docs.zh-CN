---
author: daspek
ms.author: dspektor
title: 获取 websocket 终结点
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 4d4577ea69c65d6ce003af96b0d96b55fe178fb5
ms.sourcegitcommit: 3615f9475d57bfbb3a8c4402af863897f592dfbd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2019
ms.locfileid: "30791950"
---
# <a name="get-websocket-endpoint"></a>获取 websocket 终结点

允许您使用[socket.io][]接收[驱动器][]的近实时更改通知。
Socket.io 是适用于 JavaScript 的热门通知库, 可利用 websocket。 若要了解详细信息, 请参阅[socket.io](https://socket.io)。

[drive]: ../resources/drive.md
[socket.io]: https://socket.io/

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权）
|:---------------------------------------|:-------------------------------------------
| 委派（工作或学校帐户）     | 文件. 读取、文件读写、全部、读写全部。
| 委派（个人 Microsoft 帐户） | Read, 文件. readwrite, 全部文件。
| 应用程序                            | 不支持。

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
GET /me/drive/root/subscriptions/socketIo
GET /drives/{driveId}/root/subscriptions/socketIo
GET /groups/{groupId}/drive/root/subscriptions/socketIo
GET /sites/{siteId}/lists/{listId}/drive/root/subscriptions/socketIo
```

## <a name="example"></a>示例

### <a name="request"></a>请求

<!-- { "blockType": "request", "name": "drive_root_subscriptions_socketIo" } -->
```http
GET /me/drive/root/subscriptions/socketIo
```

### <a name="response"></a>响应

如果成功, 此方法在响应`200 OK`正文中返回响应代码和[订阅](../resources/subscription.md)对象。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.subscription"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "opaqueId-fj3hd7yf283jfk193726nvc2w3i2diemdu8",
  "notificationUrl": "https://f3hb0mpua.svc.ms/zbaehwg/callback?snthgk=1ff3-2345672zz831837523"
}
```

`notificationUrl`返回的是 socket.io 终结点 URL。
若要将它与 socket.io 客户端一起使用, 请拆分`/callback?`令牌上的字符串。
之前`/callback?`的字符串部分是 socket.io 终结点 URL, 后面的字符串部分是必须向库提供的不透明查询字符串。

下面的示例演示如何在 JavaScript 中`notificationUrl`将 with socket.io。

```javascript
// this is the notificationUrl returned from this API
var notificationUrl = "https://f3hb0mpua.svc.ms/zbaehwg/callback?snthgk=1ff3-2345672zz831837523";

// after the split, split[0] will be everything leading up to '/callback?' and split[1] will be everything after.
var split = notificationUrl.split("/callback?");

// 'io' comes from the socket.io client library
var socket = io(split[0], { query: split[1] });

// these examples log to the console.
// your app would provide its own callbacks
socket.on("connect", ()=>console.log("Connected!"));
socket.on("notification", (data)=>console.log("Notification!", data));
```

<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/driveItem-subscriptions-socketio.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

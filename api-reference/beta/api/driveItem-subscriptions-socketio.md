---
title: 获取 websocket 终结点
description: 不支持在生产应用程序中使用这些 API。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 5a608dc938fd0a57108ffd8361aed5de575ec92c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27915821"
---
# <a name="get-websocket-endpoint"></a>获取 websocket 终结点

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。
不支持在生产应用程序中使用这些 API。

允许您接收使用[socket.io][]的[驱动器][]的近乎实时的更改通知。
Socket.io 是 JavaScript 利用 Websocket 的常用通知库。 若要了解详细信息，请参阅[socket.io](https://socket.io)。

[驱动器]: ../resources/drive.md
[socket.io]: https://socket.io/

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权）
|:---------------------------------------|:-------------------------------------------
| 委派（工作或学校帐户）     | Files.Read，Files.ReadWrite，Files.ReadWrite.All Sites.ReadWrite.All
| 委派（个人 Microsoft 帐户） | Files.Read，Files.ReadWrite，Files.ReadWrite.All
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

如果成功，此方法返回`200 OK`响应代码和响应正文中的[订阅](../resources/subscription.md)对象。

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

`notificationUrl`返回是 socket.io 终结点 URL。
若要使用 socket.io 客户端中使用它，拆分字符串，在`/callback?`标记。
前的字符串的一部分`/callback?`是 socket.io 终结点 URL 并且后的字符串的一部分必须授予对库不透明的查询字符串。

下面的示例演示如何使用`notificationUrl`socket.io JavaScript 中使用。

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

<!-- {
  "type": "#page.annotation"
}-->

---
title: 获取 websocket 终结点
description: 不支持在生产应用程序中使用这些 API。
localization_priority: Normal
ms.openlocfilehash: a981a4d02d2e40fec0cb2bca397c7b7794d36867
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27859792"
---
# <a name="get-websocket-endpoint"></a><span data-ttu-id="0ed1d-103">获取 websocket 终结点</span><span class="sxs-lookup"><span data-stu-id="0ed1d-103">Get websocket endpoint</span></span>

> <span data-ttu-id="0ed1d-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="0ed1d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span>
<span data-ttu-id="0ed1d-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="0ed1d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0ed1d-106">允许您接收使用[socket.io][]的[驱动器][]的近乎实时的更改通知。</span><span class="sxs-lookup"><span data-stu-id="0ed1d-106">Allows you to receive near-real-time change notifications for a [drive][] using [socket.io][].</span></span>
<span data-ttu-id="0ed1d-107">Socket.io 是 JavaScript 利用 Websocket 的常用通知库。</span><span class="sxs-lookup"><span data-stu-id="0ed1d-107">Socket.io is a popular notifications library for JavaScript that utilizes WebSockets.</span></span> <span data-ttu-id="0ed1d-108">若要了解详细信息，请参阅[socket.io](https://socket.io)。</span><span class="sxs-lookup"><span data-stu-id="0ed1d-108">To learn more, see [socket.io](https://socket.io).</span></span>

[驱动器]: ../resources/drive.md
[drive]: ../resources/drive.md
[socket.io]: https://socket.io/

## <a name="permissions"></a><span data-ttu-id="0ed1d-111">权限</span><span class="sxs-lookup"><span data-stu-id="0ed1d-111">Permissions</span></span>

<span data-ttu-id="0ed1d-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0ed1d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0ed1d-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="0ed1d-114">Permission type</span></span>                        | <span data-ttu-id="0ed1d-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0ed1d-115">Permissions (from least to most privileged)</span></span>
|:---------------------------------------|:-------------------------------------------
| <span data-ttu-id="0ed1d-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0ed1d-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="0ed1d-117">Files.Read，Files.ReadWrite，Files.ReadWrite.All Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ed1d-117">Files.Read, Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>
| <span data-ttu-id="0ed1d-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0ed1d-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0ed1d-119">Files.Read，Files.ReadWrite，Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ed1d-119">Files.Read, Files.ReadWrite, Files.ReadWrite.All</span></span>
| <span data-ttu-id="0ed1d-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="0ed1d-120">Application</span></span>                            | <span data-ttu-id="0ed1d-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="0ed1d-121">Not supported.</span></span>

## <a name="http-request"></a><span data-ttu-id="0ed1d-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0ed1d-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/drive/root/subscriptions/socketIo
GET /drives/{driveId}/root/subscriptions/socketIo
GET /groups/{groupId}/drive/root/subscriptions/socketIo
GET /sites/{siteId}/lists/{listId}/drive/root/subscriptions/socketIo
```

## <a name="example"></a><span data-ttu-id="0ed1d-123">示例</span><span class="sxs-lookup"><span data-stu-id="0ed1d-123">Example</span></span>

### <a name="request"></a><span data-ttu-id="0ed1d-124">请求</span><span class="sxs-lookup"><span data-stu-id="0ed1d-124">Request</span></span>

<!-- { "blockType": "request", "name": "drive_root_subscriptions_socketIo" } -->
```http
GET /me/drive/root/subscriptions/socketIo
```

### <a name="response"></a><span data-ttu-id="0ed1d-125">响应</span><span class="sxs-lookup"><span data-stu-id="0ed1d-125">Response</span></span>

<span data-ttu-id="0ed1d-126">如果成功，此方法返回`200 OK`响应代码和响应正文中的[订阅](../resources/subscription.md)对象。</span><span class="sxs-lookup"><span data-stu-id="0ed1d-126">If successful, this method returns a `200 OK` response code and a [subscription](../resources/subscription.md) object in the response body.</span></span>

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

<span data-ttu-id="0ed1d-127">`notificationUrl`返回是 socket.io 终结点 URL。</span><span class="sxs-lookup"><span data-stu-id="0ed1d-127">The `notificationUrl` returned is a socket.io endpoint URL.</span></span>
<span data-ttu-id="0ed1d-128">若要使用 socket.io 客户端中使用它，拆分字符串，在`/callback?`标记。</span><span class="sxs-lookup"><span data-stu-id="0ed1d-128">To use it with a socket.io client, split the string on the `/callback?` token.</span></span>
<span data-ttu-id="0ed1d-129">前的字符串的一部分`/callback?`是 socket.io 终结点 URL 并且后的字符串的一部分必须授予对库不透明的查询字符串。</span><span class="sxs-lookup"><span data-stu-id="0ed1d-129">The part of the string before `/callback?` is the socket.io endpoint URL and the part of the string after is an opaque query string that must be given to the libary.</span></span>

<span data-ttu-id="0ed1d-130">下面的示例演示如何使用`notificationUrl`socket.io JavaScript 中使用。</span><span class="sxs-lookup"><span data-stu-id="0ed1d-130">The following example shows how to use the `notificationUrl` with socket.io in JavaScript.</span></span>

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

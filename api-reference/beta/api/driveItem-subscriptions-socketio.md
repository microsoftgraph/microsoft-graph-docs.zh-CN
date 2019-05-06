---
title: 获取 websocket 终结点
description: 不支持在生产应用程序中使用这些 API。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 03dbaf8522005c2bb0c038c8ba885becc41f72dc
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33591811"
---
# <a name="get-websocket-endpoint"></a><span data-ttu-id="77470-103">获取 websocket 终结点</span><span class="sxs-lookup"><span data-stu-id="77470-103">Get websocket endpoint</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="77470-104">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="77470-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="77470-105">允许您使用[socket.io][]接收[驱动器][]的近实时更改通知。</span><span class="sxs-lookup"><span data-stu-id="77470-105">Allows you to receive near-real-time change notifications for a [drive][] using [socket.io][].</span></span>
<span data-ttu-id="77470-106">Socket.io 是适用于 JavaScript 的热门通知库, 可利用 Websocket。</span><span class="sxs-lookup"><span data-stu-id="77470-106">Socket.io is a popular notifications library for JavaScript that utilizes WebSockets.</span></span> <span data-ttu-id="77470-107">若要了解详细信息, 请参阅[socket.io](https://socket.io)。</span><span class="sxs-lookup"><span data-stu-id="77470-107">To learn more, see [socket.io](https://socket.io).</span></span>

[drive]: ../resources/drive.md
[socket.io]: https://socket.io/

## <a name="permissions"></a><span data-ttu-id="77470-110">权限</span><span class="sxs-lookup"><span data-stu-id="77470-110">Permissions</span></span>

<span data-ttu-id="77470-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="77470-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="77470-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="77470-113">Permission type</span></span>                        | <span data-ttu-id="77470-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="77470-114">Permissions (from least to most privileged)</span></span>
|:---------------------------------------|:-------------------------------------------
| <span data-ttu-id="77470-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="77470-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="77470-116">文件。读取、文件读写、全部、读写全部。</span><span class="sxs-lookup"><span data-stu-id="77470-116">Files.Read, Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>
| <span data-ttu-id="77470-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="77470-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="77470-118">Read, 文件。 ReadWrite, 全部文件。</span><span class="sxs-lookup"><span data-stu-id="77470-118">Files.Read, Files.ReadWrite, Files.ReadWrite.All</span></span>
| <span data-ttu-id="77470-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="77470-119">Application</span></span>                            | <span data-ttu-id="77470-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="77470-120">Not supported.</span></span>

## <a name="http-request"></a><span data-ttu-id="77470-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="77470-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/drive/root/subscriptions/socketIo
GET /drives/{driveId}/root/subscriptions/socketIo
GET /groups/{groupId}/drive/root/subscriptions/socketIo
GET /sites/{siteId}/lists/{listId}/drive/root/subscriptions/socketIo
```

## <a name="example"></a><span data-ttu-id="77470-122">示例</span><span class="sxs-lookup"><span data-stu-id="77470-122">Example</span></span>

### <a name="request"></a><span data-ttu-id="77470-123">请求</span><span class="sxs-lookup"><span data-stu-id="77470-123">Request</span></span>

<!-- { "blockType": "request", "name": "drive_root_subscriptions_socketIo" } -->
```http
GET /me/drive/root/subscriptions/socketIo
```

### <a name="response"></a><span data-ttu-id="77470-124">响应</span><span class="sxs-lookup"><span data-stu-id="77470-124">Response</span></span>

<span data-ttu-id="77470-125">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[订阅](../resources/subscription.md)对象。</span><span class="sxs-lookup"><span data-stu-id="77470-125">If successful, this method returns a `200 OK` response code and a [subscription](../resources/subscription.md) object in the response body.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="77470-126">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="77470-126">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="77470-127">语言</span><span class="sxs-lookup"><span data-stu-id="77470-127">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/drive_root_subscriptions_socketIo-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="77470-128">Javascript</span><span class="sxs-lookup"><span data-stu-id="77470-128">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/drive_root_subscriptions_socketIo-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="77470-129">`notificationUrl`返回的是 socket.io 终结点 URL。</span><span class="sxs-lookup"><span data-stu-id="77470-129">The `notificationUrl` returned is a socket.io endpoint URL.</span></span>
<span data-ttu-id="77470-130">若要将它与 socket.io 客户端一起使用, 请拆分`/callback?`令牌上的字符串。</span><span class="sxs-lookup"><span data-stu-id="77470-130">To use it with a socket.io client, split the string on the `/callback?` token.</span></span>
<span data-ttu-id="77470-131">之前`/callback?`的字符串部分是 socket.io 终结点 URL, 后面的字符串部分是必须向库提供的不透明查询字符串。</span><span class="sxs-lookup"><span data-stu-id="77470-131">The part of the string before `/callback?` is the socket.io endpoint URL and the part of the string after is an opaque query string that must be given to the libary.</span></span>

<span data-ttu-id="77470-132">下面的示例演示如何在 JavaScript 中`notificationUrl`将 with socket.io。</span><span class="sxs-lookup"><span data-stu-id="77470-132">The following example shows how to use the `notificationUrl` with socket.io in JavaScript.</span></span>

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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/driveItem-subscriptions-socketio.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/driveItem-subscriptions-socketio.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->

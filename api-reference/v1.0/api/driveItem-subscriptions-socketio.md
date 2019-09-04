---
author: daspek
ms.author: dspektor
title: 获取 websocket 终结点
localization_priority: Normal
ms.prod: sharepoint
description: 允许您使用 socket.io 接收驱动器的近实时更改通知。
doc_type: apiPageType
ms.openlocfilehash: a53c172ca6c6347ec6051d62f2b8830dd1553392
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36726338"
---
# <a name="get-websocket-endpoint"></a><span data-ttu-id="0df26-103">获取 websocket 终结点</span><span class="sxs-lookup"><span data-stu-id="0df26-103">Get websocket endpoint</span></span>

<span data-ttu-id="0df26-104">允许您使用[socket.io][]接收[驱动器][]的近实时更改通知。</span><span class="sxs-lookup"><span data-stu-id="0df26-104">Allows you to receive near-real-time change notifications for a [drive][] using [socket.io][].</span></span>
<span data-ttu-id="0df26-105">Socket.io 是适用于 JavaScript 的热门通知库, 可利用 Websocket。</span><span class="sxs-lookup"><span data-stu-id="0df26-105">Socket.io is a popular notifications library for JavaScript that utilizes WebSockets.</span></span> <span data-ttu-id="0df26-106">若要了解详细信息, 请参阅[socket.io](https://socket.io)。</span><span class="sxs-lookup"><span data-stu-id="0df26-106">To learn more, see [socket.io](https://socket.io).</span></span>

[drive]: ../resources/drive.md
[socket.io]: https://socket.io/

## <a name="permissions"></a><span data-ttu-id="0df26-109">权限</span><span class="sxs-lookup"><span data-stu-id="0df26-109">Permissions</span></span>

<span data-ttu-id="0df26-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0df26-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0df26-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="0df26-112">Permission type</span></span>                        | <span data-ttu-id="0df26-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0df26-113">Permissions (from least to most privileged)</span></span>
|:---------------------------------------|:-------------------------------------------
| <span data-ttu-id="0df26-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0df26-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="0df26-115">文件. 读取、文件读写、全部、读写全部。</span><span class="sxs-lookup"><span data-stu-id="0df26-115">Files.Read, Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>
| <span data-ttu-id="0df26-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0df26-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0df26-117">Read, 文件. ReadWrite, 全部文件。</span><span class="sxs-lookup"><span data-stu-id="0df26-117">Files.Read, Files.ReadWrite, Files.ReadWrite.All</span></span>
| <span data-ttu-id="0df26-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="0df26-118">Application</span></span>                            | <span data-ttu-id="0df26-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="0df26-119">Not supported.</span></span>

## <a name="http-request"></a><span data-ttu-id="0df26-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0df26-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/drive/root/subscriptions/socketIo
GET /drives/{driveId}/root/subscriptions/socketIo
GET /groups/{groupId}/drive/root/subscriptions/socketIo
GET /sites/{siteId}/lists/{listId}/drive/root/subscriptions/socketIo
```

## <a name="example"></a><span data-ttu-id="0df26-121">示例</span><span class="sxs-lookup"><span data-stu-id="0df26-121">Example</span></span>

### <a name="request"></a><span data-ttu-id="0df26-122">请求</span><span class="sxs-lookup"><span data-stu-id="0df26-122">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="0df26-123">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="0df26-123">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "drive_root_subscriptions_socketIo" } -->
```msgraph-interactive
GET /me/drive/root/subscriptions/socketIo
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0df26-124">C#</span><span class="sxs-lookup"><span data-stu-id="0df26-124">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/drive-root-subscriptions-socketio-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0df26-125">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0df26-125">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/drive-root-subscriptions-socketio-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0df26-126">目标-C</span><span class="sxs-lookup"><span data-stu-id="0df26-126">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/drive-root-subscriptions-socketio-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="0df26-127">Java</span><span class="sxs-lookup"><span data-stu-id="0df26-127">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/drive-root-subscriptions-socketio-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0df26-128">响应</span><span class="sxs-lookup"><span data-stu-id="0df26-128">Response</span></span>

<span data-ttu-id="0df26-129">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[订阅](../resources/subscription.md)对象。</span><span class="sxs-lookup"><span data-stu-id="0df26-129">If successful, this method returns a `200 OK` response code and a [subscription](../resources/subscription.md) object in the response body.</span></span>

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

<span data-ttu-id="0df26-130">`notificationUrl`返回的是 socket.io 终结点 URL。</span><span class="sxs-lookup"><span data-stu-id="0df26-130">The `notificationUrl` returned is a socket.io endpoint URL.</span></span>
<span data-ttu-id="0df26-131">若要将它与 socket.io 客户端一起使用, 请拆分`/callback?`令牌上的字符串。</span><span class="sxs-lookup"><span data-stu-id="0df26-131">To use it with a socket.io client, split the string on the `/callback?` token.</span></span>
<span data-ttu-id="0df26-132">之前`/callback?`的字符串部分是 socket.io 终结点 URL, 后面的字符串部分是必须向库提供的不透明查询字符串。</span><span class="sxs-lookup"><span data-stu-id="0df26-132">The part of the string before `/callback?` is the socket.io endpoint URL and the part of the string after is an opaque query string that must be given to the libary.</span></span>

<span data-ttu-id="0df26-133">下面的示例演示如何在 JavaScript 中`notificationUrl`将 with socket.io。</span><span class="sxs-lookup"><span data-stu-id="0df26-133">The following example shows how to use the `notificationUrl` with socket.io in JavaScript.</span></span>

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
  ]
}-->

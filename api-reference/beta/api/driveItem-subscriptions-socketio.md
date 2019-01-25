---
title: 获取 websocket 终结点
description: 不支持在生产应用程序中使用这些 API。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 736684812d2cbc10affed82a3f946d75731f6768
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519792"
---
# <a name="get-websocket-endpoint"></a><span data-ttu-id="35cc5-103">获取 websocket 终结点</span><span class="sxs-lookup"><span data-stu-id="35cc5-103">Get websocket endpoint</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="35cc5-104">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="35cc5-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="35cc5-105">允许您接收使用[socket.io][]的[驱动器][]的近乎实时的更改通知。</span><span class="sxs-lookup"><span data-stu-id="35cc5-105">Allows you to receive near-real-time change notifications for a [drive][] using [socket.io][].</span></span>
<span data-ttu-id="35cc5-106">Socket.io 是 JavaScript 利用 Websocket 的常用通知库。</span><span class="sxs-lookup"><span data-stu-id="35cc5-106">Socket.io is a popular notifications library for JavaScript that utilizes WebSockets.</span></span> <span data-ttu-id="35cc5-107">若要了解详细信息，请参阅[socket.io](https://socket.io)。</span><span class="sxs-lookup"><span data-stu-id="35cc5-107">To learn more, see [socket.io](https://socket.io).</span></span>

[drive]: ../resources/drive.md
[socket.io]: https://socket.io/

## <a name="permissions"></a><span data-ttu-id="35cc5-110">权限</span><span class="sxs-lookup"><span data-stu-id="35cc5-110">Permissions</span></span>

<span data-ttu-id="35cc5-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="35cc5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="35cc5-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="35cc5-113">Permission type</span></span>                        | <span data-ttu-id="35cc5-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="35cc5-114">Permissions (from least to most privileged)</span></span>
|:---------------------------------------|:-------------------------------------------
| <span data-ttu-id="35cc5-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="35cc5-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="35cc5-116">Files.Read，Files.ReadWrite，Files.ReadWrite.All Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="35cc5-116">Files.Read, Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>
| <span data-ttu-id="35cc5-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="35cc5-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="35cc5-118">Files.Read，Files.ReadWrite，Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="35cc5-118">Files.Read, Files.ReadWrite, Files.ReadWrite.All</span></span>
| <span data-ttu-id="35cc5-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="35cc5-119">Application</span></span>                            | <span data-ttu-id="35cc5-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="35cc5-120">Not supported.</span></span>

## <a name="http-request"></a><span data-ttu-id="35cc5-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="35cc5-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/drive/root/subscriptions/socketIo
GET /drives/{driveId}/root/subscriptions/socketIo
GET /groups/{groupId}/drive/root/subscriptions/socketIo
GET /sites/{siteId}/lists/{listId}/drive/root/subscriptions/socketIo
```

## <a name="example"></a><span data-ttu-id="35cc5-122">示例</span><span class="sxs-lookup"><span data-stu-id="35cc5-122">Example</span></span>

### <a name="request"></a><span data-ttu-id="35cc5-123">请求</span><span class="sxs-lookup"><span data-stu-id="35cc5-123">Request</span></span>

<!-- { "blockType": "request", "name": "drive_root_subscriptions_socketIo" } -->
```http
GET /me/drive/root/subscriptions/socketIo
```

### <a name="response"></a><span data-ttu-id="35cc5-124">响应</span><span class="sxs-lookup"><span data-stu-id="35cc5-124">Response</span></span>

<span data-ttu-id="35cc5-125">如果成功，此方法返回`200 OK`响应代码和响应正文中的[订阅](../resources/subscription.md)对象。</span><span class="sxs-lookup"><span data-stu-id="35cc5-125">If successful, this method returns a `200 OK` response code and a [subscription](../resources/subscription.md) object in the response body.</span></span>

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

<span data-ttu-id="35cc5-126">`notificationUrl`返回是 socket.io 终结点 URL。</span><span class="sxs-lookup"><span data-stu-id="35cc5-126">The `notificationUrl` returned is a socket.io endpoint URL.</span></span>
<span data-ttu-id="35cc5-127">若要使用 socket.io 客户端中使用它，拆分字符串，在`/callback?`标记。</span><span class="sxs-lookup"><span data-stu-id="35cc5-127">To use it with a socket.io client, split the string on the `/callback?` token.</span></span>
<span data-ttu-id="35cc5-128">前的字符串的一部分`/callback?`是 socket.io 终结点 URL 并且后的字符串的一部分必须授予对库不透明的查询字符串。</span><span class="sxs-lookup"><span data-stu-id="35cc5-128">The part of the string before `/callback?` is the socket.io endpoint URL and the part of the string after is an opaque query string that must be given to the libary.</span></span>

<span data-ttu-id="35cc5-129">下面的示例演示如何使用`notificationUrl`socket.io JavaScript 中使用。</span><span class="sxs-lookup"><span data-stu-id="35cc5-129">The following example shows how to use the `notificationUrl` with socket.io in JavaScript.</span></span>

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

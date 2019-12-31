---
title: 呼叫：拒绝
description: 启用机器人以拒绝传入呼叫。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: e76dfb6a3d04be14347616bf5f52f7dc77659be2
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/31/2019
ms.locfileid: "40912809"
---
# <a name="call-reject"></a><span data-ttu-id="b829c-103">呼叫：拒绝</span><span class="sxs-lookup"><span data-stu-id="b829c-103">call: reject</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b829c-104">启用机器人以拒绝传入呼叫。</span><span class="sxs-lookup"><span data-stu-id="b829c-104">Enable a bot to reject an incoming call.</span></span> <span data-ttu-id="b829c-105">传入呼叫请求可以是来自组呼叫或对等呼叫中参与者的邀请。</span><span class="sxs-lookup"><span data-stu-id="b829c-105">The incoming call request can be an invite from a participant in a group call or a peer-to-peer call.</span></span> <span data-ttu-id="b829c-106">如果收到某个组呼叫邀请，则通知将包含**chatInfo**和**meetingInfo**参数。</span><span class="sxs-lookup"><span data-stu-id="b829c-106">If an invite to a group call is received, the notification will contain the **chatInfo** and **meetingInfo** parameters.</span></span>

<span data-ttu-id="b829c-107">在呼叫超时之前，机器人应应答或拒绝呼叫。当前超时值为15秒。</span><span class="sxs-lookup"><span data-stu-id="b829c-107">The bot is expected to answer or reject the call before the call times out. The current timeout value is 15 seconds.</span></span>

<span data-ttu-id="b829c-108">此 API 不会结束已应答的现有呼叫。</span><span class="sxs-lookup"><span data-stu-id="b829c-108">This API does not end existing calls that have already been answered.</span></span> <span data-ttu-id="b829c-109">使用[删除呼叫](../api/call-delete.md)结束呼叫。</span><span class="sxs-lookup"><span data-stu-id="b829c-109">Use [delete call](../api/call-delete.md) to end a call.</span></span>

## <a name="permissions"></a><span data-ttu-id="b829c-110">权限</span><span class="sxs-lookup"><span data-stu-id="b829c-110">Permissions</span></span>
<span data-ttu-id="b829c-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b829c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b829c-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="b829c-113">Permission type</span></span> | <span data-ttu-id="b829c-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b829c-114">Permissions (from least to most privileged)</span></span>                |
| :-------------- | :--------------------------------------------------------- |
| <span data-ttu-id="b829c-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b829c-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="b829c-116">不支持</span><span class="sxs-lookup"><span data-stu-id="b829c-116">Not Supported</span></span>                       |
| <span data-ttu-id="b829c-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b829c-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b829c-118">不支持</span><span class="sxs-lookup"><span data-stu-id="b829c-118">Not Supported</span></span>                       |
| <span data-ttu-id="b829c-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="b829c-119">Application</span></span>     | <span data-ttu-id="b829c-120">无</span><span class="sxs-lookup"><span data-stu-id="b829c-120">None</span></span>                                                       |

## <a name="http-request"></a><span data-ttu-id="b829c-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b829c-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/reject
POST /communications/calls/{id}/reject
```
> <span data-ttu-id="b829c-122">**注意：**`/app` 路径已弃用。</span><span class="sxs-lookup"><span data-stu-id="b829c-122">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="b829c-123">今后将使用 `/communications` 路径。</span><span class="sxs-lookup"><span data-stu-id="b829c-123">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b829c-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="b829c-124">Request headers</span></span>
| <span data-ttu-id="b829c-125">名称</span><span class="sxs-lookup"><span data-stu-id="b829c-125">Name</span></span>          | <span data-ttu-id="b829c-126">说明</span><span class="sxs-lookup"><span data-stu-id="b829c-126">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="b829c-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="b829c-127">Authorization</span></span> | <span data-ttu-id="b829c-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b829c-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b829c-130">Content-type</span><span class="sxs-lookup"><span data-stu-id="b829c-130">Content-type</span></span>  | <span data-ttu-id="b829c-p106">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="b829c-p106">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b829c-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="b829c-133">Request body</span></span>
<span data-ttu-id="b829c-134">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="b829c-134">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b829c-135">参数</span><span class="sxs-lookup"><span data-stu-id="b829c-135">Parameter</span></span>      | <span data-ttu-id="b829c-136">类型</span><span class="sxs-lookup"><span data-stu-id="b829c-136">Type</span></span>    |<span data-ttu-id="b829c-137">说明</span><span class="sxs-lookup"><span data-stu-id="b829c-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b829c-138">reason</span><span class="sxs-lookup"><span data-stu-id="b829c-138">reason</span></span>|<span data-ttu-id="b829c-139">String</span><span class="sxs-lookup"><span data-stu-id="b829c-139">String</span></span>|<span data-ttu-id="b829c-140">拒绝原因。</span><span class="sxs-lookup"><span data-stu-id="b829c-140">The rejection reason.</span></span> <span data-ttu-id="b829c-141">可能的值`None`为`Busy`和`Forbidden`</span><span class="sxs-lookup"><span data-stu-id="b829c-141">Possible values are `None`, `Busy` and `Forbidden`</span></span> |
|<span data-ttu-id="b829c-142">callbackUri</span><span class="sxs-lookup"><span data-stu-id="b829c-142">callbackUri</span></span>|<span data-ttu-id="b829c-143">String</span><span class="sxs-lookup"><span data-stu-id="b829c-143">String</span></span>|<span data-ttu-id="b829c-144">这将允许 bot 为当前呼叫提供特定的回调 URI，以接收后续通知。</span><span class="sxs-lookup"><span data-stu-id="b829c-144">This allows bots to provide a specific callback URI for the current call to receive later notifications.</span></span> <span data-ttu-id="b829c-145">如果尚未设置此属性，则将改为使用 bot 的全局回调 URI。</span><span class="sxs-lookup"><span data-stu-id="b829c-145">If this property has not been set, the bot's global callback URI will be used instead.</span></span> <span data-ttu-id="b829c-146">这必须是`https`。</span><span class="sxs-lookup"><span data-stu-id="b829c-146">This must be `https`.</span></span>|

## <a name="response"></a><span data-ttu-id="b829c-147">响应</span><span class="sxs-lookup"><span data-stu-id="b829c-147">Response</span></span>
<span data-ttu-id="b829c-p109">如果成功，此方法返回 `202 Accepted` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="b829c-p109">If successful, this method returns a `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b829c-150">示例</span><span class="sxs-lookup"><span data-stu-id="b829c-150">Examples</span></span>
<span data-ttu-id="b829c-151">下面的示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="b829c-151">The following examples show how to call this API.</span></span>

### <a name="example-1-reject-an-incoming-call-with-busy-reason"></a><span data-ttu-id="b829c-152">示例1：拒绝传入呼叫并使用 ' 占线 ' 原因</span><span class="sxs-lookup"><span data-stu-id="b829c-152">Example 1: Reject an incoming call with 'Busy' reason</span></span>
#### <a name="request"></a><span data-ttu-id="b829c-153">请求</span><span class="sxs-lookup"><span data-stu-id="b829c-153">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b829c-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="b829c-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-reject"
}-->
```http
POST https://graph.microsoft.com/beta/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/reject
Content-Type: application/json
Content-Length: 24

{
  "reason": "busy"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b829c-155">C#</span><span class="sxs-lookup"><span data-stu-id="b829c-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-reject-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)] 

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b829c-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b829c-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-reject-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)] 

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b829c-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b829c-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-reject-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)] 

--- 


##### <a name="response"></a><span data-ttu-id="b829c-158">响应</span><span class="sxs-lookup"><span data-stu-id="b829c-158">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```

### <a name="example-2-reject-an-incoming-call-with-none-reason"></a><span data-ttu-id="b829c-159">示例2：拒绝具有 "无" 原因的传入呼叫</span><span class="sxs-lookup"><span data-stu-id="b829c-159">Example 2: Reject an incoming call with 'None' reason</span></span>

##### <a name="notification---incoming"></a><span data-ttu-id="b829c-160">通知传入</span><span class="sxs-lookup"><span data-stu-id="b829c-160">Notification - incoming</span></span>

```http
POST https://bot.contoso.com/api/call
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "@odata.type": "#microsoft.graph.commsNotifications",
  "value": [
    {
      "@odata.type": "#microsoft.graph.commsNotification",
      "changeType": "created",
      "resourceUrl": "/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "@odata.id": "/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896",
        "state": "incoming",
        "direction": "incoming",
        "source": {
          "identity": {
            "user": {
              "displayName": "John",
              "id": "112f7296-5fa4-42ca-bae8-6a692b15d4b8"
            }
          },
          "region": "westus",
          "languageId": "en-US"
        },
        "targets": [
          {
            "identity": {
              "application": {
                "displayName": "Calling Bot",
                "id": "2891555a-92ff-42e6-80fa-6e1300c6b5c6"
              }
            },
            "region": "westus",
            "languageId": "en-US"
          }
        ],
        "requestedModalities": [ "audio", "video" ]
      }
    }
  ]
}
```

##### <a name="request"></a><span data-ttu-id="b829c-161">请求</span><span class="sxs-lookup"><span data-stu-id="b829c-161">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="b829c-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="b829c-162">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-reject-none-reason"
}-->
```http
POST https://graph.microsoft.com/beta/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/reject
Content-Type: application/json
Content-Length: 24

{
  "reason": "none"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b829c-163">C#</span><span class="sxs-lookup"><span data-stu-id="b829c-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-reject-none-reason-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b829c-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b829c-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-reject-none-reason-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b829c-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b829c-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-reject-none-reason-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="b829c-166">响应</span><span class="sxs-lookup"><span data-stu-id="b829c-166">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---deleted"></a><span data-ttu-id="b829c-167">通知-已删除</span><span class="sxs-lookup"><span data-stu-id="b829c-167">Notification - deleted</span></span>

```http
POST https://bot.contoso.com/api/calls
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "@odata.type": "#microsoft.graph.commsNotifications",
  "value": [
    {
      "@odata.type": "#microsoft.graph.commsNotification",
      "changeType": "deleted",
      "resourceUrl": "/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "@odata.id": "/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896"
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
  "description": "call: reject",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

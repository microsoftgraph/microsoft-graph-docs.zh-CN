---
title: call： reject
description: 使机器人能够拒绝传入呼叫。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 1355a826ab3bfaeea3392e20a6e40c71a279ca58
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787490"
---
# <a name="call-reject"></a><span data-ttu-id="704ab-103">call： reject</span><span class="sxs-lookup"><span data-stu-id="704ab-103">call: reject</span></span>

<span data-ttu-id="704ab-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="704ab-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="704ab-105">使机器人能够拒绝传入呼叫。</span><span class="sxs-lookup"><span data-stu-id="704ab-105">Enable a bot to reject an incoming call.</span></span> <span data-ttu-id="704ab-106">传入呼叫请求可以是来自组呼叫参与者的邀请或对等呼叫。</span><span class="sxs-lookup"><span data-stu-id="704ab-106">The incoming call request can be an invite from a participant in a group call or a peer-to-peer call.</span></span> <span data-ttu-id="704ab-107">如果收到组呼叫邀请，通知将包含 **chatInfo** 和 **meetingInfo** 参数。</span><span class="sxs-lookup"><span data-stu-id="704ab-107">If an invite to a group call is received, the notification will contain the **chatInfo** and **meetingInfo** parameters.</span></span>

<span data-ttu-id="704ab-108">机器人预期在呼叫退出之前应答或拒绝呼叫。当前超时值为 15 秒。</span><span class="sxs-lookup"><span data-stu-id="704ab-108">The bot is expected to answer or reject the call before the call times out. The current timeout value is 15 seconds.</span></span>

<span data-ttu-id="704ab-109">此 API 不会结束已应答的现有调用。</span><span class="sxs-lookup"><span data-stu-id="704ab-109">This API does not end existing calls that have already been answered.</span></span> <span data-ttu-id="704ab-110">使用 [删除呼叫](../api/call-delete.md) 结束呼叫。</span><span class="sxs-lookup"><span data-stu-id="704ab-110">Use [delete call](../api/call-delete.md) to end a call.</span></span>

## <a name="permissions"></a><span data-ttu-id="704ab-111">权限</span><span class="sxs-lookup"><span data-stu-id="704ab-111">Permissions</span></span>
<span data-ttu-id="704ab-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="704ab-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="704ab-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="704ab-114">Permission type</span></span> | <span data-ttu-id="704ab-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="704ab-115">Permissions (from least to most privileged)</span></span>                |
| :-------------- | :--------------------------------------------------------- |
| <span data-ttu-id="704ab-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="704ab-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="704ab-117">不支持</span><span class="sxs-lookup"><span data-stu-id="704ab-117">Not Supported</span></span>                       |
| <span data-ttu-id="704ab-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="704ab-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="704ab-119">不支持</span><span class="sxs-lookup"><span data-stu-id="704ab-119">Not Supported</span></span>                       |
| <span data-ttu-id="704ab-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="704ab-120">Application</span></span>     | <span data-ttu-id="704ab-121">无</span><span class="sxs-lookup"><span data-stu-id="704ab-121">None</span></span>                                                       |

## <a name="http-request"></a><span data-ttu-id="704ab-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="704ab-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /communications/calls/{id}/reject
```

## <a name="request-headers"></a><span data-ttu-id="704ab-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="704ab-123">Request headers</span></span>
| <span data-ttu-id="704ab-124">名称</span><span class="sxs-lookup"><span data-stu-id="704ab-124">Name</span></span>          | <span data-ttu-id="704ab-125">说明</span><span class="sxs-lookup"><span data-stu-id="704ab-125">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="704ab-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="704ab-126">Authorization</span></span> | <span data-ttu-id="704ab-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="704ab-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="704ab-129">Content-type</span><span class="sxs-lookup"><span data-stu-id="704ab-129">Content-type</span></span>  | <span data-ttu-id="704ab-p105">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="704ab-p105">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="704ab-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="704ab-132">Request body</span></span>
<span data-ttu-id="704ab-133">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="704ab-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="704ab-134">参数</span><span class="sxs-lookup"><span data-stu-id="704ab-134">Parameter</span></span>      | <span data-ttu-id="704ab-135">类型</span><span class="sxs-lookup"><span data-stu-id="704ab-135">Type</span></span>    |<span data-ttu-id="704ab-136">说明</span><span class="sxs-lookup"><span data-stu-id="704ab-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="704ab-137">reason</span><span class="sxs-lookup"><span data-stu-id="704ab-137">reason</span></span>|<span data-ttu-id="704ab-138">String</span><span class="sxs-lookup"><span data-stu-id="704ab-138">String</span></span>|<span data-ttu-id="704ab-139">拒绝原因。</span><span class="sxs-lookup"><span data-stu-id="704ab-139">The rejection reason.</span></span> <span data-ttu-id="704ab-140">可能的值是 `None` 、 `Busy` 和 `Forbidden`</span><span class="sxs-lookup"><span data-stu-id="704ab-140">Possible values are `None`, `Busy` and `Forbidden`</span></span> |
|<span data-ttu-id="704ab-141">callbackUri</span><span class="sxs-lookup"><span data-stu-id="704ab-141">callbackUri</span></span>|<span data-ttu-id="704ab-142">String</span><span class="sxs-lookup"><span data-stu-id="704ab-142">String</span></span>|<span data-ttu-id="704ab-143">这允许机器人为当前呼叫提供特定的回调 URI，以接收以后的通知。</span><span class="sxs-lookup"><span data-stu-id="704ab-143">This allows bots to provide a specific callback URI for the current call to receive later notifications.</span></span> <span data-ttu-id="704ab-144">如果尚未设置此属性，将改为使用自动程序全局回调 URI。</span><span class="sxs-lookup"><span data-stu-id="704ab-144">If this property has not been set, the bot's global callback URI will be used instead.</span></span> <span data-ttu-id="704ab-145">这必须是 `https` 。</span><span class="sxs-lookup"><span data-stu-id="704ab-145">This must be `https`.</span></span>|

## <a name="response"></a><span data-ttu-id="704ab-146">响应</span><span class="sxs-lookup"><span data-stu-id="704ab-146">Response</span></span>
<span data-ttu-id="704ab-p108">如果成功，此方法返回 `202 Accepted` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="704ab-p108">If successful, this method returns a `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="704ab-149">示例</span><span class="sxs-lookup"><span data-stu-id="704ab-149">Examples</span></span>
<span data-ttu-id="704ab-150">以下示例显示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="704ab-150">The following examples show how to call this API.</span></span>

### <a name="example-1-reject-an-incoming-call-with-busy-reason"></a><span data-ttu-id="704ab-151">示例 1：拒绝具有"Busy"原因的传入呼叫</span><span class="sxs-lookup"><span data-stu-id="704ab-151">Example 1: Reject an incoming call with 'Busy' reason</span></span>
#### <a name="request"></a><span data-ttu-id="704ab-152">请求</span><span class="sxs-lookup"><span data-stu-id="704ab-152">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="704ab-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="704ab-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-reject"
}-->
```http
POST https://graph.microsoft.com/v1.0/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/reject
Content-Type: application/json
Content-Length: 24

{
  "reason": "busy"
}
```
# <a name="c"></a>[<span data-ttu-id="704ab-154">C#</span><span class="sxs-lookup"><span data-stu-id="704ab-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-reject-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)] 

# <a name="javascript"></a>[<span data-ttu-id="704ab-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="704ab-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-reject-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)] 

# <a name="objective-c"></a>[<span data-ttu-id="704ab-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="704ab-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-reject-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)] 

# <a name="java"></a>[<span data-ttu-id="704ab-157">Java</span><span class="sxs-lookup"><span data-stu-id="704ab-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/call-reject-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

--- 


##### <a name="response"></a><span data-ttu-id="704ab-158">响应</span><span class="sxs-lookup"><span data-stu-id="704ab-158">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

### <a name="example-2-reject-an-incoming-call-with-none-reason"></a><span data-ttu-id="704ab-159">示例 2：拒绝具有"无"原因的传入呼叫</span><span class="sxs-lookup"><span data-stu-id="704ab-159">Example 2: Reject an incoming call with 'None' reason</span></span>

##### <a name="notification---incoming"></a><span data-ttu-id="704ab-160">通知 - 传入</span><span class="sxs-lookup"><span data-stu-id="704ab-160">Notification - incoming</span></span>

```http
POST https://bot.contoso.com/api/call
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "name": "call-reject-none",
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
            }
          }
        ],
        "requestedModalities": [ "audio", "video" ]
      }
    }
  ]
}
```

##### <a name="request"></a><span data-ttu-id="704ab-161">请求</span><span class="sxs-lookup"><span data-stu-id="704ab-161">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="704ab-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="704ab-162">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-reject-none-reason"
}-->
```http
POST https://graph.microsoft.com/v1.0/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/reject
Content-Type: application/json
Content-Length: 24

{
  "reason": "none"
}
```
# <a name="c"></a>[<span data-ttu-id="704ab-163">C#</span><span class="sxs-lookup"><span data-stu-id="704ab-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-reject-none-reason-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="704ab-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="704ab-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-reject-none-reason-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="704ab-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="704ab-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-reject-none-reason-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="704ab-166">Java</span><span class="sxs-lookup"><span data-stu-id="704ab-166">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/call-reject-none-reason-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="704ab-167">响应</span><span class="sxs-lookup"><span data-stu-id="704ab-167">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---deleted"></a><span data-ttu-id="704ab-168">通知 - 已删除</span><span class="sxs-lookup"><span data-stu-id="704ab-168">Notification - deleted</span></span>

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


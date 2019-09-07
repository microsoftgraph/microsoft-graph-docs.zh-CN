---
title: 呼叫：拒绝
description: 拒绝传入呼叫。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 0134b03e27deeaf24eba3deb9c58b56865ab72d8
ms.sourcegitcommit: c68a83d28fa4bfca6e0618467934813a9ae17b12
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/07/2019
ms.locfileid: "36792280"
---
# <a name="call-reject"></a><span data-ttu-id="d315c-103">呼叫：拒绝</span><span class="sxs-lookup"><span data-stu-id="d315c-103">call: reject</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d315c-104">启用机器人以拒绝传入[呼叫](../resources/call.md)。</span><span class="sxs-lookup"><span data-stu-id="d315c-104">Enables the bot to reject an incoming [call](../resources/call.md).</span></span> <span data-ttu-id="d315c-105">传入呼叫请求可以是邀请参加会议或对等呼叫。</span><span class="sxs-lookup"><span data-stu-id="d315c-105">The incoming call request can be an invite to a meeting or a peer to peer call.</span></span> <span data-ttu-id="d315c-106">传入呼叫请求在15秒后超时。</span><span class="sxs-lookup"><span data-stu-id="d315c-106">The incoming call request times out after 15 seconds.</span></span> <span data-ttu-id="d315c-107">如果在此期间未发送任何响应，则会自动拒绝该呼叫。</span><span class="sxs-lookup"><span data-stu-id="d315c-107">If no response is sent during this time, the call is automatically rejected.</span></span>

<span data-ttu-id="d315c-108">在 Azure 门户中使用有效的回调 URL 注册 bot 后，传入呼叫将作为[commsNotification](../resources/commsnotification.md)传递，其`changeType`设置为`created`。</span><span class="sxs-lookup"><span data-stu-id="d315c-108">Once the bot is registered with a valid callback URL in the Azure portal, the incoming call is delivered as a [commsNotification](../resources/commsnotification.md) with `changeType` set to `created`.</span></span> <span data-ttu-id="d315c-109">应将机器人`Answer`或`Reject`呼叫超时之前的时间。</span><span class="sxs-lookup"><span data-stu-id="d315c-109">The bot is expected to `Answer` or `Reject` the call before it times out.</span></span>

> <span data-ttu-id="d315c-110">**注意：** 此 API 仅用于拒绝传入的呼叫。</span><span class="sxs-lookup"><span data-stu-id="d315c-110">**Note:** This API is only used to reject incoming calls.</span></span> <span data-ttu-id="d315c-111">若要终止现有呼叫，应改为使用 "[删除呼叫](../api/call-delete.md)"。</span><span class="sxs-lookup"><span data-stu-id="d315c-111">To terminate existing calls, [Delete Call](../api/call-delete.md) should be used instead.</span></span>

## <a name="permissions"></a><span data-ttu-id="d315c-112">权限</span><span class="sxs-lookup"><span data-stu-id="d315c-112">Permissions</span></span>
<span data-ttu-id="d315c-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d315c-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d315c-115">权限类型</span><span class="sxs-lookup"><span data-stu-id="d315c-115">Permission type</span></span> | <span data-ttu-id="d315c-116">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d315c-116">Permissions (from least to most privileged)</span></span>                |
| :-------------- | :--------------------------------------------------------- |
| <span data-ttu-id="d315c-117">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d315c-117">Delegated (work or school account)</span></span>     | <span data-ttu-id="d315c-118">不支持</span><span class="sxs-lookup"><span data-stu-id="d315c-118">Not Supported</span></span>                       |
| <span data-ttu-id="d315c-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d315c-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d315c-120">不支持</span><span class="sxs-lookup"><span data-stu-id="d315c-120">Not Supported</span></span>                       |
| <span data-ttu-id="d315c-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="d315c-121">Application</span></span>     | <span data-ttu-id="d315c-122">无</span><span class="sxs-lookup"><span data-stu-id="d315c-122">None</span></span>                                                       |

## <a name="http-request"></a><span data-ttu-id="d315c-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d315c-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/reject
```

## <a name="request-headers"></a><span data-ttu-id="d315c-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="d315c-124">Request headers</span></span>
| <span data-ttu-id="d315c-125">名称</span><span class="sxs-lookup"><span data-stu-id="d315c-125">Name</span></span>          | <span data-ttu-id="d315c-126">说明</span><span class="sxs-lookup"><span data-stu-id="d315c-126">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="d315c-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="d315c-127">Authorization</span></span> | <span data-ttu-id="d315c-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d315c-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d315c-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="d315c-130">Request body</span></span>
<span data-ttu-id="d315c-131">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="d315c-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="d315c-132">参数</span><span class="sxs-lookup"><span data-stu-id="d315c-132">Parameter</span></span>      | <span data-ttu-id="d315c-133">类型</span><span class="sxs-lookup"><span data-stu-id="d315c-133">Type</span></span>    |<span data-ttu-id="d315c-134">说明</span><span class="sxs-lookup"><span data-stu-id="d315c-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d315c-135">在于</span><span class="sxs-lookup"><span data-stu-id="d315c-135">reason</span></span>|<span data-ttu-id="d315c-136">String</span><span class="sxs-lookup"><span data-stu-id="d315c-136">String</span></span>|<span data-ttu-id="d315c-137">拒绝原因。</span><span class="sxs-lookup"><span data-stu-id="d315c-137">The rejection reason.</span></span> <span data-ttu-id="d315c-138">可能的值`None`为`Busy`和`Forbidden`</span><span class="sxs-lookup"><span data-stu-id="d315c-138">Possible values are `None`, `Busy` and `Forbidden`</span></span> |
|<span data-ttu-id="d315c-139">callbackUri</span><span class="sxs-lookup"><span data-stu-id="d315c-139">callbackUri</span></span>|<span data-ttu-id="d315c-140">String</span><span class="sxs-lookup"><span data-stu-id="d315c-140">String</span></span>|<span data-ttu-id="d315c-141">允许 bot 提供特定的回调 URI，将在其中发布拒绝操作的结果。</span><span class="sxs-lookup"><span data-stu-id="d315c-141">Allows bots to provide a specific callback URI where the result of the Reject action will be posted.</span></span> <span data-ttu-id="d315c-142">这允许将结果发送到触发拒绝操作的相同特定 bot 实例。</span><span class="sxs-lookup"><span data-stu-id="d315c-142">This allows sending the result to the same specific bot instance that triggered the Reject action.</span></span> <span data-ttu-id="d315c-143">如果未提供，则将使用 bot 的全局回调 URI。</span><span class="sxs-lookup"><span data-stu-id="d315c-143">If none is provided, the bot's global callback URI will be used.</span></span>|

## <a name="response"></a><span data-ttu-id="d315c-144">响应</span><span class="sxs-lookup"><span data-stu-id="d315c-144">Response</span></span>
<span data-ttu-id="d315c-p108">如果成功，此方法返回 `202 Accepted` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="d315c-p108">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d315c-147">示例</span><span class="sxs-lookup"><span data-stu-id="d315c-147">Examples</span></span>
<span data-ttu-id="d315c-148">下面的示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="d315c-148">The following examples shows how to call this API.</span></span>

#### <a name="request"></a><span data-ttu-id="d315c-149">请求</span><span class="sxs-lookup"><span data-stu-id="d315c-149">Request</span></span>
<span data-ttu-id="d315c-150">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="d315c-150">The following example shows the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="d315c-151">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="d315c-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-reject"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/57dab8b1-894c-409a-b240-bd8beae78896/reject
Content-Type: application/json
Content-Length: 24

{
  "reason": "busy"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d315c-152">C#</span><span class="sxs-lookup"><span data-stu-id="d315c-152">C#</span></span>](#tab/csharp) 
[!INCLUDE [sample-code](../includes/snippets/csharp/call-reject-csharp-snippets.md)]    
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)] 

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d315c-153">Javascript</span><span class="sxs-lookup"><span data-stu-id="d315c-153">Javascript</span></span>](#tab/javascript) 
[!INCLUDE [sample-code](../includes/snippets/javascript/call-reject-javascript-snippets.md)]    
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)] 

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d315c-154">目标-C</span><span class="sxs-lookup"><span data-stu-id="d315c-154">Objective-C</span></span>](#tab/objc)  
[!INCLUDE [sample-code](../includes/snippets/objc/call-reject-objc-snippets.md)]    
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)] 

--- 


##### <a name="response"></a><span data-ttu-id="d315c-155">响应</span><span class="sxs-lookup"><span data-stu-id="d315c-155">Response</span></span>
<span data-ttu-id="d315c-156">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="d315c-156">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```

### <a name="reject-an-incoming-call-with-none-reason"></a><span data-ttu-id="d315c-157">拒绝具有 "无" 原因的传入呼叫</span><span class="sxs-lookup"><span data-stu-id="d315c-157">Reject an incoming call with 'None' reason</span></span>

##### <a name="notification---incoming"></a><span data-ttu-id="d315c-158">通知传入</span><span class="sxs-lookup"><span data-stu-id="d315c-158">Notification - incoming</span></span>

```http
POST https://bot.contoso.com/api/call
Authorization: Bearer <TOKEN>
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
      "resource": "/app/calls/57dab8b1-894c-409a-b240-bd8beae78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "@odata.id": "/app/calls/57dab8b1-894c-409a-b240-bd8beae78896",
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

##### <a name="request"></a><span data-ttu-id="d315c-159">请求</span><span class="sxs-lookup"><span data-stu-id="d315c-159">Request</span></span>
<span data-ttu-id="d315c-160">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="d315c-160">The following example shows the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "call-reject"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/57dab8b1-894c-409a-b240-bd8beae78896/reject
Content-Type: application/json
Content-Length: 24

{
  "reason": "none"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d315c-161">C#</span><span class="sxs-lookup"><span data-stu-id="d315c-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-reject-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d315c-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d315c-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-reject-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d315c-163">目标-C</span><span class="sxs-lookup"><span data-stu-id="d315c-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-reject-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d315c-164">响应</span><span class="sxs-lookup"><span data-stu-id="d315c-164">Response</span></span>

```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---deleted"></a><span data-ttu-id="d315c-165">通知-已删除</span><span class="sxs-lookup"><span data-stu-id="d315c-165">Notification - deleted</span></span>

```http
POST https://bot.contoso.com/api/calls
Authorization: Bearer <TOKEN>
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
      "resource": "/app/calls/57dab8b1-894c-409a-b240-bd8beae78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "@odata.id": "/app/calls/57dab8b1-894c-409a-b240-bd8beae78896"
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

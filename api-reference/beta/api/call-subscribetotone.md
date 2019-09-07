---
title: 调用： subscribeToTone
description: 订阅 DTMF （双音多频信号）。 这样，您就可以在用户按 "Dialpad" 上的键时收到通知。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: a81c6440d320f74411f1ffefb94a6fea14945b14
ms.sourcegitcommit: c68a83d28fa4bfca6e0618467934813a9ae17b12
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/07/2019
ms.locfileid: "36792525"
---
# <a name="call-subscribetotone"></a><span data-ttu-id="1579e-104">调用： subscribeToTone</span><span class="sxs-lookup"><span data-stu-id="1579e-104">call: subscribeToTone</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1579e-105">订阅 DTMF （双音多频信号）。</span><span class="sxs-lookup"><span data-stu-id="1579e-105">Subscribe to DTMF (dual-tone multi-frequency signaling).</span></span> <span data-ttu-id="1579e-106">这样，您就可以在用户按 "Dialpad" 上的键时收到通知。</span><span class="sxs-lookup"><span data-stu-id="1579e-106">This allows you to be notified when the user presses keys on a "Dialpad".</span></span>

> [!Note]
> <span data-ttu-id="1579e-107">仅使用[serviceHostedMediaConfig](../resources/servicehostedmediaconfig.md)启动的[调用](../resources/call.md)支持**subscribeToTone**操作。</span><span class="sxs-lookup"><span data-stu-id="1579e-107">The **subscribeToTone** action is supported only for [calls](../resources/call.md) that are initiated with [serviceHostedMediaConfig](../resources/servicehostedmediaconfig.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="1579e-108">权限</span><span class="sxs-lookup"><span data-stu-id="1579e-108">Permissions</span></span>
<span data-ttu-id="1579e-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1579e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1579e-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="1579e-111">Permission type</span></span> | <span data-ttu-id="1579e-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1579e-112">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="1579e-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1579e-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="1579e-114">不支持</span><span class="sxs-lookup"><span data-stu-id="1579e-114">Not Supported</span></span>        |
| <span data-ttu-id="1579e-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1579e-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1579e-116">不支持</span><span class="sxs-lookup"><span data-stu-id="1579e-116">Not Supported</span></span>        |
| <span data-ttu-id="1579e-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="1579e-117">Application</span></span>     | <span data-ttu-id="1579e-118">Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="1579e-118">Calls.AccessMedia.All</span></span>                       |

## <a name="http-request"></a><span data-ttu-id="1579e-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1579e-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/subscribeToTone
```

## <a name="request-headers"></a><span data-ttu-id="1579e-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="1579e-120">Request headers</span></span>
| <span data-ttu-id="1579e-121">名称</span><span class="sxs-lookup"><span data-stu-id="1579e-121">Name</span></span>          | <span data-ttu-id="1579e-122">说明</span><span class="sxs-lookup"><span data-stu-id="1579e-122">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="1579e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1579e-123">Authorization</span></span> | <span data-ttu-id="1579e-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1579e-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1579e-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="1579e-126">Request body</span></span>
<span data-ttu-id="1579e-127">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="1579e-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="1579e-128">参数</span><span class="sxs-lookup"><span data-stu-id="1579e-128">Parameter</span></span>      | <span data-ttu-id="1579e-129">类型</span><span class="sxs-lookup"><span data-stu-id="1579e-129">Type</span></span>    | <span data-ttu-id="1579e-130">说明</span><span class="sxs-lookup"><span data-stu-id="1579e-130">Description</span></span> |
|:---------------|:--------|:------------|
| <span data-ttu-id="1579e-131">适用</span><span class="sxs-lookup"><span data-stu-id="1579e-131">clientContext</span></span>  | <span data-ttu-id="1579e-132">String</span><span class="sxs-lookup"><span data-stu-id="1579e-132">String</span></span>  | <span data-ttu-id="1579e-133">唯一的客户端上下文字符串。</span><span class="sxs-lookup"><span data-stu-id="1579e-133">Unique client context string.</span></span> <span data-ttu-id="1579e-134">最多可以有256个字符。</span><span class="sxs-lookup"><span data-stu-id="1579e-134">Can have a maximum of 256 characters.</span></span> |

## <a name="response"></a><span data-ttu-id="1579e-135">响应</span><span class="sxs-lookup"><span data-stu-id="1579e-135">Response</span></span>
<span data-ttu-id="1579e-136">如果成功，此方法返回 `200 OK` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="1579e-136">If successful, this method returns `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="1579e-137">示例</span><span class="sxs-lookup"><span data-stu-id="1579e-137">Example</span></span>
<span data-ttu-id="1579e-138">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="1579e-138">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="1579e-139">请求</span><span class="sxs-lookup"><span data-stu-id="1579e-139">Request</span></span>
<span data-ttu-id="1579e-140">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="1579e-140">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="1579e-141">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="1579e-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-subscribeToTone"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/subscribeToTone
Content-Type: application/json
Content-Length: 46

{
  "clientContext": "fd1c7836-4d84-4e24-b6aa-23188688cc54"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="1579e-142">C#</span><span class="sxs-lookup"><span data-stu-id="1579e-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-subscribetotone-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1579e-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1579e-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-subscribetotone-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1579e-144">目标-C</span><span class="sxs-lookup"><span data-stu-id="1579e-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-subscribetotone-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="1579e-145">响应</span><span class="sxs-lookup"><span data-stu-id="1579e-145">Response</span></span>

> <span data-ttu-id="1579e-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="1579e-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.commsOperation"
} -->
```http
HTTP/1.1 200 OK

{
  "id": "ea91863c-d0a6-4de0-b73a-4c8d63da5d87",
  "status": "completed",
  "createdDateTime": "2019-07-18T19:52:30Z",
  "lastActionDateTime": "2019-07-18T19:52:31Z",
  "clientContext": "fd1c7836-4d84-4e24-b6aa-23188688cc54",
}
```


##### <a name="notification---tone-notification"></a><span data-ttu-id="1579e-148">通知-音调通知</span><span class="sxs-lookup"><span data-stu-id="1579e-148">Notification - Tone notification</span></span>

<span data-ttu-id="1579e-149">通知包含[toneinfo](../resources/toneinfo.md)资源中所按音调的信息。</span><span class="sxs-lookup"><span data-stu-id="1579e-149">The notification contain information of the tone pressed in the [toneinfo](../resources/toneinfo.md) resource.</span></span>

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
  "value": [
    {
      "changeType": "updated",
      "resource": "/app/calls/421f1100-411f-4a29-8514-dbbb9caff45",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "state": "established",
        "toneInfo": {
          "@odata.type": "#microsoft.graph.toneInfo",
          "sequenceId": 1,
          "tone": "tone1"
        }
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
  "description": "call: subscribeToTone",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

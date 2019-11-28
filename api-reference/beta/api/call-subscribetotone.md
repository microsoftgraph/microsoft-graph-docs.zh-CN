---
title: 调用： subscribeToTone
description: 订阅 DTMF （双音多频信号）。 这样，您就可以在用户按 "Dialpad" 上的键时收到通知。
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 390a8a92b321541c3cf3dc53a181dce70afb505d
ms.sourcegitcommit: fce7ce328f0c88c6310af9cc85d12bcebc88a6c3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/28/2019
ms.locfileid: "39636678"
---
# <a name="call-subscribetotone"></a><span data-ttu-id="74c3b-104">调用： subscribeToTone</span><span class="sxs-lookup"><span data-stu-id="74c3b-104">call: subscribeToTone</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="74c3b-105">订阅 DTMF （双音多频信号）。</span><span class="sxs-lookup"><span data-stu-id="74c3b-105">Subscribe to DTMF (dual-tone multi-frequency signaling).</span></span> <span data-ttu-id="74c3b-106">这样，您就可以在用户按 "Dialpad" 上的键时收到通知。</span><span class="sxs-lookup"><span data-stu-id="74c3b-106">This allows you to be notified when the user presses keys on a "Dialpad".</span></span>

> [!Note]
> <span data-ttu-id="74c3b-107">仅使用[serviceHostedMediaConfig](../resources/servicehostedmediaconfig.md)启动的[调用](../resources/call.md)支持**subscribeToTone**操作。</span><span class="sxs-lookup"><span data-stu-id="74c3b-107">The **subscribeToTone** action is supported only for [calls](../resources/call.md) that are initiated with [serviceHostedMediaConfig](../resources/servicehostedmediaconfig.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="74c3b-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="74c3b-108">Permissions</span></span>
<span data-ttu-id="74c3b-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="74c3b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="74c3b-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="74c3b-111">Permission type</span></span> | <span data-ttu-id="74c3b-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="74c3b-112">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="74c3b-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="74c3b-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="74c3b-114">不支持</span><span class="sxs-lookup"><span data-stu-id="74c3b-114">Not Supported</span></span>        |
| <span data-ttu-id="74c3b-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="74c3b-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="74c3b-116">不支持</span><span class="sxs-lookup"><span data-stu-id="74c3b-116">Not Supported</span></span>        |
| <span data-ttu-id="74c3b-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="74c3b-117">Application</span></span>     | <span data-ttu-id="74c3b-118">Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="74c3b-118">Calls.AccessMedia.All</span></span>                       |

## <a name="http-request"></a><span data-ttu-id="74c3b-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="74c3b-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/subscribeToTone
POST /communications/calls/{id}/subscribeToTone
```
> <span data-ttu-id="74c3b-120">**注意：**`/app` 路径已弃用。</span><span class="sxs-lookup"><span data-stu-id="74c3b-120">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="74c3b-121">今后将使用 `/communications` 路径。</span><span class="sxs-lookup"><span data-stu-id="74c3b-121">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="74c3b-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="74c3b-122">Request headers</span></span>
| <span data-ttu-id="74c3b-123">名称</span><span class="sxs-lookup"><span data-stu-id="74c3b-123">Name</span></span>          | <span data-ttu-id="74c3b-124">说明</span><span class="sxs-lookup"><span data-stu-id="74c3b-124">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="74c3b-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="74c3b-125">Authorization</span></span> | <span data-ttu-id="74c3b-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="74c3b-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="74c3b-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="74c3b-128">Request body</span></span>
<span data-ttu-id="74c3b-129">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="74c3b-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="74c3b-130">参数</span><span class="sxs-lookup"><span data-stu-id="74c3b-130">Parameter</span></span>      | <span data-ttu-id="74c3b-131">类型</span><span class="sxs-lookup"><span data-stu-id="74c3b-131">Type</span></span>    | <span data-ttu-id="74c3b-132">说明</span><span class="sxs-lookup"><span data-stu-id="74c3b-132">Description</span></span> |
|:---------------|:--------|:------------|
| <span data-ttu-id="74c3b-133">适用</span><span class="sxs-lookup"><span data-stu-id="74c3b-133">clientContext</span></span>  | <span data-ttu-id="74c3b-134">String</span><span class="sxs-lookup"><span data-stu-id="74c3b-134">String</span></span>  | <span data-ttu-id="74c3b-135">唯一的客户端上下文字符串。</span><span class="sxs-lookup"><span data-stu-id="74c3b-135">Unique client context string.</span></span> <span data-ttu-id="74c3b-136">最多可以有256个字符。</span><span class="sxs-lookup"><span data-stu-id="74c3b-136">Can have a maximum of 256 characters.</span></span> |

## <a name="response"></a><span data-ttu-id="74c3b-137">响应</span><span class="sxs-lookup"><span data-stu-id="74c3b-137">Response</span></span>
<span data-ttu-id="74c3b-138">如果成功，此方法返回 `200 OK` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="74c3b-138">If successful, this method returns `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="74c3b-139">示例</span><span class="sxs-lookup"><span data-stu-id="74c3b-139">Example</span></span>
<span data-ttu-id="74c3b-140">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="74c3b-140">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="74c3b-141">请求</span><span class="sxs-lookup"><span data-stu-id="74c3b-141">Request</span></span>
<span data-ttu-id="74c3b-142">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="74c3b-142">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="74c3b-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="74c3b-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-subscribeToTone"
}-->
```http
POST https://graph.microsoft.com/beta/communications/calls/{id}/subscribeToTone
Content-Type: application/json
Content-Length: 46

{
  "clientContext": "fd1c7836-4d84-4e24-b6aa-23188688cc54"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="74c3b-144">C#</span><span class="sxs-lookup"><span data-stu-id="74c3b-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-subscribetotone-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="74c3b-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="74c3b-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-subscribetotone-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="74c3b-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="74c3b-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-subscribetotone-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="74c3b-147">响应</span><span class="sxs-lookup"><span data-stu-id="74c3b-147">Response</span></span>

> <span data-ttu-id="74c3b-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="74c3b-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "name": "call-subscribeToTone",
  "truncated": true,
  "@odata.type": "microsoft.graph.subscribeToToneOperation"
} -->
```http
HTTP/1.1 200 OK
Location: https://graph.microsoft.com/beta/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5

{
  "@odata.type": "#microsoft.graph.subscribeToToneOperation",
  "clientContext": "clientContext-value",
  "id": "0fe0623f-d628-42ed-b4bd-8ac290072cc5",
  "resultInfo": null,
  "status": "completed"
}
```


##### <a name="notification---tone-notification"></a><span data-ttu-id="74c3b-150">通知-音调通知</span><span class="sxs-lookup"><span data-stu-id="74c3b-150">Notification - tone notification</span></span>

<span data-ttu-id="74c3b-151">通知包含[toneinfo](../resources/toneinfo.md)资源中所按音调的信息。</span><span class="sxs-lookup"><span data-stu-id="74c3b-151">The notification contain information of the tone pressed in the [toneinfo](../resources/toneinfo.md) resource.</span></span>

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
      "changeType": "updated",
      "resourceUrl": "/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896",
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

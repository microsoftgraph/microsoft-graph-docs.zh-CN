---
title: 调用： subscribeToTone
description: 订阅 DTMF （双音多频信号）。 这样，您就可以在用户按 "Dialpad" 上的键时收到通知。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 4aade47d641cbeb129b199858956f144e2d4bd0d
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/31/2019
ms.locfileid: "40912746"
---
# <a name="call-subscribetotone"></a><span data-ttu-id="a6926-104">调用： subscribeToTone</span><span class="sxs-lookup"><span data-stu-id="a6926-104">call: subscribeToTone</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a6926-105">订阅 DTMF （双音多频信号）。</span><span class="sxs-lookup"><span data-stu-id="a6926-105">Subscribe to DTMF (dual-tone multi-frequency signaling).</span></span> <span data-ttu-id="a6926-106">这样，您就可以在用户按 "Dialpad" 上的键时收到通知。</span><span class="sxs-lookup"><span data-stu-id="a6926-106">This allows you to be notified when the user presses keys on a "Dialpad".</span></span>

> [!Note]
> <span data-ttu-id="a6926-107">仅使用[serviceHostedMediaConfig](../resources/servicehostedmediaconfig.md)启动的[调用](../resources/call.md)支持**subscribeToTone**操作。</span><span class="sxs-lookup"><span data-stu-id="a6926-107">The **subscribeToTone** action is supported only for [calls](../resources/call.md) that are initiated with [serviceHostedMediaConfig](../resources/servicehostedmediaconfig.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="a6926-108">权限</span><span class="sxs-lookup"><span data-stu-id="a6926-108">Permissions</span></span>
<span data-ttu-id="a6926-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a6926-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a6926-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="a6926-111">Permission type</span></span> | <span data-ttu-id="a6926-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a6926-112">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="a6926-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a6926-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="a6926-114">不支持</span><span class="sxs-lookup"><span data-stu-id="a6926-114">Not Supported</span></span>        |
| <span data-ttu-id="a6926-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a6926-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a6926-116">不支持</span><span class="sxs-lookup"><span data-stu-id="a6926-116">Not Supported</span></span>        |
| <span data-ttu-id="a6926-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="a6926-117">Application</span></span>     | <span data-ttu-id="a6926-118">Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="a6926-118">Calls.AccessMedia.All</span></span>                       |

><span data-ttu-id="a6926-119">**注意：** 提供的任何音调数据不能持久化。</span><span class="sxs-lookup"><span data-stu-id="a6926-119">**Note:** Any tone data provided may not be persisted.</span></span> <span data-ttu-id="a6926-120">请确保您符合有关通信的数据保护和机密性的法律和法规。</span><span class="sxs-lookup"><span data-stu-id="a6926-120">Make sure you are compliant with the laws and regulations of your area regarding data protection and confidentiality of communications.</span></span> <span data-ttu-id="a6926-121">有关详细信息，请参阅[使用条款](https://docs.microsoft.com/legal/microsoft-apis/terms-of-use)并咨询法律顾问。</span><span class="sxs-lookup"><span data-stu-id="a6926-121">Please see the [Terms of Use](https://docs.microsoft.com/legal/microsoft-apis/terms-of-use) and consult with your legal counsel for more information.</span></span>
## <a name="http-request"></a><span data-ttu-id="a6926-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a6926-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/subscribeToTone
POST /communications/calls/{id}/subscribeToTone
```
> <span data-ttu-id="a6926-123">**注意：**`/app` 路径已弃用。</span><span class="sxs-lookup"><span data-stu-id="a6926-123">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="a6926-124">今后将使用 `/communications` 路径。</span><span class="sxs-lookup"><span data-stu-id="a6926-124">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a6926-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="a6926-125">Request headers</span></span>
| <span data-ttu-id="a6926-126">名称</span><span class="sxs-lookup"><span data-stu-id="a6926-126">Name</span></span>          | <span data-ttu-id="a6926-127">说明</span><span class="sxs-lookup"><span data-stu-id="a6926-127">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="a6926-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="a6926-128">Authorization</span></span> | <span data-ttu-id="a6926-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a6926-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a6926-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="a6926-131">Request body</span></span>
<span data-ttu-id="a6926-132">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="a6926-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="a6926-133">参数</span><span class="sxs-lookup"><span data-stu-id="a6926-133">Parameter</span></span>      | <span data-ttu-id="a6926-134">类型</span><span class="sxs-lookup"><span data-stu-id="a6926-134">Type</span></span>    | <span data-ttu-id="a6926-135">说明</span><span class="sxs-lookup"><span data-stu-id="a6926-135">Description</span></span> |
|:---------------|:--------|:------------|
| <span data-ttu-id="a6926-136">适用</span><span class="sxs-lookup"><span data-stu-id="a6926-136">clientContext</span></span>  | <span data-ttu-id="a6926-137">String</span><span class="sxs-lookup"><span data-stu-id="a6926-137">String</span></span>  | <span data-ttu-id="a6926-138">唯一的客户端上下文字符串。</span><span class="sxs-lookup"><span data-stu-id="a6926-138">Unique client context string.</span></span> <span data-ttu-id="a6926-139">最多可以有256个字符。</span><span class="sxs-lookup"><span data-stu-id="a6926-139">Can have a maximum of 256 characters.</span></span> |

## <a name="response"></a><span data-ttu-id="a6926-140">响应</span><span class="sxs-lookup"><span data-stu-id="a6926-140">Response</span></span>
<span data-ttu-id="a6926-141">如果成功，此方法返回 `200 OK` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="a6926-141">If successful, this method returns `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="a6926-142">示例</span><span class="sxs-lookup"><span data-stu-id="a6926-142">Example</span></span>
<span data-ttu-id="a6926-143">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="a6926-143">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="a6926-144">请求</span><span class="sxs-lookup"><span data-stu-id="a6926-144">Request</span></span>
<span data-ttu-id="a6926-145">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="a6926-145">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="a6926-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="a6926-146">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="a6926-147">C#</span><span class="sxs-lookup"><span data-stu-id="a6926-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-subscribetotone-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a6926-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a6926-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-subscribetotone-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a6926-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a6926-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-subscribetotone-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="a6926-150">响应</span><span class="sxs-lookup"><span data-stu-id="a6926-150">Response</span></span>

> <span data-ttu-id="a6926-p108">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="a6926-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


##### <a name="notification---tone-notification"></a><span data-ttu-id="a6926-153">通知-音调通知</span><span class="sxs-lookup"><span data-stu-id="a6926-153">Notification - tone notification</span></span>

<span data-ttu-id="a6926-154">通知包含[toneinfo](../resources/toneinfo.md)资源中所按音调的信息。</span><span class="sxs-lookup"><span data-stu-id="a6926-154">The notification contain information of the tone pressed in the [toneinfo](../resources/toneinfo.md) resource.</span></span>

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

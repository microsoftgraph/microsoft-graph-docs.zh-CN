---
title: 调用： playPrompt
description: 在呼叫中播放提示。
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 2c62afeac5870d288c546aa3761b60a270d85219
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40868266"
---
# <a name="call-playprompt"></a><span data-ttu-id="e3ae1-103">调用： playPrompt</span><span class="sxs-lookup"><span data-stu-id="e3ae1-103">call: playPrompt</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e3ae1-104">在呼叫中播放提示。</span><span class="sxs-lookup"><span data-stu-id="e3ae1-104">Play a prompt in the call.</span></span>

<span data-ttu-id="e3ae1-105">有关如何处理操作的详细信息，请参阅[commsOperation](../resources/commsoperation.md)</span><span class="sxs-lookup"><span data-stu-id="e3ae1-105">For more information about how to handle operations, see [commsOperation](../resources/commsoperation.md)</span></span>

> [!Note]
> <span data-ttu-id="e3ae1-106">仅使用[serviceHostedMediaConfig](../resources/servicehostedmediaconfig.md)启动的[调用](../resources/call.md)支持**playPrompt**操作。</span><span class="sxs-lookup"><span data-stu-id="e3ae1-106">The **playPrompt** action is supported only for [calls](../resources/call.md) that are initiated with [serviceHostedMediaConfig](../resources/servicehostedmediaconfig.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e3ae1-107">权限</span><span class="sxs-lookup"><span data-stu-id="e3ae1-107">Permissions</span></span>
<span data-ttu-id="e3ae1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e3ae1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e3ae1-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="e3ae1-110">Permission type</span></span>                        | <span data-ttu-id="e3ae1-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e3ae1-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e3ae1-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e3ae1-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="e3ae1-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="e3ae1-113">Not Supported.</span></span>                               |
| <span data-ttu-id="e3ae1-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e3ae1-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e3ae1-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="e3ae1-115">Not Supported.</span></span>                               |
| <span data-ttu-id="e3ae1-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="e3ae1-116">Application</span></span>                            | <span data-ttu-id="e3ae1-117">无。</span><span class="sxs-lookup"><span data-stu-id="e3ae1-117">None.</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="e3ae1-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e3ae1-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/playPrompt
POST /communications/calls/{id}/playPrompt
```
> <span data-ttu-id="e3ae1-119">**注意：**`/app` 路径已弃用。</span><span class="sxs-lookup"><span data-stu-id="e3ae1-119">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="e3ae1-120">今后将使用 `/communications` 路径。</span><span class="sxs-lookup"><span data-stu-id="e3ae1-120">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e3ae1-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="e3ae1-121">Request headers</span></span>
| <span data-ttu-id="e3ae1-122">名称</span><span class="sxs-lookup"><span data-stu-id="e3ae1-122">Name</span></span>          | <span data-ttu-id="e3ae1-123">说明</span><span class="sxs-lookup"><span data-stu-id="e3ae1-123">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="e3ae1-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="e3ae1-124">Authorization</span></span> | <span data-ttu-id="e3ae1-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e3ae1-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e3ae1-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="e3ae1-127">Request body</span></span>
<span data-ttu-id="e3ae1-128">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="e3ae1-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e3ae1-129">参数</span><span class="sxs-lookup"><span data-stu-id="e3ae1-129">Parameter</span></span>      | <span data-ttu-id="e3ae1-130">类型</span><span class="sxs-lookup"><span data-stu-id="e3ae1-130">Type</span></span>    |<span data-ttu-id="e3ae1-131">说明</span><span class="sxs-lookup"><span data-stu-id="e3ae1-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e3ae1-132">提示</span><span class="sxs-lookup"><span data-stu-id="e3ae1-132">prompts</span></span>|<span data-ttu-id="e3ae1-133">[MediaPrompt](../resources/mediaprompt.md)集合</span><span class="sxs-lookup"><span data-stu-id="e3ae1-133">[MediaPrompt](../resources/mediaprompt.md) collection</span></span>| <span data-ttu-id="e3ae1-134">要播放的提示。</span><span class="sxs-lookup"><span data-stu-id="e3ae1-134">The prompts to be played.</span></span> <span data-ttu-id="e3ae1-135">支持的最大 mediaPrompt 集合大小为20。</span><span class="sxs-lookup"><span data-stu-id="e3ae1-135">The maximum supported mediaPrompt collection size is 20.</span></span>|
|<span data-ttu-id="e3ae1-136">loop</span><span class="sxs-lookup"><span data-stu-id="e3ae1-136">loop</span></span>|<span data-ttu-id="e3ae1-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="e3ae1-137">Boolean</span></span>| <span data-ttu-id="e3ae1-138">循环值。</span><span class="sxs-lookup"><span data-stu-id="e3ae1-138">The loop value.</span></span> <span data-ttu-id="e3ae1-139">如果为 True，则表示无限循环。</span><span class="sxs-lookup"><span data-stu-id="e3ae1-139">True indicates to loop infinitely.</span></span> <span data-ttu-id="e3ae1-140">默认值为 false。</span><span class="sxs-lookup"><span data-stu-id="e3ae1-140">The default value is false.</span></span> |
|<span data-ttu-id="e3ae1-141">适用</span><span class="sxs-lookup"><span data-stu-id="e3ae1-141">clientContext</span></span>|<span data-ttu-id="e3ae1-142">String</span><span class="sxs-lookup"><span data-stu-id="e3ae1-142">String</span></span>|<span data-ttu-id="e3ae1-143">唯一的客户端上下文字符串。</span><span class="sxs-lookup"><span data-stu-id="e3ae1-143">Unique client context string.</span></span> <span data-ttu-id="e3ae1-144">最多可以有256个字符。</span><span class="sxs-lookup"><span data-stu-id="e3ae1-144">Can have a maximum of 256 characters.</span></span>|

## <a name="response"></a><span data-ttu-id="e3ae1-145">响应</span><span class="sxs-lookup"><span data-stu-id="e3ae1-145">Response</span></span>
<span data-ttu-id="e3ae1-146">如果成功，此方法在响应`200 OK`正文中返回响应代码和[playPromptOperation](../resources/playpromptoperation.md)对象。</span><span class="sxs-lookup"><span data-stu-id="e3ae1-146">If successful, this method returns a `200 OK` response code and a [playPromptOperation](../resources/playpromptoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e3ae1-147">示例</span><span class="sxs-lookup"><span data-stu-id="e3ae1-147">Example</span></span>
<span data-ttu-id="e3ae1-148">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="e3ae1-148">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="e3ae1-149">请求</span><span class="sxs-lookup"><span data-stu-id="e3ae1-149">Request</span></span>
<span data-ttu-id="e3ae1-150">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="e3ae1-150">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="e3ae1-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="e3ae1-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-playPrompt"
}-->
```http
POST https://graph.microsoft.com/beta/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/playPrompt
Content-Type: application/json
Content-Length: 166

{
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c",
  "prompts": [
    {
      "@odata.type": "#microsoft.graph.mediaPrompt",
      "mediaInfo": {
        "@odata.type": "#microsoft.graph.mediaInfo",
        "uri": "https://cdn.contoso.com/beep.wav",
        "resourceId": "1D6DE2D4-CD51-4309-8DAA-70768651088E"
      },
    },
  ],
  "loop": false
}
```
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e3ae1-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e3ae1-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-playprompt-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="e3ae1-153">响应</span><span class="sxs-lookup"><span data-stu-id="e3ae1-153">Response</span></span>
<span data-ttu-id="e3ae1-154">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="e3ae1-154">The following is an example of the response.</span></span>

> <span data-ttu-id="e3ae1-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="e3ae1-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.playPromptOperation"
} -->
```http
HTTP/1.1 200 OK
Location: https://graph.microsoft.com/beta/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5

{
  "@odata.type": "#microsoft.graph.playPromptOperation",
  "id": "0fe0623f-d628-42ed-b4bd-8ac290072cc5",
  "status": "running",
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c"
}

```

##### <a name="notification---operation-completed"></a><span data-ttu-id="e3ae1-157">通知-操作已完成</span><span class="sxs-lookup"><span data-stu-id="e3ae1-157">Notification - operation completed</span></span>

 ><span data-ttu-id="e3ae1-158">**注意：** 如果发生无限循环，则不会发送此通知。</span><span class="sxs-lookup"><span data-stu-id="e3ae1-158">**Note:** If infinite looping occurs, this notification is not sent.</span></span>
 
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
      "resourceUrl": "/communications/calls/57DAB8B1894C409AB240BD8BEAE78896/operations/0FE0623FD62842EDB4BD8AC290072CC5",
      "resourceData": {
        "@odata.type": "#microsoft.graph.playPromptOperation",
        "@odata.id": "/communications/calls/57DAB8B1894C409AB240BD8BEAE78896/operations/0FE0623FD62842EDB4BD8AC290072CC5",
        "@odata.etag": "W/\"54451\"",
        "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c",
        "status": "completed"
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
  "description": "call: playPrompt",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

---
title: '调用: playPrompt'
description: 在呼叫中播放提示。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 8ca1a83628ebbb5da2bfec41307b53e01c381883
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35944456"
---
# <a name="call-playprompt"></a><span data-ttu-id="adbcc-103">调用: playPrompt</span><span class="sxs-lookup"><span data-stu-id="adbcc-103">call: playPrompt</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="adbcc-104">在呼叫中播放提示。</span><span class="sxs-lookup"><span data-stu-id="adbcc-104">Play a prompt in the call.</span></span>

<span data-ttu-id="adbcc-105">有关如何处理操作的详细信息, 请参阅[commsOperation](../resources/commsoperation.md)</span><span class="sxs-lookup"><span data-stu-id="adbcc-105">For more information about how to handle operations, see [commsOperation](../resources/commsoperation.md)</span></span>

## <a name="permissions"></a><span data-ttu-id="adbcc-106">权限</span><span class="sxs-lookup"><span data-stu-id="adbcc-106">Permissions</span></span>
<span data-ttu-id="adbcc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="adbcc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="adbcc-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="adbcc-109">Permission type</span></span>                        | <span data-ttu-id="adbcc-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="adbcc-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="adbcc-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="adbcc-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="adbcc-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="adbcc-112">Not Supported.</span></span>                               |
| <span data-ttu-id="adbcc-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="adbcc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="adbcc-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="adbcc-114">Not Supported.</span></span>                               |
| <span data-ttu-id="adbcc-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="adbcc-115">Application</span></span>                            | <span data-ttu-id="adbcc-116">无。</span><span class="sxs-lookup"><span data-stu-id="adbcc-116">None.</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="adbcc-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="adbcc-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/playPrompt
POST /applications/{id}/calls/{id}/playPrompt
```

## <a name="request-headers"></a><span data-ttu-id="adbcc-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="adbcc-118">Request headers</span></span>
| <span data-ttu-id="adbcc-119">名称</span><span class="sxs-lookup"><span data-stu-id="adbcc-119">Name</span></span>          | <span data-ttu-id="adbcc-120">说明</span><span class="sxs-lookup"><span data-stu-id="adbcc-120">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="adbcc-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="adbcc-121">Authorization</span></span> | <span data-ttu-id="adbcc-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="adbcc-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="adbcc-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="adbcc-124">Request body</span></span>
<span data-ttu-id="adbcc-125">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="adbcc-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="adbcc-126">参数</span><span class="sxs-lookup"><span data-stu-id="adbcc-126">Parameter</span></span>      | <span data-ttu-id="adbcc-127">类型</span><span class="sxs-lookup"><span data-stu-id="adbcc-127">Type</span></span>    |<span data-ttu-id="adbcc-128">说明</span><span class="sxs-lookup"><span data-stu-id="adbcc-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="adbcc-129">提示</span><span class="sxs-lookup"><span data-stu-id="adbcc-129">prompts</span></span>|<span data-ttu-id="adbcc-130">[提示符](../resources/prompt.md)集合</span><span class="sxs-lookup"><span data-stu-id="adbcc-130">[prompt](../resources/prompt.md) collection</span></span>| <span data-ttu-id="adbcc-131">目前, 仅支持单个提示符, 类型[MediaPrompt](../resources/mediaprompt.md) 。</span><span class="sxs-lookup"><span data-stu-id="adbcc-131">Currently only a single prompt and of type [MediaPrompt](../resources/mediaprompt.md) is supported.</span></span>|
|<span data-ttu-id="adbcc-132">loop</span><span class="sxs-lookup"><span data-stu-id="adbcc-132">loop</span></span>|<span data-ttu-id="adbcc-133">布尔值</span><span class="sxs-lookup"><span data-stu-id="adbcc-133">bool</span></span>| <span data-ttu-id="adbcc-134">循环值。</span><span class="sxs-lookup"><span data-stu-id="adbcc-134">The loop value.</span></span> <span data-ttu-id="adbcc-135">如果为 true, 则表示无限循环。</span><span class="sxs-lookup"><span data-stu-id="adbcc-135">true indicates to loop infinitely.</span></span> <span data-ttu-id="adbcc-136">默认值为 false。</span><span class="sxs-lookup"><span data-stu-id="adbcc-136">The default value is false.</span></span> |
|<span data-ttu-id="adbcc-137">适用</span><span class="sxs-lookup"><span data-stu-id="adbcc-137">clientContext</span></span>|<span data-ttu-id="adbcc-138">String</span><span class="sxs-lookup"><span data-stu-id="adbcc-138">String</span></span>|<span data-ttu-id="adbcc-139">客户端上下文。</span><span class="sxs-lookup"><span data-stu-id="adbcc-139">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="adbcc-140">响应</span><span class="sxs-lookup"><span data-stu-id="adbcc-140">Response</span></span>
<span data-ttu-id="adbcc-141">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[playPromptOperation](../resources/playpromptoperation.md)对象。</span><span class="sxs-lookup"><span data-stu-id="adbcc-141">If successful, this method returns a `200 OK` response code and a [playPromptOperation](../resources/playpromptoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="adbcc-142">示例</span><span class="sxs-lookup"><span data-stu-id="adbcc-142">Example</span></span>
<span data-ttu-id="adbcc-143">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="adbcc-143">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="adbcc-144">请求</span><span class="sxs-lookup"><span data-stu-id="adbcc-144">Request</span></span>
<span data-ttu-id="adbcc-145">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="adbcc-145">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="adbcc-146">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="adbcc-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-playPrompt"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/57dab8b1-894c-409a-b240-bd8beae78896/playPrompt
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
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="adbcc-147">Javascript</span><span class="sxs-lookup"><span data-stu-id="adbcc-147">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-playprompt-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="adbcc-148">响应</span><span class="sxs-lookup"><span data-stu-id="adbcc-148">Response</span></span>

> <span data-ttu-id="adbcc-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="adbcc-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.playPromptOperation"
} -->
```http
HTTP/1.1 200 OK
Location: https://graph.microsoft.com/beta/app/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5

{
  "@odata.type": "#microsoft.graph.playPromptOperation",
  "id": "0fe0623f-d628-42ed-b4bd-8ac290072cc5",
  "status": "running",
  "createdDateTime": "2018-09-06T15:58:41Z",
  "lastActionDateTime": "2018-09-06T15:58:41Z",
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c"
}

```

##### <a name="notification---operation-completed"></a><span data-ttu-id="adbcc-151">通知-操作已完成</span><span class="sxs-lookup"><span data-stu-id="adbcc-151">Notification - operation completed</span></span>

 ><span data-ttu-id="adbcc-152">**注意:** 如果发生无限循环, 则不会发送此通知。</span><span class="sxs-lookup"><span data-stu-id="adbcc-152">**Note:** If infinite looping occurs, this notification is not sent.</span></span>
 
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
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896/operations/0FE0623FD62842EDB4BD8AC290072CC5",
      "resourceData": {
        "@odata.type": "#microsoft.graph.playPromptOperation",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896/operations/0FE0623FD62842EDB4BD8AC290072CC5",
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

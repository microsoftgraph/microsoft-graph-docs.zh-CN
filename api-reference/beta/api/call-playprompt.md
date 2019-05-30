---
title: '调用: playPrompt'
description: 在呼叫中播放提示。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: ad0001c1961f1c6e9126a39609d368104e133aec
ms.sourcegitcommit: c0df90d66cb2072848d4bb0bf730c47a601b99ce
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/29/2019
ms.locfileid: "34536069"
---
# <a name="call-playprompt"></a><span data-ttu-id="51b41-103">调用: playPrompt</span><span class="sxs-lookup"><span data-stu-id="51b41-103">call: playPrompt</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="51b41-104">在呼叫中播放提示。</span><span class="sxs-lookup"><span data-stu-id="51b41-104">Play a prompt in the call.</span></span>

## <a name="permissions"></a><span data-ttu-id="51b41-105">权限</span><span class="sxs-lookup"><span data-stu-id="51b41-105">Permissions</span></span>
<span data-ttu-id="51b41-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="51b41-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="51b41-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="51b41-108">Permission type</span></span>                        | <span data-ttu-id="51b41-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="51b41-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="51b41-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="51b41-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="51b41-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="51b41-111">Not Supported.</span></span>                               |
| <span data-ttu-id="51b41-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="51b41-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="51b41-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="51b41-113">Not Supported.</span></span>                               |
| <span data-ttu-id="51b41-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="51b41-114">Application</span></span>                            | <span data-ttu-id="51b41-115">无。</span><span class="sxs-lookup"><span data-stu-id="51b41-115">None.</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="51b41-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="51b41-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/playPrompt
POST /applications/{id}/calls/{id}/playPrompt
```

## <a name="request-headers"></a><span data-ttu-id="51b41-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="51b41-117">Request headers</span></span>
| <span data-ttu-id="51b41-118">名称</span><span class="sxs-lookup"><span data-stu-id="51b41-118">Name</span></span>          | <span data-ttu-id="51b41-119">说明</span><span class="sxs-lookup"><span data-stu-id="51b41-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="51b41-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="51b41-120">Authorization</span></span> | <span data-ttu-id="51b41-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="51b41-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="51b41-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="51b41-123">Request body</span></span>
<span data-ttu-id="51b41-124">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="51b41-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="51b41-125">参数</span><span class="sxs-lookup"><span data-stu-id="51b41-125">Parameter</span></span>      | <span data-ttu-id="51b41-126">类型</span><span class="sxs-lookup"><span data-stu-id="51b41-126">Type</span></span>    |<span data-ttu-id="51b41-127">说明</span><span class="sxs-lookup"><span data-stu-id="51b41-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="51b41-128">提示</span><span class="sxs-lookup"><span data-stu-id="51b41-128">prompts</span></span>|<span data-ttu-id="51b41-129">[提示符](../resources/prompt.md)集合</span><span class="sxs-lookup"><span data-stu-id="51b41-129">[prompt](../resources/prompt.md) collection</span></span>||
|<span data-ttu-id="51b41-130">适用</span><span class="sxs-lookup"><span data-stu-id="51b41-130">clientContext</span></span>|<span data-ttu-id="51b41-131">String</span><span class="sxs-lookup"><span data-stu-id="51b41-131">String</span></span>|<span data-ttu-id="51b41-132">客户端上下文。</span><span class="sxs-lookup"><span data-stu-id="51b41-132">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="51b41-133">响应</span><span class="sxs-lookup"><span data-stu-id="51b41-133">Response</span></span>
<span data-ttu-id="51b41-134">如果成功, 此方法在`200 OK`响应正文中返回响应代码和[playPromptOperation](../resources/playpromptoperation.md)对象。</span><span class="sxs-lookup"><span data-stu-id="51b41-134">If successful, this method returns `200 OK` response code and [playPromptOperation](../resources/playpromptoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="51b41-135">示例</span><span class="sxs-lookup"><span data-stu-id="51b41-135">Example</span></span>
<span data-ttu-id="51b41-136">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="51b41-136">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="51b41-137">请求</span><span class="sxs-lookup"><span data-stu-id="51b41-137">Request</span></span>
<span data-ttu-id="51b41-138">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="51b41-138">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "call-playPrompt"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/playPrompt
Content-Type: application/json
Content-Length: 166

{
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c",
  "prompts": [
    {
      "@odata.type": "#microsoft.graph.mediaPrompt",
      "mediaInfo": {
        "uri": "https://cdn.contoso.com/beep.wav",
        "resourceId": "1D6DE2D4-CD51-4309-8DAA-70768651088E"
      },
      "loop": 5
    }
  ]
}
```

##### <a name="response"></a><span data-ttu-id="51b41-139">响应</span><span class="sxs-lookup"><span data-stu-id="51b41-139">Response</span></span>

> <span data-ttu-id="51b41-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="51b41-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.playPromptOperation"
} -->
```http
HTTP/1.1 200 OK
Location: https://graph.microsoft.com/beta/app/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="51b41-142">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="51b41-142">SDK sample code</span></span>

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="51b41-143">Javascript</span><span class="sxs-lookup"><span data-stu-id="51b41-143">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/call-playPrompt-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

##### <a name="notification---operation-completed"></a><span data-ttu-id="51b41-144">通知-操作已完成</span><span class="sxs-lookup"><span data-stu-id="51b41-144">Notification - operation completed</span></span>

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
    "Error: /api-reference/beta/api/call-playprompt.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->

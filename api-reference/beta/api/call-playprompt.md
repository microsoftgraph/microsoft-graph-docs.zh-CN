---
title: 呼叫： playPrompt
description: 在呼叫中播放提示。
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: 47d4dac56f1424f71fff20f63c9d68f3f09d3926
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27883655"
---
# <a name="call-playprompt"></a><span data-ttu-id="7889e-103">呼叫： playPrompt</span><span class="sxs-lookup"><span data-stu-id="7889e-103">call: playPrompt</span></span>

> <span data-ttu-id="7889e-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="7889e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7889e-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="7889e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7889e-106">在呼叫中播放提示。</span><span class="sxs-lookup"><span data-stu-id="7889e-106">Play a prompt in the call.</span></span>

## <a name="permissions"></a><span data-ttu-id="7889e-107">权限</span><span class="sxs-lookup"><span data-stu-id="7889e-107">Permissions</span></span>
<span data-ttu-id="7889e-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7889e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7889e-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="7889e-110">Permission type</span></span>                        | <span data-ttu-id="7889e-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7889e-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="7889e-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7889e-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="7889e-113">不受支持。</span><span class="sxs-lookup"><span data-stu-id="7889e-113">Not Supported.</span></span>                               |
| <span data-ttu-id="7889e-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7889e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7889e-115">不受支持。</span><span class="sxs-lookup"><span data-stu-id="7889e-115">Not Supported.</span></span>                               |
| <span data-ttu-id="7889e-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="7889e-116">Application</span></span>                            | <span data-ttu-id="7889e-117">无。</span><span class="sxs-lookup"><span data-stu-id="7889e-117">None.</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="7889e-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7889e-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/playPrompt
POST /applications/{id}/calls/{id}/playPrompt
```

## <a name="request-headers"></a><span data-ttu-id="7889e-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="7889e-119">Request headers</span></span>
| <span data-ttu-id="7889e-120">名称</span><span class="sxs-lookup"><span data-stu-id="7889e-120">Name</span></span>          | <span data-ttu-id="7889e-121">说明</span><span class="sxs-lookup"><span data-stu-id="7889e-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="7889e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7889e-122">Authorization</span></span> | <span data-ttu-id="7889e-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7889e-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7889e-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="7889e-125">Request body</span></span>
<span data-ttu-id="7889e-126">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="7889e-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="7889e-127">参数</span><span class="sxs-lookup"><span data-stu-id="7889e-127">Parameter</span></span>      | <span data-ttu-id="7889e-128">类型</span><span class="sxs-lookup"><span data-stu-id="7889e-128">Type</span></span>    |<span data-ttu-id="7889e-129">Description</span><span class="sxs-lookup"><span data-stu-id="7889e-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7889e-130">提示</span><span class="sxs-lookup"><span data-stu-id="7889e-130">prompts</span></span>|<span data-ttu-id="7889e-131">[提示](../resources/prompt.md)集合</span><span class="sxs-lookup"><span data-stu-id="7889e-131">[prompt](../resources/prompt.md) collection</span></span>||
|<span data-ttu-id="7889e-132">clientContext</span><span class="sxs-lookup"><span data-stu-id="7889e-132">clientContext</span></span>|<span data-ttu-id="7889e-133">字符串</span><span class="sxs-lookup"><span data-stu-id="7889e-133">String</span></span>|<span data-ttu-id="7889e-134">客户端上下文。</span><span class="sxs-lookup"><span data-stu-id="7889e-134">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="7889e-135">响应</span><span class="sxs-lookup"><span data-stu-id="7889e-135">Response</span></span>
<span data-ttu-id="7889e-136">如果成功，此方法返回`200 OK`响应正文中的响应代码和[playPromptOperation](../resources/playPromptOperation.md)对象。</span><span class="sxs-lookup"><span data-stu-id="7889e-136">If successful, this method returns `200 OK` response code and [playPromptOperation](../resources/playPromptOperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7889e-137">示例</span><span class="sxs-lookup"><span data-stu-id="7889e-137">Example</span></span>
<span data-ttu-id="7889e-138">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="7889e-138">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="7889e-139">请求</span><span class="sxs-lookup"><span data-stu-id="7889e-139">Request</span></span>
<span data-ttu-id="7889e-140">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="7889e-140">The following example shows the request.</span></span>

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

##### <a name="response"></a><span data-ttu-id="7889e-141">响应</span><span class="sxs-lookup"><span data-stu-id="7889e-141">Response</span></span>

> <span data-ttu-id="7889e-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="7889e-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.playPromptOperation"
} -->
```http
HTTP/1.1 200 OK
Location: https://graph.microsoft.com/beta/app/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5
```

##### <a name="notification---operation-completed"></a><span data-ttu-id="7889e-144">通知-完成的操作</span><span class="sxs-lookup"><span data-stu-id="7889e-144">Notification - operation completed</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "call: playPrompt",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

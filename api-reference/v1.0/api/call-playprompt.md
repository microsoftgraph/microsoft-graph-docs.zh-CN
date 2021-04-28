---
title: call： playPrompt
description: 在呼叫中播放提示。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: ce89f0bbdaf665bb9f459f554a2e605324ead609
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52051604"
---
# <a name="call-playprompt"></a><span data-ttu-id="b9251-103">call： playPrompt</span><span class="sxs-lookup"><span data-stu-id="b9251-103">call: playPrompt</span></span>

<span data-ttu-id="b9251-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b9251-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b9251-105">在呼叫中播放提示。</span><span class="sxs-lookup"><span data-stu-id="b9251-105">Play a prompt in the call.</span></span>

<span data-ttu-id="b9251-106">若要详细了解如何处理操作，请参阅 [commsOperation](../resources/commsoperation.md)</span><span class="sxs-lookup"><span data-stu-id="b9251-106">For more information about how to handle operations, see [commsOperation](../resources/commsoperation.md)</span></span>

> [!Note]
> <span data-ttu-id="b9251-107">**playPrompt** 操作仅支持 [通过](../resources/call.md) [serviceHostedMediaConfig 启动的呼叫](../resources/servicehostedmediaconfig.md)。</span><span class="sxs-lookup"><span data-stu-id="b9251-107">The **playPrompt** action is supported only for [calls](../resources/call.md) that are initiated with [serviceHostedMediaConfig](../resources/servicehostedmediaconfig.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b9251-108">权限</span><span class="sxs-lookup"><span data-stu-id="b9251-108">Permissions</span></span>
<span data-ttu-id="b9251-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b9251-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b9251-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="b9251-111">Permission type</span></span>                        | <span data-ttu-id="b9251-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b9251-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b9251-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b9251-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="b9251-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="b9251-114">Not Supported.</span></span>                               |
| <span data-ttu-id="b9251-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b9251-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b9251-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b9251-116">Not Supported.</span></span>                               |
| <span data-ttu-id="b9251-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="b9251-117">Application</span></span>                            | <span data-ttu-id="b9251-118">无。</span><span class="sxs-lookup"><span data-stu-id="b9251-118">None.</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="b9251-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b9251-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /communications/calls/{id}/playPrompt
```

## <a name="request-headers"></a><span data-ttu-id="b9251-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="b9251-120">Request headers</span></span>
| <span data-ttu-id="b9251-121">名称</span><span class="sxs-lookup"><span data-stu-id="b9251-121">Name</span></span>          | <span data-ttu-id="b9251-122">说明</span><span class="sxs-lookup"><span data-stu-id="b9251-122">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="b9251-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b9251-123">Authorization</span></span> | <span data-ttu-id="b9251-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b9251-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b9251-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="b9251-126">Request body</span></span>
<span data-ttu-id="b9251-127">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="b9251-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b9251-128">参数</span><span class="sxs-lookup"><span data-stu-id="b9251-128">Parameter</span></span>      | <span data-ttu-id="b9251-129">类型</span><span class="sxs-lookup"><span data-stu-id="b9251-129">Type</span></span>    |<span data-ttu-id="b9251-130">说明</span><span class="sxs-lookup"><span data-stu-id="b9251-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b9251-131">prompts</span><span class="sxs-lookup"><span data-stu-id="b9251-131">prompts</span></span>|<span data-ttu-id="b9251-132">[MediaPrompt](../resources/mediaprompt.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b9251-132">[MediaPrompt](../resources/mediaprompt.md) collection</span></span>| <span data-ttu-id="b9251-133">要播放的提示。</span><span class="sxs-lookup"><span data-stu-id="b9251-133">The prompts to be played.</span></span> <span data-ttu-id="b9251-134">支持的最大 MediaPrompt 集合大小为 20。</span><span class="sxs-lookup"><span data-stu-id="b9251-134">The maximum supported MediaPrompt collection size is 20.</span></span>|
|<span data-ttu-id="b9251-135">clientContext</span><span class="sxs-lookup"><span data-stu-id="b9251-135">clientContext</span></span>|<span data-ttu-id="b9251-136">String</span><span class="sxs-lookup"><span data-stu-id="b9251-136">String</span></span>|<span data-ttu-id="b9251-137">唯一的客户端上下文字符串。</span><span class="sxs-lookup"><span data-stu-id="b9251-137">Unique client context string.</span></span> <span data-ttu-id="b9251-138">最多可包含 256 个字符。</span><span class="sxs-lookup"><span data-stu-id="b9251-138">Can have a maximum of 256 characters.</span></span>|

## <a name="response"></a><span data-ttu-id="b9251-139">响应</span><span class="sxs-lookup"><span data-stu-id="b9251-139">Response</span></span>
<span data-ttu-id="b9251-140">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [playPromptOperation](../resources/playpromptoperation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b9251-140">If successful, this method returns a `200 OK` response code and a [playPromptOperation](../resources/playpromptoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b9251-141">示例</span><span class="sxs-lookup"><span data-stu-id="b9251-141">Example</span></span>
<span data-ttu-id="b9251-142">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="b9251-142">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="b9251-143">请求</span><span class="sxs-lookup"><span data-stu-id="b9251-143">Request</span></span>
<span data-ttu-id="b9251-144">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="b9251-144">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="b9251-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="b9251-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-playPrompt"
}-->
```http
POST https://graph.microsoft.com/v1.0/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/playPrompt
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
      }
    }
  ]
}
```
# <a name="javascript"></a>[<span data-ttu-id="b9251-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b9251-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-playprompt-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="b9251-147">C#</span><span class="sxs-lookup"><span data-stu-id="b9251-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-playprompt-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b9251-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b9251-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-playprompt-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b9251-149">Java</span><span class="sxs-lookup"><span data-stu-id="b9251-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/call-playprompt-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="b9251-150">响应</span><span class="sxs-lookup"><span data-stu-id="b9251-150">Response</span></span>
<span data-ttu-id="b9251-151">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b9251-151">The following is an example of the response.</span></span>

> <span data-ttu-id="b9251-152">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="b9251-152">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.playPromptOperation"
} -->
```http
HTTP/1.1 200 OK
Location: https://graph.microsoft.com/v1.0/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.playPromptOperation",
  "id": "0fe0623f-d628-42ed-b4bd-8ac290072cc5",
  "status": "running",
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c"
}

```

##### <a name="notification---operation-completed"></a><span data-ttu-id="b9251-153">通知 - 操作已完成</span><span class="sxs-lookup"><span data-stu-id="b9251-153">Notification - operation completed</span></span>
 
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
        "resultInfo": {
          "@odata.type": "#microsoft.graph.resultInfo",
          "code": 200,
          "subcode": 0,
          "message": "Action completed successfully."
        },
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


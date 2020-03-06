---
title: 调用： playPrompt
description: 在呼叫中播放提示。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 82026017e3d82b5daa792c0cbe73718751cc2efd
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42518691"
---
# <a name="call-playprompt"></a><span data-ttu-id="4bd21-103">调用： playPrompt</span><span class="sxs-lookup"><span data-stu-id="4bd21-103">call: playPrompt</span></span>

<span data-ttu-id="4bd21-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4bd21-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4bd21-105">在呼叫中播放提示。</span><span class="sxs-lookup"><span data-stu-id="4bd21-105">Play a prompt in the call.</span></span>

<span data-ttu-id="4bd21-106">有关如何处理操作的详细信息，请参阅[commsOperation](../resources/commsoperation.md)</span><span class="sxs-lookup"><span data-stu-id="4bd21-106">For more information about how to handle operations, see [commsOperation](../resources/commsoperation.md)</span></span>

> [!Note]
> <span data-ttu-id="4bd21-107">仅使用[serviceHostedMediaConfig](../resources/servicehostedmediaconfig.md)启动的[调用](../resources/call.md)支持**playPrompt**操作。</span><span class="sxs-lookup"><span data-stu-id="4bd21-107">The **playPrompt** action is supported only for [calls](../resources/call.md) that are initiated with [serviceHostedMediaConfig](../resources/servicehostedmediaconfig.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="4bd21-108">权限</span><span class="sxs-lookup"><span data-stu-id="4bd21-108">Permissions</span></span>
<span data-ttu-id="4bd21-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4bd21-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4bd21-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="4bd21-111">Permission type</span></span>                        | <span data-ttu-id="4bd21-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4bd21-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="4bd21-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4bd21-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="4bd21-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="4bd21-114">Not Supported.</span></span>                               |
| <span data-ttu-id="4bd21-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4bd21-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4bd21-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="4bd21-116">Not Supported.</span></span>                               |
| <span data-ttu-id="4bd21-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="4bd21-117">Application</span></span>                            | <span data-ttu-id="4bd21-118">无。</span><span class="sxs-lookup"><span data-stu-id="4bd21-118">None.</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="4bd21-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4bd21-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /communications/calls/{id}/playPrompt
```

## <a name="request-headers"></a><span data-ttu-id="4bd21-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="4bd21-120">Request headers</span></span>
| <span data-ttu-id="4bd21-121">名称</span><span class="sxs-lookup"><span data-stu-id="4bd21-121">Name</span></span>          | <span data-ttu-id="4bd21-122">说明</span><span class="sxs-lookup"><span data-stu-id="4bd21-122">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="4bd21-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4bd21-123">Authorization</span></span> | <span data-ttu-id="4bd21-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4bd21-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4bd21-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="4bd21-126">Request body</span></span>
<span data-ttu-id="4bd21-127">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="4bd21-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="4bd21-128">参数</span><span class="sxs-lookup"><span data-stu-id="4bd21-128">Parameter</span></span>      | <span data-ttu-id="4bd21-129">类型</span><span class="sxs-lookup"><span data-stu-id="4bd21-129">Type</span></span>    |<span data-ttu-id="4bd21-130">说明</span><span class="sxs-lookup"><span data-stu-id="4bd21-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4bd21-131">提示</span><span class="sxs-lookup"><span data-stu-id="4bd21-131">prompts</span></span>|<span data-ttu-id="4bd21-132">[MediaPrompt](../resources/mediaprompt.md)集合</span><span class="sxs-lookup"><span data-stu-id="4bd21-132">[MediaPrompt](../resources/mediaprompt.md) collection</span></span>| <span data-ttu-id="4bd21-133">要播放的提示。</span><span class="sxs-lookup"><span data-stu-id="4bd21-133">The prompts to be played.</span></span> <span data-ttu-id="4bd21-134">支持的最大 MediaPrompt 集合大小为20。</span><span class="sxs-lookup"><span data-stu-id="4bd21-134">The maximum supported MediaPrompt collection size is 20.</span></span>|
|<span data-ttu-id="4bd21-135">适用</span><span class="sxs-lookup"><span data-stu-id="4bd21-135">clientContext</span></span>|<span data-ttu-id="4bd21-136">字符串</span><span class="sxs-lookup"><span data-stu-id="4bd21-136">String</span></span>|<span data-ttu-id="4bd21-137">唯一的客户端上下文字符串。</span><span class="sxs-lookup"><span data-stu-id="4bd21-137">Unique client context string.</span></span> <span data-ttu-id="4bd21-138">最多可以有256个字符。</span><span class="sxs-lookup"><span data-stu-id="4bd21-138">Can have a maximum of 256 characters.</span></span>|

## <a name="response"></a><span data-ttu-id="4bd21-139">响应</span><span class="sxs-lookup"><span data-stu-id="4bd21-139">Response</span></span>
<span data-ttu-id="4bd21-140">如果成功，此方法在响应`200 OK`正文中返回响应代码和[playPromptOperation](../resources/playpromptoperation.md)对象。</span><span class="sxs-lookup"><span data-stu-id="4bd21-140">If successful, this method returns a `200 OK` response code and a [playPromptOperation](../resources/playpromptoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4bd21-141">示例</span><span class="sxs-lookup"><span data-stu-id="4bd21-141">Example</span></span>
<span data-ttu-id="4bd21-142">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="4bd21-142">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="4bd21-143">请求</span><span class="sxs-lookup"><span data-stu-id="4bd21-143">Request</span></span>
<span data-ttu-id="4bd21-144">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="4bd21-144">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="4bd21-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="4bd21-145">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="4bd21-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4bd21-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-playprompt-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="4bd21-147">响应</span><span class="sxs-lookup"><span data-stu-id="4bd21-147">Response</span></span>
<span data-ttu-id="4bd21-148">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="4bd21-148">The following is an example of the response.</span></span>

> <span data-ttu-id="4bd21-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="4bd21-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

##### <a name="notification---operation-completed"></a><span data-ttu-id="4bd21-151">通知-操作已完成</span><span class="sxs-lookup"><span data-stu-id="4bd21-151">Notification - operation completed</span></span>
 
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

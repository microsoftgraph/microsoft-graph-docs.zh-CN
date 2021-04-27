---
title: call： cancelMediaProcessing
description: 取消任何进行中的 playPrompt 或 recordResponse 运算的媒体处理。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: fe6ecbedcb0d66e5261f08eb3a4aee48db25a493
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047663"
---
# <a name="call-cancelmediaprocessing"></a><span data-ttu-id="7e8de-103">call： cancelMediaProcessing</span><span class="sxs-lookup"><span data-stu-id="7e8de-103">call: cancelMediaProcessing</span></span>

<span data-ttu-id="7e8de-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7e8de-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7e8de-105">取消处理任何进行中的媒体操作。</span><span class="sxs-lookup"><span data-stu-id="7e8de-105">Cancels processing for any in-progress media operations.</span></span>

<span data-ttu-id="7e8de-106">媒体操作是指 IVR 操作 [playPrompt](./call-playprompt.md) 和 [recordResponse，](./call-record.md)它们默认排队等待处理。</span><span class="sxs-lookup"><span data-stu-id="7e8de-106">Media operations refer to the IVR operations [playPrompt](./call-playprompt.md) and [recordResponse](./call-record.md), which are by default queued to process in order.</span></span> <span data-ttu-id="7e8de-107">**cancelMediaProcessing** 方法取消进程内的任何操作以及已排队的操作。</span><span class="sxs-lookup"><span data-stu-id="7e8de-107">The **cancelMediaProcessing** method cancels any operation that is in-process as well as operations that are queued.</span></span> <span data-ttu-id="7e8de-108">例如，此 API 可用于清理新媒体操作的 IVR 操作队列。</span><span class="sxs-lookup"><span data-stu-id="7e8de-108">For example, this API can be used to clean up the IVR operation queue for a new media operation.</span></span> <span data-ttu-id="7e8de-109">但是，它将不会取消 **ubscribeToTone** 操作，因为它独立于任何操作队列运行。</span><span class="sxs-lookup"><span data-stu-id="7e8de-109">However, it will not cancel a **ubscribeToTone** operation because it operates independent of any operation queue.</span></span>

## <a name="permissions"></a><span data-ttu-id="7e8de-110">权限</span><span class="sxs-lookup"><span data-stu-id="7e8de-110">Permissions</span></span>
<span data-ttu-id="7e8de-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7e8de-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7e8de-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="7e8de-113">Permission type</span></span>                        | <span data-ttu-id="7e8de-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7e8de-114">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="7e8de-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7e8de-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="7e8de-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="7e8de-116">Not Supported.</span></span>                              |
| <span data-ttu-id="7e8de-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7e8de-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7e8de-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="7e8de-118">Not Supported.</span></span>                              |
| <span data-ttu-id="7e8de-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="7e8de-119">Application</span></span>                            | <span data-ttu-id="7e8de-120">无。</span><span class="sxs-lookup"><span data-stu-id="7e8de-120">None.</span></span>                                       |

## <a name="http-request"></a><span data-ttu-id="7e8de-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7e8de-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/cancelMediaProcessing
POST /communications/calls/{id}/cancelMediaProcessing
```
> <span data-ttu-id="7e8de-122">**注意：**`/app` 路径已弃用。</span><span class="sxs-lookup"><span data-stu-id="7e8de-122">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="7e8de-123">今后将使用 `/communications` 路径。</span><span class="sxs-lookup"><span data-stu-id="7e8de-123">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7e8de-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="7e8de-124">Request headers</span></span>
| <span data-ttu-id="7e8de-125">名称</span><span class="sxs-lookup"><span data-stu-id="7e8de-125">Name</span></span>          | <span data-ttu-id="7e8de-126">说明</span><span class="sxs-lookup"><span data-stu-id="7e8de-126">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="7e8de-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="7e8de-127">Authorization</span></span> | <span data-ttu-id="7e8de-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7e8de-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7e8de-130">Content-type</span><span class="sxs-lookup"><span data-stu-id="7e8de-130">Content-type</span></span> | <span data-ttu-id="7e8de-p105">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="7e8de-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7e8de-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="7e8de-133">Request body</span></span>
<span data-ttu-id="7e8de-134">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="7e8de-134">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="7e8de-135">参数</span><span class="sxs-lookup"><span data-stu-id="7e8de-135">Parameter</span></span>      | <span data-ttu-id="7e8de-136">类型</span><span class="sxs-lookup"><span data-stu-id="7e8de-136">Type</span></span>    | <span data-ttu-id="7e8de-137">说明</span><span class="sxs-lookup"><span data-stu-id="7e8de-137">Description</span></span>                                                    |
|:---------------|:--------|:---------------------------------------------------------------|
| <span data-ttu-id="7e8de-138">clientContext</span><span class="sxs-lookup"><span data-stu-id="7e8de-138">clientContext</span></span>  | <span data-ttu-id="7e8de-139">String</span><span class="sxs-lookup"><span data-stu-id="7e8de-139">String</span></span>  | <span data-ttu-id="7e8de-140">客户端上下文。</span><span class="sxs-lookup"><span data-stu-id="7e8de-140">The client context.</span></span>                                            |

## <a name="response"></a><span data-ttu-id="7e8de-141">响应</span><span class="sxs-lookup"><span data-stu-id="7e8de-141">Response</span></span>
<span data-ttu-id="7e8de-142">如果成功，此方法将返回 HTTP 响应代码和具有为此请求创建的 `200 OK` [commsOperation](../resources/commsoperation.md) 的 URI 的位置标头。</span><span class="sxs-lookup"><span data-stu-id="7e8de-142">If successful, this method returns a `200 OK` HTTP response code and a Location header with a URI to the [commsOperation](../resources/commsoperation.md) created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="7e8de-143">示例</span><span class="sxs-lookup"><span data-stu-id="7e8de-143">Example</span></span>
<span data-ttu-id="7e8de-144">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="7e8de-144">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="7e8de-145">请求</span><span class="sxs-lookup"><span data-stu-id="7e8de-145">Request</span></span>
<span data-ttu-id="7e8de-146">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="7e8de-146">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="7e8de-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="7e8de-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-cancelMediaProcessing"
}-->
```http
POST https://graph.microsoft.com/beta/communications/calls/{id}/cancelMediaProcessing
Content-Type: application/json
Content-Length: 62

{
  "clientContext": "clientContext-value"
}
```
# <a name="c"></a>[<span data-ttu-id="7e8de-148">C#</span><span class="sxs-lookup"><span data-stu-id="7e8de-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-cancelmediaprocessing-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7e8de-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7e8de-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-cancelmediaprocessing-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7e8de-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7e8de-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-cancelmediaprocessing-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7e8de-151">Java</span><span class="sxs-lookup"><span data-stu-id="7e8de-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/call-cancelmediaprocessing-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="7e8de-152">响应</span><span class="sxs-lookup"><span data-stu-id="7e8de-152">Response</span></span>

> <span data-ttu-id="7e8de-153">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="7e8de-153">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.cancelMediaProcessingOperation"
} -->
```http
HTTP/1.1 200 OK
Location: https://graph.microsoft.com/beta/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/17e3b46c-f61d-4f4d-9635-c626ef18e6ad
Content-Type: application/json
Content-Length: 259

{
  "@odata.type": "#microsoft.graph.cancelMediaProcessingOperation",
  "status": "completed",
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c",
  "id": "0fe0623f-d628-42ed-b4bd-8ac290072cc5"
}
```

##### <a name="notification---operation-canceled-for-recordresponse"></a><span data-ttu-id="7e8de-154">通知 - 已取消 recordResponse 的操作</span><span class="sxs-lookup"><span data-stu-id="7e8de-154">Notification - Operation canceled for recordResponse</span></span>

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
        "@odata.type": "#microsoft.graph.recordOperation",
        "@odata.id": "/communications/calls/57DAB8B1894C409AB240BD8BEAE78896/operations/0FE0623FD62842EDB4BD8AC290072CC5",
        "@odata.etag": "W/\"54451\"",
        "id": "0fe0623f-d628-42ed-b4bd-8ac290072cc5",
        "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c",
        "status": "failed",
        "resultInfo": {
          "@odata.type": "#microsoft.graph.resultInfo",
          "code": 400,
          "subcode": 8508,
          "message": "Action failed, the operation was cancelled."
        },
        "recordingLocation": "",
        "recordingAccessToken": "",
        "completionReason": "operationCanceled"
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
  "description": "call: cancelMediaProcessing",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->



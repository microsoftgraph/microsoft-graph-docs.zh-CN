---
title: 调用： cancelMediaProcessing
description: 取消对任何正在进行的 playPrompt 或 recordResponse 操作的媒体处理。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 1df48c9321b03d3548bd2c971ac733fcd6849a53
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47987461"
---
# <a name="call-cancelmediaprocessing"></a><span data-ttu-id="2b995-103">调用： cancelMediaProcessing</span><span class="sxs-lookup"><span data-stu-id="2b995-103">call: cancelMediaProcessing</span></span>

<span data-ttu-id="2b995-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2b995-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2b995-105">取消对正在进行的媒体操作的处理。</span><span class="sxs-lookup"><span data-stu-id="2b995-105">Cancels processing for any in-progress media operations.</span></span>

<span data-ttu-id="2b995-106">媒体操作指的是 IVR 操作 [playPrompt](./call-playprompt.md) 和 [recordResponse](./call-record.md)，这些操作在默认情况下排队为按顺序处理。</span><span class="sxs-lookup"><span data-stu-id="2b995-106">Media operations refer to the IVR operations [playPrompt](./call-playprompt.md) and [recordResponse](./call-record.md), which are by default queued to process in order.</span></span> <span data-ttu-id="2b995-107">**CancelMediaProcessing**方法将取消进程中的任何操作以及排队的操作。</span><span class="sxs-lookup"><span data-stu-id="2b995-107">The **cancelMediaProcessing** method cancels any operation that is in-process as well as operations that are queued.</span></span> <span data-ttu-id="2b995-108">例如，此 API 可用于清理新媒体操作的 IVR 操作队列。</span><span class="sxs-lookup"><span data-stu-id="2b995-108">For example, this API can be used to clean up the IVR operation queue for a new media operation.</span></span> <span data-ttu-id="2b995-109">但是，它不会取消 **ubscribeToTone** 操作，因为它独立于任何操作队列运行。</span><span class="sxs-lookup"><span data-stu-id="2b995-109">However, it will not cancel a **ubscribeToTone** operation because it operates independent of any operation queue.</span></span>

## <a name="permissions"></a><span data-ttu-id="2b995-110">权限</span><span class="sxs-lookup"><span data-stu-id="2b995-110">Permissions</span></span>
<span data-ttu-id="2b995-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2b995-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2b995-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="2b995-113">Permission type</span></span>                        | <span data-ttu-id="2b995-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2b995-114">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="2b995-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2b995-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="2b995-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="2b995-116">Not Supported.</span></span>                              |
| <span data-ttu-id="2b995-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2b995-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2b995-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="2b995-118">Not Supported.</span></span>                              |
| <span data-ttu-id="2b995-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="2b995-119">Application</span></span>                            | <span data-ttu-id="2b995-120">无。</span><span class="sxs-lookup"><span data-stu-id="2b995-120">None.</span></span>                                       |

## <a name="http-request"></a><span data-ttu-id="2b995-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2b995-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/cancelMediaProcessing
POST /communications/calls/{id}/cancelMediaProcessing
```
> <span data-ttu-id="2b995-122">**注意：**`/app` 路径已弃用。</span><span class="sxs-lookup"><span data-stu-id="2b995-122">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="2b995-123">今后将使用 `/communications` 路径。</span><span class="sxs-lookup"><span data-stu-id="2b995-123">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2b995-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="2b995-124">Request headers</span></span>
| <span data-ttu-id="2b995-125">名称</span><span class="sxs-lookup"><span data-stu-id="2b995-125">Name</span></span>          | <span data-ttu-id="2b995-126">说明</span><span class="sxs-lookup"><span data-stu-id="2b995-126">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="2b995-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="2b995-127">Authorization</span></span> | <span data-ttu-id="2b995-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2b995-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2b995-130">Content-type</span><span class="sxs-lookup"><span data-stu-id="2b995-130">Content-type</span></span> | <span data-ttu-id="2b995-p105">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="2b995-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2b995-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="2b995-133">Request body</span></span>
<span data-ttu-id="2b995-134">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="2b995-134">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="2b995-135">参数</span><span class="sxs-lookup"><span data-stu-id="2b995-135">Parameter</span></span>      | <span data-ttu-id="2b995-136">类型</span><span class="sxs-lookup"><span data-stu-id="2b995-136">Type</span></span>    | <span data-ttu-id="2b995-137">说明</span><span class="sxs-lookup"><span data-stu-id="2b995-137">Description</span></span>                                                    |
|:---------------|:--------|:---------------------------------------------------------------|
| <span data-ttu-id="2b995-138">适用</span><span class="sxs-lookup"><span data-stu-id="2b995-138">clientContext</span></span>  | <span data-ttu-id="2b995-139">String</span><span class="sxs-lookup"><span data-stu-id="2b995-139">String</span></span>  | <span data-ttu-id="2b995-140">客户端上下文。</span><span class="sxs-lookup"><span data-stu-id="2b995-140">The client context.</span></span>                                            |

## <a name="response"></a><span data-ttu-id="2b995-141">响应</span><span class="sxs-lookup"><span data-stu-id="2b995-141">Response</span></span>
<span data-ttu-id="2b995-142">如果成功，此方法将返回一个 `200 OK` HTTP 响应代码和一个位置标头，其中包含为此请求创建的 [COMMSOPERATION](../resources/commsoperation.md) 的 URI。</span><span class="sxs-lookup"><span data-stu-id="2b995-142">If successful, this method returns a `200 OK` HTTP response code and a Location header with a URI to the [commsOperation](../resources/commsoperation.md) created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="2b995-143">示例</span><span class="sxs-lookup"><span data-stu-id="2b995-143">Example</span></span>
<span data-ttu-id="2b995-144">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="2b995-144">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="2b995-145">请求</span><span class="sxs-lookup"><span data-stu-id="2b995-145">Request</span></span>
<span data-ttu-id="2b995-146">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="2b995-146">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="2b995-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="2b995-147">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="2b995-148">C#</span><span class="sxs-lookup"><span data-stu-id="2b995-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-cancelmediaprocessing-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2b995-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2b995-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-cancelmediaprocessing-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2b995-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2b995-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-cancelmediaprocessing-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="2b995-151">响应</span><span class="sxs-lookup"><span data-stu-id="2b995-151">Response</span></span>

> <span data-ttu-id="2b995-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="2b995-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

##### <a name="notification---operation-canceled-for-recordresponse"></a><span data-ttu-id="2b995-154">通知-已取消对 recordResponse 的操作</span><span class="sxs-lookup"><span data-stu-id="2b995-154">Notification - Operation canceled for recordResponse</span></span>

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



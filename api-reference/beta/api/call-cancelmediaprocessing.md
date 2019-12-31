---
title: 调用： cancelMediaProcessing
description: 取消对任何正在进行的 PlayPrompt 或 RecordResponse 操作的媒体处理。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: a11b42affaa2cc4c21dd50e2d2474f3e2ffa77d1
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/31/2019
ms.locfileid: "40912918"
---
# <a name="call-cancelmediaprocessing"></a><span data-ttu-id="50a3e-103">调用： cancelMediaProcessing</span><span class="sxs-lookup"><span data-stu-id="50a3e-103">call: cancelMediaProcessing</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="50a3e-104">取消对任何正在进行的[播放提示](./call-playprompt.md)或[记录响应](./call-record.md)操作的处理。</span><span class="sxs-lookup"><span data-stu-id="50a3e-104">Cancels processing for any in-progress [play prompt](./call-playprompt.md) or [record response](./call-record.md) operations.</span></span>

## <a name="permissions"></a><span data-ttu-id="50a3e-105">权限</span><span class="sxs-lookup"><span data-stu-id="50a3e-105">Permissions</span></span>
<span data-ttu-id="50a3e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="50a3e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="50a3e-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="50a3e-108">Permission type</span></span>                        | <span data-ttu-id="50a3e-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="50a3e-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="50a3e-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="50a3e-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="50a3e-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="50a3e-111">Not Supported.</span></span>                              |
| <span data-ttu-id="50a3e-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="50a3e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="50a3e-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="50a3e-113">Not Supported.</span></span>                              |
| <span data-ttu-id="50a3e-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="50a3e-114">Application</span></span>                            | <span data-ttu-id="50a3e-115">无。</span><span class="sxs-lookup"><span data-stu-id="50a3e-115">None.</span></span>                                       |

## <a name="http-request"></a><span data-ttu-id="50a3e-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="50a3e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/cancelMediaProcessing
POST /communications/calls/{id}/cancelMediaProcessing
```
> <span data-ttu-id="50a3e-117">**注意：**`/app` 路径已弃用。</span><span class="sxs-lookup"><span data-stu-id="50a3e-117">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="50a3e-118">今后将使用 `/communications` 路径。</span><span class="sxs-lookup"><span data-stu-id="50a3e-118">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="50a3e-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="50a3e-119">Request headers</span></span>
| <span data-ttu-id="50a3e-120">名称</span><span class="sxs-lookup"><span data-stu-id="50a3e-120">Name</span></span>          | <span data-ttu-id="50a3e-121">说明</span><span class="sxs-lookup"><span data-stu-id="50a3e-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="50a3e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="50a3e-122">Authorization</span></span> | <span data-ttu-id="50a3e-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="50a3e-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="50a3e-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="50a3e-125">Content-type</span></span> | <span data-ttu-id="50a3e-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="50a3e-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="50a3e-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="50a3e-128">Request body</span></span>
<span data-ttu-id="50a3e-129">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="50a3e-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="50a3e-130">参数</span><span class="sxs-lookup"><span data-stu-id="50a3e-130">Parameter</span></span>      | <span data-ttu-id="50a3e-131">类型</span><span class="sxs-lookup"><span data-stu-id="50a3e-131">Type</span></span>    | <span data-ttu-id="50a3e-132">说明</span><span class="sxs-lookup"><span data-stu-id="50a3e-132">Description</span></span>                                                    |
|:---------------|:--------|:---------------------------------------------------------------|
| <span data-ttu-id="50a3e-133">适用</span><span class="sxs-lookup"><span data-stu-id="50a3e-133">clientContext</span></span>  | <span data-ttu-id="50a3e-134">String</span><span class="sxs-lookup"><span data-stu-id="50a3e-134">String</span></span>  | <span data-ttu-id="50a3e-135">客户端上下文。</span><span class="sxs-lookup"><span data-stu-id="50a3e-135">The client context.</span></span>                                            |

## <a name="response"></a><span data-ttu-id="50a3e-136">响应</span><span class="sxs-lookup"><span data-stu-id="50a3e-136">Response</span></span>
<span data-ttu-id="50a3e-137">如果成功，此方法将返回`200 OK`一个 HTTP 响应代码和一个位置标头，其中包含为此请求创建的[commsOperation](../resources/commsoperation.md)的 URI。</span><span class="sxs-lookup"><span data-stu-id="50a3e-137">If successful, this method returns a `200 OK` HTTP response code and a Location header with a URI to the [commsOperation](../resources/commsoperation.md) created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="50a3e-138">示例</span><span class="sxs-lookup"><span data-stu-id="50a3e-138">Example</span></span>
<span data-ttu-id="50a3e-139">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="50a3e-139">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="50a3e-140">请求</span><span class="sxs-lookup"><span data-stu-id="50a3e-140">Request</span></span>
<span data-ttu-id="50a3e-141">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="50a3e-141">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="50a3e-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="50a3e-142">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="50a3e-143">C#</span><span class="sxs-lookup"><span data-stu-id="50a3e-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-cancelmediaprocessing-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="50a3e-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="50a3e-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-cancelmediaprocessing-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="50a3e-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="50a3e-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-cancelmediaprocessing-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="50a3e-146">响应</span><span class="sxs-lookup"><span data-stu-id="50a3e-146">Response</span></span>

> <span data-ttu-id="50a3e-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="50a3e-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

##### <a name="notification---operation-canceled-for-recordresponse"></a><span data-ttu-id="50a3e-149">通知-已取消对 recordResponse 的操作</span><span class="sxs-lookup"><span data-stu-id="50a3e-149">Notification - Operation canceled for recordResponse</span></span>

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
          "message": "Action falied, the operation was cancelled."
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

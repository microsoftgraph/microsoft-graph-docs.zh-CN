---
title: 调用： cancelMediaProcessing
description: 取消对任何正在进行的 PlayPrompt 或 RecordResponse 操作的媒体处理。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 0f9ec0eaede3383d6e99a05e4aa4023dd914d9b3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42440883"
---
# <a name="call-cancelmediaprocessing"></a><span data-ttu-id="66da7-103">调用： cancelMediaProcessing</span><span class="sxs-lookup"><span data-stu-id="66da7-103">call: cancelMediaProcessing</span></span>

<span data-ttu-id="66da7-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="66da7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="66da7-105">取消对任何正在进行的[播放提示](./call-playprompt.md)或[记录响应](./call-record.md)操作的处理。</span><span class="sxs-lookup"><span data-stu-id="66da7-105">Cancels processing for any in-progress [play prompt](./call-playprompt.md) or [record response](./call-record.md) operations.</span></span>

## <a name="permissions"></a><span data-ttu-id="66da7-106">权限</span><span class="sxs-lookup"><span data-stu-id="66da7-106">Permissions</span></span>
<span data-ttu-id="66da7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="66da7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="66da7-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="66da7-109">Permission type</span></span>                        | <span data-ttu-id="66da7-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="66da7-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="66da7-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="66da7-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="66da7-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="66da7-112">Not Supported.</span></span>                              |
| <span data-ttu-id="66da7-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="66da7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="66da7-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="66da7-114">Not Supported.</span></span>                              |
| <span data-ttu-id="66da7-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="66da7-115">Application</span></span>                            | <span data-ttu-id="66da7-116">无。</span><span class="sxs-lookup"><span data-stu-id="66da7-116">None.</span></span>                                       |

## <a name="http-request"></a><span data-ttu-id="66da7-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="66da7-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/cancelMediaProcessing
POST /communications/calls/{id}/cancelMediaProcessing
```
> <span data-ttu-id="66da7-118">**注意：**`/app` 路径已弃用。</span><span class="sxs-lookup"><span data-stu-id="66da7-118">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="66da7-119">今后将使用 `/communications` 路径。</span><span class="sxs-lookup"><span data-stu-id="66da7-119">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="66da7-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="66da7-120">Request headers</span></span>
| <span data-ttu-id="66da7-121">名称</span><span class="sxs-lookup"><span data-stu-id="66da7-121">Name</span></span>          | <span data-ttu-id="66da7-122">说明</span><span class="sxs-lookup"><span data-stu-id="66da7-122">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="66da7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="66da7-123">Authorization</span></span> | <span data-ttu-id="66da7-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="66da7-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="66da7-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="66da7-126">Content-type</span></span> | <span data-ttu-id="66da7-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="66da7-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="66da7-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="66da7-129">Request body</span></span>
<span data-ttu-id="66da7-130">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="66da7-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="66da7-131">参数</span><span class="sxs-lookup"><span data-stu-id="66da7-131">Parameter</span></span>      | <span data-ttu-id="66da7-132">类型</span><span class="sxs-lookup"><span data-stu-id="66da7-132">Type</span></span>    | <span data-ttu-id="66da7-133">说明</span><span class="sxs-lookup"><span data-stu-id="66da7-133">Description</span></span>                                                    |
|:---------------|:--------|:---------------------------------------------------------------|
| <span data-ttu-id="66da7-134">适用</span><span class="sxs-lookup"><span data-stu-id="66da7-134">clientContext</span></span>  | <span data-ttu-id="66da7-135">String</span><span class="sxs-lookup"><span data-stu-id="66da7-135">String</span></span>  | <span data-ttu-id="66da7-136">客户端上下文。</span><span class="sxs-lookup"><span data-stu-id="66da7-136">The client context.</span></span>                                            |

## <a name="response"></a><span data-ttu-id="66da7-137">响应</span><span class="sxs-lookup"><span data-stu-id="66da7-137">Response</span></span>
<span data-ttu-id="66da7-138">如果成功，此方法将返回`200 OK`一个 HTTP 响应代码和一个位置标头，其中包含为此请求创建的[commsOperation](../resources/commsoperation.md)的 URI。</span><span class="sxs-lookup"><span data-stu-id="66da7-138">If successful, this method returns a `200 OK` HTTP response code and a Location header with a URI to the [commsOperation](../resources/commsoperation.md) created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="66da7-139">示例</span><span class="sxs-lookup"><span data-stu-id="66da7-139">Example</span></span>
<span data-ttu-id="66da7-140">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="66da7-140">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="66da7-141">请求</span><span class="sxs-lookup"><span data-stu-id="66da7-141">Request</span></span>
<span data-ttu-id="66da7-142">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="66da7-142">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="66da7-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="66da7-143">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="66da7-144">C#</span><span class="sxs-lookup"><span data-stu-id="66da7-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-cancelmediaprocessing-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="66da7-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="66da7-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-cancelmediaprocessing-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="66da7-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="66da7-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-cancelmediaprocessing-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="66da7-147">响应</span><span class="sxs-lookup"><span data-stu-id="66da7-147">Response</span></span>

> <span data-ttu-id="66da7-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="66da7-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

##### <a name="notification---operation-canceled-for-recordresponse"></a><span data-ttu-id="66da7-150">通知-已取消对 recordResponse 的操作</span><span class="sxs-lookup"><span data-stu-id="66da7-150">Notification - Operation canceled for recordResponse</span></span>

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

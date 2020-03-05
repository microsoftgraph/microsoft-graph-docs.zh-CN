---
title: 调用： updateRecordingStatus
description: 更新与呼叫关联的应用程序的录制状态。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 7a86276b42244b6fc1443d07d5170175f7166a92
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42440680"
---
# <a name="call-updaterecordingstatus"></a><span data-ttu-id="a0cb1-103">调用： updateRecordingStatus</span><span class="sxs-lookup"><span data-stu-id="a0cb1-103">call: updateRecordingStatus</span></span>

<span data-ttu-id="a0cb1-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="a0cb1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a0cb1-105">更新与呼叫关联的应用程序的录制状态。</span><span class="sxs-lookup"><span data-stu-id="a0cb1-105">Update the application's recording status associated with a call.</span></span>

## <a name="permissions"></a><span data-ttu-id="a0cb1-106">权限</span><span class="sxs-lookup"><span data-stu-id="a0cb1-106">Permissions</span></span>
<span data-ttu-id="a0cb1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a0cb1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a0cb1-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="a0cb1-109">Permission type</span></span>                        | <span data-ttu-id="a0cb1-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a0cb1-110">Permissions (from least to most privileged)</span></span>      |
|:---------------------------------------|:-------------------------------------------------|
| <span data-ttu-id="a0cb1-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a0cb1-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="a0cb1-112">不支持</span><span class="sxs-lookup"><span data-stu-id="a0cb1-112">Not Supported</span></span>                                    |
| <span data-ttu-id="a0cb1-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a0cb1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a0cb1-114">不支持</span><span class="sxs-lookup"><span data-stu-id="a0cb1-114">Not Supported</span></span>                                    |
| <span data-ttu-id="a0cb1-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="a0cb1-115">Application</span></span>                            | <span data-ttu-id="a0cb1-116">JoinGroupCalls、AccessMedia 和所有调用</span><span class="sxs-lookup"><span data-stu-id="a0cb1-116">Calls.JoinGroupCalls.All, Calls.AccessMedia.All</span></span>  |

## <a name="http-request"></a><span data-ttu-id="a0cb1-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a0cb1-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/updateRecordingStatus
POST /communications/calls/{id}/updateRecordingStatus
```
> <span data-ttu-id="a0cb1-118">**注意：**`/app` 路径已弃用。</span><span class="sxs-lookup"><span data-stu-id="a0cb1-118">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="a0cb1-119">今后将使用 `/communications` 路径。</span><span class="sxs-lookup"><span data-stu-id="a0cb1-119">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a0cb1-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="a0cb1-120">Request headers</span></span>
| <span data-ttu-id="a0cb1-121">名称</span><span class="sxs-lookup"><span data-stu-id="a0cb1-121">Name</span></span>          | <span data-ttu-id="a0cb1-122">说明</span><span class="sxs-lookup"><span data-stu-id="a0cb1-122">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="a0cb1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a0cb1-123">Authorization</span></span> | <span data-ttu-id="a0cb1-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a0cb1-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a0cb1-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="a0cb1-126">Content-type</span></span> | <span data-ttu-id="a0cb1-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="a0cb1-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a0cb1-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="a0cb1-129">Request body</span></span>
<span data-ttu-id="a0cb1-130">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="a0cb1-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="a0cb1-131">参数</span><span class="sxs-lookup"><span data-stu-id="a0cb1-131">Parameter</span></span>       | <span data-ttu-id="a0cb1-132">类型</span><span class="sxs-lookup"><span data-stu-id="a0cb1-132">Type</span></span>    | <span data-ttu-id="a0cb1-133">说明</span><span class="sxs-lookup"><span data-stu-id="a0cb1-133">Description</span></span>                                                                           |
|:----------------|:--------|:--------------------------------------------------------------------------------------|
| <span data-ttu-id="a0cb1-134">适用</span><span class="sxs-lookup"><span data-stu-id="a0cb1-134">clientContext</span></span>   | <span data-ttu-id="a0cb1-135">String</span><span class="sxs-lookup"><span data-stu-id="a0cb1-135">String</span></span>  | <span data-ttu-id="a0cb1-136">唯一的客户端上下文字符串。</span><span class="sxs-lookup"><span data-stu-id="a0cb1-136">Unique Client Context string.</span></span> <span data-ttu-id="a0cb1-137">最大限制为256个字符。</span><span class="sxs-lookup"><span data-stu-id="a0cb1-137">Max limit is 256 chars.</span></span>                                 |
| <span data-ttu-id="a0cb1-138">status</span><span class="sxs-lookup"><span data-stu-id="a0cb1-138">status</span></span>          | <span data-ttu-id="a0cb1-139">String</span><span class="sxs-lookup"><span data-stu-id="a0cb1-139">String</span></span>  | <span data-ttu-id="a0cb1-140">录制状态。</span><span class="sxs-lookup"><span data-stu-id="a0cb1-140">The recording status.</span></span> <span data-ttu-id="a0cb1-141">可能的值包括`notRecording`： `recording`、或`failed`。</span><span class="sxs-lookup"><span data-stu-id="a0cb1-141">Possible values are: `notRecording`, `recording`, or `failed`.</span></span>  |

## <a name="response"></a><span data-ttu-id="a0cb1-142">响应</span><span class="sxs-lookup"><span data-stu-id="a0cb1-142">Response</span></span>
<span data-ttu-id="a0cb1-143">此方法返回`200 OK`响应代码和位置标头，其中包含为此请求创建的[UPDATERECORDINGSTATUSOPERATION](../resources/updaterecordingstatusoperation.md)对象的 URI。</span><span class="sxs-lookup"><span data-stu-id="a0cb1-143">This method returns a `200 OK` response code and a Location header with a URI to the [updateRecordingStatusOperation](../resources/updaterecordingstatusoperation.md) object created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="a0cb1-144">示例</span><span class="sxs-lookup"><span data-stu-id="a0cb1-144">Example</span></span>
<span data-ttu-id="a0cb1-145">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="a0cb1-145">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="a0cb1-146">请求</span><span class="sxs-lookup"><span data-stu-id="a0cb1-146">Request</span></span>
<span data-ttu-id="a0cb1-147">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="a0cb1-147">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="a0cb1-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="a0cb1-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-updateRecordingStatus"
}-->
```http
POST https://graph.microsoft.com/beta/communications/calls/{id}/updateRecordingStatus
Content-Type: application/json
Content-Length: 79

{
  "clientContext": "clientContext-value",
  "status": "notRecording | recording | failed"
}
```
# <a name="c"></a>[<span data-ttu-id="a0cb1-149">C#</span><span class="sxs-lookup"><span data-stu-id="a0cb1-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-updaterecordingstatus-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a0cb1-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a0cb1-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-updaterecordingstatus-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a0cb1-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a0cb1-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-updaterecordingstatus-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a0cb1-152">响应</span><span class="sxs-lookup"><span data-stu-id="a0cb1-152">Response</span></span>

> <span data-ttu-id="a0cb1-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="a0cb1-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "name": "call-updateRecordingStatus",
  "truncated": true,
  "@odata.type": "microsoft.graph.updateRecordingStatusOperation"
} -->
```http
HTTP/1.1 200 OK
Location: https://graph.microsoft.com/beta/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5

{
  "@odata.type": "#microsoft.graph.updateRecordingStatusOperation",
  "clientContext": "clientContext-value",
  "id": "0fe0623f-d628-42ed-b4bd-8ac290072cc5",
  "resultInfo": null,
  "status": "completed"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "call: updateRecordingStatus",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

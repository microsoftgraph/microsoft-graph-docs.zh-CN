---
title: 调用： updateRecordingStatus
description: 更新与呼叫关联的应用程序的录制状态。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 7e6312d862940aeff840e74094b4b1e75734634e
ms.sourcegitcommit: 66a52d2e63cf3447ec50bd28e562d99e7c344814
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2020
ms.locfileid: "43062565"
---
# <a name="call-updaterecordingstatus"></a><span data-ttu-id="09528-103">调用： updateRecordingStatus</span><span class="sxs-lookup"><span data-stu-id="09528-103">call: updateRecordingStatus</span></span>

<span data-ttu-id="09528-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="09528-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="09528-105">更新与呼叫关联的应用程序的录制状态。</span><span class="sxs-lookup"><span data-stu-id="09528-105">Update the application's recording status associated with a call.</span></span>

> <span data-ttu-id="09528-106">**其他限制**：不能使用媒体访问 API 来记录或保留来自应用程序访问的呼叫或会议的媒体内容，或从该媒体内容派生的数据（"record" 或 "record"），而无需先调用**updateRecordingStatus** API 来指示已开始录制，并从该 api 接收成功答复。</span><span class="sxs-lookup"><span data-stu-id="09528-106">**Additional Restriction**: You may NOT use the Media Access API to record or otherwise persist media content from calls or meetings that your application accesses, or data derived from that media content ("record" or "recording"), without first calling the **updateRecordingStatus** API to indicate that recording has begun, and receiving a success reply from that API.</span></span> <span data-ttu-id="09528-107">如果您的应用程序开始录制任何会议，则它必须在调用**updateRecordingStatus** API 之前结束录制，以指示录制已结束。</span><span class="sxs-lookup"><span data-stu-id="09528-107">If your application begins recording any meeting, it must end the recording prior to calling the **updateRecordingStatus** API to indicate that the recording has ended.</span></span>

## <a name="permissions"></a><span data-ttu-id="09528-108">权限</span><span class="sxs-lookup"><span data-stu-id="09528-108">Permissions</span></span>
<span data-ttu-id="09528-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="09528-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="09528-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="09528-111">Permission type</span></span>                        | <span data-ttu-id="09528-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="09528-112">Permissions (from least to most privileged)</span></span>      |
|:---------------------------------------|:-------------------------------------------------|
| <span data-ttu-id="09528-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="09528-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="09528-114">不支持</span><span class="sxs-lookup"><span data-stu-id="09528-114">Not Supported</span></span>                                    |
| <span data-ttu-id="09528-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="09528-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="09528-116">不支持</span><span class="sxs-lookup"><span data-stu-id="09528-116">Not Supported</span></span>                                    |
| <span data-ttu-id="09528-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="09528-117">Application</span></span>                            | <span data-ttu-id="09528-118">JoinGroupCalls、AccessMedia 和所有调用</span><span class="sxs-lookup"><span data-stu-id="09528-118">Calls.JoinGroupCalls.All, Calls.AccessMedia.All</span></span>  |

## <a name="http-request"></a><span data-ttu-id="09528-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="09528-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/updateRecordingStatus
POST /communications/calls/{id}/updateRecordingStatus
```
> <span data-ttu-id="09528-120">**注意：**`/app` 路径已弃用。</span><span class="sxs-lookup"><span data-stu-id="09528-120">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="09528-121">今后将使用 `/communications` 路径。</span><span class="sxs-lookup"><span data-stu-id="09528-121">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="09528-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="09528-122">Request headers</span></span>
| <span data-ttu-id="09528-123">名称</span><span class="sxs-lookup"><span data-stu-id="09528-123">Name</span></span>          | <span data-ttu-id="09528-124">说明</span><span class="sxs-lookup"><span data-stu-id="09528-124">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="09528-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="09528-125">Authorization</span></span> | <span data-ttu-id="09528-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="09528-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="09528-128">Content-type</span><span class="sxs-lookup"><span data-stu-id="09528-128">Content-type</span></span> | <span data-ttu-id="09528-p105">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="09528-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="09528-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="09528-131">Request body</span></span>
<span data-ttu-id="09528-132">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="09528-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="09528-133">参数</span><span class="sxs-lookup"><span data-stu-id="09528-133">Parameter</span></span>       | <span data-ttu-id="09528-134">类型</span><span class="sxs-lookup"><span data-stu-id="09528-134">Type</span></span>    | <span data-ttu-id="09528-135">说明</span><span class="sxs-lookup"><span data-stu-id="09528-135">Description</span></span>                                                                           |
|:----------------|:--------|:--------------------------------------------------------------------------------------|
| <span data-ttu-id="09528-136">适用</span><span class="sxs-lookup"><span data-stu-id="09528-136">clientContext</span></span>   | <span data-ttu-id="09528-137">String</span><span class="sxs-lookup"><span data-stu-id="09528-137">String</span></span>  | <span data-ttu-id="09528-138">唯一的客户端上下文字符串。</span><span class="sxs-lookup"><span data-stu-id="09528-138">Unique Client Context string.</span></span> <span data-ttu-id="09528-139">最大限制为256个字符。</span><span class="sxs-lookup"><span data-stu-id="09528-139">Max limit is 256 chars.</span></span>                                 |
| <span data-ttu-id="09528-140">状态</span><span class="sxs-lookup"><span data-stu-id="09528-140">status</span></span>          | <span data-ttu-id="09528-141">String</span><span class="sxs-lookup"><span data-stu-id="09528-141">String</span></span>  | <span data-ttu-id="09528-142">录制状态。</span><span class="sxs-lookup"><span data-stu-id="09528-142">The recording status.</span></span> <span data-ttu-id="09528-143">可能的值包括`notRecording`： `recording`、或`failed`。</span><span class="sxs-lookup"><span data-stu-id="09528-143">Possible values are: `notRecording`, `recording`, or `failed`.</span></span>  |

## <a name="response"></a><span data-ttu-id="09528-144">响应</span><span class="sxs-lookup"><span data-stu-id="09528-144">Response</span></span>
<span data-ttu-id="09528-145">此方法返回`200 OK`响应代码和位置标头，其中包含为此请求创建的[UPDATERECORDINGSTATUSOPERATION](../resources/updaterecordingstatusoperation.md)对象的 URI。</span><span class="sxs-lookup"><span data-stu-id="09528-145">This method returns a `200 OK` response code and a Location header with a URI to the [updateRecordingStatusOperation](../resources/updaterecordingstatusoperation.md) object created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="09528-146">示例</span><span class="sxs-lookup"><span data-stu-id="09528-146">Example</span></span>
<span data-ttu-id="09528-147">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="09528-147">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="09528-148">请求</span><span class="sxs-lookup"><span data-stu-id="09528-148">Request</span></span>
<span data-ttu-id="09528-149">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="09528-149">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="09528-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="09528-150">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="09528-151">C#</span><span class="sxs-lookup"><span data-stu-id="09528-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-updaterecordingstatus-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="09528-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="09528-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-updaterecordingstatus-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="09528-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="09528-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-updaterecordingstatus-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="09528-154">响应</span><span class="sxs-lookup"><span data-stu-id="09528-154">Response</span></span>

> <span data-ttu-id="09528-p108">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="09528-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

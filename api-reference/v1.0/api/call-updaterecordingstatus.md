---
title: 调用： updateRecordingStatus
description: 更新与呼叫关联的应用程序的录制状态。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 38ffbea47dd955526279bdacfd1efd665857a745
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/14/2020
ms.locfileid: "48461284"
---
# <a name="call-updaterecordingstatus"></a><span data-ttu-id="b24cc-103">调用： updateRecordingStatus</span><span class="sxs-lookup"><span data-stu-id="b24cc-103">call: updateRecordingStatus</span></span>

<span data-ttu-id="b24cc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b24cc-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b24cc-105">更新与呼叫关联的应用程序的录制状态。</span><span class="sxs-lookup"><span data-stu-id="b24cc-105">Update the application's recording status associated with a call.</span></span> <span data-ttu-id="b24cc-106">这需要使用 [基于团队策略的录制](/MicrosoftTeams/teams-recording-policy) 解决方案。</span><span class="sxs-lookup"><span data-stu-id="b24cc-106">This requires the use of the [Teams policy-based recording](/MicrosoftTeams/teams-recording-policy) solution.</span></span>

> <span data-ttu-id="b24cc-107">**其他限制**：不能使用媒体访问 API 记录或以其他方式保留应用程序访问的呼叫或会议中的媒体内容，或从该媒体内容派生的数据 ( "record" 或 "record" ) ，而无需先调用 **updateRecordingStatus** API 来指示已开始录制，并从该 api 接收成功答复。</span><span class="sxs-lookup"><span data-stu-id="b24cc-107">**Additional Restriction**: You may NOT use the Media Access API to record or otherwise persist media content from calls or meetings that your application accesses, or data derived from that media content ("record" or "recording"), without first calling the **updateRecordingStatus** API to indicate that recording has begun, and receiving a success reply from that API.</span></span> <span data-ttu-id="b24cc-108">如果您的应用程序开始录制任何会议，则它必须在调用 **updateRecordingStatus** API 之前结束录制，以指示录制已结束。</span><span class="sxs-lookup"><span data-stu-id="b24cc-108">If your application begins recording any meeting, it must end the recording prior to calling the **updateRecordingStatus** API to indicate that the recording has ended.</span></span>

## <a name="permissions"></a><span data-ttu-id="b24cc-109">Permissions</span><span class="sxs-lookup"><span data-stu-id="b24cc-109">Permissions</span></span>
<span data-ttu-id="b24cc-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b24cc-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b24cc-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="b24cc-112">Permission type</span></span>                        | <span data-ttu-id="b24cc-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b24cc-113">Permissions (from least to most privileged)</span></span>      |
|:---------------------------------------|:-------------------------------------------------|
| <span data-ttu-id="b24cc-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b24cc-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="b24cc-115">不支持</span><span class="sxs-lookup"><span data-stu-id="b24cc-115">Not Supported</span></span>                                    |
| <span data-ttu-id="b24cc-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b24cc-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b24cc-117">不支持</span><span class="sxs-lookup"><span data-stu-id="b24cc-117">Not Supported</span></span>                                    |
| <span data-ttu-id="b24cc-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="b24cc-118">Application</span></span>                            | <span data-ttu-id="b24cc-119">JoinGroupCalls、AccessMedia 和所有调用</span><span class="sxs-lookup"><span data-stu-id="b24cc-119">Calls.JoinGroupCalls.All, Calls.AccessMedia.All</span></span>  |

## <a name="http-request"></a><span data-ttu-id="b24cc-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b24cc-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /communications/calls/{id}/updateRecordingStatus
```

## <a name="request-headers"></a><span data-ttu-id="b24cc-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="b24cc-121">Request headers</span></span>
| <span data-ttu-id="b24cc-122">名称</span><span class="sxs-lookup"><span data-stu-id="b24cc-122">Name</span></span>          | <span data-ttu-id="b24cc-123">说明</span><span class="sxs-lookup"><span data-stu-id="b24cc-123">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="b24cc-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="b24cc-124">Authorization</span></span> | <span data-ttu-id="b24cc-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b24cc-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b24cc-127">Content-type</span><span class="sxs-lookup"><span data-stu-id="b24cc-127">Content-type</span></span> | <span data-ttu-id="b24cc-p105">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="b24cc-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b24cc-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="b24cc-130">Request body</span></span>
<span data-ttu-id="b24cc-131">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="b24cc-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b24cc-132">参数</span><span class="sxs-lookup"><span data-stu-id="b24cc-132">Parameter</span></span>       | <span data-ttu-id="b24cc-133">类型</span><span class="sxs-lookup"><span data-stu-id="b24cc-133">Type</span></span>    | <span data-ttu-id="b24cc-134">Description</span><span class="sxs-lookup"><span data-stu-id="b24cc-134">Description</span></span>                                                                           |
|:----------------|:--------|:--------------------------------------------------------------------------------------|
| <span data-ttu-id="b24cc-135">适用</span><span class="sxs-lookup"><span data-stu-id="b24cc-135">clientContext</span></span>   | <span data-ttu-id="b24cc-136">字符串</span><span class="sxs-lookup"><span data-stu-id="b24cc-136">String</span></span>  | <span data-ttu-id="b24cc-137">唯一的客户端上下文字符串。</span><span class="sxs-lookup"><span data-stu-id="b24cc-137">Unique client context string.</span></span> <span data-ttu-id="b24cc-138">最大限制为256个字符。</span><span class="sxs-lookup"><span data-stu-id="b24cc-138">Max limit is 256 chars.</span></span>                                 |
| <span data-ttu-id="b24cc-139">status</span><span class="sxs-lookup"><span data-stu-id="b24cc-139">status</span></span>          | <span data-ttu-id="b24cc-140">字符串</span><span class="sxs-lookup"><span data-stu-id="b24cc-140">String</span></span>  | <span data-ttu-id="b24cc-141">录制状态。</span><span class="sxs-lookup"><span data-stu-id="b24cc-141">The recording status.</span></span> <span data-ttu-id="b24cc-142">可能的值包括： `notRecording` 、 `recording` 或 `failed` 。</span><span class="sxs-lookup"><span data-stu-id="b24cc-142">Possible values are: `notRecording`, `recording`, or `failed`.</span></span>  |

## <a name="response"></a><span data-ttu-id="b24cc-143">响应</span><span class="sxs-lookup"><span data-stu-id="b24cc-143">Response</span></span>
<span data-ttu-id="b24cc-144">此方法返回 `200 OK` 响应代码和位置标头，其中包含为此请求创建的 [updateRecordingStatusOperation](../resources/updaterecordingstatusoperation.md) 对象的 URI。</span><span class="sxs-lookup"><span data-stu-id="b24cc-144">This method returns a `200 OK` response code and a Location header with a URI to the [updateRecordingStatusOperation](../resources/updaterecordingstatusoperation.md) object created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="b24cc-145">示例</span><span class="sxs-lookup"><span data-stu-id="b24cc-145">Example</span></span>
<span data-ttu-id="b24cc-146">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="b24cc-146">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="b24cc-147">请求</span><span class="sxs-lookup"><span data-stu-id="b24cc-147">Request</span></span>
<span data-ttu-id="b24cc-148">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="b24cc-148">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="b24cc-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="b24cc-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-updateRecordingStatus"
}-->
```http
POST https://graph.microsoft.com/v1.0/communications/calls/{id}/updateRecordingStatus
Content-Type: application/json
Content-Length: 79

{
  "clientContext": "clientContext-value",
  "status": "notRecording | recording | failed"
}
```
# <a name="c"></a>[<span data-ttu-id="b24cc-150">C#</span><span class="sxs-lookup"><span data-stu-id="b24cc-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-updaterecordingstatus-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b24cc-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b24cc-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-updaterecordingstatus-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b24cc-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b24cc-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-updaterecordingstatus-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b24cc-153">Java</span><span class="sxs-lookup"><span data-stu-id="b24cc-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/call-updaterecordingstatus-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---

### <a name="response"></a><span data-ttu-id="b24cc-154">响应</span><span class="sxs-lookup"><span data-stu-id="b24cc-154">Response</span></span>

> <span data-ttu-id="b24cc-p108">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="b24cc-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "name": "call-updateRecordingStatus",
  "truncated": true,
  "@odata.type": "microsoft.graph.updateRecordingStatusOperation"
} -->
```http
HTTP/1.1 200 OK
Location: https://graph.microsoft.com/v1.0/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5

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

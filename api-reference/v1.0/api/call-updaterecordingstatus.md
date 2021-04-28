---
title: call： updateRecordingStatus
description: 更新与呼叫关联的应用程序录制状态。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: f9581584e415bd52b402ab6c677378e7f4cb8d8d
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052486"
---
# <a name="call-updaterecordingstatus"></a><span data-ttu-id="583e7-103">call： updateRecordingStatus</span><span class="sxs-lookup"><span data-stu-id="583e7-103">call: updateRecordingStatus</span></span>

<span data-ttu-id="583e7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="583e7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="583e7-105">更新与呼叫关联的应用程序录制状态。</span><span class="sxs-lookup"><span data-stu-id="583e7-105">Update the application's recording status associated with a call.</span></span> <span data-ttu-id="583e7-106">这需要使用基于Teams[录制解决方案](/MicrosoftTeams/teams-recording-policy)。</span><span class="sxs-lookup"><span data-stu-id="583e7-106">This requires the use of the [Teams policy-based recording](/MicrosoftTeams/teams-recording-policy) solution.</span></span>

> <span data-ttu-id="583e7-107">其他限制：如果不首先调用 **updateRecordingStatus** API 以指示录制已开始，并且从该 API 收到成功回复，则不得使用媒体访问 API 记录或以其他方式保留应用程序访问的呼叫或会议中的媒体内容，或者记录派生自该媒体内容 ("record"或"recording") 的数据。</span><span class="sxs-lookup"><span data-stu-id="583e7-107">**Additional Restriction**: You may NOT use the Media Access API to record or otherwise persist media content from calls or meetings that your application accesses, or data derived from that media content ("record" or "recording"), without first calling the **updateRecordingStatus** API to indicate that recording has begun, and receiving a success reply from that API.</span></span> <span data-ttu-id="583e7-108">如果应用程序开始录制任何会议，则必须在调用 **updateRecordingStatus** API 之前结束录制，以指示录制已结束。</span><span class="sxs-lookup"><span data-stu-id="583e7-108">If your application begins recording any meeting, it must end the recording prior to calling the **updateRecordingStatus** API to indicate that the recording has ended.</span></span>

## <a name="permissions"></a><span data-ttu-id="583e7-109">权限</span><span class="sxs-lookup"><span data-stu-id="583e7-109">Permissions</span></span>
<span data-ttu-id="583e7-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="583e7-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="583e7-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="583e7-112">Permission type</span></span>                        | <span data-ttu-id="583e7-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="583e7-113">Permissions (from least to most privileged)</span></span>      |
|:---------------------------------------|:-------------------------------------------------|
| <span data-ttu-id="583e7-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="583e7-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="583e7-115">不支持</span><span class="sxs-lookup"><span data-stu-id="583e7-115">Not Supported</span></span>                                    |
| <span data-ttu-id="583e7-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="583e7-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="583e7-117">不支持</span><span class="sxs-lookup"><span data-stu-id="583e7-117">Not Supported</span></span>                                    |
| <span data-ttu-id="583e7-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="583e7-118">Application</span></span>                            | <span data-ttu-id="583e7-119">Calls.JoinGroupCalls.All、Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="583e7-119">Calls.JoinGroupCalls.All, Calls.AccessMedia.All</span></span>  |

## <a name="http-request"></a><span data-ttu-id="583e7-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="583e7-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /communications/calls/{id}/updateRecordingStatus
```

## <a name="request-headers"></a><span data-ttu-id="583e7-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="583e7-121">Request headers</span></span>
| <span data-ttu-id="583e7-122">名称</span><span class="sxs-lookup"><span data-stu-id="583e7-122">Name</span></span>          | <span data-ttu-id="583e7-123">说明</span><span class="sxs-lookup"><span data-stu-id="583e7-123">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="583e7-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="583e7-124">Authorization</span></span> | <span data-ttu-id="583e7-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="583e7-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="583e7-127">Content-type</span><span class="sxs-lookup"><span data-stu-id="583e7-127">Content-type</span></span> | <span data-ttu-id="583e7-p105">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="583e7-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="583e7-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="583e7-130">Request body</span></span>
<span data-ttu-id="583e7-131">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="583e7-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="583e7-132">参数</span><span class="sxs-lookup"><span data-stu-id="583e7-132">Parameter</span></span>       | <span data-ttu-id="583e7-133">类型</span><span class="sxs-lookup"><span data-stu-id="583e7-133">Type</span></span>    | <span data-ttu-id="583e7-134">说明</span><span class="sxs-lookup"><span data-stu-id="583e7-134">Description</span></span>                                                                           |
|:----------------|:--------|:--------------------------------------------------------------------------------------|
| <span data-ttu-id="583e7-135">clientContext</span><span class="sxs-lookup"><span data-stu-id="583e7-135">clientContext</span></span>   | <span data-ttu-id="583e7-136">String</span><span class="sxs-lookup"><span data-stu-id="583e7-136">String</span></span>  | <span data-ttu-id="583e7-137">唯一的客户端上下文字符串。</span><span class="sxs-lookup"><span data-stu-id="583e7-137">Unique client context string.</span></span> <span data-ttu-id="583e7-138">最大限制为 256 个字符。</span><span class="sxs-lookup"><span data-stu-id="583e7-138">Max limit is 256 chars.</span></span>                                 |
| <span data-ttu-id="583e7-139">状态</span><span class="sxs-lookup"><span data-stu-id="583e7-139">status</span></span>          | <span data-ttu-id="583e7-140">String</span><span class="sxs-lookup"><span data-stu-id="583e7-140">String</span></span>  | <span data-ttu-id="583e7-141">录制状态。</span><span class="sxs-lookup"><span data-stu-id="583e7-141">The recording status.</span></span> <span data-ttu-id="583e7-142">可能的值为： `notRecording`、 `recording`或 `failed`。</span><span class="sxs-lookup"><span data-stu-id="583e7-142">Possible values are: `notRecording`, `recording`, or `failed`.</span></span>  |

## <a name="response"></a><span data-ttu-id="583e7-143">响应</span><span class="sxs-lookup"><span data-stu-id="583e7-143">Response</span></span>
<span data-ttu-id="583e7-144">此方法向为此 `200 OK` 请求创建的 [updateRecordingStatusOperation](../resources/updaterecordingstatusoperation.md) 对象返回响应代码和具有 URI 的位置标头。</span><span class="sxs-lookup"><span data-stu-id="583e7-144">This method returns a `200 OK` response code and a Location header with a URI to the [updateRecordingStatusOperation](../resources/updaterecordingstatusoperation.md) object created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="583e7-145">示例</span><span class="sxs-lookup"><span data-stu-id="583e7-145">Example</span></span>
<span data-ttu-id="583e7-146">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="583e7-146">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="583e7-147">请求</span><span class="sxs-lookup"><span data-stu-id="583e7-147">Request</span></span>
<span data-ttu-id="583e7-148">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="583e7-148">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="583e7-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="583e7-149">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="583e7-150">C#</span><span class="sxs-lookup"><span data-stu-id="583e7-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-updaterecordingstatus-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="583e7-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="583e7-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-updaterecordingstatus-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="583e7-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="583e7-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-updaterecordingstatus-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="583e7-153">Java</span><span class="sxs-lookup"><span data-stu-id="583e7-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/call-updaterecordingstatus-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---

### <a name="response"></a><span data-ttu-id="583e7-154">响应</span><span class="sxs-lookup"><span data-stu-id="583e7-154">Response</span></span>

> <span data-ttu-id="583e7-155">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="583e7-155">**Note:** The response object shown here might be shortened for readability.</span></span>

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

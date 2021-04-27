---
title: call： updateRecordingStatus
description: 更新与呼叫关联的应用程序录制状态。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 69893f1ff55a080e94ded88722614856c0dcf8c2
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047593"
---
# <a name="call-updaterecordingstatus"></a><span data-ttu-id="0af41-103">call： updateRecordingStatus</span><span class="sxs-lookup"><span data-stu-id="0af41-103">call: updateRecordingStatus</span></span>

<span data-ttu-id="0af41-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0af41-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0af41-105">更新与呼叫关联的应用程序录制状态。</span><span class="sxs-lookup"><span data-stu-id="0af41-105">Update the application's recording status associated with a call.</span></span> <span data-ttu-id="0af41-106">这需要使用基于Teams[录制解决方案](/MicrosoftTeams/teams-recording-policy)。</span><span class="sxs-lookup"><span data-stu-id="0af41-106">This requires the use of the [Teams policy-based recording](/MicrosoftTeams/teams-recording-policy) solution.</span></span>

> <span data-ttu-id="0af41-107">其他限制：如果不首先调用 **updateRecordingStatus** API 以指示录制已开始，并且从该 API 收到成功回复，则不得使用媒体访问 API 记录或以其他方式保留应用程序访问的呼叫或会议中的媒体内容，或者记录派生自该媒体内容 ("record"或"recording") 的数据。</span><span class="sxs-lookup"><span data-stu-id="0af41-107">**Additional Restriction**: You may NOT use the Media Access API to record or otherwise persist media content from calls or meetings that your application accesses, or data derived from that media content ("record" or "recording"), without first calling the **updateRecordingStatus** API to indicate that recording has begun, and receiving a success reply from that API.</span></span> <span data-ttu-id="0af41-108">如果应用程序开始录制任何会议，则必须在调用 **updateRecordingStatus** API 之前结束录制，以指示录制已结束。</span><span class="sxs-lookup"><span data-stu-id="0af41-108">If your application begins recording any meeting, it must end the recording prior to calling the **updateRecordingStatus** API to indicate that the recording has ended.</span></span>

## <a name="permissions"></a><span data-ttu-id="0af41-109">权限</span><span class="sxs-lookup"><span data-stu-id="0af41-109">Permissions</span></span>
<span data-ttu-id="0af41-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0af41-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0af41-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="0af41-112">Permission type</span></span>                        | <span data-ttu-id="0af41-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0af41-113">Permissions (from least to most privileged)</span></span>      |
|:---------------------------------------|:-------------------------------------------------|
| <span data-ttu-id="0af41-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0af41-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="0af41-115">不支持</span><span class="sxs-lookup"><span data-stu-id="0af41-115">Not Supported</span></span>                                    |
| <span data-ttu-id="0af41-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0af41-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0af41-117">不支持</span><span class="sxs-lookup"><span data-stu-id="0af41-117">Not Supported</span></span>                                    |
| <span data-ttu-id="0af41-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="0af41-118">Application</span></span>                            | <span data-ttu-id="0af41-119">Calls.JoinGroupCalls.All、Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="0af41-119">Calls.JoinGroupCalls.All, Calls.AccessMedia.All</span></span>  |

## <a name="http-request"></a><span data-ttu-id="0af41-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0af41-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/updateRecordingStatus
POST /communications/calls/{id}/updateRecordingStatus
```
> <span data-ttu-id="0af41-121">**注意：**`/app` 路径已弃用。</span><span class="sxs-lookup"><span data-stu-id="0af41-121">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="0af41-122">今后将使用 `/communications` 路径。</span><span class="sxs-lookup"><span data-stu-id="0af41-122">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0af41-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="0af41-123">Request headers</span></span>
| <span data-ttu-id="0af41-124">名称</span><span class="sxs-lookup"><span data-stu-id="0af41-124">Name</span></span>          | <span data-ttu-id="0af41-125">说明</span><span class="sxs-lookup"><span data-stu-id="0af41-125">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="0af41-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="0af41-126">Authorization</span></span> | <span data-ttu-id="0af41-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0af41-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0af41-129">Content-type</span><span class="sxs-lookup"><span data-stu-id="0af41-129">Content-type</span></span> | <span data-ttu-id="0af41-p106">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="0af41-p106">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0af41-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="0af41-132">Request body</span></span>
<span data-ttu-id="0af41-133">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="0af41-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="0af41-134">参数</span><span class="sxs-lookup"><span data-stu-id="0af41-134">Parameter</span></span>       | <span data-ttu-id="0af41-135">类型</span><span class="sxs-lookup"><span data-stu-id="0af41-135">Type</span></span>    | <span data-ttu-id="0af41-136">说明</span><span class="sxs-lookup"><span data-stu-id="0af41-136">Description</span></span>                                                                           |
|:----------------|:--------|:--------------------------------------------------------------------------------------|
| <span data-ttu-id="0af41-137">clientContext</span><span class="sxs-lookup"><span data-stu-id="0af41-137">clientContext</span></span>   | <span data-ttu-id="0af41-138">String</span><span class="sxs-lookup"><span data-stu-id="0af41-138">String</span></span>  | <span data-ttu-id="0af41-139">唯一的客户端上下文字符串。</span><span class="sxs-lookup"><span data-stu-id="0af41-139">Unique Client Context string.</span></span> <span data-ttu-id="0af41-140">最大限制为 256 个字符。</span><span class="sxs-lookup"><span data-stu-id="0af41-140">Max limit is 256 chars.</span></span>                                 |
| <span data-ttu-id="0af41-141">状态</span><span class="sxs-lookup"><span data-stu-id="0af41-141">status</span></span>          | <span data-ttu-id="0af41-142">String</span><span class="sxs-lookup"><span data-stu-id="0af41-142">String</span></span>  | <span data-ttu-id="0af41-143">录制状态。</span><span class="sxs-lookup"><span data-stu-id="0af41-143">The recording status.</span></span> <span data-ttu-id="0af41-144">可能的值为： `notRecording`、 `recording`或 `failed`。</span><span class="sxs-lookup"><span data-stu-id="0af41-144">Possible values are: `notRecording`, `recording`, or `failed`.</span></span>  |

## <a name="response"></a><span data-ttu-id="0af41-145">响应</span><span class="sxs-lookup"><span data-stu-id="0af41-145">Response</span></span>
<span data-ttu-id="0af41-146">此方法向为此 `200 OK` 请求创建的 [updateRecordingStatusOperation](../resources/updaterecordingstatusoperation.md) 对象返回响应代码和具有 URI 的位置标头。</span><span class="sxs-lookup"><span data-stu-id="0af41-146">This method returns a `200 OK` response code and a Location header with a URI to the [updateRecordingStatusOperation](../resources/updaterecordingstatusoperation.md) object created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="0af41-147">示例</span><span class="sxs-lookup"><span data-stu-id="0af41-147">Example</span></span>
<span data-ttu-id="0af41-148">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="0af41-148">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="0af41-149">请求</span><span class="sxs-lookup"><span data-stu-id="0af41-149">Request</span></span>
<span data-ttu-id="0af41-150">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="0af41-150">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="0af41-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="0af41-151">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="0af41-152">C#</span><span class="sxs-lookup"><span data-stu-id="0af41-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-updaterecordingstatus-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0af41-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0af41-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-updaterecordingstatus-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0af41-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0af41-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-updaterecordingstatus-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0af41-155">Java</span><span class="sxs-lookup"><span data-stu-id="0af41-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/call-updaterecordingstatus-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0af41-156">响应</span><span class="sxs-lookup"><span data-stu-id="0af41-156">Response</span></span>

> <span data-ttu-id="0af41-157">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="0af41-157">**Note:** The response object shown here might be shortened for readability.</span></span>

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

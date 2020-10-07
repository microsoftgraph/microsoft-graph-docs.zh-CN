---
title: 调用： updateRecordingStatus
description: 更新与呼叫关联的应用程序的录制状态。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 8220ec180180cddb32e6f4f119c71f5ccbcc6ab9
ms.sourcegitcommit: c20276369a8834a259f24038e7ee5c33de02660b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/07/2020
ms.locfileid: "48372038"
---
# <a name="call-updaterecordingstatus"></a><span data-ttu-id="63168-103">调用： updateRecordingStatus</span><span class="sxs-lookup"><span data-stu-id="63168-103">call: updateRecordingStatus</span></span>

<span data-ttu-id="63168-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="63168-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="63168-105">更新与呼叫关联的应用程序的录制状态。</span><span class="sxs-lookup"><span data-stu-id="63168-105">Update the application's recording status associated with a call.</span></span> <span data-ttu-id="63168-106">这需要使用 [基于团队策略的录制](/MicrosoftTeams/teams-recording-policy) 解决方案。</span><span class="sxs-lookup"><span data-stu-id="63168-106">This requires the use of the [Teams policy-based recording](/MicrosoftTeams/teams-recording-policy) solution.</span></span>

> <span data-ttu-id="63168-107">**其他限制**：不能使用媒体访问 API 记录或以其他方式保留应用程序访问的呼叫或会议中的媒体内容，或从该媒体内容派生的数据 ( "record" 或 "record" ) ，而无需先调用 **updateRecordingStatus** API 来指示已开始录制，并从该 api 接收成功答复。</span><span class="sxs-lookup"><span data-stu-id="63168-107">**Additional Restriction**: You may NOT use the Media Access API to record or otherwise persist media content from calls or meetings that your application accesses, or data derived from that media content ("record" or "recording"), without first calling the **updateRecordingStatus** API to indicate that recording has begun, and receiving a success reply from that API.</span></span> <span data-ttu-id="63168-108">如果您的应用程序开始录制任何会议，则它必须在调用 **updateRecordingStatus** API 之前结束录制，以指示录制已结束。</span><span class="sxs-lookup"><span data-stu-id="63168-108">If your application begins recording any meeting, it must end the recording prior to calling the **updateRecordingStatus** API to indicate that the recording has ended.</span></span>

## <a name="permissions"></a><span data-ttu-id="63168-109">权限</span><span class="sxs-lookup"><span data-stu-id="63168-109">Permissions</span></span>
<span data-ttu-id="63168-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="63168-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="63168-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="63168-112">Permission type</span></span>                        | <span data-ttu-id="63168-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="63168-113">Permissions (from least to most privileged)</span></span>      |
|:---------------------------------------|:-------------------------------------------------|
| <span data-ttu-id="63168-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="63168-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="63168-115">不支持</span><span class="sxs-lookup"><span data-stu-id="63168-115">Not Supported</span></span>                                    |
| <span data-ttu-id="63168-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="63168-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="63168-117">不支持</span><span class="sxs-lookup"><span data-stu-id="63168-117">Not Supported</span></span>                                    |
| <span data-ttu-id="63168-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="63168-118">Application</span></span>                            | <span data-ttu-id="63168-119">JoinGroupCalls、AccessMedia 和所有调用</span><span class="sxs-lookup"><span data-stu-id="63168-119">Calls.JoinGroupCalls.All, Calls.AccessMedia.All</span></span>  |

## <a name="http-request"></a><span data-ttu-id="63168-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="63168-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/updateRecordingStatus
POST /communications/calls/{id}/updateRecordingStatus
```
> <span data-ttu-id="63168-121">**注意：**`/app` 路径已弃用。</span><span class="sxs-lookup"><span data-stu-id="63168-121">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="63168-122">今后将使用 `/communications` 路径。</span><span class="sxs-lookup"><span data-stu-id="63168-122">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="63168-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="63168-123">Request headers</span></span>
| <span data-ttu-id="63168-124">名称</span><span class="sxs-lookup"><span data-stu-id="63168-124">Name</span></span>          | <span data-ttu-id="63168-125">说明</span><span class="sxs-lookup"><span data-stu-id="63168-125">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="63168-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="63168-126">Authorization</span></span> | <span data-ttu-id="63168-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="63168-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="63168-129">Content-type</span><span class="sxs-lookup"><span data-stu-id="63168-129">Content-type</span></span> | <span data-ttu-id="63168-p106">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="63168-p106">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="63168-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="63168-132">Request body</span></span>
<span data-ttu-id="63168-133">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="63168-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="63168-134">参数</span><span class="sxs-lookup"><span data-stu-id="63168-134">Parameter</span></span>       | <span data-ttu-id="63168-135">类型</span><span class="sxs-lookup"><span data-stu-id="63168-135">Type</span></span>    | <span data-ttu-id="63168-136">说明</span><span class="sxs-lookup"><span data-stu-id="63168-136">Description</span></span>                                                                           |
|:----------------|:--------|:--------------------------------------------------------------------------------------|
| <span data-ttu-id="63168-137">适用</span><span class="sxs-lookup"><span data-stu-id="63168-137">clientContext</span></span>   | <span data-ttu-id="63168-138">String</span><span class="sxs-lookup"><span data-stu-id="63168-138">String</span></span>  | <span data-ttu-id="63168-139">唯一的客户端上下文字符串。</span><span class="sxs-lookup"><span data-stu-id="63168-139">Unique Client Context string.</span></span> <span data-ttu-id="63168-140">最大限制为256个字符。</span><span class="sxs-lookup"><span data-stu-id="63168-140">Max limit is 256 chars.</span></span>                                 |
| <span data-ttu-id="63168-141">状态</span><span class="sxs-lookup"><span data-stu-id="63168-141">status</span></span>          | <span data-ttu-id="63168-142">String</span><span class="sxs-lookup"><span data-stu-id="63168-142">String</span></span>  | <span data-ttu-id="63168-143">录制状态。</span><span class="sxs-lookup"><span data-stu-id="63168-143">The recording status.</span></span> <span data-ttu-id="63168-144">可能的值包括： `notRecording` 、 `recording` 或 `failed` 。</span><span class="sxs-lookup"><span data-stu-id="63168-144">Possible values are: `notRecording`, `recording`, or `failed`.</span></span>  |

## <a name="response"></a><span data-ttu-id="63168-145">响应</span><span class="sxs-lookup"><span data-stu-id="63168-145">Response</span></span>
<span data-ttu-id="63168-146">此方法返回 `200 OK` 响应代码和位置标头，其中包含为此请求创建的 [updateRecordingStatusOperation](../resources/updaterecordingstatusoperation.md) 对象的 URI。</span><span class="sxs-lookup"><span data-stu-id="63168-146">This method returns a `200 OK` response code and a Location header with a URI to the [updateRecordingStatusOperation](../resources/updaterecordingstatusoperation.md) object created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="63168-147">示例</span><span class="sxs-lookup"><span data-stu-id="63168-147">Example</span></span>
<span data-ttu-id="63168-148">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="63168-148">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="63168-149">请求</span><span class="sxs-lookup"><span data-stu-id="63168-149">Request</span></span>
<span data-ttu-id="63168-150">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="63168-150">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="63168-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="63168-151">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="63168-152">C#</span><span class="sxs-lookup"><span data-stu-id="63168-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-updaterecordingstatus-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="63168-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="63168-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-updaterecordingstatus-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="63168-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="63168-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-updaterecordingstatus-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="63168-155">响应</span><span class="sxs-lookup"><span data-stu-id="63168-155">Response</span></span>

> <span data-ttu-id="63168-p109">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="63168-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

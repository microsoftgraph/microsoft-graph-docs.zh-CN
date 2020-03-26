---
title: 调用： updateRecordingStatus
description: 更新与呼叫关联的应用程序的录制状态。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: f1109cdaa02d5715335fd0948f64cff9bff8c4dd
ms.sourcegitcommit: 115890bc7e7a54db8a2befeb8f720a9ca94f42b5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/26/2020
ms.locfileid: "42962524"
---
# <a name="call-updaterecordingstatus"></a><span data-ttu-id="7990e-103">调用： updateRecordingStatus</span><span class="sxs-lookup"><span data-stu-id="7990e-103">call: updateRecordingStatus</span></span>

<span data-ttu-id="7990e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7990e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7990e-105">更新与呼叫关联的应用程序的录制状态。</span><span class="sxs-lookup"><span data-stu-id="7990e-105">Update the application's recording status associated with a call.</span></span>

> [!NOTE]
> <span data-ttu-id="7990e-106">**其他限制**：不能使用媒体访问 API 来记录或保留来自应用程序访问的呼叫或会议的媒体内容，或从该媒体内容派生的数据（"record" 或 "record"），而无需先调用**updateRecordingStatus** API 来指示已开始录制，并从该 api 接收成功答复。</span><span class="sxs-lookup"><span data-stu-id="7990e-106">**Additional Restriction**: You may NOT use the Media Access API to record or otherwise persist media content from calls or meetings that your application accesses, or data derived from that media content ("record" or "recording"), without first calling the **updateRecordingStatus** API to indicate that recording has begun, and receiving a success reply from that API.</span></span> <span data-ttu-id="7990e-107">如果您的应用程序开始录制任何会议，则它必须在调用**updateRecordingStatus** API 之前结束录制，以指示录制已结束。</span><span class="sxs-lookup"><span data-stu-id="7990e-107">If your application begins recording any meeting, it must end the recording prior to calling the **updateRecordingStatus** API to indicate that the recording has ended.</span></span>

## <a name="permissions"></a><span data-ttu-id="7990e-108">权限</span><span class="sxs-lookup"><span data-stu-id="7990e-108">Permissions</span></span>
<span data-ttu-id="7990e-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7990e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7990e-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="7990e-111">Permission type</span></span>                        | <span data-ttu-id="7990e-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7990e-112">Permissions (from least to most privileged)</span></span>      |
|:---------------------------------------|:-------------------------------------------------|
| <span data-ttu-id="7990e-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7990e-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="7990e-114">不支持</span><span class="sxs-lookup"><span data-stu-id="7990e-114">Not Supported</span></span>                                    |
| <span data-ttu-id="7990e-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7990e-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7990e-116">不支持</span><span class="sxs-lookup"><span data-stu-id="7990e-116">Not Supported</span></span>                                    |
| <span data-ttu-id="7990e-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="7990e-117">Application</span></span>                            | <span data-ttu-id="7990e-118">JoinGroupCalls、AccessMedia 和所有调用</span><span class="sxs-lookup"><span data-stu-id="7990e-118">Calls.JoinGroupCalls.All, Calls.AccessMedia.All</span></span>  |

## <a name="http-request"></a><span data-ttu-id="7990e-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7990e-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /communications/calls/{id}/updateRecordingStatus
```

## <a name="request-headers"></a><span data-ttu-id="7990e-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="7990e-120">Request headers</span></span>
| <span data-ttu-id="7990e-121">名称</span><span class="sxs-lookup"><span data-stu-id="7990e-121">Name</span></span>          | <span data-ttu-id="7990e-122">说明</span><span class="sxs-lookup"><span data-stu-id="7990e-122">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="7990e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7990e-123">Authorization</span></span> | <span data-ttu-id="7990e-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7990e-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7990e-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="7990e-126">Content-type</span></span> | <span data-ttu-id="7990e-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="7990e-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7990e-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="7990e-129">Request body</span></span>
<span data-ttu-id="7990e-130">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="7990e-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="7990e-131">参数</span><span class="sxs-lookup"><span data-stu-id="7990e-131">Parameter</span></span>       | <span data-ttu-id="7990e-132">类型</span><span class="sxs-lookup"><span data-stu-id="7990e-132">Type</span></span>    | <span data-ttu-id="7990e-133">说明</span><span class="sxs-lookup"><span data-stu-id="7990e-133">Description</span></span>                                                                           |
|:----------------|:--------|:--------------------------------------------------------------------------------------|
| <span data-ttu-id="7990e-134">适用</span><span class="sxs-lookup"><span data-stu-id="7990e-134">clientContext</span></span>   | <span data-ttu-id="7990e-135">String</span><span class="sxs-lookup"><span data-stu-id="7990e-135">String</span></span>  | <span data-ttu-id="7990e-136">唯一的客户端上下文字符串。</span><span class="sxs-lookup"><span data-stu-id="7990e-136">Unique client context string.</span></span> <span data-ttu-id="7990e-137">最大限制为256个字符。</span><span class="sxs-lookup"><span data-stu-id="7990e-137">Max limit is 256 chars.</span></span>                                 |
| <span data-ttu-id="7990e-138">状态</span><span class="sxs-lookup"><span data-stu-id="7990e-138">status</span></span>          | <span data-ttu-id="7990e-139">String</span><span class="sxs-lookup"><span data-stu-id="7990e-139">String</span></span>  | <span data-ttu-id="7990e-140">录制状态。</span><span class="sxs-lookup"><span data-stu-id="7990e-140">The recording status.</span></span> <span data-ttu-id="7990e-141">可能的值包括`notRecording`： `recording`、或`failed`。</span><span class="sxs-lookup"><span data-stu-id="7990e-141">Possible values are: `notRecording`, `recording`, or `failed`.</span></span>  |

## <a name="response"></a><span data-ttu-id="7990e-142">响应</span><span class="sxs-lookup"><span data-stu-id="7990e-142">Response</span></span>
<span data-ttu-id="7990e-143">此方法返回`200 OK`响应代码和位置标头，其中包含为此请求创建的[UPDATERECORDINGSTATUSOPERATION](../resources/updaterecordingstatusoperation.md)对象的 URI。</span><span class="sxs-lookup"><span data-stu-id="7990e-143">This method returns a `200 OK` response code and a Location header with a URI to the [updateRecordingStatusOperation](../resources/updaterecordingstatusoperation.md) object created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="7990e-144">示例</span><span class="sxs-lookup"><span data-stu-id="7990e-144">Example</span></span>
<span data-ttu-id="7990e-145">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="7990e-145">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="7990e-146">请求</span><span class="sxs-lookup"><span data-stu-id="7990e-146">Request</span></span>
<span data-ttu-id="7990e-147">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="7990e-147">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="7990e-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="7990e-148">HTTP</span></span>](#tab/http)
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
---

### <a name="response"></a><span data-ttu-id="7990e-149">响应</span><span class="sxs-lookup"><span data-stu-id="7990e-149">Response</span></span>

> <span data-ttu-id="7990e-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="7990e-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

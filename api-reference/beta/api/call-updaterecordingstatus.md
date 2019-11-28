---
title: 调用： updateRecordingStatus
description: 更新与呼叫关联的应用程序的录制状态。
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 90f550d50361d3e8ad1b0fd590cbad3e291d7b96
ms.sourcegitcommit: fce7ce328f0c88c6310af9cc85d12bcebc88a6c3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/28/2019
ms.locfileid: "39636867"
---
# <a name="call-updaterecordingstatus"></a><span data-ttu-id="5aad4-103">调用： updateRecordingStatus</span><span class="sxs-lookup"><span data-stu-id="5aad4-103">call: updateRecordingStatus</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5aad4-104">更新与呼叫关联的应用程序的录制状态。</span><span class="sxs-lookup"><span data-stu-id="5aad4-104">Update the application's recording status associated with a call.</span></span>

## <a name="permissions"></a><span data-ttu-id="5aad4-105">Permissions</span><span class="sxs-lookup"><span data-stu-id="5aad4-105">Permissions</span></span>
<span data-ttu-id="5aad4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5aad4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5aad4-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="5aad4-108">Permission type</span></span>                        | <span data-ttu-id="5aad4-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5aad4-109">Permissions (from least to most privileged)</span></span>      |
|:---------------------------------------|:-------------------------------------------------|
| <span data-ttu-id="5aad4-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5aad4-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="5aad4-111">不支持</span><span class="sxs-lookup"><span data-stu-id="5aad4-111">Not Supported</span></span>                                    |
| <span data-ttu-id="5aad4-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5aad4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5aad4-113">不支持</span><span class="sxs-lookup"><span data-stu-id="5aad4-113">Not Supported</span></span>                                    |
| <span data-ttu-id="5aad4-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="5aad4-114">Application</span></span>                            | <span data-ttu-id="5aad4-115">JoinGroupCalls、AccessMedia 和所有调用</span><span class="sxs-lookup"><span data-stu-id="5aad4-115">Calls.JoinGroupCalls.All, Calls.AccessMedia.All</span></span>  |

## <a name="http-request"></a><span data-ttu-id="5aad4-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5aad4-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/updateRecordingStatus
POST /communications/calls/{id}/updateRecordingStatus
```
> <span data-ttu-id="5aad4-117">**注意：**`/app` 路径已弃用。</span><span class="sxs-lookup"><span data-stu-id="5aad4-117">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="5aad4-118">今后将使用 `/communications` 路径。</span><span class="sxs-lookup"><span data-stu-id="5aad4-118">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5aad4-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="5aad4-119">Request headers</span></span>
| <span data-ttu-id="5aad4-120">名称</span><span class="sxs-lookup"><span data-stu-id="5aad4-120">Name</span></span>          | <span data-ttu-id="5aad4-121">说明</span><span class="sxs-lookup"><span data-stu-id="5aad4-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="5aad4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5aad4-122">Authorization</span></span> | <span data-ttu-id="5aad4-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5aad4-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5aad4-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="5aad4-125">Content-type</span></span> | <span data-ttu-id="5aad4-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="5aad4-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5aad4-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="5aad4-128">Request body</span></span>
<span data-ttu-id="5aad4-129">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="5aad4-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="5aad4-130">参数</span><span class="sxs-lookup"><span data-stu-id="5aad4-130">Parameter</span></span>       | <span data-ttu-id="5aad4-131">类型</span><span class="sxs-lookup"><span data-stu-id="5aad4-131">Type</span></span>    | <span data-ttu-id="5aad4-132">说明</span><span class="sxs-lookup"><span data-stu-id="5aad4-132">Description</span></span>                                                                           |
|:----------------|:--------|:--------------------------------------------------------------------------------------|
| <span data-ttu-id="5aad4-133">适用</span><span class="sxs-lookup"><span data-stu-id="5aad4-133">clientContext</span></span>   | <span data-ttu-id="5aad4-134">String</span><span class="sxs-lookup"><span data-stu-id="5aad4-134">String</span></span>  | <span data-ttu-id="5aad4-135">唯一的客户端上下文字符串。</span><span class="sxs-lookup"><span data-stu-id="5aad4-135">Unique Client Context string.</span></span> <span data-ttu-id="5aad4-136">最大限制为256个字符。</span><span class="sxs-lookup"><span data-stu-id="5aad4-136">Max limit is 256 chars.</span></span>                                 |
| <span data-ttu-id="5aad4-137">状态</span><span class="sxs-lookup"><span data-stu-id="5aad4-137">status</span></span>          | <span data-ttu-id="5aad4-138">String</span><span class="sxs-lookup"><span data-stu-id="5aad4-138">String</span></span>  | <span data-ttu-id="5aad4-139">录制状态。</span><span class="sxs-lookup"><span data-stu-id="5aad4-139">The recording status.</span></span> <span data-ttu-id="5aad4-140">可能的值包括`notRecording`： `recording`、或`failed`。</span><span class="sxs-lookup"><span data-stu-id="5aad4-140">Possible values are: `notRecording`, `recording`, or `failed`.</span></span>  |

## <a name="response"></a><span data-ttu-id="5aad4-141">响应</span><span class="sxs-lookup"><span data-stu-id="5aad4-141">Response</span></span>
<span data-ttu-id="5aad4-142">此方法返回`200 OK`响应代码和位置标头，其中包含为此请求创建的[UPDATERECORDINGSTATUSOPERATION](../resources/updaterecordingstatusoperation.md)对象的 URI。</span><span class="sxs-lookup"><span data-stu-id="5aad4-142">This method returns a `200 OK` response code and a Location header with a URI to the [updateRecordingStatusOperation](../resources/updaterecordingstatusoperation.md) object created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="5aad4-143">示例</span><span class="sxs-lookup"><span data-stu-id="5aad4-143">Example</span></span>
<span data-ttu-id="5aad4-144">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="5aad4-144">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="5aad4-145">请求</span><span class="sxs-lookup"><span data-stu-id="5aad4-145">Request</span></span>
<span data-ttu-id="5aad4-146">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="5aad4-146">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="5aad4-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="5aad4-147">HTTP</span></span>](#tab/http)
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

---


### <a name="response"></a><span data-ttu-id="5aad4-148">响应</span><span class="sxs-lookup"><span data-stu-id="5aad4-148">Response</span></span>

> <span data-ttu-id="5aad4-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="5aad4-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

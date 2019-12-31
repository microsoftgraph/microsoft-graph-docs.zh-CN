---
title: 参与者： muteAll
description: 将呼叫中的所有参与者设为静音。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 2ccf39562f3fe2e9ad3755388aa37e9264b7a486
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913098"
---
# <a name="participant-muteall"></a><span data-ttu-id="36f40-103">参与者： muteAll</span><span class="sxs-lookup"><span data-stu-id="36f40-103">participant: muteAll</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="36f40-104">将呼叫中的所有参与者设为静音。</span><span class="sxs-lookup"><span data-stu-id="36f40-104">Mute all participants in the call.</span></span>

> <span data-ttu-id="36f40-105">**注意：** 此 API 已弃用，将在2020年3月15日之前删除。</span><span class="sxs-lookup"><span data-stu-id="36f40-105">**Note:** This API is deprecated and will be removed by March 15th, 2020.</span></span> <span data-ttu-id="36f40-106">若要使单个参与者静音，请参阅[参与者：静音](participant-mute.md)。</span><span class="sxs-lookup"><span data-stu-id="36f40-106">To mute a single participant, see [participant: mute](participant-mute.md).</span></span>


## <a name="permissions"></a><span data-ttu-id="36f40-107">权限</span><span class="sxs-lookup"><span data-stu-id="36f40-107">Permissions</span></span>
<span data-ttu-id="36f40-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="36f40-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="36f40-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="36f40-110">Permission type</span></span>                        | <span data-ttu-id="36f40-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="36f40-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="36f40-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="36f40-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="36f40-113">不支持</span><span class="sxs-lookup"><span data-stu-id="36f40-113">Not Supported</span></span>                               |
| <span data-ttu-id="36f40-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="36f40-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="36f40-115">不支持</span><span class="sxs-lookup"><span data-stu-id="36f40-115">Not Supported</span></span>                               |
| <span data-ttu-id="36f40-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="36f40-116">Application</span></span>                            | <span data-ttu-id="36f40-117">无</span><span class="sxs-lookup"><span data-stu-id="36f40-117">None</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="36f40-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="36f40-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/participants/muteAll
POST /communications/calls/{id}/participants/muteAll
```
> <span data-ttu-id="36f40-119">**注意：**`/app` 路径已弃用。</span><span class="sxs-lookup"><span data-stu-id="36f40-119">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="36f40-120">今后将使用 `/communications` 路径。</span><span class="sxs-lookup"><span data-stu-id="36f40-120">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="36f40-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="36f40-121">Request headers</span></span>
| <span data-ttu-id="36f40-122">名称</span><span class="sxs-lookup"><span data-stu-id="36f40-122">Name</span></span>          | <span data-ttu-id="36f40-123">说明</span><span class="sxs-lookup"><span data-stu-id="36f40-123">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="36f40-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="36f40-124">Authorization</span></span> | <span data-ttu-id="36f40-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="36f40-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="36f40-127">Content-type</span><span class="sxs-lookup"><span data-stu-id="36f40-127">Content-type</span></span> | <span data-ttu-id="36f40-p105">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="36f40-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="36f40-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="36f40-130">Request body</span></span>
<span data-ttu-id="36f40-131">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="36f40-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="36f40-132">参数</span><span class="sxs-lookup"><span data-stu-id="36f40-132">Parameter</span></span>      | <span data-ttu-id="36f40-133">类型</span><span class="sxs-lookup"><span data-stu-id="36f40-133">Type</span></span>    |<span data-ttu-id="36f40-134">说明</span><span class="sxs-lookup"><span data-stu-id="36f40-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="36f40-135">participants</span><span class="sxs-lookup"><span data-stu-id="36f40-135">participants</span></span>|<span data-ttu-id="36f40-136">String collection</span><span class="sxs-lookup"><span data-stu-id="36f40-136">String collection</span></span>|<span data-ttu-id="36f40-137">要静音的参与者。</span><span class="sxs-lookup"><span data-stu-id="36f40-137">The participants to be muted.</span></span>|
|<span data-ttu-id="36f40-138">适用</span><span class="sxs-lookup"><span data-stu-id="36f40-138">clientContext</span></span>|<span data-ttu-id="36f40-139">String</span><span class="sxs-lookup"><span data-stu-id="36f40-139">String</span></span>|<span data-ttu-id="36f40-140">客户端上下文。</span><span class="sxs-lookup"><span data-stu-id="36f40-140">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="36f40-141">响应</span><span class="sxs-lookup"><span data-stu-id="36f40-141">Response</span></span>
<span data-ttu-id="36f40-142">如果成功，此方法在响应`200 OK`正文中返回响应代码和[commsOperation](../resources/commsoperation.md)对象。</span><span class="sxs-lookup"><span data-stu-id="36f40-142">If successful, this method returns a `200 OK` response code and a [commsOperation](../resources/commsoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="36f40-143">示例</span><span class="sxs-lookup"><span data-stu-id="36f40-143">Example</span></span>
<span data-ttu-id="36f40-144">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="36f40-144">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="36f40-145">请求</span><span class="sxs-lookup"><span data-stu-id="36f40-145">Request</span></span>
<span data-ttu-id="36f40-146">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="36f40-146">The following example shows the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="36f40-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="36f40-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "participant-muteAll"
}-->
```http
POST https://graph.microsoft.com/beta/communications/calls/{id}/participants/muteAll
Content-Type: application/json
Content-Length: 81

{
  "participants": [
    ""
  ],
  "clientContext": "clientContext-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="36f40-148">C#</span><span class="sxs-lookup"><span data-stu-id="36f40-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/participant-muteall-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="36f40-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="36f40-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/participant-muteall-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="36f40-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="36f40-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/participant-muteall-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="36f40-151">响应</span><span class="sxs-lookup"><span data-stu-id="36f40-151">Response</span></span>

> <span data-ttu-id="36f40-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="36f40-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "name": "participant-muteAll",
  "truncated": true,
  "@odata.type": "microsoft.graph.commsOperation"
} -->
```http
HTTP/1.1 200 OK
Location: https://graph.microsoft.com/beta/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5

{
  "@odata.type": "#microsoft.graph.commsOperation",
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
  "description": "participant: muteAll",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

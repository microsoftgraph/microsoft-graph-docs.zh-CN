---
title: 参与者： muteAll
description: 将呼叫中的所有参与者设为静音。
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 00ace588a763a9e6d1df64830820be1ad6308567
ms.sourcegitcommit: 9bddc0b7746383e8d05ce50d163af3f4196f12a6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/06/2019
ms.locfileid: "38006464"
---
# <a name="participant-muteall"></a><span data-ttu-id="94e23-103">参与者： muteAll</span><span class="sxs-lookup"><span data-stu-id="94e23-103">participant: muteAll</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="94e23-104">将呼叫中的所有参与者设为静音。</span><span class="sxs-lookup"><span data-stu-id="94e23-104">Mute all participants in the call.</span></span>

## <a name="permissions"></a><span data-ttu-id="94e23-105">Permissions</span><span class="sxs-lookup"><span data-stu-id="94e23-105">Permissions</span></span>
<span data-ttu-id="94e23-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="94e23-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="94e23-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="94e23-108">Permission type</span></span>                        | <span data-ttu-id="94e23-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="94e23-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="94e23-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="94e23-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="94e23-111">不支持</span><span class="sxs-lookup"><span data-stu-id="94e23-111">Not Supported</span></span>                               |
| <span data-ttu-id="94e23-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="94e23-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="94e23-113">不支持</span><span class="sxs-lookup"><span data-stu-id="94e23-113">Not Supported</span></span>                               |
| <span data-ttu-id="94e23-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="94e23-114">Application</span></span>                            | <span data-ttu-id="94e23-115">无</span><span class="sxs-lookup"><span data-stu-id="94e23-115">None</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="94e23-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="94e23-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/participants/muteAll
POST /communications/calls/{id}/participants/muteAll
```
> <span data-ttu-id="94e23-117">**注意：**`/app`路径已被弃用。</span><span class="sxs-lookup"><span data-stu-id="94e23-117">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="94e23-118">接下来，请使用`/communications`路径。</span><span class="sxs-lookup"><span data-stu-id="94e23-118">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="94e23-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="94e23-119">Request headers</span></span>
| <span data-ttu-id="94e23-120">名称</span><span class="sxs-lookup"><span data-stu-id="94e23-120">Name</span></span>          | <span data-ttu-id="94e23-121">说明</span><span class="sxs-lookup"><span data-stu-id="94e23-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="94e23-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="94e23-122">Authorization</span></span> | <span data-ttu-id="94e23-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="94e23-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="94e23-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="94e23-125">Request body</span></span>
<span data-ttu-id="94e23-126">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="94e23-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="94e23-127">参数</span><span class="sxs-lookup"><span data-stu-id="94e23-127">Parameter</span></span>      | <span data-ttu-id="94e23-128">类型</span><span class="sxs-lookup"><span data-stu-id="94e23-128">Type</span></span>    |<span data-ttu-id="94e23-129">说明</span><span class="sxs-lookup"><span data-stu-id="94e23-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="94e23-130">participants</span><span class="sxs-lookup"><span data-stu-id="94e23-130">participants</span></span>|<span data-ttu-id="94e23-131">String 集合</span><span class="sxs-lookup"><span data-stu-id="94e23-131">String collection</span></span>|<span data-ttu-id="94e23-132">要静音的参与者。</span><span class="sxs-lookup"><span data-stu-id="94e23-132">The participants to be muted.</span></span>|
|<span data-ttu-id="94e23-133">适用</span><span class="sxs-lookup"><span data-stu-id="94e23-133">clientContext</span></span>|<span data-ttu-id="94e23-134">String</span><span class="sxs-lookup"><span data-stu-id="94e23-134">String</span></span>|<span data-ttu-id="94e23-135">客户端上下文。</span><span class="sxs-lookup"><span data-stu-id="94e23-135">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="94e23-136">响应</span><span class="sxs-lookup"><span data-stu-id="94e23-136">Response</span></span>
<span data-ttu-id="94e23-137">如果成功，此方法在`200 OK`响应正文中返回响应代码和[commsOperation](../resources/commsoperation.md)对象。</span><span class="sxs-lookup"><span data-stu-id="94e23-137">If successful, this method returns `200 OK` response code and [commsOperation](../resources/commsoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="94e23-138">示例</span><span class="sxs-lookup"><span data-stu-id="94e23-138">Example</span></span>
<span data-ttu-id="94e23-139">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="94e23-139">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="94e23-140">请求</span><span class="sxs-lookup"><span data-stu-id="94e23-140">Request</span></span>
<span data-ttu-id="94e23-141">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="94e23-141">The following example shows the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="94e23-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="94e23-142">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="94e23-143">C#</span><span class="sxs-lookup"><span data-stu-id="94e23-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/participant-muteall-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="94e23-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="94e23-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/participant-muteall-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="94e23-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="94e23-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/participant-muteall-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="94e23-146">响应</span><span class="sxs-lookup"><span data-stu-id="94e23-146">Response</span></span>

> <span data-ttu-id="94e23-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="94e23-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.commsOperation"
} -->
```http
HTTP/1.1 200 OK
Location: https://graph.microsoft.com/beta/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/17e3b46c-f61d-4f4d-9635-c626ef18e6ad
Content-Type: application/json
Content-Length: 259

{
  "id": "17e3b46c-f61d-4f4d-9635-c626ef18e6ad",
  "status": "completed",
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c"
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

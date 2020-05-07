---
title: swapShiftsChangeRequest：拒绝
description: 拒绝交换转换请求。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 9c6852d09ce244469c4f0d29e179b25f6f081157
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/07/2020
ms.locfileid: "44154372"
---
# <a name="swapshiftschangerequest-decline"></a><span data-ttu-id="644cb-103">swapShiftsChangeRequest：拒绝</span><span class="sxs-lookup"><span data-stu-id="644cb-103">swapShiftsChangeRequest: decline</span></span>

<span data-ttu-id="644cb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="644cb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="644cb-105">拒绝[swapShiftsChangeRequest](../resources/swapshiftschangerequest.md)对象。</span><span class="sxs-lookup"><span data-stu-id="644cb-105">Decline a [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="644cb-106">权限</span><span class="sxs-lookup"><span data-stu-id="644cb-106">Permissions</span></span>

<span data-ttu-id="644cb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="644cb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="644cb-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="644cb-109">Permission type</span></span>                        | <span data-ttu-id="644cb-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="644cb-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="644cb-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="644cb-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="644cb-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="644cb-112">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="644cb-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="644cb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="644cb-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="644cb-114">Not supported.</span></span> |
| <span data-ttu-id="644cb-115">Application</span><span class="sxs-lookup"><span data-stu-id="644cb-115">Application</span></span>                            | <span data-ttu-id="644cb-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="644cb-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="644cb-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="644cb-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/swapShiftsChangeRequests/{swapShiftChangeRequestId}/decline
```

## <a name="request-headers"></a><span data-ttu-id="644cb-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="644cb-118">Request headers</span></span>

| <span data-ttu-id="644cb-119">名称</span><span class="sxs-lookup"><span data-stu-id="644cb-119">Name</span></span>          | <span data-ttu-id="644cb-120">说明</span><span class="sxs-lookup"><span data-stu-id="644cb-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="644cb-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="644cb-121">Authorization</span></span> | <span data-ttu-id="644cb-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="644cb-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="644cb-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="644cb-124">Content-type</span></span> | <span data-ttu-id="644cb-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="644cb-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="644cb-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="644cb-127">Request body</span></span>

<span data-ttu-id="644cb-128">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="644cb-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="644cb-129">参数</span><span class="sxs-lookup"><span data-stu-id="644cb-129">Parameter</span></span>    | <span data-ttu-id="644cb-130">类型</span><span class="sxs-lookup"><span data-stu-id="644cb-130">Type</span></span>        | <span data-ttu-id="644cb-131">描述</span><span class="sxs-lookup"><span data-stu-id="644cb-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="644cb-132">message</span><span class="sxs-lookup"><span data-stu-id="644cb-132">message</span></span>|<span data-ttu-id="644cb-133">String</span><span class="sxs-lookup"><span data-stu-id="644cb-133">String</span></span>|<span data-ttu-id="644cb-134">自定义拒绝邮件。</span><span class="sxs-lookup"><span data-stu-id="644cb-134">A custom decline message.</span></span>|

## <a name="response"></a><span data-ttu-id="644cb-135">响应</span><span class="sxs-lookup"><span data-stu-id="644cb-135">Response</span></span>

<span data-ttu-id="644cb-p104">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="644cb-p104">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="644cb-138">示例</span><span class="sxs-lookup"><span data-stu-id="644cb-138">Examples</span></span>

<span data-ttu-id="644cb-139">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="644cb-139">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="644cb-140">请求</span><span class="sxs-lookup"><span data-stu-id="644cb-140">Request</span></span>

<span data-ttu-id="644cb-141">请求示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="644cb-141">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="644cb-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="644cb-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "swapshiftchangerequest_decline"
}-->

```http
POST https://graph.microsoft.com/beta/teams/{teamId}/schedule/swapShiftsChangeRequests/{swapShiftChangeRequestId}/decline
Content-type: application/json

{
  "message": "message-value"
}
```
# <a name="c"></a>[<span data-ttu-id="644cb-143">C#</span><span class="sxs-lookup"><span data-stu-id="644cb-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/swapshiftchangerequest-decline-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="644cb-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="644cb-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/swapshiftchangerequest-decline-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="644cb-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="644cb-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/swapshiftchangerequest-decline-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="644cb-146">响应</span><span class="sxs-lookup"><span data-stu-id="644cb-146">Response</span></span>

<span data-ttu-id="644cb-147">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="644cb-147">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->

```http
HTTP/1.1 204 NO CONTENT
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "swapShiftChangeRequest: decline",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

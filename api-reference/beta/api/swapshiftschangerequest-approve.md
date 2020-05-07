---
title: swapShiftsChangeRequest：批准
description: 批准交换转换请求。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: b564884e57cd5ce1e4350034b0b98380eb8f8b7c
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/07/2020
ms.locfileid: "44154127"
---
# <a name="swapshiftschangerequest-approve"></a><span data-ttu-id="8cd78-103">swapShiftsChangeRequest：批准</span><span class="sxs-lookup"><span data-stu-id="8cd78-103">swapShiftsChangeRequest: approve</span></span>

<span data-ttu-id="8cd78-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8cd78-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8cd78-105">批准[swapShiftsChangeRequest](../resources/swapshiftschangerequest.md)对象。</span><span class="sxs-lookup"><span data-stu-id="8cd78-105">Approve a [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="8cd78-106">权限</span><span class="sxs-lookup"><span data-stu-id="8cd78-106">Permissions</span></span>

<span data-ttu-id="8cd78-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8cd78-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8cd78-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="8cd78-109">Permission type</span></span>                        | <span data-ttu-id="8cd78-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8cd78-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="8cd78-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8cd78-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="8cd78-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8cd78-112">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="8cd78-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8cd78-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8cd78-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="8cd78-114">Not supported.</span></span> |
| <span data-ttu-id="8cd78-115">Application</span><span class="sxs-lookup"><span data-stu-id="8cd78-115">Application</span></span>                            | <span data-ttu-id="8cd78-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="8cd78-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8cd78-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8cd78-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/swapShiftsChangeRequests/{swapShiftChangeRequestId}/approve
```

## <a name="request-headers"></a><span data-ttu-id="8cd78-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="8cd78-118">Request headers</span></span>

| <span data-ttu-id="8cd78-119">名称</span><span class="sxs-lookup"><span data-stu-id="8cd78-119">Name</span></span>          | <span data-ttu-id="8cd78-120">说明</span><span class="sxs-lookup"><span data-stu-id="8cd78-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="8cd78-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="8cd78-121">Authorization</span></span> | <span data-ttu-id="8cd78-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8cd78-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8cd78-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="8cd78-124">Content-type</span></span> | <span data-ttu-id="8cd78-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="8cd78-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8cd78-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="8cd78-127">Request body</span></span>

<span data-ttu-id="8cd78-128">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="8cd78-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="8cd78-129">参数</span><span class="sxs-lookup"><span data-stu-id="8cd78-129">Parameter</span></span>    | <span data-ttu-id="8cd78-130">类型</span><span class="sxs-lookup"><span data-stu-id="8cd78-130">Type</span></span>        | <span data-ttu-id="8cd78-131">描述</span><span class="sxs-lookup"><span data-stu-id="8cd78-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8cd78-132">message</span><span class="sxs-lookup"><span data-stu-id="8cd78-132">message</span></span>|<span data-ttu-id="8cd78-133">String</span><span class="sxs-lookup"><span data-stu-id="8cd78-133">String</span></span>|<span data-ttu-id="8cd78-134">自定义审批邮件。</span><span class="sxs-lookup"><span data-stu-id="8cd78-134">A custom approval message.</span></span>|

## <a name="response"></a><span data-ttu-id="8cd78-135">响应</span><span class="sxs-lookup"><span data-stu-id="8cd78-135">Response</span></span>

<span data-ttu-id="8cd78-p104">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="8cd78-p104">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8cd78-138">示例</span><span class="sxs-lookup"><span data-stu-id="8cd78-138">Examples</span></span>

<span data-ttu-id="8cd78-139">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="8cd78-139">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="8cd78-140">请求</span><span class="sxs-lookup"><span data-stu-id="8cd78-140">Request</span></span>

<span data-ttu-id="8cd78-141">请求示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="8cd78-141">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8cd78-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="8cd78-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "swapshiftchangerequest_approve"
}-->

```http
POST https://graph.microsoft.com/beta/teams/{teamId}/schedule/swapShiftsChangeRequests/{swapShiftChangeRequestId}/approve
Content-type: application/json

{
  "message": "message-value"
}
```
# <a name="c"></a>[<span data-ttu-id="8cd78-143">C#</span><span class="sxs-lookup"><span data-stu-id="8cd78-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/swapshiftchangerequest-approve-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8cd78-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8cd78-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/swapshiftchangerequest-approve-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8cd78-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8cd78-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/swapshiftchangerequest-approve-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8cd78-146">响应</span><span class="sxs-lookup"><span data-stu-id="8cd78-146">Response</span></span>

<span data-ttu-id="8cd78-147">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="8cd78-147">The following is an example of the response.</span></span>
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
  "description": "swapShiftChangeRequest: approve",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

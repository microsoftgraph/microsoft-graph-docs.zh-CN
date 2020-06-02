---
title: swapShiftsChangeRequest：批准
description: 批准交换转换请求。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: b564884e57cd5ce1e4350034b0b98380eb8f8b7c
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/02/2020
ms.locfileid: "44154127"
---
# <a name="swapshiftschangerequest-approve"></a><span data-ttu-id="9b0ae-103">swapShiftsChangeRequest：批准</span><span class="sxs-lookup"><span data-stu-id="9b0ae-103">swapShiftsChangeRequest: approve</span></span>

<span data-ttu-id="9b0ae-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9b0ae-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9b0ae-105">批准[swapShiftsChangeRequest](../resources/swapshiftschangerequest.md)对象。</span><span class="sxs-lookup"><span data-stu-id="9b0ae-105">Approve a [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="9b0ae-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="9b0ae-106">Permissions</span></span>

<span data-ttu-id="9b0ae-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9b0ae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9b0ae-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="9b0ae-109">Permission type</span></span>                        | <span data-ttu-id="9b0ae-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9b0ae-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="9b0ae-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9b0ae-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="9b0ae-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9b0ae-112">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="9b0ae-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9b0ae-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9b0ae-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="9b0ae-114">Not supported.</span></span> |
| <span data-ttu-id="9b0ae-115">Application</span><span class="sxs-lookup"><span data-stu-id="9b0ae-115">Application</span></span>                            | <span data-ttu-id="9b0ae-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9b0ae-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9b0ae-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9b0ae-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/swapShiftsChangeRequests/{swapShiftChangeRequestId}/approve
```

## <a name="request-headers"></a><span data-ttu-id="9b0ae-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="9b0ae-118">Request headers</span></span>

| <span data-ttu-id="9b0ae-119">名称</span><span class="sxs-lookup"><span data-stu-id="9b0ae-119">Name</span></span>          | <span data-ttu-id="9b0ae-120">说明</span><span class="sxs-lookup"><span data-stu-id="9b0ae-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="9b0ae-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="9b0ae-121">Authorization</span></span> | <span data-ttu-id="9b0ae-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9b0ae-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9b0ae-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="9b0ae-124">Content-type</span></span> | <span data-ttu-id="9b0ae-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="9b0ae-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9b0ae-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="9b0ae-127">Request body</span></span>

<span data-ttu-id="9b0ae-128">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="9b0ae-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="9b0ae-129">参数</span><span class="sxs-lookup"><span data-stu-id="9b0ae-129">Parameter</span></span>    | <span data-ttu-id="9b0ae-130">类型</span><span class="sxs-lookup"><span data-stu-id="9b0ae-130">Type</span></span>        | <span data-ttu-id="9b0ae-131">描述</span><span class="sxs-lookup"><span data-stu-id="9b0ae-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="9b0ae-132">message</span><span class="sxs-lookup"><span data-stu-id="9b0ae-132">message</span></span>|<span data-ttu-id="9b0ae-133">String</span><span class="sxs-lookup"><span data-stu-id="9b0ae-133">String</span></span>|<span data-ttu-id="9b0ae-134">自定义审批邮件。</span><span class="sxs-lookup"><span data-stu-id="9b0ae-134">A custom approval message.</span></span>|

## <a name="response"></a><span data-ttu-id="9b0ae-135">响应</span><span class="sxs-lookup"><span data-stu-id="9b0ae-135">Response</span></span>

<span data-ttu-id="9b0ae-p104">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="9b0ae-p104">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9b0ae-138">示例</span><span class="sxs-lookup"><span data-stu-id="9b0ae-138">Examples</span></span>

<span data-ttu-id="9b0ae-139">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="9b0ae-139">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="9b0ae-140">请求</span><span class="sxs-lookup"><span data-stu-id="9b0ae-140">Request</span></span>

<span data-ttu-id="9b0ae-141">请求示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="9b0ae-141">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9b0ae-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="9b0ae-142">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="9b0ae-143">C#</span><span class="sxs-lookup"><span data-stu-id="9b0ae-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/swapshiftchangerequest-approve-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9b0ae-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9b0ae-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/swapshiftchangerequest-approve-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9b0ae-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9b0ae-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/swapshiftchangerequest-approve-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="9b0ae-146">响应</span><span class="sxs-lookup"><span data-stu-id="9b0ae-146">Response</span></span>

<span data-ttu-id="9b0ae-147">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="9b0ae-147">The following is an example of the response.</span></span>
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

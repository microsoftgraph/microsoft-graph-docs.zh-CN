---
title: Delete taskDefinition
description: 删除任务定义。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 5183e95e05e30e078b1bb771472700f4b5900a56
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48093103"
---
# <a name="delete-taskdefinition"></a><span data-ttu-id="d9da1-103">Delete taskDefinition</span><span class="sxs-lookup"><span data-stu-id="d9da1-103">Delete taskDefinition</span></span>

<span data-ttu-id="d9da1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d9da1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d9da1-105">删除 **taskDefinition**。</span><span class="sxs-lookup"><span data-stu-id="d9da1-105">Delete a **taskDefinition**.</span></span>

<span data-ttu-id="d9da1-106">有关如何使用此 API 将拉取打印支持添加到通用打印的详细信息，请参阅 [扩展通用打印以支持请求打印](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing)。</span><span class="sxs-lookup"><span data-stu-id="d9da1-106">For details about how to use this API to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="d9da1-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="d9da1-107">Permissions</span></span>
<span data-ttu-id="d9da1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d9da1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="d9da1-110">除了以下权限之外，用户的租户还必须具有活动的通用打印订阅。</span><span class="sxs-lookup"><span data-stu-id="d9da1-110">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="d9da1-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="d9da1-111">Permission type</span></span> | <span data-ttu-id="d9da1-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d9da1-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="d9da1-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d9da1-113">Delegated (work or school account)</span></span>| <span data-ttu-id="d9da1-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="d9da1-114">Not supported.</span></span> |
|<span data-ttu-id="d9da1-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d9da1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d9da1-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d9da1-116">Not Supported.</span></span>|
|<span data-ttu-id="d9da1-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="d9da1-117">Application</span></span>| <span data-ttu-id="d9da1-118">PrintTaskDefinition.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9da1-118">PrintTaskDefinition.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d9da1-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d9da1-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /print/taskDefinitions/{id}
```
## <a name="request-headers"></a><span data-ttu-id="d9da1-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="d9da1-120">Request headers</span></span>
| <span data-ttu-id="d9da1-121">名称</span><span class="sxs-lookup"><span data-stu-id="d9da1-121">Name</span></span>          | <span data-ttu-id="d9da1-122">说明</span><span class="sxs-lookup"><span data-stu-id="d9da1-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="d9da1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d9da1-123">Authorization</span></span> | <span data-ttu-id="d9da1-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d9da1-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d9da1-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="d9da1-126">Request body</span></span>
<span data-ttu-id="d9da1-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d9da1-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d9da1-128">响应</span><span class="sxs-lookup"><span data-stu-id="d9da1-128">Response</span></span>
<span data-ttu-id="d9da1-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="d9da1-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d9da1-131">示例</span><span class="sxs-lookup"><span data-stu-id="d9da1-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="d9da1-132">请求</span><span class="sxs-lookup"><span data-stu-id="d9da1-132">Request</span></span>
<span data-ttu-id="d9da1-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d9da1-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="d9da1-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="d9da1-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_taskdefinition"
}-->
```http
DELETE https://graph.microsoft.com/beta/print/taskDefinitions/4c6a0f26-8e5d-4bf6-91e6-4a5731adec19
```
# <a name="c"></a>[<span data-ttu-id="d9da1-135">C#</span><span class="sxs-lookup"><span data-stu-id="d9da1-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-taskdefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d9da1-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d9da1-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-taskdefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d9da1-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d9da1-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-taskdefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

### <a name="response"></a><span data-ttu-id="d9da1-138">响应</span><span class="sxs-lookup"><span data-stu-id="d9da1-138">Response</span></span>
<span data-ttu-id="d9da1-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="d9da1-139">The following is an example of the response.</span></span>
><span data-ttu-id="d9da1-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="d9da1-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete taskDefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->



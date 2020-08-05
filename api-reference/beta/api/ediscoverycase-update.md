---
title: 更新 ediscoverycase
description: 更新 ediscoveryCase 对象的属性。
localization_priority: Normal
author: mahage-msft
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: 0014f0a173d190ab581be5ce21d78cebdfd20590
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2020
ms.locfileid: "46566917"
---
# <a name="update-ediscoverycase"></a><span data-ttu-id="4fe0d-103">更新 ediscoveryCase</span><span class="sxs-lookup"><span data-stu-id="4fe0d-103">Update ediscoveryCase</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4fe0d-104">更新[ediscoveryCase](../resources/ediscoverycase.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="4fe0d-104">Update the properties of an [ediscoveryCase](../resources/ediscoverycase.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="4fe0d-105">权限</span><span class="sxs-lookup"><span data-stu-id="4fe0d-105">Permissions</span></span>

<span data-ttu-id="4fe0d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4fe0d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4fe0d-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="4fe0d-108">Permission type</span></span>                        | <span data-ttu-id="4fe0d-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4fe0d-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="4fe0d-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4fe0d-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="4fe0d-111">User.Read</span><span class="sxs-lookup"><span data-stu-id="4fe0d-111">User.Read</span></span>      |
| <span data-ttu-id="4fe0d-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4fe0d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4fe0d-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="4fe0d-113">Not supported.</span></span> |
| <span data-ttu-id="4fe0d-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="4fe0d-114">Application</span></span>                            | <span data-ttu-id="4fe0d-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="4fe0d-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4fe0d-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4fe0d-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /compliance/ediscovery/cases/{id}
```

## <a name="request-headers"></a><span data-ttu-id="4fe0d-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="4fe0d-117">Request headers</span></span>

| <span data-ttu-id="4fe0d-118">名称</span><span class="sxs-lookup"><span data-stu-id="4fe0d-118">Name</span></span>       | <span data-ttu-id="4fe0d-119">说明</span><span class="sxs-lookup"><span data-stu-id="4fe0d-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="4fe0d-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="4fe0d-120">Authorization</span></span> | <span data-ttu-id="4fe0d-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4fe0d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4fe0d-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="4fe0d-123">Request body</span></span>

<span data-ttu-id="4fe0d-124">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="4fe0d-124">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="4fe0d-125">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="4fe0d-125">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="4fe0d-126">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="4fe0d-126">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="4fe0d-127">属性</span><span class="sxs-lookup"><span data-stu-id="4fe0d-127">Property</span></span>     | <span data-ttu-id="4fe0d-128">类型</span><span class="sxs-lookup"><span data-stu-id="4fe0d-128">Type</span></span>        | <span data-ttu-id="4fe0d-129">说明</span><span class="sxs-lookup"><span data-stu-id="4fe0d-129">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="4fe0d-130">说明</span><span class="sxs-lookup"><span data-stu-id="4fe0d-130">description</span></span>|<span data-ttu-id="4fe0d-131">String</span><span class="sxs-lookup"><span data-stu-id="4fe0d-131">String</span></span>| <span data-ttu-id="4fe0d-132">事例说明。</span><span class="sxs-lookup"><span data-stu-id="4fe0d-132">The case description.</span></span> |
|<span data-ttu-id="4fe0d-133">displayName</span><span class="sxs-lookup"><span data-stu-id="4fe0d-133">displayName</span></span>|<span data-ttu-id="4fe0d-134">字符串</span><span class="sxs-lookup"><span data-stu-id="4fe0d-134">String</span></span>| <span data-ttu-id="4fe0d-135">事例名称。</span><span class="sxs-lookup"><span data-stu-id="4fe0d-135">The case name.</span></span> |
|<span data-ttu-id="4fe0d-136">externalId</span><span class="sxs-lookup"><span data-stu-id="4fe0d-136">externalId</span></span>|<span data-ttu-id="4fe0d-137">String</span><span class="sxs-lookup"><span data-stu-id="4fe0d-137">String</span></span>| <span data-ttu-id="4fe0d-138">Customer reference 的外部事例编号。</span><span class="sxs-lookup"><span data-stu-id="4fe0d-138">The external case number for customer reference.</span></span> |

## <a name="response"></a><span data-ttu-id="4fe0d-139">响应</span><span class="sxs-lookup"><span data-stu-id="4fe0d-139">Response</span></span>

<span data-ttu-id="4fe0d-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="4fe0d-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4fe0d-142">示例</span><span class="sxs-lookup"><span data-stu-id="4fe0d-142">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4fe0d-143">请求</span><span class="sxs-lookup"><span data-stu-id="4fe0d-143">Request</span></span>

<span data-ttu-id="4fe0d-144">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="4fe0d-144">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4fe0d-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="4fe0d-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_ediscoverycase"
}-->

```http
PATCH https://graph.microsoft.com/beta/compliance/ediscovery/cases/061b9a92-8926-4bd9-b41d-abf35edc7583
Content-type: application/json

{
  "displayName": "My Case 1 - Renamed",
  "description": "Updated description",
  "externalId": "Updated externalId"
}
```
# <a name="c"></a>[<span data-ttu-id="4fe0d-146">C#</span><span class="sxs-lookup"><span data-stu-id="4fe0d-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-ediscoverycase-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4fe0d-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4fe0d-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-ediscoverycase-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4fe0d-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4fe0d-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-ediscoverycase-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4fe0d-149">响应</span><span class="sxs-lookup"><span data-stu-id="4fe0d-149">Response</span></span>

<span data-ttu-id="4fe0d-150">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="4fe0d-150">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscoveryCase"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update ediscoverycase",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

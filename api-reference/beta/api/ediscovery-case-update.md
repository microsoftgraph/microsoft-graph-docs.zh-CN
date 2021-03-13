---
title: 更新案例
description: 更新 case 对象的属性。
localization_priority: Normal
author: mahage-msft
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 79b2e56cdb0e7e6ad4acf09625af54e413291b08
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50773653"
---
# <a name="update-case"></a><span data-ttu-id="70cd4-103">更新案例</span><span class="sxs-lookup"><span data-stu-id="70cd4-103">Update case</span></span>

<span data-ttu-id="70cd4-104">命名空间：microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="70cd4-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="70cd4-105">更新 [case](../resources/ediscovery-case.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="70cd4-105">Update the properties of a [case](../resources/ediscovery-case.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="70cd4-106">权限</span><span class="sxs-lookup"><span data-stu-id="70cd4-106">Permissions</span></span>

<span data-ttu-id="70cd4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="70cd4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="70cd4-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="70cd4-109">Permission type</span></span>|<span data-ttu-id="70cd4-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="70cd4-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="70cd4-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="70cd4-111">Delegated (work or school account)</span></span>|<span data-ttu-id="70cd4-112">eDiscovery.Read.All、eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="70cd4-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="70cd4-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="70cd4-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="70cd4-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="70cd4-114">Not supported.</span></span>|
|<span data-ttu-id="70cd4-115">Application</span><span class="sxs-lookup"><span data-stu-id="70cd4-115">Application</span></span>|<span data-ttu-id="70cd4-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="70cd4-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="70cd4-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="70cd4-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /compliance/ediscovery/cases/{id}
```

## <a name="request-headers"></a><span data-ttu-id="70cd4-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="70cd4-118">Request headers</span></span>

| <span data-ttu-id="70cd4-119">名称</span><span class="sxs-lookup"><span data-stu-id="70cd4-119">Name</span></span>       | <span data-ttu-id="70cd4-120">说明</span><span class="sxs-lookup"><span data-stu-id="70cd4-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="70cd4-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="70cd4-121">Authorization</span></span> | <span data-ttu-id="70cd4-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="70cd4-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="70cd4-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="70cd4-124">Request body</span></span>

<span data-ttu-id="70cd4-125">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="70cd4-125">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="70cd4-126">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="70cd4-126">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="70cd4-127">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="70cd4-127">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="70cd4-128">属性</span><span class="sxs-lookup"><span data-stu-id="70cd4-128">Property</span></span>     | <span data-ttu-id="70cd4-129">类型</span><span class="sxs-lookup"><span data-stu-id="70cd4-129">Type</span></span>        | <span data-ttu-id="70cd4-130">说明</span><span class="sxs-lookup"><span data-stu-id="70cd4-130">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="70cd4-131">说明</span><span class="sxs-lookup"><span data-stu-id="70cd4-131">description</span></span>|<span data-ttu-id="70cd4-132">字符串</span><span class="sxs-lookup"><span data-stu-id="70cd4-132">String</span></span>|<span data-ttu-id="70cd4-133">案例描述。</span><span class="sxs-lookup"><span data-stu-id="70cd4-133">The case description.</span></span>|
|<span data-ttu-id="70cd4-134">displayName</span><span class="sxs-lookup"><span data-stu-id="70cd4-134">displayName</span></span>|<span data-ttu-id="70cd4-135">字符串</span><span class="sxs-lookup"><span data-stu-id="70cd4-135">String</span></span>|<span data-ttu-id="70cd4-136">大小写名称。</span><span class="sxs-lookup"><span data-stu-id="70cd4-136">The case name.</span></span>|
|<span data-ttu-id="70cd4-137">externalId</span><span class="sxs-lookup"><span data-stu-id="70cd4-137">externalId</span></span>|<span data-ttu-id="70cd4-138">String</span><span class="sxs-lookup"><span data-stu-id="70cd4-138">String</span></span>|<span data-ttu-id="70cd4-139">客户参考的外部案例编号。</span><span class="sxs-lookup"><span data-stu-id="70cd4-139">The external case number for customer reference.</span></span>|

## <a name="response"></a><span data-ttu-id="70cd4-140">响应</span><span class="sxs-lookup"><span data-stu-id="70cd4-140">Response</span></span>

<span data-ttu-id="70cd4-141">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [microsoft.graph.ediscovery.case](../resources/ediscovery-case.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="70cd4-141">If successful, this method returns a `200 OK` response code and an updated [microsoft.graph.ediscovery.case](../resources/ediscovery-case.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="70cd4-142">示例</span><span class="sxs-lookup"><span data-stu-id="70cd4-142">Examples</span></span>

### <a name="request"></a><span data-ttu-id="70cd4-143">请求</span><span class="sxs-lookup"><span data-stu-id="70cd4-143">Request</span></span>

<span data-ttu-id="70cd4-144">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="70cd4-144">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="70cd4-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="70cd4-145">HTTP</span></span>](#tab/http)

<!-- {
  "blockType": "request",
  "name": "update_case"
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

# <a name="c"></a>[<span data-ttu-id="70cd4-146">C#</span><span class="sxs-lookup"><span data-stu-id="70cd4-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-case-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="70cd4-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="70cd4-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-case-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="70cd4-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="70cd4-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-case-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="70cd4-149">Java</span><span class="sxs-lookup"><span data-stu-id="70cd4-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-case-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="70cd4-150">响应</span><span class="sxs-lookup"><span data-stu-id="70cd4-150">Response</span></span>

<span data-ttu-id="70cd4-151">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="70cd4-151">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscovery.case"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update case",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

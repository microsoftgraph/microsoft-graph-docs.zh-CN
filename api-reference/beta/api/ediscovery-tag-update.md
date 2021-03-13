---
title: 更新标记
description: 更新 tag 对象的属性。
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: ee8d46d92b7f5e29a4612d3399028dacc36ad6fc
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50776394"
---
# <a name="update-tag"></a><span data-ttu-id="e5709-103">更新标记</span><span class="sxs-lookup"><span data-stu-id="e5709-103">Update tag</span></span>

<span data-ttu-id="e5709-104">命名空间：microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="e5709-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e5709-105">更新 [tag](../resources/ediscovery-tag.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="e5709-105">Update the properties of a [tag](../resources/ediscovery-tag.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e5709-106">权限</span><span class="sxs-lookup"><span data-stu-id="e5709-106">Permissions</span></span>

<span data-ttu-id="e5709-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e5709-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e5709-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="e5709-109">Permission type</span></span>|<span data-ttu-id="e5709-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e5709-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e5709-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e5709-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e5709-112">eDiscovery.Read.All、eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5709-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="e5709-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e5709-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e5709-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="e5709-114">Not supported.</span></span>|
|<span data-ttu-id="e5709-115">Application</span><span class="sxs-lookup"><span data-stu-id="e5709-115">Application</span></span>|<span data-ttu-id="e5709-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e5709-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e5709-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e5709-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
PATCH /compliance/ediscovery/cases/{caseId}/tags/{tagId}
```

## <a name="request-headers"></a><span data-ttu-id="e5709-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="e5709-118">Request headers</span></span>

|<span data-ttu-id="e5709-119">名称</span><span class="sxs-lookup"><span data-stu-id="e5709-119">Name</span></span>|<span data-ttu-id="e5709-120">说明</span><span class="sxs-lookup"><span data-stu-id="e5709-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="e5709-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e5709-121">Authorization</span></span>|<span data-ttu-id="e5709-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e5709-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="e5709-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e5709-124">Content-Type</span></span>|<span data-ttu-id="e5709-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="e5709-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e5709-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="e5709-127">Request body</span></span>

<span data-ttu-id="e5709-128">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="e5709-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="e5709-129">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="e5709-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="e5709-130">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="e5709-130">For best performance, don't include existing values that haven't changed.</span></span>

|<span data-ttu-id="e5709-131">属性</span><span class="sxs-lookup"><span data-stu-id="e5709-131">Property</span></span>|<span data-ttu-id="e5709-132">类型</span><span class="sxs-lookup"><span data-stu-id="e5709-132">Type</span></span>|<span data-ttu-id="e5709-133">说明</span><span class="sxs-lookup"><span data-stu-id="e5709-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e5709-134">说明</span><span class="sxs-lookup"><span data-stu-id="e5709-134">description</span></span>|<span data-ttu-id="e5709-135">字符串</span><span class="sxs-lookup"><span data-stu-id="e5709-135">String</span></span>|<span data-ttu-id="e5709-136">标记的说明。</span><span class="sxs-lookup"><span data-stu-id="e5709-136">The description for the tag.</span></span>|
|<span data-ttu-id="e5709-137">displayName</span><span class="sxs-lookup"><span data-stu-id="e5709-137">displayName</span></span>|<span data-ttu-id="e5709-138">字符串</span><span class="sxs-lookup"><span data-stu-id="e5709-138">String</span></span>|<span data-ttu-id="e5709-139">标记的显示名称。</span><span class="sxs-lookup"><span data-stu-id="e5709-139">Display name of the tag.</span></span>|

## <a name="response"></a><span data-ttu-id="e5709-140">响应</span><span class="sxs-lookup"><span data-stu-id="e5709-140">Response</span></span>

<span data-ttu-id="e5709-141">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="e5709-141">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="e5709-142">示例</span><span class="sxs-lookup"><span data-stu-id="e5709-142">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e5709-143">请求</span><span class="sxs-lookup"><span data-stu-id="e5709-143">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="e5709-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="e5709-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_tag"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/tags/e54b3f535b434a9a8743b84e34c00504
Content-Type: application/json
Content-length: 210

{
  "description":"This is an updated description."
}
```
# <a name="c"></a>[<span data-ttu-id="e5709-145">C#</span><span class="sxs-lookup"><span data-stu-id="e5709-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-tag-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e5709-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e5709-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-tag-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e5709-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e5709-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-tag-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e5709-148">Java</span><span class="sxs-lookup"><span data-stu-id="e5709-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-tag-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e5709-149">响应</span><span class="sxs-lookup"><span data-stu-id="e5709-149">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```

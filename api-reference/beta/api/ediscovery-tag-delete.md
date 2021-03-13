---
title: 删除标记
description: 删除 tag 对象。
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 8c21df5939cde9b707dd913dbfa383ba1e950d53
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50776457"
---
# <a name="delete-tag"></a><span data-ttu-id="9e6c5-103">删除标记</span><span class="sxs-lookup"><span data-stu-id="9e6c5-103">Delete tag</span></span>

<span data-ttu-id="9e6c5-104">命名空间：microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="9e6c5-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9e6c5-105">删除 [tag](../resources/ediscovery-tag.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9e6c5-105">Delete a [tag](../resources/ediscovery-tag.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="9e6c5-106">权限</span><span class="sxs-lookup"><span data-stu-id="9e6c5-106">Permissions</span></span>

<span data-ttu-id="9e6c5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9e6c5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9e6c5-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="9e6c5-109">Permission type</span></span>|<span data-ttu-id="9e6c5-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9e6c5-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9e6c5-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9e6c5-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9e6c5-112">eDiscovery.Read.All、eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9e6c5-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="9e6c5-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9e6c5-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9e6c5-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="9e6c5-114">Not supported.</span></span>|
|<span data-ttu-id="9e6c5-115">Application</span><span class="sxs-lookup"><span data-stu-id="9e6c5-115">Application</span></span>|<span data-ttu-id="9e6c5-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9e6c5-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9e6c5-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9e6c5-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /compliance/ediscovery/cases/{caseId}/tags/{tagId}?forcedelete=true
```

## <a name="query-parameters"></a><span data-ttu-id="9e6c5-118">查询参数</span><span class="sxs-lookup"><span data-stu-id="9e6c5-118">Query parameters</span></span>

<span data-ttu-id="9e6c5-119">在请求 URL 中，提供以下必需的查询参数。</span><span class="sxs-lookup"><span data-stu-id="9e6c5-119">In the request URL, provide the following required query parameter.</span></span>

| <span data-ttu-id="9e6c5-120">参数</span><span class="sxs-lookup"><span data-stu-id="9e6c5-120">Parameter</span></span>     | <span data-ttu-id="9e6c5-121">类型</span><span class="sxs-lookup"><span data-stu-id="9e6c5-121">Type</span></span>    | <span data-ttu-id="9e6c5-122">说明</span><span class="sxs-lookup"><span data-stu-id="9e6c5-122">Description</span></span>                                                                              |
|:--------------|:--------|:-----------------------------------------------------------------------------------------|
| <span data-ttu-id="9e6c5-123">forcedelete</span><span class="sxs-lookup"><span data-stu-id="9e6c5-123">forcedelete</span></span>   | <span data-ttu-id="9e6c5-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e6c5-124">Boolean</span></span> | <span data-ttu-id="9e6c5-125">如果设置为 true，则标记和子项将被删除（如果为 false）并且标记具有子标记，则删除将失败。</span><span class="sxs-lookup"><span data-stu-id="9e6c5-125">If set to true, the tag and children will be deleted, if false, and the tag has children, the delete will fail.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="9e6c5-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="9e6c5-126">Request headers</span></span>

|<span data-ttu-id="9e6c5-127">名称</span><span class="sxs-lookup"><span data-stu-id="9e6c5-127">Name</span></span>|<span data-ttu-id="9e6c5-128">说明</span><span class="sxs-lookup"><span data-stu-id="9e6c5-128">Description</span></span>|
|:---|:---|
|<span data-ttu-id="9e6c5-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="9e6c5-129">Authorization</span></span>|<span data-ttu-id="9e6c5-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9e6c5-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9e6c5-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="9e6c5-132">Request body</span></span>

<span data-ttu-id="9e6c5-133">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9e6c5-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9e6c5-134">响应</span><span class="sxs-lookup"><span data-stu-id="9e6c5-134">Response</span></span>

<span data-ttu-id="9e6c5-135">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="9e6c5-135">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="9e6c5-136">示例</span><span class="sxs-lookup"><span data-stu-id="9e6c5-136">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9e6c5-137">请求</span><span class="sxs-lookup"><span data-stu-id="9e6c5-137">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="9e6c5-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="9e6c5-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_tag"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/tags/9985bd266f2f459cbebc81522734b452?forcedelete=true
```
# <a name="c"></a>[<span data-ttu-id="9e6c5-139">C#</span><span class="sxs-lookup"><span data-stu-id="9e6c5-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-tag-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9e6c5-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9e6c5-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-tag-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9e6c5-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9e6c5-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-tag-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9e6c5-142">Java</span><span class="sxs-lookup"><span data-stu-id="9e6c5-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-tag-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="9e6c5-143">响应</span><span class="sxs-lookup"><span data-stu-id="9e6c5-143">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```

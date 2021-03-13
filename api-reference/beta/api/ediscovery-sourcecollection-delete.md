---
title: 删除 sourceCollection
description: 删除 sourceCollection 对象。
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 13380114c2d2e7a1f0ff4d1f612a411d8efad6f5
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50772742"
---
# <a name="delete-sourcecollection"></a><span data-ttu-id="b0824-103">删除 sourceCollection</span><span class="sxs-lookup"><span data-stu-id="b0824-103">Delete sourceCollection</span></span>

<span data-ttu-id="b0824-104">命名空间：microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="b0824-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b0824-105">删除 [sourceCollection](../resources/ediscovery-sourcecollection.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b0824-105">Delete a [sourceCollection](../resources/ediscovery-sourcecollection.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b0824-106">权限</span><span class="sxs-lookup"><span data-stu-id="b0824-106">Permissions</span></span>

<span data-ttu-id="b0824-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b0824-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b0824-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="b0824-109">Permission type</span></span>|<span data-ttu-id="b0824-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b0824-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b0824-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b0824-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b0824-112">eDiscovery.Read.All、eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b0824-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="b0824-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b0824-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b0824-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="b0824-114">Not supported.</span></span>|
|<span data-ttu-id="b0824-115">Application</span><span class="sxs-lookup"><span data-stu-id="b0824-115">Application</span></span>|<span data-ttu-id="b0824-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b0824-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b0824-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b0824-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /compliance/ediscovery/cases/{caseId}/sourceCollections/{sourceCollectionId}
```

## <a name="request-headers"></a><span data-ttu-id="b0824-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="b0824-118">Request headers</span></span>

|<span data-ttu-id="b0824-119">名称</span><span class="sxs-lookup"><span data-stu-id="b0824-119">Name</span></span>|<span data-ttu-id="b0824-120">说明</span><span class="sxs-lookup"><span data-stu-id="b0824-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="b0824-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b0824-121">Authorization</span></span>|<span data-ttu-id="b0824-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b0824-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b0824-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="b0824-124">Request body</span></span>

<span data-ttu-id="b0824-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b0824-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b0824-126">响应</span><span class="sxs-lookup"><span data-stu-id="b0824-126">Response</span></span>

<span data-ttu-id="b0824-127">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="b0824-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="b0824-128">示例</span><span class="sxs-lookup"><span data-stu-id="b0824-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b0824-129">请求</span><span class="sxs-lookup"><span data-stu-id="b0824-129">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="b0824-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="b0824-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_sourcecollection"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/compliance/ediscovery/cases/{caseId}/sourceCollections/{sourceCollectionId}
```
# <a name="c"></a>[<span data-ttu-id="b0824-131">C#</span><span class="sxs-lookup"><span data-stu-id="b0824-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-sourcecollection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b0824-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b0824-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-sourcecollection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b0824-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b0824-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-sourcecollection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b0824-134">Java</span><span class="sxs-lookup"><span data-stu-id="b0824-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-sourcecollection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b0824-135">响应</span><span class="sxs-lookup"><span data-stu-id="b0824-135">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```

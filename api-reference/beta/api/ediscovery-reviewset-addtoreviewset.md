---
title: reviewSet： addToReviewSet
description: 开始将集合从 Microsoft 365 服务添加到审阅集的过程。
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: a1002d8b322876f753f424a1bffeb7ef8a278b35
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50772911"
---
# <a name="reviewset-addtoreviewset"></a><span data-ttu-id="bf2df-103">reviewSet： addToReviewSet</span><span class="sxs-lookup"><span data-stu-id="bf2df-103">reviewSet: addToReviewSet</span></span>

<span data-ttu-id="bf2df-104">命名空间：microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="bf2df-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bf2df-105">开始将集合从 Microsoft 365 服务添加到审阅集的过程。</span><span class="sxs-lookup"><span data-stu-id="bf2df-105">Start the process of adding a collection from Microsoft 365 services to a review set.</span></span> <span data-ttu-id="bf2df-106">创建操作后，可以通过从响应标头中检索参数获取 `Location` 操作的状态。</span><span class="sxs-lookup"><span data-stu-id="bf2df-106">After the operation is created, you can get the status of the operation by retrieving the `Location` parameter from the response headers.</span></span> <span data-ttu-id="bf2df-107">该位置提供将返回 [caseExportOperation](../resources/ediscovery-caseexportoperation.md)的 URL。</span><span class="sxs-lookup"><span data-stu-id="bf2df-107">The location provides a URL that will return a [caseExportOperation](../resources/ediscovery-caseexportoperation.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="bf2df-108">权限</span><span class="sxs-lookup"><span data-stu-id="bf2df-108">Permissions</span></span>

<span data-ttu-id="bf2df-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bf2df-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bf2df-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="bf2df-111">Permission type</span></span>|<span data-ttu-id="bf2df-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bf2df-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bf2df-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bf2df-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bf2df-114">eDiscovery.Read.All、eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bf2df-114">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="bf2df-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bf2df-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bf2df-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="bf2df-116">Not supported.</span></span>|
|<span data-ttu-id="bf2df-117">Application</span><span class="sxs-lookup"><span data-stu-id="bf2df-117">Application</span></span>|<span data-ttu-id="bf2df-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="bf2df-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bf2df-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bf2df-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{caseId}/reviewSets/{reviewsetId}/addToReviewSet
```

## <a name="request-headers"></a><span data-ttu-id="bf2df-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="bf2df-120">Request headers</span></span>

|<span data-ttu-id="bf2df-121">名称</span><span class="sxs-lookup"><span data-stu-id="bf2df-121">Name</span></span>|<span data-ttu-id="bf2df-122">说明</span><span class="sxs-lookup"><span data-stu-id="bf2df-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="bf2df-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bf2df-123">Authorization</span></span>|<span data-ttu-id="bf2df-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="bf2df-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="bf2df-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bf2df-126">Content-Type</span></span>|<span data-ttu-id="bf2df-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="bf2df-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="bf2df-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="bf2df-129">Request body</span></span>

<span data-ttu-id="bf2df-130">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bf2df-130">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="bf2df-131">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="bf2df-131">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="bf2df-132">参数</span><span class="sxs-lookup"><span data-stu-id="bf2df-132">Parameter</span></span>|<span data-ttu-id="bf2df-133">类型</span><span class="sxs-lookup"><span data-stu-id="bf2df-133">Type</span></span>|<span data-ttu-id="bf2df-134">说明</span><span class="sxs-lookup"><span data-stu-id="bf2df-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bf2df-135">sourceCollection</span><span class="sxs-lookup"><span data-stu-id="bf2df-135">sourceCollection</span></span>|[<span data-ttu-id="bf2df-136">microsoft.graph.ediscovery.sourceCollection</span><span class="sxs-lookup"><span data-stu-id="bf2df-136">microsoft.graph.ediscovery.sourceCollection</span></span>](../resources/ediscovery-sourcecollection.md)|<span data-ttu-id="bf2df-137">**sourceCollection 的** ID。</span><span class="sxs-lookup"><span data-stu-id="bf2df-137">The ID of the **sourceCollection**.</span></span>|
|<span data-ttu-id="bf2df-138">additionalData</span><span class="sxs-lookup"><span data-stu-id="bf2df-138">additionalData</span></span>|[<span data-ttu-id="bf2df-139">microsoft.graph.ediscovery.dataCollectionScope</span><span class="sxs-lookup"><span data-stu-id="bf2df-139">microsoft.graph.ediscovery.dataCollectionScope</span></span>](../resources/ediscovery-addtoreviewsetoperation.md#datacollectionscope-values)|<span data-ttu-id="bf2df-140">集合 **中将包含的 dataCollectionScope。**</span><span class="sxs-lookup"><span data-stu-id="bf2df-140">The **dataCollectionScope** that will be included with the collection.</span></span>|

## <a name="response"></a><span data-ttu-id="bf2df-141">响应</span><span class="sxs-lookup"><span data-stu-id="bf2df-141">Response</span></span>

<span data-ttu-id="bf2df-142">如果成功，此操作返回 `202 Accepted` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="bf2df-142">If successful, this action returns a `202 Accepted` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="bf2df-143">示例</span><span class="sxs-lookup"><span data-stu-id="bf2df-143">Examples</span></span>

### <a name="request"></a><span data-ttu-id="bf2df-144">请求</span><span class="sxs-lookup"><span data-stu-id="bf2df-144">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="bf2df-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="bf2df-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reviewset_addtoreviewset"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/080e8cad-f21f-4452-8826-0ddf7e949fdd/reviewSets/6fe25d32-8167-4625-b75c-c4181ccbd9d5/addToReviewSet
Content-Type: application/json
Content-length: 531

{
    "sourceCollection": {
        "id": "1a9b4145d8f84e39bc45a7f68c5c5119"
    },
    "additionalData": "linkedFiles"
}
```
# <a name="c"></a>[<span data-ttu-id="bf2df-146">C#</span><span class="sxs-lookup"><span data-stu-id="bf2df-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reviewset-addtoreviewset-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bf2df-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bf2df-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reviewset-addtoreviewset-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bf2df-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bf2df-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reviewset-addtoreviewset-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bf2df-149">Java</span><span class="sxs-lookup"><span data-stu-id="bf2df-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reviewset-addtoreviewset-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="bf2df-150">响应</span><span class="sxs-lookup"><span data-stu-id="bf2df-150">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 202 Accepted
```

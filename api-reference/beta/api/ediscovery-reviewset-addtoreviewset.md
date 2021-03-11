---
title: reviewSet：addToReviewSet
description: 开始将 Microsoft 365 服务中的集合添加到审阅集的过程。
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 4eb0a7c2de533332c57f3e26d3b6fba25a68259d
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720373"
---
# <a name="reviewset-addtoreviewset"></a><span data-ttu-id="1aa25-103">reviewSet：addToReviewSet</span><span class="sxs-lookup"><span data-stu-id="1aa25-103">reviewSet: addToReviewSet</span></span>

<span data-ttu-id="1aa25-104">命名空间：microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="1aa25-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1aa25-105">开始将 Microsoft 365 服务中的集合添加到审阅集的过程。</span><span class="sxs-lookup"><span data-stu-id="1aa25-105">Start the process of adding a collection from Microsoft 365 services to a review set.</span></span> <span data-ttu-id="1aa25-106">创建操作后，可以通过从响应标头中检索参数获取 `Location` 操作的状态。</span><span class="sxs-lookup"><span data-stu-id="1aa25-106">After the operation is created, you can get the status of the operation by retrieving the `Location` parameter from the response headers.</span></span> <span data-ttu-id="1aa25-107">该位置提供将返回 [caseExportOperation 的](../resources/ediscovery-caseexportoperation.md)URL。</span><span class="sxs-lookup"><span data-stu-id="1aa25-107">The location provides a URL that will return a [caseExportOperation](../resources/ediscovery-caseexportoperation.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="1aa25-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="1aa25-108">Permissions</span></span>

<span data-ttu-id="1aa25-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1aa25-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1aa25-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="1aa25-111">Permission type</span></span>|<span data-ttu-id="1aa25-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1aa25-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1aa25-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1aa25-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1aa25-114">eDiscovery.Read.All、eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1aa25-114">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="1aa25-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1aa25-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1aa25-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="1aa25-116">Not supported.</span></span>|
|<span data-ttu-id="1aa25-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="1aa25-117">Application</span></span>|<span data-ttu-id="1aa25-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="1aa25-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1aa25-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1aa25-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{caseId}/reviewSets/{reviewsetId}/addToReviewSet
```

## <a name="request-headers"></a><span data-ttu-id="1aa25-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="1aa25-120">Request headers</span></span>

|<span data-ttu-id="1aa25-121">名称</span><span class="sxs-lookup"><span data-stu-id="1aa25-121">Name</span></span>|<span data-ttu-id="1aa25-122">说明</span><span class="sxs-lookup"><span data-stu-id="1aa25-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="1aa25-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1aa25-123">Authorization</span></span>|<span data-ttu-id="1aa25-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1aa25-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="1aa25-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1aa25-126">Content-Type</span></span>|<span data-ttu-id="1aa25-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="1aa25-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1aa25-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="1aa25-129">Request body</span></span>

<span data-ttu-id="1aa25-130">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1aa25-130">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="1aa25-131">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="1aa25-131">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="1aa25-132">参数</span><span class="sxs-lookup"><span data-stu-id="1aa25-132">Parameter</span></span>|<span data-ttu-id="1aa25-133">类型</span><span class="sxs-lookup"><span data-stu-id="1aa25-133">Type</span></span>|<span data-ttu-id="1aa25-134">说明</span><span class="sxs-lookup"><span data-stu-id="1aa25-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1aa25-135">sourceCollection</span><span class="sxs-lookup"><span data-stu-id="1aa25-135">sourceCollection</span></span>|[<span data-ttu-id="1aa25-136">microsoft.graph.ediscovery.sourceCollection</span><span class="sxs-lookup"><span data-stu-id="1aa25-136">microsoft.graph.ediscovery.sourceCollection</span></span>](../resources/ediscovery-sourcecollection.md)|<span data-ttu-id="1aa25-137">**sourceCollection 的** ID。</span><span class="sxs-lookup"><span data-stu-id="1aa25-137">The ID of the **sourceCollection**.</span></span>|
|<span data-ttu-id="1aa25-138">additionalData</span><span class="sxs-lookup"><span data-stu-id="1aa25-138">additionalData</span></span>|[<span data-ttu-id="1aa25-139">microsoft.graph.ediscovery.dataCollectionScope</span><span class="sxs-lookup"><span data-stu-id="1aa25-139">microsoft.graph.ediscovery.dataCollectionScope</span></span>](../resources/ediscovery-addtoreviewsetoperation.md#datacollectionscope-values)|<span data-ttu-id="1aa25-140">**集合中将包含的 dataCollectionScope。**</span><span class="sxs-lookup"><span data-stu-id="1aa25-140">The **dataCollectionScope** that will be included with the collection.</span></span>|

## <a name="response"></a><span data-ttu-id="1aa25-141">响应</span><span class="sxs-lookup"><span data-stu-id="1aa25-141">Response</span></span>

<span data-ttu-id="1aa25-142">如果成功，此操作返回 `202 Accepted` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="1aa25-142">If successful, this action returns a `202 Accepted` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="1aa25-143">示例</span><span class="sxs-lookup"><span data-stu-id="1aa25-143">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1aa25-144">请求</span><span class="sxs-lookup"><span data-stu-id="1aa25-144">Request</span></span>

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

### <a name="response"></a><span data-ttu-id="1aa25-145">响应</span><span class="sxs-lookup"><span data-stu-id="1aa25-145">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 202 Accepted
```

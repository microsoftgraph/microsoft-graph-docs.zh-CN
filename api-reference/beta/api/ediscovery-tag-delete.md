---
title: 删除标记
description: 删除标记对象。
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 1ec395a45ee3720797228952b1f9047822fed11c
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50445985"
---
# <a name="delete-tag"></a><span data-ttu-id="d5f8b-103">删除标记</span><span class="sxs-lookup"><span data-stu-id="d5f8b-103">Delete tag</span></span>

<span data-ttu-id="d5f8b-104">命名空间：microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="d5f8b-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d5f8b-105">删除 [标记](../resources/ediscovery-tag.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d5f8b-105">Delete a [tag](../resources/ediscovery-tag.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d5f8b-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="d5f8b-106">Permissions</span></span>

<span data-ttu-id="d5f8b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d5f8b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d5f8b-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d5f8b-109">Permission type</span></span>|<span data-ttu-id="d5f8b-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d5f8b-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d5f8b-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d5f8b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d5f8b-112">eDiscovery.Read.All、eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d5f8b-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="d5f8b-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d5f8b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d5f8b-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="d5f8b-114">Not supported.</span></span>|
|<span data-ttu-id="d5f8b-115">Application</span><span class="sxs-lookup"><span data-stu-id="d5f8b-115">Application</span></span>|<span data-ttu-id="d5f8b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d5f8b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d5f8b-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d5f8b-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /compliance/ediscovery/cases/{caseId}/tags/{tagId}?forcedelete=true
```

## <a name="query-parameters"></a><span data-ttu-id="d5f8b-118">查询参数</span><span class="sxs-lookup"><span data-stu-id="d5f8b-118">Query parameters</span></span>

<span data-ttu-id="d5f8b-119">在请求 URL 中，提供以下所需的查询参数。</span><span class="sxs-lookup"><span data-stu-id="d5f8b-119">In the request URL, provide the following required query parameter.</span></span>

| <span data-ttu-id="d5f8b-120">参数</span><span class="sxs-lookup"><span data-stu-id="d5f8b-120">Parameter</span></span>     | <span data-ttu-id="d5f8b-121">类型</span><span class="sxs-lookup"><span data-stu-id="d5f8b-121">Type</span></span>    | <span data-ttu-id="d5f8b-122">说明</span><span class="sxs-lookup"><span data-stu-id="d5f8b-122">Description</span></span>                                                                              |
|:--------------|:--------|:-----------------------------------------------------------------------------------------|
| <span data-ttu-id="d5f8b-123">forcedelete</span><span class="sxs-lookup"><span data-stu-id="d5f8b-123">forcedelete</span></span>   | <span data-ttu-id="d5f8b-124">布尔</span><span class="sxs-lookup"><span data-stu-id="d5f8b-124">Boolean</span></span> | <span data-ttu-id="d5f8b-125">如果设置为 true，则删除标记和子项（如果为 false）并且标记具有子项，则删除将失败。</span><span class="sxs-lookup"><span data-stu-id="d5f8b-125">If set to true, the tag and children will be deleted, if false, and the tag has children, the delete will fail.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="d5f8b-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="d5f8b-126">Request headers</span></span>

|<span data-ttu-id="d5f8b-127">名称</span><span class="sxs-lookup"><span data-stu-id="d5f8b-127">Name</span></span>|<span data-ttu-id="d5f8b-128">说明</span><span class="sxs-lookup"><span data-stu-id="d5f8b-128">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d5f8b-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="d5f8b-129">Authorization</span></span>|<span data-ttu-id="d5f8b-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d5f8b-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d5f8b-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="d5f8b-132">Request body</span></span>

<span data-ttu-id="d5f8b-133">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d5f8b-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d5f8b-134">响应</span><span class="sxs-lookup"><span data-stu-id="d5f8b-134">Response</span></span>

<span data-ttu-id="d5f8b-135">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="d5f8b-135">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="d5f8b-136">示例</span><span class="sxs-lookup"><span data-stu-id="d5f8b-136">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d5f8b-137">请求</span><span class="sxs-lookup"><span data-stu-id="d5f8b-137">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_tag"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/tags/9985bd266f2f459cbebc81522734b452?forcedelete=true
```

### <a name="response"></a><span data-ttu-id="d5f8b-138">响应</span><span class="sxs-lookup"><span data-stu-id="d5f8b-138">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```

---
title: 更新 sourceCollection
description: 更新 sourceCollection 对象的属性。
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 254d2422c344580e1a02dbbce0d76330d6df3ef8
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50445995"
---
# <a name="update-sourcecollection"></a><span data-ttu-id="2a43a-103">更新 sourceCollection</span><span class="sxs-lookup"><span data-stu-id="2a43a-103">Update sourceCollection</span></span>

<span data-ttu-id="2a43a-104">命名空间：microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="2a43a-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2a43a-105">更新 [sourceCollection](../resources/ediscovery-sourcecollection.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="2a43a-105">Update the properties of a [sourceCollection](../resources/ediscovery-sourcecollection.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="2a43a-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="2a43a-106">Permissions</span></span>

<span data-ttu-id="2a43a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2a43a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2a43a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="2a43a-109">Permission type</span></span>|<span data-ttu-id="2a43a-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2a43a-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2a43a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2a43a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2a43a-112">eDiscovery.Read.All、eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a43a-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="2a43a-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2a43a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2a43a-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="2a43a-114">Not supported.</span></span>|
|<span data-ttu-id="2a43a-115">Application</span><span class="sxs-lookup"><span data-stu-id="2a43a-115">Application</span></span>|<span data-ttu-id="2a43a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="2a43a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2a43a-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2a43a-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
PATCH /compliance/ediscovery/cases/{caseId}/sourceCollections/{sourceCollectionId}
```

## <a name="request-headers"></a><span data-ttu-id="2a43a-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="2a43a-118">Request headers</span></span>

|<span data-ttu-id="2a43a-119">名称</span><span class="sxs-lookup"><span data-stu-id="2a43a-119">Name</span></span>|<span data-ttu-id="2a43a-120">说明</span><span class="sxs-lookup"><span data-stu-id="2a43a-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="2a43a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="2a43a-121">Authorization</span></span>|<span data-ttu-id="2a43a-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2a43a-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="2a43a-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2a43a-124">Content-Type</span></span>|<span data-ttu-id="2a43a-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="2a43a-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2a43a-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="2a43a-127">Request body</span></span>

<span data-ttu-id="2a43a-128">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="2a43a-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="2a43a-129">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="2a43a-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="2a43a-130">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="2a43a-130">For best performance, don't include existing values that haven't changed.</span></span>

|<span data-ttu-id="2a43a-131">属性</span><span class="sxs-lookup"><span data-stu-id="2a43a-131">Property</span></span>|<span data-ttu-id="2a43a-132">类型</span><span class="sxs-lookup"><span data-stu-id="2a43a-132">Type</span></span>|<span data-ttu-id="2a43a-133">说明</span><span class="sxs-lookup"><span data-stu-id="2a43a-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2a43a-134">contentQuery</span><span class="sxs-lookup"><span data-stu-id="2a43a-134">contentQuery</span></span>|<span data-ttu-id="2a43a-135">String</span><span class="sxs-lookup"><span data-stu-id="2a43a-135">String</span></span>|<span data-ttu-id="2a43a-136">KQL 中的查询字符串 (关键字查询语言) 查询。</span><span class="sxs-lookup"><span data-stu-id="2a43a-136">The query string in KQL (Keyword Query Language) query.</span></span> <span data-ttu-id="2a43a-137">有关详细信息，请参阅内容搜索和电子数据展示的关键字 [查询和搜索条件](/microsoft-365/compliance/keyword-queries-and-search-conditions)。</span><span class="sxs-lookup"><span data-stu-id="2a43a-137">For details, see [Keyword queries and search conditions for Content Search and eDiscovery](/microsoft-365/compliance/keyword-queries-and-search-conditions).</span></span>  <span data-ttu-id="2a43a-138">可以使用与值配对的字段来优化搜索;例如 `subject:"Quarterly Financials" AND Date>=06/01/2016 AND Date<=07/01/2016` ，。</span><span class="sxs-lookup"><span data-stu-id="2a43a-138">You can refine searches by using fields paired with values; for example, `subject:"Quarterly Financials" AND Date>=06/01/2016 AND Date<=07/01/2016`.</span></span>|
|<span data-ttu-id="2a43a-139">说明</span><span class="sxs-lookup"><span data-stu-id="2a43a-139">description</span></span>|<span data-ttu-id="2a43a-140">String</span><span class="sxs-lookup"><span data-stu-id="2a43a-140">String</span></span>|<span data-ttu-id="2a43a-141">**sourceCollection 的说明**。</span><span class="sxs-lookup"><span data-stu-id="2a43a-141">The description of the **sourceCollection**.</span></span>|
|<span data-ttu-id="2a43a-142">displayName</span><span class="sxs-lookup"><span data-stu-id="2a43a-142">displayName</span></span>|<span data-ttu-id="2a43a-143">String</span><span class="sxs-lookup"><span data-stu-id="2a43a-143">String</span></span>|<span data-ttu-id="2a43a-144">**sourceCollection** 的 显示名称 。</span><span class="sxs-lookup"><span data-stu-id="2a43a-144">The display name of the **sourceCollection**.</span></span>|
|<span data-ttu-id="2a43a-145">tenantSources</span><span class="sxs-lookup"><span data-stu-id="2a43a-145">tenantSources</span></span>|<span data-ttu-id="2a43a-146">microsoft.graph.ediscovery.tenantSources</span><span class="sxs-lookup"><span data-stu-id="2a43a-146">microsoft.graph.ediscovery.tenantSources</span></span>|<span data-ttu-id="2a43a-147">指定此参数时，集合将跨越整个工作负荷的服务。</span><span class="sxs-lookup"><span data-stu-id="2a43a-147">When specified, the collection will span across a service for an entire workload.</span></span> <span data-ttu-id="2a43a-148">可取值为：`allMailboxes`、`allSites`。</span><span class="sxs-lookup"><span data-stu-id="2a43a-148">Possible values are: `allMailboxes`, `allSites`.</span></span>|

## <a name="response"></a><span data-ttu-id="2a43a-149">响应</span><span class="sxs-lookup"><span data-stu-id="2a43a-149">Response</span></span>

<span data-ttu-id="2a43a-150">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="2a43a-150">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="2a43a-151">示例</span><span class="sxs-lookup"><span data-stu-id="2a43a-151">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2a43a-152">请求</span><span class="sxs-lookup"><span data-stu-id="2a43a-152">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "update_sourcecollection"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/compliance/ediscovery/cases/{caseId}/sourceCollections/1a9b4145d8f84e39bc45a7f68c5c5119
Content-Type: application/json
Content-length: 247

{
    "displayName": "Quarterly Financials search",
}
```

### <a name="response"></a><span data-ttu-id="2a43a-153">响应</span><span class="sxs-lookup"><span data-stu-id="2a43a-153">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```

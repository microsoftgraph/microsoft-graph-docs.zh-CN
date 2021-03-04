---
title: estimateStatisticsOperation 资源类型
description: 表示处理估计源集合的计数和大小的操作。
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: e816ba01d4bb648a8e78b5b96369236f63fb163e
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446623"
---
# <a name="estimatestatisticsoperation-resource-type"></a><span data-ttu-id="07e7f-103">estimateStatisticsOperation 资源类型</span><span class="sxs-lookup"><span data-stu-id="07e7f-103">estimateStatisticsOperation resource type</span></span>

<span data-ttu-id="07e7f-104">命名空间：microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="07e7f-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="07e7f-105">表示处理估计 [sourceCollection](../resources/ediscovery-sourcecollection.md)的计数和大小的操作。</span><span class="sxs-lookup"><span data-stu-id="07e7f-105">Represents the operation that handles estimating the count and size of a [sourceCollection](../resources/ediscovery-sourcecollection.md).</span></span> <span data-ttu-id="07e7f-106">有关详细信息，请参阅 ["收集高级电子数据展示](/microsoft-365/compliance/collecting-data-for-ediscovery)"中案例的数据。</span><span class="sxs-lookup"><span data-stu-id="07e7f-106">For details, see [Collect data for a case in Advanced eDiscovery](/microsoft-365/compliance/collecting-data-for-ediscovery).</span></span>

<span data-ttu-id="07e7f-107">继承自 [caseOperation](../resources/ediscovery-caseoperation.md)。</span><span class="sxs-lookup"><span data-stu-id="07e7f-107">Inherits from [caseOperation](../resources/ediscovery-caseoperation.md).</span></span>

## <a name="methods"></a><span data-ttu-id="07e7f-108">Methods</span><span class="sxs-lookup"><span data-stu-id="07e7f-108">Methods</span></span>

<span data-ttu-id="07e7f-109">无。</span><span class="sxs-lookup"><span data-stu-id="07e7f-109">None.</span></span>

## <a name="properties"></a><span data-ttu-id="07e7f-110">属性</span><span class="sxs-lookup"><span data-stu-id="07e7f-110">Properties</span></span>

|<span data-ttu-id="07e7f-111">属性</span><span class="sxs-lookup"><span data-stu-id="07e7f-111">Property</span></span>|<span data-ttu-id="07e7f-112">类型</span><span class="sxs-lookup"><span data-stu-id="07e7f-112">Type</span></span>|<span data-ttu-id="07e7f-113">说明</span><span class="sxs-lookup"><span data-stu-id="07e7f-113">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="07e7f-114">action</span><span class="sxs-lookup"><span data-stu-id="07e7f-114">action</span></span>|<span data-ttu-id="07e7f-115">microsoft.graph.ediscovery.caseAction</span><span class="sxs-lookup"><span data-stu-id="07e7f-115">microsoft.graph.ediscovery.caseAction</span></span>| <span data-ttu-id="07e7f-116">操作类型。</span><span class="sxs-lookup"><span data-stu-id="07e7f-116">The type of operation.</span></span> <span data-ttu-id="07e7f-117">此实体的大小写操作将始终为 `estimateStatistics` 。</span><span class="sxs-lookup"><span data-stu-id="07e7f-117">The case action for this entity will always be `estimateStatistics`.</span></span> <span data-ttu-id="07e7f-118">只读。</span><span class="sxs-lookup"><span data-stu-id="07e7f-118">Read-only.</span></span> <span data-ttu-id="07e7f-119">继承自 [caseOperation](../resources/ediscovery-caseoperation.md)。</span><span class="sxs-lookup"><span data-stu-id="07e7f-119">Inherited from [caseOperation](../resources/ediscovery-caseoperation.md).</span></span>|
|<span data-ttu-id="07e7f-120">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="07e7f-120">completedDateTime</span></span>|<span data-ttu-id="07e7f-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="07e7f-121">DateTimeOffset</span></span>|<span data-ttu-id="07e7f-122">操作完成的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="07e7f-122">The date and time the operation was completed.</span></span> <span data-ttu-id="07e7f-123">只读。</span><span class="sxs-lookup"><span data-stu-id="07e7f-123">Read-only.</span></span> <span data-ttu-id="07e7f-124">继承自 [caseOperation](../resources/ediscovery-caseoperation.md)。</span><span class="sxs-lookup"><span data-stu-id="07e7f-124">Inherited from [caseOperation](../resources/ediscovery-caseoperation.md).</span></span>|
|<span data-ttu-id="07e7f-125">createdBy</span><span class="sxs-lookup"><span data-stu-id="07e7f-125">createdBy</span></span>|[<span data-ttu-id="07e7f-126">identitySet</span><span class="sxs-lookup"><span data-stu-id="07e7f-126">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="07e7f-127">创建操作的用户。</span><span class="sxs-lookup"><span data-stu-id="07e7f-127">The user who created the operation.</span></span> <span data-ttu-id="07e7f-128">只读。</span><span class="sxs-lookup"><span data-stu-id="07e7f-128">Read-only.</span></span> <span data-ttu-id="07e7f-129">继承自 [caseOperation](../resources/ediscovery-caseoperation.md)。</span><span class="sxs-lookup"><span data-stu-id="07e7f-129">Inherited from [caseOperation](../resources/ediscovery-caseoperation.md).</span></span>|
|<span data-ttu-id="07e7f-130">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="07e7f-130">createdDateTime</span></span>|<span data-ttu-id="07e7f-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="07e7f-131">DateTimeOffset</span></span>|<span data-ttu-id="07e7f-132">操作开始的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="07e7f-132">The date and time the operation was started.</span></span> <span data-ttu-id="07e7f-133">只读。</span><span class="sxs-lookup"><span data-stu-id="07e7f-133">Read-only.</span></span> <span data-ttu-id="07e7f-134">继承自 [caseOperation](../resources/ediscovery-caseoperation.md)。</span><span class="sxs-lookup"><span data-stu-id="07e7f-134">Inherited from [caseOperation](../resources/ediscovery-caseoperation.md).</span></span>|
|<span data-ttu-id="07e7f-135">id</span><span class="sxs-lookup"><span data-stu-id="07e7f-135">id</span></span>|<span data-ttu-id="07e7f-136">String</span><span class="sxs-lookup"><span data-stu-id="07e7f-136">String</span></span>| <span data-ttu-id="07e7f-137">操作 ID。</span><span class="sxs-lookup"><span data-stu-id="07e7f-137">The ID for the operation.</span></span> <span data-ttu-id="07e7f-138">只读。</span><span class="sxs-lookup"><span data-stu-id="07e7f-138">Read-only.</span></span> <span data-ttu-id="07e7f-139">继承自 [caseOperation](../resources/ediscovery-caseoperation.md)。</span><span class="sxs-lookup"><span data-stu-id="07e7f-139">Inherited from [caseOperation](../resources/ediscovery-caseoperation.md).</span></span>|
|<span data-ttu-id="07e7f-140">indexedItemCount</span><span class="sxs-lookup"><span data-stu-id="07e7f-140">indexedItemCount</span></span>|<span data-ttu-id="07e7f-141">Int64</span><span class="sxs-lookup"><span data-stu-id="07e7f-141">Int64</span></span>|<span data-ttu-id="07e7f-142">与内容查询匹配的 **sourceCollection** 的预计项目计数。</span><span class="sxs-lookup"><span data-stu-id="07e7f-142">The estimated count of items for the **sourceCollection** that matched the content query.</span></span>|
|<span data-ttu-id="07e7f-143">indexedItemsSize</span><span class="sxs-lookup"><span data-stu-id="07e7f-143">indexedItemsSize</span></span>|<span data-ttu-id="07e7f-144">Int64</span><span class="sxs-lookup"><span data-stu-id="07e7f-144">Int64</span></span>|<span data-ttu-id="07e7f-145">与内容查询匹配的 **sourceCollection** 项目的估计大小。</span><span class="sxs-lookup"><span data-stu-id="07e7f-145">The estimated size of items for the **sourceCollection** that matched the content query.</span></span>|
|<span data-ttu-id="07e7f-146">mailboxCount</span><span class="sxs-lookup"><span data-stu-id="07e7f-146">mailboxCount</span></span>|<span data-ttu-id="07e7f-147">Int32</span><span class="sxs-lookup"><span data-stu-id="07e7f-147">Int32</span></span>|<span data-ttu-id="07e7f-148">搜索命中的邮箱数。</span><span class="sxs-lookup"><span data-stu-id="07e7f-148">The number of mailboxes that had search hits.</span></span>|
|<span data-ttu-id="07e7f-149">percentProgress</span><span class="sxs-lookup"><span data-stu-id="07e7f-149">percentProgress</span></span>|<span data-ttu-id="07e7f-150">Int32</span><span class="sxs-lookup"><span data-stu-id="07e7f-150">Int32</span></span>|<span data-ttu-id="07e7f-151">操作的进度。</span><span class="sxs-lookup"><span data-stu-id="07e7f-151">The progress of the operation.</span></span> <span data-ttu-id="07e7f-152">只读。</span><span class="sxs-lookup"><span data-stu-id="07e7f-152">Read-only.</span></span> <span data-ttu-id="07e7f-153">继承自 [caseOperation](../resources/ediscovery-caseoperation.md)。</span><span class="sxs-lookup"><span data-stu-id="07e7f-153">Inherited from [caseOperation](../resources/ediscovery-caseoperation.md).</span></span>|
|<span data-ttu-id="07e7f-154">resultInfo</span><span class="sxs-lookup"><span data-stu-id="07e7f-154">resultInfo</span></span>|[<span data-ttu-id="07e7f-155">resultInfo</span><span class="sxs-lookup"><span data-stu-id="07e7f-155">resultInfo</span></span>](../resources/resultinfo.md)|<span data-ttu-id="07e7f-156">包含特定于成功和失败的结果信息。</span><span class="sxs-lookup"><span data-stu-id="07e7f-156">Contains success and failure-specific result information.</span></span> <span data-ttu-id="07e7f-157">继承自 [caseOperation](../resources/ediscovery-caseoperation.md)。</span><span class="sxs-lookup"><span data-stu-id="07e7f-157">Inherited from [caseOperation](../resources/ediscovery-caseoperation.md).</span></span>|
|<span data-ttu-id="07e7f-158">siteCount</span><span class="sxs-lookup"><span data-stu-id="07e7f-158">siteCount</span></span>|<span data-ttu-id="07e7f-159">Int32</span><span class="sxs-lookup"><span data-stu-id="07e7f-159">Int32</span></span>|<span data-ttu-id="07e7f-160">搜索命中的邮箱数。</span><span class="sxs-lookup"><span data-stu-id="07e7f-160">The number of mailboxes that had search hits.</span></span>|
|<span data-ttu-id="07e7f-161">status</span><span class="sxs-lookup"><span data-stu-id="07e7f-161">status</span></span>|[<span data-ttu-id="07e7f-162">microsoft.graph.ediscovery.caseOperationStatus</span><span class="sxs-lookup"><span data-stu-id="07e7f-162">microsoft.graph.ediscovery.caseOperationStatus</span></span>](../resources/ediscovery-caseoperation.md#caseoperationstatus-values)|<span data-ttu-id="07e7f-163">案例操作的状态。</span><span class="sxs-lookup"><span data-stu-id="07e7f-163">The status of the case operation.</span></span> <span data-ttu-id="07e7f-164">继承自 [caseOperation](../resources/ediscovery-caseoperation.md)。</span><span class="sxs-lookup"><span data-stu-id="07e7f-164">Inherited from [caseOperation](../resources/ediscovery-caseoperation.md).</span></span> <span data-ttu-id="07e7f-165">可取值为：`notStarted`、`submissionFailed`、`running`、`succeeded`、`partiallySucceeded`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="07e7f-165">Possible values are: `notStarted`, `submissionFailed`, `running`, `succeeded`, `partiallySucceeded`, `failed`.</span></span>|
|<span data-ttu-id="07e7f-166">unindexedItemCount</span><span class="sxs-lookup"><span data-stu-id="07e7f-166">unindexedItemCount</span></span>|<span data-ttu-id="07e7f-167">Int64</span><span class="sxs-lookup"><span data-stu-id="07e7f-167">Int64</span></span>|<span data-ttu-id="07e7f-168">集合的未索引项的估计计数。</span><span class="sxs-lookup"><span data-stu-id="07e7f-168">The estimated count of unindexed items for the collection.</span></span>|
|<span data-ttu-id="07e7f-169">unindexedItemsSize</span><span class="sxs-lookup"><span data-stu-id="07e7f-169">unindexedItemsSize</span></span>|<span data-ttu-id="07e7f-170">Int64</span><span class="sxs-lookup"><span data-stu-id="07e7f-170">Int64</span></span>|<span data-ttu-id="07e7f-171">集合的未索引项的估计大小。</span><span class="sxs-lookup"><span data-stu-id="07e7f-171">The estimated size of unindexed items for the collection.</span></span>|

## <a name="relationships"></a><span data-ttu-id="07e7f-172">关系</span><span class="sxs-lookup"><span data-stu-id="07e7f-172">Relationships</span></span>

|<span data-ttu-id="07e7f-173">关系</span><span class="sxs-lookup"><span data-stu-id="07e7f-173">Relationship</span></span>|<span data-ttu-id="07e7f-174">类型</span><span class="sxs-lookup"><span data-stu-id="07e7f-174">Type</span></span>|<span data-ttu-id="07e7f-175">说明</span><span class="sxs-lookup"><span data-stu-id="07e7f-175">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="07e7f-176">sourceCollection</span><span class="sxs-lookup"><span data-stu-id="07e7f-176">sourceCollection</span></span>|[<span data-ttu-id="07e7f-177">microsoft.graph.ediscovery.sourceCollection</span><span class="sxs-lookup"><span data-stu-id="07e7f-177">microsoft.graph.ediscovery.sourceCollection</span></span>](../resources/ediscovery-sourcecollection.md)|<span data-ttu-id="07e7f-178">电子数据展示集合，通常称为搜索。</span><span class="sxs-lookup"><span data-stu-id="07e7f-178">eDiscovery collection, commonly known as a search.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="07e7f-179">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="07e7f-179">JSON representation</span></span>

<span data-ttu-id="07e7f-180">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="07e7f-180">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.ediscovery.estimateStatisticsOperation",
  "baseType": "microsoft.graph.ediscovery.caseOperation",
  "openType": false
}
-->

``` json
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/operations/$entity",
    "@odata.type": "#microsoft.graph.ediscovery.estimateStatisticsOperation",
    "createdDateTime": "2021-01-12T18:47:23.3974907Z",
    "completedDateTime": "2021-01-12T18:47:51.1461805Z",
    "percentProgress": 100,
    "status": "succeeded",
    "action": "estimateStatistics",
    "id": "82edd40e182a464fa02c24a36fa94873",
    "indexedItemCount": 2,
    "indexedItemsSize": 39276,
    "unindexedItemCount": 0,
    "unindexedItemsSize": 0,
    "mailboxCount": 1,
    "siteCount": 0,
    "createdBy": {
        "user": {
            "id": "c1db6f13-332a-4d84-b111-914383ff9fc9",
            "displayName": null,
            "userPrincipalName": "admin@contoso.com"
        }
    }
}
```

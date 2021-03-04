---
title: sourceCollection 资源类型
description: 表示一个电子数据展示集合，通常称为搜索。
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 86ecf3adb64be2b216fdc167b29c10a850e25af6
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446149"
---
# <a name="sourcecollection-resource-type"></a><span data-ttu-id="92cde-103">sourceCollection 资源类型</span><span class="sxs-lookup"><span data-stu-id="92cde-103">sourceCollection resource type</span></span>

<span data-ttu-id="92cde-104">命名空间：microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="92cde-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="92cde-105">表示一个电子数据展示集合，通常称为搜索。</span><span class="sxs-lookup"><span data-stu-id="92cde-105">Represents an eDiscovery collection, commonly known as a search.</span></span> <span data-ttu-id="92cde-106">有关详细信息，请参阅 ["收集高级电子数据展示](/microsoft-365/compliance/collecting-data-for-ediscovery)"中案例的数据。</span><span class="sxs-lookup"><span data-stu-id="92cde-106">For details, see [Collect data for a case in Advanced eDiscovery](/microsoft-365/compliance/collecting-data-for-ediscovery).</span></span>

## <a name="methods"></a><span data-ttu-id="92cde-107">Methods</span><span class="sxs-lookup"><span data-stu-id="92cde-107">Methods</span></span>

|<span data-ttu-id="92cde-108">方法</span><span class="sxs-lookup"><span data-stu-id="92cde-108">Method</span></span>|<span data-ttu-id="92cde-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="92cde-109">Return type</span></span>|<span data-ttu-id="92cde-110">说明</span><span class="sxs-lookup"><span data-stu-id="92cde-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="92cde-111">列出 sourceCollections</span><span class="sxs-lookup"><span data-stu-id="92cde-111">List sourceCollections</span></span>](../api/ediscovery-case-list-sourcecollections.md)|<span data-ttu-id="92cde-112">[microsoft.graph.ediscovery.sourceCollection](../resources/ediscovery-sourcecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="92cde-112">[microsoft.graph.ediscovery.sourceCollection](../resources/ediscovery-sourcecollection.md) collection</span></span>|<span data-ttu-id="92cde-113">获取 **sourceCollection** 对象及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="92cde-113">Get a list of the **sourceCollection** objects and their properties.</span></span>|
|[<span data-ttu-id="92cde-114">创建 sourceCollection</span><span class="sxs-lookup"><span data-stu-id="92cde-114">Create sourceCollection</span></span>](../api/ediscovery-case-post-sourcecollections.md)|[<span data-ttu-id="92cde-115">microsoft.graph.ediscovery.sourceCollection</span><span class="sxs-lookup"><span data-stu-id="92cde-115">microsoft.graph.ediscovery.sourceCollection</span></span>](../resources/ediscovery-sourcecollection.md)|<span data-ttu-id="92cde-116">创建新的 **sourceCollection** 对象。</span><span class="sxs-lookup"><span data-stu-id="92cde-116">Create a new **sourceCollection** object.</span></span>|
|[<span data-ttu-id="92cde-117">获取 sourceCollection</span><span class="sxs-lookup"><span data-stu-id="92cde-117">Get sourceCollection</span></span>](../api/ediscovery-sourcecollection-get.md)|[<span data-ttu-id="92cde-118">microsoft.graph.ediscovery.sourceCollection</span><span class="sxs-lookup"><span data-stu-id="92cde-118">microsoft.graph.ediscovery.sourceCollection</span></span>](../resources/ediscovery-sourcecollection.md)|<span data-ttu-id="92cde-119">读取 **sourceCollection 对象的属性和** 关系。</span><span class="sxs-lookup"><span data-stu-id="92cde-119">Read the properties and relationships of a **sourceCollection** object.</span></span>|
|[<span data-ttu-id="92cde-120">更新 sourceCollection</span><span class="sxs-lookup"><span data-stu-id="92cde-120">Update sourceCollection</span></span>](../api/ediscovery-sourcecollection-update.md)|[<span data-ttu-id="92cde-121">microsoft.graph.ediscovery.sourceCollection</span><span class="sxs-lookup"><span data-stu-id="92cde-121">microsoft.graph.ediscovery.sourceCollection</span></span>](../resources/ediscovery-sourcecollection.md)|<span data-ttu-id="92cde-122">更新 **sourceCollection** 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="92cde-122">Update the properties of a **sourceCollection** object.</span></span>|
|[<span data-ttu-id="92cde-123">删除 sourceCollection</span><span class="sxs-lookup"><span data-stu-id="92cde-123">Delete sourceCollection</span></span>](../api/ediscovery-sourcecollection-delete.md)|<span data-ttu-id="92cde-124">无</span><span class="sxs-lookup"><span data-stu-id="92cde-124">None</span></span>|<span data-ttu-id="92cde-125">删除 **sourceCollection** 对象。</span><span class="sxs-lookup"><span data-stu-id="92cde-125">Delete a **sourceCollection** object.</span></span>|
|[<span data-ttu-id="92cde-126">estimateStatistics</span><span class="sxs-lookup"><span data-stu-id="92cde-126">estimateStatistics</span></span>](../api/ediscovery-sourcecollection-estimatestatistics.md)|<span data-ttu-id="92cde-127">无</span><span class="sxs-lookup"><span data-stu-id="92cde-127">None</span></span>|<span data-ttu-id="92cde-128">运行源集合中电子邮件和文档的估计数量。</span><span class="sxs-lookup"><span data-stu-id="92cde-128">Run an estimate of the number of emails and documents in the source collection.</span></span>|
|[<span data-ttu-id="92cde-129">列出 additionalSources</span><span class="sxs-lookup"><span data-stu-id="92cde-129">List additionalSources</span></span>](../api/ediscovery-sourcecollection-list-additionalsources.md)|<span data-ttu-id="92cde-130">[microsoft.graph.ediscovery.dataSource](../resources/ediscovery-datasource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="92cde-130">[microsoft.graph.ediscovery.dataSource](../resources/ediscovery-datasource.md) collection</span></span>|<span data-ttu-id="92cde-131">获取与源集合关联的其他 **DataSource** 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="92cde-131">Get a list of additional **dataSource** objects associated with a source collection.</span></span>|
|[<span data-ttu-id="92cde-132">列出 custodianSources</span><span class="sxs-lookup"><span data-stu-id="92cde-132">List custodianSources</span></span>](../api/ediscovery-sourcecollection-list-custodiansources.md)|<span data-ttu-id="92cde-133">[microsoft.graph.ediscovery.dataSource](../resources/ediscovery-datasource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="92cde-133">[microsoft.graph.ediscovery.dataSource](../resources/ediscovery-datasource.md) collection</span></span>|<span data-ttu-id="92cde-134">获取与源集合关联的其他 **DataSource** 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="92cde-134">Get a list of additional **dataSource** objects associated with a source collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="92cde-135">属性</span><span class="sxs-lookup"><span data-stu-id="92cde-135">Properties</span></span>

|<span data-ttu-id="92cde-136">属性</span><span class="sxs-lookup"><span data-stu-id="92cde-136">Property</span></span>|<span data-ttu-id="92cde-137">类型</span><span class="sxs-lookup"><span data-stu-id="92cde-137">Type</span></span>|<span data-ttu-id="92cde-138">说明</span><span class="sxs-lookup"><span data-stu-id="92cde-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="92cde-139">contentQuery</span><span class="sxs-lookup"><span data-stu-id="92cde-139">contentQuery</span></span>|<span data-ttu-id="92cde-140">String</span><span class="sxs-lookup"><span data-stu-id="92cde-140">String</span></span>|<span data-ttu-id="92cde-141">KQL 中的查询字符串 (关键字查询语言) 查询。</span><span class="sxs-lookup"><span data-stu-id="92cde-141">The query string in KQL (Keyword Query Language) query.</span></span> <span data-ttu-id="92cde-142">有关详细信息，请参阅内容搜索和电子数据展示的关键字 [查询和搜索条件](https://docs.microsoft.com/microsoft-365/compliance/keyword-queries-and-search-conditions)。</span><span class="sxs-lookup"><span data-stu-id="92cde-142">For details, see [Keyword queries and search conditions for Content Search and eDiscovery](https://docs.microsoft.com/microsoft-365/compliance/keyword-queries-and-search-conditions).</span></span>  <span data-ttu-id="92cde-143">可以使用与值配对的字段来优化搜索;例如 *，subject："Quarterly Financials" AND Date>=06/01/2016 AND Date<=07/01/2016*</span><span class="sxs-lookup"><span data-stu-id="92cde-143">You can refine searches by using fields paired with values; for example, *subject:"Quarterly Financials" AND Date>=06/01/2016 AND Date<=07/01/2016*</span></span>|
|<span data-ttu-id="92cde-144">createdBy</span><span class="sxs-lookup"><span data-stu-id="92cde-144">createdBy</span></span>|[<span data-ttu-id="92cde-145">identitySet</span><span class="sxs-lookup"><span data-stu-id="92cde-145">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="92cde-146">创建 **sourceCollection 的用户**。</span><span class="sxs-lookup"><span data-stu-id="92cde-146">The user who created the **sourceCollection**.</span></span>|
|<span data-ttu-id="92cde-147">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="92cde-147">createdDateTime</span></span>|<span data-ttu-id="92cde-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="92cde-148">DateTimeOffset</span></span>|<span data-ttu-id="92cde-149">创建 **sourceCollection 的** 日期和时间。</span><span class="sxs-lookup"><span data-stu-id="92cde-149">The date and time the **sourceCollection** was created.</span></span>|
|<span data-ttu-id="92cde-150">说明</span><span class="sxs-lookup"><span data-stu-id="92cde-150">description</span></span>|<span data-ttu-id="92cde-151">String</span><span class="sxs-lookup"><span data-stu-id="92cde-151">String</span></span>|<span data-ttu-id="92cde-152">**sourceCollection 的说明**</span><span class="sxs-lookup"><span data-stu-id="92cde-152">The description of the **sourceCollection**</span></span>|
|<span data-ttu-id="92cde-153">displayName</span><span class="sxs-lookup"><span data-stu-id="92cde-153">displayName</span></span>|<span data-ttu-id="92cde-154">String</span><span class="sxs-lookup"><span data-stu-id="92cde-154">String</span></span>|<span data-ttu-id="92cde-155">**sourceCollection** 显示名称</span><span class="sxs-lookup"><span data-stu-id="92cde-155">The display name of the **sourceCollection**</span></span>|
|<span data-ttu-id="92cde-156">id</span><span class="sxs-lookup"><span data-stu-id="92cde-156">id</span></span>|<span data-ttu-id="92cde-157">String</span><span class="sxs-lookup"><span data-stu-id="92cde-157">String</span></span>| <span data-ttu-id="92cde-158">**sourceCollection** 的 ID。</span><span class="sxs-lookup"><span data-stu-id="92cde-158">The ID for the **sourceCollection**.</span></span> <span data-ttu-id="92cde-159">只读。</span><span class="sxs-lookup"><span data-stu-id="92cde-159">Read-only.</span></span> |
|<span data-ttu-id="92cde-160">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="92cde-160">lastModifiedBy</span></span>|[<span data-ttu-id="92cde-161">identitySet</span><span class="sxs-lookup"><span data-stu-id="92cde-161">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="92cde-162">上次修改 **sourceCollection 的用户**。</span><span class="sxs-lookup"><span data-stu-id="92cde-162">The last user who modified the **sourceCollection**.</span></span>|
|<span data-ttu-id="92cde-163">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="92cde-163">lastModifiedDateTime</span></span>|<span data-ttu-id="92cde-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="92cde-164">DateTimeOffset</span></span>|<span data-ttu-id="92cde-165">上次修改 **sourceCollection** 的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="92cde-165">The last date and time the **sourceCollection** was modified.</span></span>|
|<span data-ttu-id="92cde-166">tenantSources</span><span class="sxs-lookup"><span data-stu-id="92cde-166">tenantSources</span></span>|<span data-ttu-id="92cde-167">microsoft.graph.ediscovery.tenantSources</span><span class="sxs-lookup"><span data-stu-id="92cde-167">microsoft.graph.ediscovery.tenantSources</span></span>|<span data-ttu-id="92cde-168">指定此参数时，集合将跨越整个工作负荷的服务。</span><span class="sxs-lookup"><span data-stu-id="92cde-168">When specified, the collection will span across a service for an entire workload.</span></span> <span data-ttu-id="92cde-169">可取值为：`allMailboxes`、`allSites`。</span><span class="sxs-lookup"><span data-stu-id="92cde-169">Possible values are: `allMailboxes`, `allSites`.</span></span>|

### <a name="tenantsources-values"></a><span data-ttu-id="92cde-170">tenantSources 值</span><span class="sxs-lookup"><span data-stu-id="92cde-170">tenantSources values</span></span>

|<span data-ttu-id="92cde-171">成员</span><span class="sxs-lookup"><span data-stu-id="92cde-171">Member</span></span>|<span data-ttu-id="92cde-172">说明</span><span class="sxs-lookup"><span data-stu-id="92cde-172">Description</span></span>|
|:----|-----------|
|<span data-ttu-id="92cde-173">allMailboxes</span><span class="sxs-lookup"><span data-stu-id="92cde-173">allMailboxes</span></span>| <span data-ttu-id="92cde-174">包含集合中所有邮箱。</span><span class="sxs-lookup"><span data-stu-id="92cde-174">Include all mailboxes in the collection.</span></span> |
|<span data-ttu-id="92cde-175">allSites</span><span class="sxs-lookup"><span data-stu-id="92cde-175">allSites</span></span>| <span data-ttu-id="92cde-176">包括集合中所有网站。</span><span class="sxs-lookup"><span data-stu-id="92cde-176">Include all sites in the collection.</span></span> |

## <a name="relationships"></a><span data-ttu-id="92cde-177">关系</span><span class="sxs-lookup"><span data-stu-id="92cde-177">Relationships</span></span>

|<span data-ttu-id="92cde-178">关系</span><span class="sxs-lookup"><span data-stu-id="92cde-178">Relationship</span></span>|<span data-ttu-id="92cde-179">类型</span><span class="sxs-lookup"><span data-stu-id="92cde-179">Type</span></span>|<span data-ttu-id="92cde-180">说明</span><span class="sxs-lookup"><span data-stu-id="92cde-180">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="92cde-181">additionalSources</span><span class="sxs-lookup"><span data-stu-id="92cde-181">additionalSources</span></span>|<span data-ttu-id="92cde-182">[microsoft.graph.ediscovery.dataSource](../resources/ediscovery-datasource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="92cde-182">[microsoft.graph.ediscovery.dataSource](../resources/ediscovery-datasource.md) collection</span></span>|<span data-ttu-id="92cde-183">向 **sourceCollection 添加其他源**。</span><span class="sxs-lookup"><span data-stu-id="92cde-183">Adds an additional source to the **sourceCollection**.</span></span>|
|<span data-ttu-id="92cde-184">addToReviewSetOperation</span><span class="sxs-lookup"><span data-stu-id="92cde-184">addToReviewSetOperation</span></span>|[<span data-ttu-id="92cde-185">microsoft.graph.ediscovery.addToReviewSetOperation</span><span class="sxs-lookup"><span data-stu-id="92cde-185">microsoft.graph.ediscovery.addToReviewSetOperation</span></span>](../resources/ediscovery-addtoreviewsetoperation.md)|<span data-ttu-id="92cde-186">将 **sourceCollection 的结果** 添加到指定的 **reviewSet**。</span><span class="sxs-lookup"><span data-stu-id="92cde-186">Adds the results of the **sourceCollection** to the specified **reviewSet**.</span></span>|
|<span data-ttu-id="92cde-187">custodianSources</span><span class="sxs-lookup"><span data-stu-id="92cde-187">custodianSources</span></span>|<span data-ttu-id="92cde-188">[microsoft.graph.ediscovery.dataSource](../resources/ediscovery-datasource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="92cde-188">[microsoft.graph.ediscovery.dataSource](../resources/ediscovery-datasource.md) collection</span></span>|<span data-ttu-id="92cde-189">**sourceCollection** 中包含的保管 **人源**。</span><span class="sxs-lookup"><span data-stu-id="92cde-189">**Custodian** sources that are included in the **sourceCollection**.</span></span>|
|<span data-ttu-id="92cde-190">lastEstimateStatisticsOperation</span><span class="sxs-lookup"><span data-stu-id="92cde-190">lastEstimateStatisticsOperation</span></span>|[<span data-ttu-id="92cde-191">microsoft.graph.ediscovery.estimateStatisticsOperation</span><span class="sxs-lookup"><span data-stu-id="92cde-191">microsoft.graph.ediscovery.estimateStatisticsOperation</span></span>](../resources/ediscovery-estimatestatisticsoperation.md)|<span data-ttu-id="92cde-192">与 **sourceCollection** 关联的最后一个估计操作。</span><span class="sxs-lookup"><span data-stu-id="92cde-192">The last estimate operation associated with the **sourceCollection**.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="92cde-193">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="92cde-193">JSON representation</span></span>

<span data-ttu-id="92cde-194">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="92cde-194">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.ediscovery.sourceCollection",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.ediscovery.sourceCollection",
  "displayName": "String",
  "description": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "createdDateTime": "String (timestamp)",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "contentQuery": "String",
  "tenantSources": "String"
}
```

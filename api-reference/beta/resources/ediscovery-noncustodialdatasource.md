---
title: noncustodialDataSource 资源类型
description: 通过非托管数据源，你可以向案例添加数据，而无需将其与保管人关联
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 1e7dd0d656a58e65e460742158cdcc70da1f1d5a
ms.sourcegitcommit: e440d855f1106390d842905d97ceb16f143db2e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/29/2021
ms.locfileid: "52080814"
---
# <a name="noncustodialdatasource-resource-type"></a><span data-ttu-id="9915d-103">noncustodialDataSource 资源类型</span><span class="sxs-lookup"><span data-stu-id="9915d-103">noncustodialDataSource resource type</span></span>

<span data-ttu-id="9915d-104">命名空间：microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="9915d-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9915d-105">通过非托管数据源，您可以向案例添加数据，而无需将其与保管人关联。</span><span class="sxs-lookup"><span data-stu-id="9915d-105">Non-custodial data sources let you add data to a case without having to associate it to a custodian.</span></span> <span data-ttu-id="9915d-106">若要了解更多信息，请访问[将非托管数据源添加到Advanced eDiscovery案例](https://docs.microsoft.com/microsoft-365/compliance/non-custodial-data-sources)</span><span class="sxs-lookup"><span data-stu-id="9915d-106">To learn more, visit [Add non-custodial data sources to an Advanced eDiscovery case ](https://docs.microsoft.com/microsoft-365/compliance/non-custodial-data-sources)</span></span>

<span data-ttu-id="9915d-107">继承自 [dataSourceContainer](../resources/ediscovery-datasourcecontainer.md)。</span><span class="sxs-lookup"><span data-stu-id="9915d-107">Inherits from [dataSourceContainer](../resources/ediscovery-datasourcecontainer.md).</span></span>

## <a name="methods"></a><span data-ttu-id="9915d-108">方法</span><span class="sxs-lookup"><span data-stu-id="9915d-108">Methods</span></span>

|<span data-ttu-id="9915d-109">方法</span><span class="sxs-lookup"><span data-stu-id="9915d-109">Method</span></span>|<span data-ttu-id="9915d-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="9915d-110">Return type</span></span>|<span data-ttu-id="9915d-111">说明</span><span class="sxs-lookup"><span data-stu-id="9915d-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="9915d-112">列出 noncustodialDataSources</span><span class="sxs-lookup"><span data-stu-id="9915d-112">List noncustodialDataSources</span></span>](../api/ediscovery-noncustodialdatasource-list.md)|<span data-ttu-id="9915d-113">[microsoft.graph.ediscovery.noncustodialDataSource](../resources/ediscovery-noncustodialdatasource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9915d-113">[microsoft.graph.ediscovery.noncustodialDataSource](../resources/ediscovery-noncustodialdatasource.md) collection</span></span>|<span data-ttu-id="9915d-114">获取 [noncustodialDataSource](../resources/ediscovery-noncustodialdatasource.md) 对象及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="9915d-114">Get a list of the [noncustodialDataSource](../resources/ediscovery-noncustodialdatasource.md) objects and their properties.</span></span>|
|[<span data-ttu-id="9915d-115">获取 noncustodialDataSource</span><span class="sxs-lookup"><span data-stu-id="9915d-115">Get noncustodialDataSource</span></span>](../api/ediscovery-noncustodialdatasource-get.md)|[<span data-ttu-id="9915d-116">microsoft.graph.ediscovery.noncustodialDataSource</span><span class="sxs-lookup"><span data-stu-id="9915d-116">microsoft.graph.ediscovery.noncustodialDataSource</span></span>](../resources/ediscovery-noncustodialdatasource.md)|<span data-ttu-id="9915d-117">读取 [noncustodialDataSource](../resources/ediscovery-noncustodialdatasource.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9915d-117">Read the properties and relationships of a [noncustodialDataSource](../resources/ediscovery-noncustodialdatasource.md) object.</span></span>|
|[<span data-ttu-id="9915d-118">Release dataSource</span><span class="sxs-lookup"><span data-stu-id="9915d-118">Release dataSource</span></span>](../api/ediscovery-noncustodialdatasource-release.md)|<span data-ttu-id="9915d-119">无</span><span class="sxs-lookup"><span data-stu-id="9915d-119">None</span></span>|<span data-ttu-id="9915d-120">释放非安全数据源。</span><span class="sxs-lookup"><span data-stu-id="9915d-120">Releases a non-custodial data source.</span></span>|
|[<span data-ttu-id="9915d-121">列出 dataSource</span><span class="sxs-lookup"><span data-stu-id="9915d-121">List dataSource</span></span>](../api/ediscovery-noncustodialdatasource-list-datasource.md)|<span data-ttu-id="9915d-122">[microsoft.graph.ediscovery.dataSource](../resources/ediscovery-datasource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9915d-122">[microsoft.graph.ediscovery.dataSource](../resources/ediscovery-datasource.md) collection</span></span>|<span data-ttu-id="9915d-123">从 dataSource 导航属性获取 dataSource 资源。</span><span class="sxs-lookup"><span data-stu-id="9915d-123">Get the dataSource resources from the dataSource navigation property.</span></span>|
|[<span data-ttu-id="9915d-124">创建 dataSource</span><span class="sxs-lookup"><span data-stu-id="9915d-124">Create dataSource</span></span>](../api/ediscovery-noncustodialdatasource-post.md)|[<span data-ttu-id="9915d-125">microsoft.graph.ediscovery.dataSource</span><span class="sxs-lookup"><span data-stu-id="9915d-125">microsoft.graph.ediscovery.dataSource</span></span>](../resources/ediscovery-datasource.md)|<span data-ttu-id="9915d-126">创建新的 dataSource 对象。</span><span class="sxs-lookup"><span data-stu-id="9915d-126">Create a new dataSource object.</span></span>|

## <a name="properties"></a><span data-ttu-id="9915d-127">属性</span><span class="sxs-lookup"><span data-stu-id="9915d-127">Properties</span></span>

|<span data-ttu-id="9915d-128">属性</span><span class="sxs-lookup"><span data-stu-id="9915d-128">Property</span></span>|<span data-ttu-id="9915d-129">类型</span><span class="sxs-lookup"><span data-stu-id="9915d-129">Type</span></span>|<span data-ttu-id="9915d-130">说明</span><span class="sxs-lookup"><span data-stu-id="9915d-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9915d-131">applyHoldToSource</span><span class="sxs-lookup"><span data-stu-id="9915d-131">applyHoldToSource</span></span>|<span data-ttu-id="9915d-132">Boolean</span><span class="sxs-lookup"><span data-stu-id="9915d-132">Boolean</span></span>|<span data-ttu-id="9915d-133">指示是否将保留应用于非 (数据源，如邮箱或网站) 。</span><span class="sxs-lookup"><span data-stu-id="9915d-133">Indicates if hold is applied to non-custodial data source (such as mailbox or site).</span></span>|
|<span data-ttu-id="9915d-134">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9915d-134">createdDateTime</span></span>|<span data-ttu-id="9915d-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9915d-135">DateTimeOffset</span></span>|<span data-ttu-id="9915d-136">创建 nonCustodialDataSource 的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="9915d-136">Created date and time of the nonCustodialDataSource.</span></span> <span data-ttu-id="9915d-137">继承自 [microsoft.graph.ediscovery.dataSourceContainer](../resources/ediscovery-datasourcecontainer.md)。</span><span class="sxs-lookup"><span data-stu-id="9915d-137">Inherited from [microsoft.graph.ediscovery.dataSourceContainer](../resources/ediscovery-datasourcecontainer.md).</span></span>|
|<span data-ttu-id="9915d-138">displayName</span><span class="sxs-lookup"><span data-stu-id="9915d-138">displayName</span></span>|<span data-ttu-id="9915d-139">String</span><span class="sxs-lookup"><span data-stu-id="9915d-139">String</span></span>|<span data-ttu-id="9915d-140">noncustodialDataSource 的显示名称。</span><span class="sxs-lookup"><span data-stu-id="9915d-140">Display name of the noncustodialDataSource.</span></span> <span data-ttu-id="9915d-141">继承自 [microsoft.graph.ediscovery.dataSourceContainer](../resources/ediscovery-datasourcecontainer.md)。</span><span class="sxs-lookup"><span data-stu-id="9915d-141">Inherited from [microsoft.graph.ediscovery.dataSourceContainer](../resources/ediscovery-datasourcecontainer.md).</span></span>|
|<span data-ttu-id="9915d-142">id</span><span class="sxs-lookup"><span data-stu-id="9915d-142">id</span></span>|<span data-ttu-id="9915d-143">String</span><span class="sxs-lookup"><span data-stu-id="9915d-143">String</span></span>|<span data-ttu-id="9915d-144">nonCustodialDataSource 的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="9915d-144">Unique identifier of the nonCustodialDataSource.</span></span> <span data-ttu-id="9915d-145">继承自 [实体](../resources/entity.md)。</span><span class="sxs-lookup"><span data-stu-id="9915d-145">Inherited from [entity](../resources/entity.md).</span></span>|
|<span data-ttu-id="9915d-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9915d-146">lastModifiedDateTime</span></span>|<span data-ttu-id="9915d-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9915d-147">DateTimeOffset</span></span>|<span data-ttu-id="9915d-148">nonCustodialDataSource 的上次修改日期和时间。</span><span class="sxs-lookup"><span data-stu-id="9915d-148">Last modified date and time of the nonCustodialDataSource.</span></span> <span data-ttu-id="9915d-149">继承自 [microsoft.graph.ediscovery.dataSourceContainer](../resources/ediscovery-datasourcecontainer.md)。</span><span class="sxs-lookup"><span data-stu-id="9915d-149">Inherited from [microsoft.graph.ediscovery.dataSourceContainer](../resources/ediscovery-datasourcecontainer.md).</span></span>|
|<span data-ttu-id="9915d-150">releasedDateTime</span><span class="sxs-lookup"><span data-stu-id="9915d-150">releasedDateTime</span></span>|<span data-ttu-id="9915d-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9915d-151">DateTimeOffset</span></span>|<span data-ttu-id="9915d-152">从案例发布 nonCustodialDataSource 的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="9915d-152">Date and time that the nonCustodialDataSource was released from the case.</span></span> <span data-ttu-id="9915d-153">继承自 [microsoft.graph.ediscovery.dataSourceContainer](../resources/ediscovery-datasourcecontainer.md)。</span><span class="sxs-lookup"><span data-stu-id="9915d-153">Inherited from [microsoft.graph.ediscovery.dataSourceContainer](../resources/ediscovery-datasourcecontainer.md).</span></span>|
|<span data-ttu-id="9915d-154">状态</span><span class="sxs-lookup"><span data-stu-id="9915d-154">status</span></span>|<span data-ttu-id="9915d-155">microsoft.graph.ediscovery.dataSourceContainerStatus</span><span class="sxs-lookup"><span data-stu-id="9915d-155">microsoft.graph.ediscovery.dataSourceContainerStatus</span></span>|<span data-ttu-id="9915d-156">nonCustodialDataSource 的最新状态。</span><span class="sxs-lookup"><span data-stu-id="9915d-156">Latest status of the nonCustodialDataSource.</span></span> <span data-ttu-id="9915d-157">继承自 [microsoft.graph.ediscovery.dataSourceContainer](../resources/ediscovery-datasourcecontainer.md)。</span><span class="sxs-lookup"><span data-stu-id="9915d-157">Inherited from [microsoft.graph.ediscovery.dataSourceContainer](../resources/ediscovery-datasourcecontainer.md).</span></span> <span data-ttu-id="9915d-158">可取值为：`Active`、`Released`。</span><span class="sxs-lookup"><span data-stu-id="9915d-158">Possible values are: `Active`, `Released`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9915d-159">关系</span><span class="sxs-lookup"><span data-stu-id="9915d-159">Relationships</span></span>

|<span data-ttu-id="9915d-160">关系</span><span class="sxs-lookup"><span data-stu-id="9915d-160">Relationship</span></span>|<span data-ttu-id="9915d-161">类型</span><span class="sxs-lookup"><span data-stu-id="9915d-161">Type</span></span>|<span data-ttu-id="9915d-162">说明</span><span class="sxs-lookup"><span data-stu-id="9915d-162">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9915d-163">dataSource</span><span class="sxs-lookup"><span data-stu-id="9915d-163">dataSource</span></span>|[<span data-ttu-id="9915d-164">microsoft.graph.ediscovery.dataSource</span><span class="sxs-lookup"><span data-stu-id="9915d-164">microsoft.graph.ediscovery.dataSource</span></span>](../resources/ediscovery-datasource.md)|<span data-ttu-id="9915d-165">用户源SharePoint网站数据源作为非安全数据源。</span><span class="sxs-lookup"><span data-stu-id="9915d-165">User source or SharePoint site data source as non-custodial data source.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9915d-166">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9915d-166">JSON representation</span></span>

<span data-ttu-id="9915d-167">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9915d-167">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.ediscovery.noncustodialDataSource",
  "baseType": "microsoft.graph.ediscovery.dataSourceContainer",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.ediscovery.noncustodialDataSource",
  "id": "String (identifier)",
  "status": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "releasedDateTime": "String (timestamp)",
  "displayName": "String",
  "createdDateTime": "String (timestamp)",
  "applyHoldToSource": "Boolean"
}
```

---
title: 保管人资源类型
description: 在电子数据展示上下文中，表示用户及其所有数字资产，如电子邮件和文档。
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 0d71542b796f5256f21e19a886533e3a88e1d7ed
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446658"
---
# <a name="custodian-resource-type"></a><span data-ttu-id="ade6e-103">保管人资源类型</span><span class="sxs-lookup"><span data-stu-id="ade6e-103">custodian resource type</span></span>

<span data-ttu-id="ade6e-104">命名空间：microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="ade6e-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ade6e-105">在电子数据展示上下文中，表示用户及其所有数字资产，如电子邮件和文档。</span><span class="sxs-lookup"><span data-stu-id="ade6e-105">In the context of eDiscovery, represents a user and all of their digital assets, such as email and documents.</span></span>

## <a name="methods"></a><span data-ttu-id="ade6e-106">Methods</span><span class="sxs-lookup"><span data-stu-id="ade6e-106">Methods</span></span>

|<span data-ttu-id="ade6e-107">方法</span><span class="sxs-lookup"><span data-stu-id="ade6e-107">Method</span></span>|<span data-ttu-id="ade6e-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="ade6e-108">Return type</span></span>|<span data-ttu-id="ade6e-109">说明</span><span class="sxs-lookup"><span data-stu-id="ade6e-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ade6e-110">列出保管人</span><span class="sxs-lookup"><span data-stu-id="ade6e-110">List custodians</span></span>](../api/ediscovery-case-list-custodians.md)|<span data-ttu-id="ade6e-111">[microsoft.graph.ediscovery.custodian](../resources/ediscovery-custodian.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ade6e-111">[microsoft.graph.ediscovery.custodian](../resources/ediscovery-custodian.md) collection</span></span>|<span data-ttu-id="ade6e-112">获取保管 **人对象及其** 属性的列表。</span><span class="sxs-lookup"><span data-stu-id="ade6e-112">Get a list of **custodian** objects and their properties.</span></span>|
|[<span data-ttu-id="ade6e-113">创建保管人</span><span class="sxs-lookup"><span data-stu-id="ade6e-113">Create custodian</span></span>](../api/ediscovery-case-post-custodians.md)|[<span data-ttu-id="ade6e-114">microsoft.graph.ediscovery.custodian</span><span class="sxs-lookup"><span data-stu-id="ade6e-114">microsoft.graph.ediscovery.custodian</span></span>](../resources/ediscovery-custodian.md)|<span data-ttu-id="ade6e-115">创建新的保管 **人** 对象。</span><span class="sxs-lookup"><span data-stu-id="ade6e-115">Create a new **custodian** object.</span></span>|
|[<span data-ttu-id="ade6e-116">获取保管人</span><span class="sxs-lookup"><span data-stu-id="ade6e-116">Get custodian</span></span>](../api/ediscovery-custodian-get.md)|[<span data-ttu-id="ade6e-117">microsoft.graph.ediscovery.custodian</span><span class="sxs-lookup"><span data-stu-id="ade6e-117">microsoft.graph.ediscovery.custodian</span></span>](../resources/ediscovery-custodian.md)|<span data-ttu-id="ade6e-118">读取保管人对象 **的属性** 和关系。</span><span class="sxs-lookup"><span data-stu-id="ade6e-118">Read the properties and relationships of a **custodian** object.</span></span>|
|[<span data-ttu-id="ade6e-119">更新保管人</span><span class="sxs-lookup"><span data-stu-id="ade6e-119">Update custodian</span></span>](../api/ediscovery-custodian-update.md)|[<span data-ttu-id="ade6e-120">microsoft.graph.ediscovery.custodian</span><span class="sxs-lookup"><span data-stu-id="ade6e-120">microsoft.graph.ediscovery.custodian</span></span>](../resources/ediscovery-custodian.md)|<span data-ttu-id="ade6e-121">更新保管人 **对象** 的属性。</span><span class="sxs-lookup"><span data-stu-id="ade6e-121">Update the properties of a **custodian** object.</span></span>|
|[<span data-ttu-id="ade6e-122">release</span><span class="sxs-lookup"><span data-stu-id="ade6e-122">release</span></span>](../api/ediscovery-custodian-release.md)|<span data-ttu-id="ade6e-123">无</span><span class="sxs-lookup"><span data-stu-id="ade6e-123">None</span></span>|<span data-ttu-id="ade6e-124">从案例释放保管人。</span><span class="sxs-lookup"><span data-stu-id="ade6e-124">Release a custodian from a case.</span></span>|
|[<span data-ttu-id="ade6e-125">activate</span><span class="sxs-lookup"><span data-stu-id="ade6e-125">activate</span></span>](../api/ediscovery-custodian-activate.md)|<span data-ttu-id="ade6e-126">无</span><span class="sxs-lookup"><span data-stu-id="ade6e-126">None</span></span>|<span data-ttu-id="ade6e-127">重新激活从案例释放的保管人，并再次将其作为案例的一部分。</span><span class="sxs-lookup"><span data-stu-id="ade6e-127">Reactivate a custodian that has been released from a case and make them part of the case again.</span></span>|
|[<span data-ttu-id="ade6e-128">列出 siteSources</span><span class="sxs-lookup"><span data-stu-id="ade6e-128">List siteSources</span></span>](../api/ediscovery-custodian-list-sitesources.md)|<span data-ttu-id="ade6e-129">[microsoft.graph.ediscovery.siteSource](../resources/ediscovery-sitesource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ade6e-129">[microsoft.graph.ediscovery.siteSource](../resources/ediscovery-sitesource.md) collection</span></span>|<span data-ttu-id="ade6e-130">获取与保管人关联的 **siteSource** 资源。</span><span class="sxs-lookup"><span data-stu-id="ade6e-130">Get the **siteSource** resources associated with the custodian.</span></span>|
|[<span data-ttu-id="ade6e-131">创建 siteSources</span><span class="sxs-lookup"><span data-stu-id="ade6e-131">Create siteSources</span></span>](../api/ediscovery-custodian-post-sitesources.md)|[<span data-ttu-id="ade6e-132">microsoft.graph.ediscovery.siteSource</span><span class="sxs-lookup"><span data-stu-id="ade6e-132">microsoft.graph.ediscovery.siteSource</span></span>](../resources/ediscovery-sitesource.md)|<span data-ttu-id="ade6e-133">创建新的 **siteSource** 对象。</span><span class="sxs-lookup"><span data-stu-id="ade6e-133">Create a new **siteSource** object.</span></span>|
|[<span data-ttu-id="ade6e-134">列出 unifiedGroupSources</span><span class="sxs-lookup"><span data-stu-id="ade6e-134">List unifiedGroupSources</span></span>](../api/ediscovery-custodian-list-unifiedgroupsources.md)|<span data-ttu-id="ade6e-135">[microsoft.graph.ediscovery.unifiedGroupSource](../resources/ediscovery-unifiedgroupsource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ade6e-135">[microsoft.graph.ediscovery.unifiedGroupSource](../resources/ediscovery-unifiedgroupsource.md) collection</span></span>|<span data-ttu-id="ade6e-136">获取与 **保管人关联的 unifiedGroupSource** 资源列表。</span><span class="sxs-lookup"><span data-stu-id="ade6e-136">Get the list of **unifiedGroupSource** resources associated with the custodian.</span></span>|
|[<span data-ttu-id="ade6e-137">创建 unifiedGroupSources</span><span class="sxs-lookup"><span data-stu-id="ade6e-137">Create unifiedGroupSources</span></span>](../api/ediscovery-custodian-post-unifiedgroupsources.md)|[<span data-ttu-id="ade6e-138">microsoft.graph.ediscovery.unifiedGroupSource</span><span class="sxs-lookup"><span data-stu-id="ade6e-138">microsoft.graph.ediscovery.unifiedGroupSource</span></span>](../resources/ediscovery-unifiedgroupsource.md)|<span data-ttu-id="ade6e-139">创建新的 **unifiedGroupSource** 对象。</span><span class="sxs-lookup"><span data-stu-id="ade6e-139">Create a new **unifiedGroupSource** object.</span></span>|
|[<span data-ttu-id="ade6e-140">列出 userSources</span><span class="sxs-lookup"><span data-stu-id="ade6e-140">List userSources</span></span>](../api/ediscovery-custodian-list-usersources.md)|<span data-ttu-id="ade6e-141">[microsoft.graph.ediscovery.userSource](../resources/ediscovery-usersource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ade6e-141">[microsoft.graph.ediscovery.userSource](../resources/ediscovery-usersource.md) collection</span></span>|<span data-ttu-id="ade6e-142">获取与 **保管人关联的 userSource** 资源列表。</span><span class="sxs-lookup"><span data-stu-id="ade6e-142">Get the list of **userSource** resources associated with the custodian.</span></span>|
|[<span data-ttu-id="ade6e-143">创建 userSources</span><span class="sxs-lookup"><span data-stu-id="ade6e-143">Create userSources</span></span>](../api/ediscovery-custodian-post-usersources.md)|[<span data-ttu-id="ade6e-144">microsoft.graph.ediscovery.userSource</span><span class="sxs-lookup"><span data-stu-id="ade6e-144">microsoft.graph.ediscovery.userSource</span></span>](../resources/ediscovery-usersource.md)|<span data-ttu-id="ade6e-145">创建新的 **userSource** 对象。</span><span class="sxs-lookup"><span data-stu-id="ade6e-145">Create a new **userSource** object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ade6e-146">属性</span><span class="sxs-lookup"><span data-stu-id="ade6e-146">Properties</span></span>

|<span data-ttu-id="ade6e-147">属性</span><span class="sxs-lookup"><span data-stu-id="ade6e-147">Property</span></span>|<span data-ttu-id="ade6e-148">类型</span><span class="sxs-lookup"><span data-stu-id="ade6e-148">Type</span></span>|<span data-ttu-id="ade6e-149">说明</span><span class="sxs-lookup"><span data-stu-id="ade6e-149">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ade6e-150">acknowledgedDateTime</span><span class="sxs-lookup"><span data-stu-id="ade6e-150">acknowledgedDateTime</span></span>|<span data-ttu-id="ade6e-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ade6e-151">DateTimeOffset</span></span>|<span data-ttu-id="ade6e-152">保管人确认保留通知的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="ade6e-152">Date and time the custodian acknowledged a hold notification.</span></span>|
|<span data-ttu-id="ade6e-153">applyHoldToSources</span><span class="sxs-lookup"><span data-stu-id="ade6e-153">applyHoldToSources</span></span>|<span data-ttu-id="ade6e-154">布尔</span><span class="sxs-lookup"><span data-stu-id="ade6e-154">Boolean</span></span>|<span data-ttu-id="ade6e-155">标识保管人的来源在创建期间是否处于保留状态。</span><span class="sxs-lookup"><span data-stu-id="ade6e-155">Identifies whether a custodian's sources were placed on hold during creation.</span></span>|
|<span data-ttu-id="ade6e-156">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ade6e-156">createdDateTime</span></span>|<span data-ttu-id="ade6e-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ade6e-157">DateTimeOffset</span></span>|<span data-ttu-id="ade6e-158">将保管人添加到案例的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="ade6e-158">Date and time when the custodian was added to the case.</span></span>|
|<span data-ttu-id="ade6e-159">displayName</span><span class="sxs-lookup"><span data-stu-id="ade6e-159">displayName</span></span>|<span data-ttu-id="ade6e-160">String</span><span class="sxs-lookup"><span data-stu-id="ade6e-160">String</span></span>|<span data-ttu-id="ade6e-161">保管人显示名称。</span><span class="sxs-lookup"><span data-stu-id="ade6e-161">Display name of the custodian.</span></span>|
|<span data-ttu-id="ade6e-162">email</span><span class="sxs-lookup"><span data-stu-id="ade6e-162">email</span></span>|<span data-ttu-id="ade6e-163">String</span><span class="sxs-lookup"><span data-stu-id="ade6e-163">String</span></span>|<span data-ttu-id="ade6e-164">保管人的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="ade6e-164">Email address of the custodian.</span></span>|
|<span data-ttu-id="ade6e-165">id</span><span class="sxs-lookup"><span data-stu-id="ade6e-165">id</span></span>|<span data-ttu-id="ade6e-166">String</span><span class="sxs-lookup"><span data-stu-id="ade6e-166">String</span></span>|<span data-ttu-id="ade6e-167">指定情况下保管人 ID。</span><span class="sxs-lookup"><span data-stu-id="ade6e-167">The ID for the custodian in the specified case.</span></span> <span data-ttu-id="ade6e-168">只读。</span><span class="sxs-lookup"><span data-stu-id="ade6e-168">Read-only.</span></span>|
|<span data-ttu-id="ade6e-169">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ade6e-169">lastModifiedDateTime</span></span>|<span data-ttu-id="ade6e-170">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ade6e-170">DateTimeOffset</span></span>|<span data-ttu-id="ade6e-171">上次修改保管人对象的日期和时间</span><span class="sxs-lookup"><span data-stu-id="ade6e-171">Date and time the custodian object was last modified</span></span>|
|<span data-ttu-id="ade6e-172">releasedDateTime</span><span class="sxs-lookup"><span data-stu-id="ade6e-172">releasedDateTime</span></span>|<span data-ttu-id="ade6e-173">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ade6e-173">DateTimeOffset</span></span>|<span data-ttu-id="ade6e-174">保管人从案例中释放的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="ade6e-174">Date and time the custodian was released from the case.</span></span>|
|<span data-ttu-id="ade6e-175">status</span><span class="sxs-lookup"><span data-stu-id="ade6e-175">status</span></span>|<span data-ttu-id="ade6e-176">microsoft.graph.ediscovery.custodianStatus</span><span class="sxs-lookup"><span data-stu-id="ade6e-176">microsoft.graph.ediscovery.custodianStatus</span></span>|<span data-ttu-id="ade6e-177">保管人的状态。</span><span class="sxs-lookup"><span data-stu-id="ade6e-177">Status of the custodian.</span></span> <span data-ttu-id="ade6e-178">可取值为：`active`、`released`。</span><span class="sxs-lookup"><span data-stu-id="ade6e-178">Possible values are: `active`, `released`.</span></span>|

### <a name="custodianstatus-values"></a><span data-ttu-id="ade6e-179">custodianStatus 值</span><span class="sxs-lookup"><span data-stu-id="ade6e-179">custodianStatus values</span></span>

|<span data-ttu-id="ade6e-180">成员</span><span class="sxs-lookup"><span data-stu-id="ade6e-180">Member</span></span>|<span data-ttu-id="ade6e-181">说明</span><span class="sxs-lookup"><span data-stu-id="ade6e-181">Description</span></span>|
|:----|-----------|
|<span data-ttu-id="ade6e-182">active</span><span class="sxs-lookup"><span data-stu-id="ade6e-182">active</span></span>|<span data-ttu-id="ade6e-183">Custodian 是案例的一个活动部分。</span><span class="sxs-lookup"><span data-stu-id="ade6e-183">Custodian is an active part of the case.</span></span> |
|<span data-ttu-id="ade6e-184">released</span><span class="sxs-lookup"><span data-stu-id="ade6e-184">released</span></span>|<span data-ttu-id="ade6e-185">保管人从案例中释放。</span><span class="sxs-lookup"><span data-stu-id="ade6e-185">Custodian is released from the case.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ade6e-186">关系</span><span class="sxs-lookup"><span data-stu-id="ade6e-186">Relationships</span></span>

|<span data-ttu-id="ade6e-187">关系</span><span class="sxs-lookup"><span data-stu-id="ade6e-187">Relationship</span></span>|<span data-ttu-id="ade6e-188">类型</span><span class="sxs-lookup"><span data-stu-id="ade6e-188">Type</span></span>|<span data-ttu-id="ade6e-189">说明</span><span class="sxs-lookup"><span data-stu-id="ade6e-189">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ade6e-190">siteSources</span><span class="sxs-lookup"><span data-stu-id="ade6e-190">siteSources</span></span>|<span data-ttu-id="ade6e-191">[microsoft.graph.ediscovery.siteSource](../resources/ediscovery-sitesource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ade6e-191">[microsoft.graph.ediscovery.siteSource](../resources/ediscovery-sitesource.md) collection</span></span>|<span data-ttu-id="ade6e-192">与保管人关联的 SharePoint 网站的数据源实体。</span><span class="sxs-lookup"><span data-stu-id="ade6e-192">Data source entity for SharePoint sites associated with the custodian.</span></span>|
|<span data-ttu-id="ade6e-193">unifiedGroupSources</span><span class="sxs-lookup"><span data-stu-id="ade6e-193">unifiedGroupSources</span></span>|<span data-ttu-id="ade6e-194">[microsoft.graph.ediscovery.unifiedGroupSource](../resources/ediscovery-unifiedgroupsource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ade6e-194">[microsoft.graph.ediscovery.unifiedGroupSource](../resources/ediscovery-unifiedgroupsource.md) collection</span></span>|<span data-ttu-id="ade6e-195">与保管人关联的组的数据源实体。</span><span class="sxs-lookup"><span data-stu-id="ade6e-195">Data source entity for groups associated with the custodian.</span></span>|
|<span data-ttu-id="ade6e-196">userSources</span><span class="sxs-lookup"><span data-stu-id="ade6e-196">userSources</span></span>|<span data-ttu-id="ade6e-197">[microsoft.graph.ediscovery.userSource](../resources/ediscovery-usersource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ade6e-197">[microsoft.graph.ediscovery.userSource](../resources/ediscovery-usersource.md) collection</span></span>|<span data-ttu-id="ade6e-198">保管人数据源实体。</span><span class="sxs-lookup"><span data-stu-id="ade6e-198">Data source entity for a the custodian.</span></span> <span data-ttu-id="ade6e-199">这是保管人邮箱和 OneDrive for Business 网站的容器。</span><span class="sxs-lookup"><span data-stu-id="ade6e-199">This is the container for a custodian's mailbox and OneDrive for Business site.</span></span>|

<!--|lastIndexOperation|[caseIndexOperation](../resources/caseindexoperation.md)|**TODO: Add Description**| -->

## <a name="json-representation"></a><span data-ttu-id="ade6e-200">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ade6e-200">JSON representation</span></span>

<span data-ttu-id="ade6e-201">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ade6e-201">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.ediscovery.custodian",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.ediscovery.custodian",
  "email": "String",
  "applyHoldToSources": "Boolean",
  "status": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "releasedDateTime": "String (timestamp)",
  "acknowledgedDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "displayName": "String"
}
```

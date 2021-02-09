---
title: 保管人资源类型
description: 在电子数据展示的上下文中，表示用户及其所有数字资产，如电子邮件和文档。
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: 6c6b2befbb4066b851e38e6e17fd8be5aa59b031
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50157678"
---
# <a name="custodian-resource-type"></a><span data-ttu-id="9f9d7-103">保管人资源类型</span><span class="sxs-lookup"><span data-stu-id="9f9d7-103">custodian resource type</span></span>

<span data-ttu-id="9f9d7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9f9d7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9f9d7-105">在电子数据展示的上下文中，表示用户及其所有数字资产，如电子邮件和文档。</span><span class="sxs-lookup"><span data-stu-id="9f9d7-105">In the context of eDiscovery, represents a user and all of their digital assets, such as email and documents.</span></span>

## <a name="methods"></a><span data-ttu-id="9f9d7-106">方法</span><span class="sxs-lookup"><span data-stu-id="9f9d7-106">Methods</span></span>

|<span data-ttu-id="9f9d7-107">方法</span><span class="sxs-lookup"><span data-stu-id="9f9d7-107">Method</span></span>|<span data-ttu-id="9f9d7-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="9f9d7-108">Return type</span></span>|<span data-ttu-id="9f9d7-109">说明</span><span class="sxs-lookup"><span data-stu-id="9f9d7-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="9f9d7-110">列出保管人</span><span class="sxs-lookup"><span data-stu-id="9f9d7-110">List custodians</span></span>](../api/ediscoverycase-list-custodians.md)|<span data-ttu-id="9f9d7-111">[custodian](../resources/custodian.md) collection</span><span class="sxs-lookup"><span data-stu-id="9f9d7-111">[custodian](../resources/custodian.md) collection</span></span>|<span data-ttu-id="9f9d7-112">获取保管 **人对象及其** 属性的列表。</span><span class="sxs-lookup"><span data-stu-id="9f9d7-112">Get a list of **custodian** objects and their properties.</span></span>|
|[<span data-ttu-id="9f9d7-113">创建保管人</span><span class="sxs-lookup"><span data-stu-id="9f9d7-113">Create custodian</span></span>](../api/ediscoverycase-post-custodians.md)|[<span data-ttu-id="9f9d7-114">custodian</span><span class="sxs-lookup"><span data-stu-id="9f9d7-114">custodian</span></span>](../resources/custodian.md)|<span data-ttu-id="9f9d7-115">创建新的保管 **人** 对象。</span><span class="sxs-lookup"><span data-stu-id="9f9d7-115">Create a new **custodian** object.</span></span>|
|[<span data-ttu-id="9f9d7-116">获取保管人</span><span class="sxs-lookup"><span data-stu-id="9f9d7-116">Get custodian</span></span>](../api/custodian-get.md)|[<span data-ttu-id="9f9d7-117">custodian</span><span class="sxs-lookup"><span data-stu-id="9f9d7-117">custodian</span></span>](../resources/custodian.md)|<span data-ttu-id="9f9d7-118">读取保管人对象 **的属性** 和关系。</span><span class="sxs-lookup"><span data-stu-id="9f9d7-118">Read the properties and relationships of a **custodian** object.</span></span>|
|[<span data-ttu-id="9f9d7-119">更新保管人</span><span class="sxs-lookup"><span data-stu-id="9f9d7-119">Update custodian</span></span>](../api/custodian-update.md)|[<span data-ttu-id="9f9d7-120">custodian</span><span class="sxs-lookup"><span data-stu-id="9f9d7-120">custodian</span></span>](../resources/custodian.md)|<span data-ttu-id="9f9d7-121">更新保管人 **对象** 的属性。</span><span class="sxs-lookup"><span data-stu-id="9f9d7-121">Update the properties of a **custodian** object.</span></span>|
|[<span data-ttu-id="9f9d7-122">release</span><span class="sxs-lookup"><span data-stu-id="9f9d7-122">release</span></span>](../api/custodian-release.md)|<span data-ttu-id="9f9d7-123">无</span><span class="sxs-lookup"><span data-stu-id="9f9d7-123">None</span></span>|<span data-ttu-id="9f9d7-124">从案例释放保管人。</span><span class="sxs-lookup"><span data-stu-id="9f9d7-124">Release a custodian from a case.</span></span>|
|[<span data-ttu-id="9f9d7-125">activate</span><span class="sxs-lookup"><span data-stu-id="9f9d7-125">activate</span></span>](../api/custodian-activate.md)|<span data-ttu-id="9f9d7-126">无</span><span class="sxs-lookup"><span data-stu-id="9f9d7-126">None</span></span>|<span data-ttu-id="9f9d7-127">重新激活从案例释放的保管人，并再次将其作为案例的一部分。</span><span class="sxs-lookup"><span data-stu-id="9f9d7-127">Reactivate a custodian that has been released from a case and make them part of the case again.</span></span>|
|[<span data-ttu-id="9f9d7-128">列出 siteSources</span><span class="sxs-lookup"><span data-stu-id="9f9d7-128">List siteSources</span></span>](../api/custodian-list-sitesources.md)|<span data-ttu-id="9f9d7-129">[siteSource](../resources/sitesource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9f9d7-129">[siteSource](../resources/sitesource.md) collection</span></span>|<span data-ttu-id="9f9d7-130">从 **siteSources** 导航属性获取 **siteSource** 资源。</span><span class="sxs-lookup"><span data-stu-id="9f9d7-130">Get the **siteSource** resources from the **siteSources** navigation property.</span></span>|
|[<span data-ttu-id="9f9d7-131">创建 siteSources</span><span class="sxs-lookup"><span data-stu-id="9f9d7-131">Create siteSources</span></span>](../api/custodian-post-sitesources.md)|[<span data-ttu-id="9f9d7-132">siteSource</span><span class="sxs-lookup"><span data-stu-id="9f9d7-132">siteSource</span></span>](../resources/sitesource.md)|<span data-ttu-id="9f9d7-133">创建新的 **siteSource** 对象。</span><span class="sxs-lookup"><span data-stu-id="9f9d7-133">Create a new **siteSource** object.</span></span>|
|[<span data-ttu-id="9f9d7-134">列出 unifiedGroupSources</span><span class="sxs-lookup"><span data-stu-id="9f9d7-134">List unifiedGroupSources</span></span>](../api/custodian-list-unifiedgroupsources.md)|<span data-ttu-id="9f9d7-135">[unifiedGroupSource](../resources/unifiedgroupsource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9f9d7-135">[unifiedGroupSource](../resources/unifiedgroupsource.md) collection</span></span>|<span data-ttu-id="9f9d7-136">从 **unifiedGroupSources** 导航属性获取 **unifiedGroupSource** 资源。</span><span class="sxs-lookup"><span data-stu-id="9f9d7-136">Get the **unifiedGroupSource** resources from the **unifiedGroupSources** navigation property.</span></span>|
|[<span data-ttu-id="9f9d7-137">创建 unifiedGroupSources</span><span class="sxs-lookup"><span data-stu-id="9f9d7-137">Create unifiedGroupSources</span></span>](../api/custodian-post-unifiedgroupsources.md)|[<span data-ttu-id="9f9d7-138">unifiedGroupSource</span><span class="sxs-lookup"><span data-stu-id="9f9d7-138">unifiedGroupSource</span></span>](../resources/unifiedgroupsource.md)|<span data-ttu-id="9f9d7-139">创建新的 **unifiedGroupSource** 对象。</span><span class="sxs-lookup"><span data-stu-id="9f9d7-139">Create a new **unifiedGroupSource** object.</span></span>|
|[<span data-ttu-id="9f9d7-140">列出 userSources</span><span class="sxs-lookup"><span data-stu-id="9f9d7-140">List userSources</span></span>](../api/custodian-list-usersources.md)|<span data-ttu-id="9f9d7-141">[userSource](../resources/usersource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9f9d7-141">[userSource](../resources/usersource.md) collection</span></span>|<span data-ttu-id="9f9d7-142">从 **userSources** 导航属性获取 **userSource** 资源。</span><span class="sxs-lookup"><span data-stu-id="9f9d7-142">Get the **userSource** resources from the **userSources** navigation property.</span></span>|
|[<span data-ttu-id="9f9d7-143">创建 userSources</span><span class="sxs-lookup"><span data-stu-id="9f9d7-143">Create userSources</span></span>](../api/custodian-post-usersources.md)|[<span data-ttu-id="9f9d7-144">userSource</span><span class="sxs-lookup"><span data-stu-id="9f9d7-144">userSource</span></span>](../resources/usersource.md)|<span data-ttu-id="9f9d7-145">创建新的 **userSource** 对象。</span><span class="sxs-lookup"><span data-stu-id="9f9d7-145">Create a new **userSource** object.</span></span>|

## <a name="properties"></a><span data-ttu-id="9f9d7-146">属性</span><span class="sxs-lookup"><span data-stu-id="9f9d7-146">Properties</span></span>

|<span data-ttu-id="9f9d7-147">属性</span><span class="sxs-lookup"><span data-stu-id="9f9d7-147">Property</span></span>|<span data-ttu-id="9f9d7-148">类型</span><span class="sxs-lookup"><span data-stu-id="9f9d7-148">Type</span></span>|<span data-ttu-id="9f9d7-149">说明</span><span class="sxs-lookup"><span data-stu-id="9f9d7-149">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9f9d7-150">acknowledgedDateTime</span><span class="sxs-lookup"><span data-stu-id="9f9d7-150">acknowledgedDateTime</span></span>|<span data-ttu-id="9f9d7-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9f9d7-151">DateTimeOffset</span></span>|<span data-ttu-id="9f9d7-152">保管人确认保留通知的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="9f9d7-152">Date and time the custodian acknowledged a hold notification.</span></span>|
|<span data-ttu-id="9f9d7-153">applyHoldToSources</span><span class="sxs-lookup"><span data-stu-id="9f9d7-153">applyHoldToSources</span></span>|<span data-ttu-id="9f9d7-154">布尔</span><span class="sxs-lookup"><span data-stu-id="9f9d7-154">Boolean</span></span>|<span data-ttu-id="9f9d7-155">标识保管人的来源在创建过程中是否处于保留状态。</span><span class="sxs-lookup"><span data-stu-id="9f9d7-155">Identifies whether a custodian's sources were placed on hold during creation.</span></span>|
|<span data-ttu-id="9f9d7-156">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9f9d7-156">createdDateTime</span></span>|<span data-ttu-id="9f9d7-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9f9d7-157">DateTimeOffset</span></span>|<span data-ttu-id="9f9d7-158">将保管人添加到案例的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="9f9d7-158">Date and time when the custodian was added to the case.</span></span>|
|<span data-ttu-id="9f9d7-159">displayName</span><span class="sxs-lookup"><span data-stu-id="9f9d7-159">displayName</span></span>|<span data-ttu-id="9f9d7-160">String</span><span class="sxs-lookup"><span data-stu-id="9f9d7-160">String</span></span>|<span data-ttu-id="9f9d7-161">保管人显示名称。</span><span class="sxs-lookup"><span data-stu-id="9f9d7-161">Display name of the custodian.</span></span>|
|<span data-ttu-id="9f9d7-162">email</span><span class="sxs-lookup"><span data-stu-id="9f9d7-162">email</span></span>|<span data-ttu-id="9f9d7-163">String</span><span class="sxs-lookup"><span data-stu-id="9f9d7-163">String</span></span>|<span data-ttu-id="9f9d7-164">保管人的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="9f9d7-164">Email address of the custodian.</span></span>|
|<span data-ttu-id="9f9d7-165">id</span><span class="sxs-lookup"><span data-stu-id="9f9d7-165">id</span></span>|<span data-ttu-id="9f9d7-166">String</span><span class="sxs-lookup"><span data-stu-id="9f9d7-166">String</span></span>|<span data-ttu-id="9f9d7-167">指定情况下保管人 ID。</span><span class="sxs-lookup"><span data-stu-id="9f9d7-167">The ID for the custodian in the specified case.</span></span> <span data-ttu-id="9f9d7-168">只读。</span><span class="sxs-lookup"><span data-stu-id="9f9d7-168">Read-only.</span></span>|
|<span data-ttu-id="9f9d7-169">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9f9d7-169">lastModifiedDateTime</span></span>|<span data-ttu-id="9f9d7-170">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9f9d7-170">DateTimeOffset</span></span>|<span data-ttu-id="9f9d7-171">保管人对象的上次修改日期和时间</span><span class="sxs-lookup"><span data-stu-id="9f9d7-171">Date and time the custodian object was last modified</span></span>|
|<span data-ttu-id="9f9d7-172">releasedDateTime</span><span class="sxs-lookup"><span data-stu-id="9f9d7-172">releasedDateTime</span></span>|<span data-ttu-id="9f9d7-173">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9f9d7-173">DateTimeOffset</span></span>|<span data-ttu-id="9f9d7-174">保管人从案例中释放的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="9f9d7-174">Date and time the custodian was released from the case.</span></span>|
|<span data-ttu-id="9f9d7-175">status</span><span class="sxs-lookup"><span data-stu-id="9f9d7-175">status</span></span>|<span data-ttu-id="9f9d7-176">custodianStatus</span><span class="sxs-lookup"><span data-stu-id="9f9d7-176">custodianStatus</span></span>|<span data-ttu-id="9f9d7-177">保管人的状态。</span><span class="sxs-lookup"><span data-stu-id="9f9d7-177">Status of the custodian.</span></span> <span data-ttu-id="9f9d7-178">可取值为：`active`、`released`。</span><span class="sxs-lookup"><span data-stu-id="9f9d7-178">Possible values are: `active`, `released`.</span></span>|

### <a name="custodianstatus-values"></a><span data-ttu-id="9f9d7-179">custodianStatus 值</span><span class="sxs-lookup"><span data-stu-id="9f9d7-179">custodianStatus values</span></span>

|<span data-ttu-id="9f9d7-180">成员</span><span class="sxs-lookup"><span data-stu-id="9f9d7-180">Member</span></span>|<span data-ttu-id="9f9d7-181">说明</span><span class="sxs-lookup"><span data-stu-id="9f9d7-181">Description</span></span>|
|:----|-----------|
|<span data-ttu-id="9f9d7-182">active</span><span class="sxs-lookup"><span data-stu-id="9f9d7-182">active</span></span>|<span data-ttu-id="9f9d7-183">保管人是案例的活跃部分。</span><span class="sxs-lookup"><span data-stu-id="9f9d7-183">Custodian is an active part of the case.</span></span> |
|<span data-ttu-id="9f9d7-184">released</span><span class="sxs-lookup"><span data-stu-id="9f9d7-184">released</span></span>|<span data-ttu-id="9f9d7-185">保管人从案例中释放。</span><span class="sxs-lookup"><span data-stu-id="9f9d7-185">Custodian is released from the case.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9f9d7-186">关系</span><span class="sxs-lookup"><span data-stu-id="9f9d7-186">Relationships</span></span>

|<span data-ttu-id="9f9d7-187">关系</span><span class="sxs-lookup"><span data-stu-id="9f9d7-187">Relationship</span></span>|<span data-ttu-id="9f9d7-188">类型</span><span class="sxs-lookup"><span data-stu-id="9f9d7-188">Type</span></span>|<span data-ttu-id="9f9d7-189">说明</span><span class="sxs-lookup"><span data-stu-id="9f9d7-189">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9f9d7-190">siteSources</span><span class="sxs-lookup"><span data-stu-id="9f9d7-190">siteSources</span></span>|<span data-ttu-id="9f9d7-191">[siteSource](../resources/sitesource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9f9d7-191">[siteSource](../resources/sitesource.md) collection</span></span>|<span data-ttu-id="9f9d7-192">与保管人关联的 SharePoint 网站的数据源实体。</span><span class="sxs-lookup"><span data-stu-id="9f9d7-192">Data source entity for SharePoint sites associated with the custodian.</span></span>|
|<span data-ttu-id="9f9d7-193">unifiedGroupSources</span><span class="sxs-lookup"><span data-stu-id="9f9d7-193">unifiedGroupSources</span></span>|<span data-ttu-id="9f9d7-194">[unifiedGroupSource](../resources/unifiedgroupsource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9f9d7-194">[unifiedGroupSource](../resources/unifiedgroupsource.md) collection</span></span>|<span data-ttu-id="9f9d7-195">与保管人关联的组的数据源实体。</span><span class="sxs-lookup"><span data-stu-id="9f9d7-195">Data source entity for groups associated with the custodian.</span></span>|
|<span data-ttu-id="9f9d7-196">userSources</span><span class="sxs-lookup"><span data-stu-id="9f9d7-196">userSources</span></span>|<span data-ttu-id="9f9d7-197">[userSource](../resources/usersource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9f9d7-197">[userSource](../resources/usersource.md) collection</span></span>|<span data-ttu-id="9f9d7-198">保管人数据源实体。</span><span class="sxs-lookup"><span data-stu-id="9f9d7-198">Data source entity for a the custodian.</span></span> <span data-ttu-id="9f9d7-199">这是保管人邮箱和 OneDrive for Business 网站的容器。</span><span class="sxs-lookup"><span data-stu-id="9f9d7-199">This is the container for a custodian's mailbox and OneDrive for Business site.</span></span>|

<!--|lastIndexOperation|[caseIndexOperation](../resources/caseindexoperation.md)|**TODO: Add Description**| -->

## <a name="json-representation"></a><span data-ttu-id="9f9d7-200">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9f9d7-200">JSON representation</span></span>

<span data-ttu-id="9f9d7-201">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9f9d7-201">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.custodian",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.custodian",
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

---
title: 保管人资源类型
description: 在电子数据展示的上下文中，表示用户及其所有数字资产，如电子邮件和文档。
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: a2e22f711eaec4cd68cc5026e36b900d5284e71a
ms.sourcegitcommit: f729068e1fbb6b0f34a3d6144b59ec9aafcd8a62
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2020
ms.locfileid: "49597595"
---
# <a name="custodian-resource-type"></a><span data-ttu-id="b808d-103">保管人资源类型</span><span class="sxs-lookup"><span data-stu-id="b808d-103">custodian resource type</span></span>

<span data-ttu-id="b808d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b808d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b808d-105">在电子数据展示的上下文中，表示用户及其所有数字资产，如电子邮件和文档。</span><span class="sxs-lookup"><span data-stu-id="b808d-105">In the context of eDiscovery, represents a user and all of their digital assets, such as email and documents.</span></span>

## <a name="methods"></a><span data-ttu-id="b808d-106">方法</span><span class="sxs-lookup"><span data-stu-id="b808d-106">Methods</span></span>

|<span data-ttu-id="b808d-107">方法</span><span class="sxs-lookup"><span data-stu-id="b808d-107">Method</span></span>|<span data-ttu-id="b808d-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="b808d-108">Return type</span></span>|<span data-ttu-id="b808d-109">Description</span><span class="sxs-lookup"><span data-stu-id="b808d-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b808d-110">列出保管人</span><span class="sxs-lookup"><span data-stu-id="b808d-110">List custodians</span></span>](../api/ediscoverycase-list-custodians.md)|<span data-ttu-id="b808d-111">[保管人](../resources/custodian.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b808d-111">[custodian](../resources/custodian.md) collection</span></span>|<span data-ttu-id="b808d-112">获取 **保管人** 对象及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="b808d-112">Get a list of **custodian** objects and their properties.</span></span>|
|[<span data-ttu-id="b808d-113">创建管理员</span><span class="sxs-lookup"><span data-stu-id="b808d-113">Create custodian</span></span>](../api/ediscoverycase-post-custodians.md)|[<span data-ttu-id="b808d-114">保管人</span><span class="sxs-lookup"><span data-stu-id="b808d-114">custodian</span></span>](../resources/custodian.md)|<span data-ttu-id="b808d-115">创建新的 **保管人** 对象。</span><span class="sxs-lookup"><span data-stu-id="b808d-115">Create a new **custodian** object.</span></span>|
|[<span data-ttu-id="b808d-116">获取管理员</span><span class="sxs-lookup"><span data-stu-id="b808d-116">Get custodian</span></span>](../api/custodian-get.md)|[<span data-ttu-id="b808d-117">保管人</span><span class="sxs-lookup"><span data-stu-id="b808d-117">custodian</span></span>](../resources/custodian.md)|<span data-ttu-id="b808d-118">读取 **保管人** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b808d-118">Read the properties and relationships of a **custodian** object.</span></span>|
|[<span data-ttu-id="b808d-119">更新管理员</span><span class="sxs-lookup"><span data-stu-id="b808d-119">Update custodian</span></span>](../api/custodian-update.md)|[<span data-ttu-id="b808d-120">保管人</span><span class="sxs-lookup"><span data-stu-id="b808d-120">custodian</span></span>](../resources/custodian.md)|<span data-ttu-id="b808d-121">更新 **保管人** 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b808d-121">Update the properties of a **custodian** object.</span></span>|
|[<span data-ttu-id="b808d-122">7.2</span><span class="sxs-lookup"><span data-stu-id="b808d-122">release</span></span>](../api/custodian-release.md)|<span data-ttu-id="b808d-123">无</span><span class="sxs-lookup"><span data-stu-id="b808d-123">None</span></span>|<span data-ttu-id="b808d-124">从案例发布管理员。</span><span class="sxs-lookup"><span data-stu-id="b808d-124">Release a custodian from a case.</span></span>|
|[<span data-ttu-id="b808d-125">启用</span><span class="sxs-lookup"><span data-stu-id="b808d-125">activate</span></span>](../api/custodian-activate.md)|<span data-ttu-id="b808d-126">无</span><span class="sxs-lookup"><span data-stu-id="b808d-126">None</span></span>|<span data-ttu-id="b808d-127">重新激活已从某个事例发布的管理员，并再次使其成为事例的一部分。</span><span class="sxs-lookup"><span data-stu-id="b808d-127">Reactivate a custodian that has been released from a case and make them part of the case again.</span></span>|
|[<span data-ttu-id="b808d-128">列出 siteSources</span><span class="sxs-lookup"><span data-stu-id="b808d-128">List siteSources</span></span>](../api/custodian-list-sitesources.md)|<span data-ttu-id="b808d-129">[siteSource](../resources/sitesource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b808d-129">[siteSource](../resources/sitesource.md) collection</span></span>|<span data-ttu-id="b808d-130">从 **siteSources** 导航属性中获取 **siteSource** 资源。</span><span class="sxs-lookup"><span data-stu-id="b808d-130">Get the **siteSource** resources from the **siteSources** navigation property.</span></span>|
|[<span data-ttu-id="b808d-131">创建 siteSources</span><span class="sxs-lookup"><span data-stu-id="b808d-131">Create siteSources</span></span>](../api/custodian-post-sitesources.md)|[<span data-ttu-id="b808d-132">siteSource</span><span class="sxs-lookup"><span data-stu-id="b808d-132">siteSource</span></span>](../resources/sitesource.md)|<span data-ttu-id="b808d-133">创建新的 **siteSource** 对象。</span><span class="sxs-lookup"><span data-stu-id="b808d-133">Create a new **siteSource** object.</span></span>|
|[<span data-ttu-id="b808d-134">列出 unifiedGroupSources</span><span class="sxs-lookup"><span data-stu-id="b808d-134">List unifiedGroupSources</span></span>](../api/custodian-list-unifiedgroupsources.md)|<span data-ttu-id="b808d-135">[unifiedGroupSource](../resources/unifiedgroupsource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b808d-135">[unifiedGroupSource](../resources/unifiedgroupsource.md) collection</span></span>|<span data-ttu-id="b808d-136">从 **unifiedGroupSources** 导航属性中获取 **unifiedGroupSource** 资源。</span><span class="sxs-lookup"><span data-stu-id="b808d-136">Get the **unifiedGroupSource** resources from the **unifiedGroupSources** navigation property.</span></span>|
|[<span data-ttu-id="b808d-137">创建 unifiedGroupSources</span><span class="sxs-lookup"><span data-stu-id="b808d-137">Create unifiedGroupSources</span></span>](../api/custodian-post-unifiedgroupsources.md)|[<span data-ttu-id="b808d-138">unifiedGroupSource</span><span class="sxs-lookup"><span data-stu-id="b808d-138">unifiedGroupSource</span></span>](../resources/unifiedgroupsource.md)|<span data-ttu-id="b808d-139">创建新的 **unifiedGroupSource** 对象。</span><span class="sxs-lookup"><span data-stu-id="b808d-139">Create a new **unifiedGroupSource** object.</span></span>|
|[<span data-ttu-id="b808d-140">列出 userSources</span><span class="sxs-lookup"><span data-stu-id="b808d-140">List userSources</span></span>](../api/custodian-list-usersources.md)|<span data-ttu-id="b808d-141">[userSource](../resources/usersource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b808d-141">[userSource](../resources/usersource.md) collection</span></span>|<span data-ttu-id="b808d-142">从 **userSources** 导航属性中获取 **userSource** 资源。</span><span class="sxs-lookup"><span data-stu-id="b808d-142">Get the **userSource** resources from the **userSources** navigation property.</span></span>|
|[<span data-ttu-id="b808d-143">创建 userSources</span><span class="sxs-lookup"><span data-stu-id="b808d-143">Create userSources</span></span>](../api/custodian-post-usersources.md)|[<span data-ttu-id="b808d-144">userSource</span><span class="sxs-lookup"><span data-stu-id="b808d-144">userSource</span></span>](../resources/usersource.md)|<span data-ttu-id="b808d-145">创建新的 **userSource** 对象。</span><span class="sxs-lookup"><span data-stu-id="b808d-145">Create a new **userSource** object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b808d-146">属性</span><span class="sxs-lookup"><span data-stu-id="b808d-146">Properties</span></span>

|<span data-ttu-id="b808d-147">属性</span><span class="sxs-lookup"><span data-stu-id="b808d-147">Property</span></span>|<span data-ttu-id="b808d-148">类型</span><span class="sxs-lookup"><span data-stu-id="b808d-148">Type</span></span>|<span data-ttu-id="b808d-149">Description</span><span class="sxs-lookup"><span data-stu-id="b808d-149">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b808d-150">acknowledgedDateTime</span><span class="sxs-lookup"><span data-stu-id="b808d-150">acknowledgedDateTime</span></span>|<span data-ttu-id="b808d-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b808d-151">DateTimeOffset</span></span>|<span data-ttu-id="b808d-152">管理员确认保留通知的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="b808d-152">Date and time the custodian acknowledged a hold notification.</span></span>|
|<span data-ttu-id="b808d-153">applyHoldToSources</span><span class="sxs-lookup"><span data-stu-id="b808d-153">applyHoldToSources</span></span>|<span data-ttu-id="b808d-154">布尔值</span><span class="sxs-lookup"><span data-stu-id="b808d-154">Boolean</span></span>|<span data-ttu-id="b808d-155">标识在创建过程中是否将保管人的源置于保留状态。</span><span class="sxs-lookup"><span data-stu-id="b808d-155">Identifies whether a custodian's sources were placed on hold during creation.</span></span>|
|<span data-ttu-id="b808d-156">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b808d-156">createdDateTime</span></span>|<span data-ttu-id="b808d-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b808d-157">DateTimeOffset</span></span>|<span data-ttu-id="b808d-158">向事例中添加管理员的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="b808d-158">Date and time when the custodian was added to the case.</span></span>|
|<span data-ttu-id="b808d-159">displayName</span><span class="sxs-lookup"><span data-stu-id="b808d-159">displayName</span></span>|<span data-ttu-id="b808d-160">String</span><span class="sxs-lookup"><span data-stu-id="b808d-160">String</span></span>|<span data-ttu-id="b808d-161">保管人的显示名称。</span><span class="sxs-lookup"><span data-stu-id="b808d-161">Display name of the custodian.</span></span>|
|<span data-ttu-id="b808d-162">email</span><span class="sxs-lookup"><span data-stu-id="b808d-162">email</span></span>|<span data-ttu-id="b808d-163">String</span><span class="sxs-lookup"><span data-stu-id="b808d-163">String</span></span>|<span data-ttu-id="b808d-164">保管人的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="b808d-164">Email address of the custodian.</span></span>|
|<span data-ttu-id="b808d-165">id</span><span class="sxs-lookup"><span data-stu-id="b808d-165">id</span></span>|<span data-ttu-id="b808d-166">String</span><span class="sxs-lookup"><span data-stu-id="b808d-166">String</span></span>|<span data-ttu-id="b808d-167">指定的事例中保管人的 ID。</span><span class="sxs-lookup"><span data-stu-id="b808d-167">The ID for the custodian in the specified case.</span></span> <span data-ttu-id="b808d-168">只读。</span><span class="sxs-lookup"><span data-stu-id="b808d-168">Read-only.</span></span>|
|<span data-ttu-id="b808d-169">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b808d-169">lastModifiedDateTime</span></span>|<span data-ttu-id="b808d-170">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b808d-170">DateTimeOffset</span></span>|<span data-ttu-id="b808d-171">上次修改保管人对象的日期和时间</span><span class="sxs-lookup"><span data-stu-id="b808d-171">Date and time the custodian object was last modified</span></span>|
|<span data-ttu-id="b808d-172">releasedDateTime</span><span class="sxs-lookup"><span data-stu-id="b808d-172">releasedDateTime</span></span>|<span data-ttu-id="b808d-173">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b808d-173">DateTimeOffset</span></span>|<span data-ttu-id="b808d-174">从事例中释放保管人的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="b808d-174">Date and time the custodian was released from the case.</span></span>|
|<span data-ttu-id="b808d-175">status</span><span class="sxs-lookup"><span data-stu-id="b808d-175">status</span></span>|<span data-ttu-id="b808d-176">custodianStatus</span><span class="sxs-lookup"><span data-stu-id="b808d-176">custodianStatus</span></span>|<span data-ttu-id="b808d-177">保管人的状态。</span><span class="sxs-lookup"><span data-stu-id="b808d-177">Status of the custodian.</span></span> <span data-ttu-id="b808d-178">可取值为：`active`、`released`。</span><span class="sxs-lookup"><span data-stu-id="b808d-178">Possible values are: `active`, `released`.</span></span>|

### <a name="custodianstatus-values"></a><span data-ttu-id="b808d-179">custodianStatus 值</span><span class="sxs-lookup"><span data-stu-id="b808d-179">custodianStatus values</span></span>

|<span data-ttu-id="b808d-180">成员</span><span class="sxs-lookup"><span data-stu-id="b808d-180">Member</span></span>|<span data-ttu-id="b808d-181">说明</span><span class="sxs-lookup"><span data-stu-id="b808d-181">Description</span></span>|
|:----|-----------|
|<span data-ttu-id="b808d-182">工作</span><span class="sxs-lookup"><span data-stu-id="b808d-182">active</span></span>|<span data-ttu-id="b808d-183">保管人是事例的活动部分。</span><span class="sxs-lookup"><span data-stu-id="b808d-183">Custodian is an active part of the case.</span></span> |
|<span data-ttu-id="b808d-184">以后</span><span class="sxs-lookup"><span data-stu-id="b808d-184">released</span></span>|<span data-ttu-id="b808d-185">在此情况下，将发布保管人。</span><span class="sxs-lookup"><span data-stu-id="b808d-185">Custodian is released from the case.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b808d-186">关系</span><span class="sxs-lookup"><span data-stu-id="b808d-186">Relationships</span></span>

|<span data-ttu-id="b808d-187">关系</span><span class="sxs-lookup"><span data-stu-id="b808d-187">Relationship</span></span>|<span data-ttu-id="b808d-188">类型</span><span class="sxs-lookup"><span data-stu-id="b808d-188">Type</span></span>|<span data-ttu-id="b808d-189">Description</span><span class="sxs-lookup"><span data-stu-id="b808d-189">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b808d-190">siteSources</span><span class="sxs-lookup"><span data-stu-id="b808d-190">siteSources</span></span>|<span data-ttu-id="b808d-191">[siteSource](../resources/sitesource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b808d-191">[siteSource](../resources/sitesource.md) collection</span></span>|<span data-ttu-id="b808d-192">与保管人关联的 SharePoint 网站的数据源实体。</span><span class="sxs-lookup"><span data-stu-id="b808d-192">Data source entity for SharePoint sites associated with the custodian.</span></span>|
|<span data-ttu-id="b808d-193">unifiedGroupSources</span><span class="sxs-lookup"><span data-stu-id="b808d-193">unifiedGroupSources</span></span>|<span data-ttu-id="b808d-194">[unifiedGroupSource](../resources/unifiedgroupsource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b808d-194">[unifiedGroupSource](../resources/unifiedgroupsource.md) collection</span></span>|<span data-ttu-id="b808d-195">与保管人关联的组的数据源实体。</span><span class="sxs-lookup"><span data-stu-id="b808d-195">Data source entity for groups associated with the custodian.</span></span>|
|<span data-ttu-id="b808d-196">userSources</span><span class="sxs-lookup"><span data-stu-id="b808d-196">userSources</span></span>|<span data-ttu-id="b808d-197">[userSource](../resources/usersource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b808d-197">[userSource](../resources/usersource.md) collection</span></span>|<span data-ttu-id="b808d-198">保管人的数据源实体。</span><span class="sxs-lookup"><span data-stu-id="b808d-198">Data source entity for a the custodian.</span></span> <span data-ttu-id="b808d-199">这是用于保管人邮箱和 OneDrive for business 网站的容器。</span><span class="sxs-lookup"><span data-stu-id="b808d-199">This is the container for a custodian's mailbox and OneDrive for Business site.</span></span>|

<!--|lastIndexOperation|[caseIndexOperation](../resources/caseindexoperation.md)|**TODO: Add Description**| -->

## <a name="json-representation"></a><span data-ttu-id="b808d-200">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b808d-200">JSON representation</span></span>

<span data-ttu-id="b808d-201">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b808d-201">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.custodian",
  "baseType": "",
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

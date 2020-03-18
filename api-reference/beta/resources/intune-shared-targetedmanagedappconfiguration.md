---
title: targetedManagedAppConfiguration 资源类型
description: 用于将一组自定义设置按原样提供给目标安全组中的所有用户的配置
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 19055e66edfd7a31735a3c628ee214c6561107fc
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42767447"
---
# <a name="targetedmanagedappconfiguration-resource-type"></a><span data-ttu-id="9e2f4-103">targetedManagedAppConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="9e2f4-103">targetedManagedAppConfiguration resource type</span></span>

> <span data-ttu-id="9e2f4-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9e2f4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9e2f4-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9e2f4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9e2f4-106">用于将一组自定义设置按原样提供给目标安全组中的所有用户的配置</span><span class="sxs-lookup"><span data-stu-id="9e2f4-106">Configuration used to deliver a set of custom settings as-is to all users in the targeted security group</span></span>


<span data-ttu-id="9e2f4-107">继承自 [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9e2f4-107">Inherits from [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="9e2f4-108">方法</span><span class="sxs-lookup"><span data-stu-id="9e2f4-108">Methods</span></span>
|<span data-ttu-id="9e2f4-109">方法</span><span class="sxs-lookup"><span data-stu-id="9e2f4-109">Method</span></span>|<span data-ttu-id="9e2f4-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="9e2f4-110">Return Type</span></span>|<span data-ttu-id="9e2f4-111">说明</span><span class="sxs-lookup"><span data-stu-id="9e2f4-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="9e2f4-112">List targetedManagedAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="9e2f4-112">List targetedManagedAppConfigurations</span></span>](../api/intune-shared-targetedmanagedappconfiguration-list.md)|<span data-ttu-id="9e2f4-113">[targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9e2f4-113">[targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) collection</span></span>|<span data-ttu-id="9e2f4-114">列出 [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9e2f4-114">List properties and relationships of the [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="9e2f4-115">Get targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="9e2f4-115">Get targetedManagedAppConfiguration</span></span>](../api/intune-shared-targetedmanagedappconfiguration-get.md)|[<span data-ttu-id="9e2f4-116">targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="9e2f4-116">targetedManagedAppConfiguration</span></span>](../resources/intune-shared-targetedmanagedappconfiguration.md)|<span data-ttu-id="9e2f4-117">读取 [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9e2f4-117">Read properties and relationships of the [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) object.</span></span>|
|[<span data-ttu-id="9e2f4-118">Create targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="9e2f4-118">Create targetedManagedAppConfiguration</span></span>](../api/intune-shared-targetedmanagedappconfiguration-create.md)|[<span data-ttu-id="9e2f4-119">targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="9e2f4-119">targetedManagedAppConfiguration</span></span>](../resources/intune-shared-targetedmanagedappconfiguration.md)|<span data-ttu-id="9e2f4-120">创建新的 [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9e2f4-120">Create a new [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) object.</span></span>|
|[<span data-ttu-id="9e2f4-121">Delete targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="9e2f4-121">Delete targetedManagedAppConfiguration</span></span>](../api/intune-shared-targetedmanagedappconfiguration-delete.md)|<span data-ttu-id="9e2f4-122">无</span><span class="sxs-lookup"><span data-stu-id="9e2f4-122">None</span></span>|<span data-ttu-id="9e2f4-123">删除 [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="9e2f4-123">Deletes a [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md).</span></span>|
|[<span data-ttu-id="9e2f4-124">Update targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="9e2f4-124">Update targetedManagedAppConfiguration</span></span>](../api/intune-shared-targetedmanagedappconfiguration-update.md)|[<span data-ttu-id="9e2f4-125">targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="9e2f4-125">targetedManagedAppConfiguration</span></span>](../resources/intune-shared-targetedmanagedappconfiguration.md)|<span data-ttu-id="9e2f4-126">更新 [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="9e2f4-126">Update the properties of a [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) object.</span></span>|
|<span data-ttu-id="9e2f4-127">**移动应用管理 (MAM)**</span><span class="sxs-lookup"><span data-stu-id="9e2f4-127">**Mobile app management (MAM)**</span></span>|
|[<span data-ttu-id="9e2f4-128">分配操作</span><span class="sxs-lookup"><span data-stu-id="9e2f4-128">assign action</span></span>](../api/intune-shared-targetedmanagedappconfiguration-assign.md)|<span data-ttu-id="9e2f4-129">None</span><span class="sxs-lookup"><span data-stu-id="9e2f4-129">None</span></span>|<span data-ttu-id="9e2f4-130">尚未记录</span><span class="sxs-lookup"><span data-stu-id="9e2f4-130">Not yet documented</span></span>|
|[<span data-ttu-id="9e2f4-131">targetApps 操作</span><span class="sxs-lookup"><span data-stu-id="9e2f4-131">targetApps action</span></span>](../api/intune-shared-targetedmanagedappconfiguration-targetapps.md)|<span data-ttu-id="9e2f4-132">None</span><span class="sxs-lookup"><span data-stu-id="9e2f4-132">None</span></span>|<span data-ttu-id="9e2f4-133">尚未记录</span><span class="sxs-lookup"><span data-stu-id="9e2f4-133">Not yet documented</span></span>|
|<span data-ttu-id="9e2f4-134">**策略集**</span><span class="sxs-lookup"><span data-stu-id="9e2f4-134">**Policy Set**</span></span>|
|[<span data-ttu-id="9e2f4-135">hasPayloadLinks 操作</span><span class="sxs-lookup"><span data-stu-id="9e2f4-135">hasPayloadLinks action</span></span>](../api/intune-shared-targetedmanagedappconfiguration-haspayloadlinks.md)|<span data-ttu-id="9e2f4-136">[hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md)集合</span><span class="sxs-lookup"><span data-stu-id="9e2f4-136">[hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md) collection</span></span>|<span data-ttu-id="9e2f4-137">尚未记录</span><span class="sxs-lookup"><span data-stu-id="9e2f4-137">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="9e2f4-138">属性</span><span class="sxs-lookup"><span data-stu-id="9e2f4-138">Properties</span></span>
|<span data-ttu-id="9e2f4-139">属性</span><span class="sxs-lookup"><span data-stu-id="9e2f4-139">Property</span></span>|<span data-ttu-id="9e2f4-140">类型</span><span class="sxs-lookup"><span data-stu-id="9e2f4-140">Type</span></span>|<span data-ttu-id="9e2f4-141">说明</span><span class="sxs-lookup"><span data-stu-id="9e2f4-141">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9e2f4-142">id</span><span class="sxs-lookup"><span data-stu-id="9e2f4-142">id</span></span>|<span data-ttu-id="9e2f4-143">字符串</span><span class="sxs-lookup"><span data-stu-id="9e2f4-143">String</span></span>|<span data-ttu-id="9e2f4-144">实体的键。</span><span class="sxs-lookup"><span data-stu-id="9e2f4-144">Key of the entity.</span></span> <span data-ttu-id="9e2f4-145">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9e2f4-145">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="9e2f4-146">displayName</span><span class="sxs-lookup"><span data-stu-id="9e2f4-146">displayName</span></span>|<span data-ttu-id="9e2f4-147">字符串</span><span class="sxs-lookup"><span data-stu-id="9e2f4-147">String</span></span>|<span data-ttu-id="9e2f4-148">策略显示名称。</span><span class="sxs-lookup"><span data-stu-id="9e2f4-148">Policy display name.</span></span> <span data-ttu-id="9e2f4-149">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9e2f4-149">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="9e2f4-150">说明</span><span class="sxs-lookup"><span data-stu-id="9e2f4-150">description</span></span>|<span data-ttu-id="9e2f4-151">String</span><span class="sxs-lookup"><span data-stu-id="9e2f4-151">String</span></span>|<span data-ttu-id="9e2f4-152">策略的说明。</span><span class="sxs-lookup"><span data-stu-id="9e2f4-152">The policy's description.</span></span> <span data-ttu-id="9e2f4-153">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9e2f4-153">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="9e2f4-154">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9e2f4-154">createdDateTime</span></span>|<span data-ttu-id="9e2f4-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9e2f4-155">DateTimeOffset</span></span>|<span data-ttu-id="9e2f4-156">创建策略的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="9e2f4-156">The date and time the policy was created.</span></span> <span data-ttu-id="9e2f4-157">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9e2f4-157">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="9e2f4-158">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9e2f4-158">lastModifiedDateTime</span></span>|<span data-ttu-id="9e2f4-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9e2f4-159">DateTimeOffset</span></span>|<span data-ttu-id="9e2f4-160">上次修改策略的时间。</span><span class="sxs-lookup"><span data-stu-id="9e2f4-160">Last time the policy was modified.</span></span> <span data-ttu-id="9e2f4-161">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9e2f4-161">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="9e2f4-162">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="9e2f4-162">roleScopeTagIds</span></span>|<span data-ttu-id="9e2f4-163">String collection</span><span class="sxs-lookup"><span data-stu-id="9e2f4-163">String collection</span></span>|<span data-ttu-id="9e2f4-164">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="9e2f4-164">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="9e2f4-165">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9e2f4-165">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="9e2f4-166">version</span><span class="sxs-lookup"><span data-stu-id="9e2f4-166">version</span></span>|<span data-ttu-id="9e2f4-167">String</span><span class="sxs-lookup"><span data-stu-id="9e2f4-167">String</span></span>|<span data-ttu-id="9e2f4-168">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="9e2f4-168">Version of the entity.</span></span> <span data-ttu-id="9e2f4-169">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9e2f4-169">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="9e2f4-170">customSettings</span><span class="sxs-lookup"><span data-stu-id="9e2f4-170">customSettings</span></span>|<span data-ttu-id="9e2f4-171">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9e2f4-171">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="9e2f4-172">要发送到配置范围确定的用户应用的一组字符串键和字符串值对，不由此服务更改。继承自 [ managedAppConfiguration ](../resources/intune-mam-managedappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9e2f4-172">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service Inherited from [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span></span>|
|<span data-ttu-id="9e2f4-173">deployedAppCount</span><span class="sxs-lookup"><span data-stu-id="9e2f4-173">deployedAppCount</span></span>|<span data-ttu-id="9e2f4-174">Int32</span><span class="sxs-lookup"><span data-stu-id="9e2f4-174">Int32</span></span>|<span data-ttu-id="9e2f4-175">当前策略部署到的应用的计数。</span><span class="sxs-lookup"><span data-stu-id="9e2f4-175">Count of apps to which the current policy is deployed.</span></span>|
|<span data-ttu-id="9e2f4-176">isAssigned</span><span class="sxs-lookup"><span data-stu-id="9e2f4-176">isAssigned</span></span>|<span data-ttu-id="9e2f4-177">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e2f4-177">Boolean</span></span>|<span data-ttu-id="9e2f4-178">指示策略是否部署到任何包含组。</span><span class="sxs-lookup"><span data-stu-id="9e2f4-178">Indicates if the policy is deployed to any inclusion groups or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9e2f4-179">关系</span><span class="sxs-lookup"><span data-stu-id="9e2f4-179">Relationships</span></span>
|<span data-ttu-id="9e2f4-180">关系</span><span class="sxs-lookup"><span data-stu-id="9e2f4-180">Relationship</span></span>|<span data-ttu-id="9e2f4-181">类型</span><span class="sxs-lookup"><span data-stu-id="9e2f4-181">Type</span></span>|<span data-ttu-id="9e2f4-182">说明</span><span class="sxs-lookup"><span data-stu-id="9e2f4-182">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9e2f4-183">**移动应用管理 (MAM)**</span><span class="sxs-lookup"><span data-stu-id="9e2f4-183">**Mobile app management (MAM)**</span></span>|
|<span data-ttu-id="9e2f4-184">apps</span><span class="sxs-lookup"><span data-stu-id="9e2f4-184">apps</span></span>|<span data-ttu-id="9e2f4-185">[managedMobileApp](../resources/intune-mam-managedmobileapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9e2f4-185">[managedMobileApp](../resources/intune-mam-managedmobileapp.md) collection</span></span>|<span data-ttu-id="9e2f4-186">策略部署到的应用的列表。</span><span class="sxs-lookup"><span data-stu-id="9e2f4-186">List of apps to which the policy is deployed.</span></span>|
|<span data-ttu-id="9e2f4-187">deploymentSummary</span><span class="sxs-lookup"><span data-stu-id="9e2f4-187">deploymentSummary</span></span>|[<span data-ttu-id="9e2f4-188">managedAppPolicyDeploymentSummary</span><span class="sxs-lookup"><span data-stu-id="9e2f4-188">managedAppPolicyDeploymentSummary</span></span>](../resources/intune-mam-managedapppolicydeploymentsummary.md)|<span data-ttu-id="9e2f4-189">配置的部署摘要的导航属性。</span><span class="sxs-lookup"><span data-stu-id="9e2f4-189">Navigation property to deployment summary of the configuration.</span></span>|
|<span data-ttu-id="9e2f4-190">assignments</span><span class="sxs-lookup"><span data-stu-id="9e2f4-190">assignments</span></span>|<span data-ttu-id="9e2f4-191">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9e2f4-191">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) collection</span></span>|<span data-ttu-id="9e2f4-192">策略部署到的包含组和排除组列表的导航属性。</span><span class="sxs-lookup"><span data-stu-id="9e2f4-192">Navigation property to list of inclusion and exclusion groups to which the policy is deployed.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9e2f4-193">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9e2f4-193">JSON Representation</span></span>
<span data-ttu-id="9e2f4-194">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9e2f4-194">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.targetedManagedAppConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.targetedManagedAppConfiguration",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "id": "String (identifier)",
  "version": "String",
  "customSettings": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "String",
      "value": "String"
    }
  ],
  "deployedAppCount": 1024,
  "isAssigned": true
}
```




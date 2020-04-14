---
title: targetedManagedAppConfiguration 资源类型
description: 用于将一组自定义设置按原样提供给目标安全组中的所有用户的配置
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 651ea39e6134626a7086909d6b4807eaa37a32a2
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43449617"
---
# <a name="targetedmanagedappconfiguration-resource-type"></a><span data-ttu-id="6115f-103">targetedManagedAppConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="6115f-103">targetedManagedAppConfiguration resource type</span></span>

<span data-ttu-id="6115f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6115f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6115f-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6115f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6115f-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6115f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6115f-107">用于将一组自定义设置按原样提供给目标安全组中的所有用户的配置</span><span class="sxs-lookup"><span data-stu-id="6115f-107">Configuration used to deliver a set of custom settings as-is to all users in the targeted security group</span></span>


<span data-ttu-id="6115f-108">继承自 [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6115f-108">Inherits from [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="6115f-109">方法</span><span class="sxs-lookup"><span data-stu-id="6115f-109">Methods</span></span>
|<span data-ttu-id="6115f-110">方法</span><span class="sxs-lookup"><span data-stu-id="6115f-110">Method</span></span>|<span data-ttu-id="6115f-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="6115f-111">Return Type</span></span>|<span data-ttu-id="6115f-112">说明</span><span class="sxs-lookup"><span data-stu-id="6115f-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6115f-113">List targetedManagedAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="6115f-113">List targetedManagedAppConfigurations</span></span>](../api/intune-shared-targetedmanagedappconfiguration-list.md)|<span data-ttu-id="6115f-114">[targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6115f-114">[targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) collection</span></span>|<span data-ttu-id="6115f-115">列出 [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="6115f-115">List properties and relationships of the [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="6115f-116">Get targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="6115f-116">Get targetedManagedAppConfiguration</span></span>](../api/intune-shared-targetedmanagedappconfiguration-get.md)|[<span data-ttu-id="6115f-117">targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="6115f-117">targetedManagedAppConfiguration</span></span>](../resources/intune-shared-targetedmanagedappconfiguration.md)|<span data-ttu-id="6115f-118">读取 [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="6115f-118">Read properties and relationships of the [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) object.</span></span>|
|[<span data-ttu-id="6115f-119">Create targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="6115f-119">Create targetedManagedAppConfiguration</span></span>](../api/intune-shared-targetedmanagedappconfiguration-create.md)|[<span data-ttu-id="6115f-120">targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="6115f-120">targetedManagedAppConfiguration</span></span>](../resources/intune-shared-targetedmanagedappconfiguration.md)|<span data-ttu-id="6115f-121">创建新的 [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6115f-121">Create a new [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) object.</span></span>|
|[<span data-ttu-id="6115f-122">Delete targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="6115f-122">Delete targetedManagedAppConfiguration</span></span>](../api/intune-shared-targetedmanagedappconfiguration-delete.md)|<span data-ttu-id="6115f-123">无</span><span class="sxs-lookup"><span data-stu-id="6115f-123">None</span></span>|<span data-ttu-id="6115f-124">删除 [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="6115f-124">Deletes a [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md).</span></span>|
|[<span data-ttu-id="6115f-125">Update targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="6115f-125">Update targetedManagedAppConfiguration</span></span>](../api/intune-shared-targetedmanagedappconfiguration-update.md)|[<span data-ttu-id="6115f-126">targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="6115f-126">targetedManagedAppConfiguration</span></span>](../resources/intune-shared-targetedmanagedappconfiguration.md)|<span data-ttu-id="6115f-127">更新 [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="6115f-127">Update the properties of a [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) object.</span></span>|
|<span data-ttu-id="6115f-128">**移动应用管理 (MAM)**</span><span class="sxs-lookup"><span data-stu-id="6115f-128">**Mobile app management (MAM)**</span></span>|
|[<span data-ttu-id="6115f-129">分配操作</span><span class="sxs-lookup"><span data-stu-id="6115f-129">assign action</span></span>](../api/intune-shared-targetedmanagedappconfiguration-assign.md)|<span data-ttu-id="6115f-130">无</span><span class="sxs-lookup"><span data-stu-id="6115f-130">None</span></span>|<span data-ttu-id="6115f-131">尚未记录</span><span class="sxs-lookup"><span data-stu-id="6115f-131">Not yet documented</span></span>|
|[<span data-ttu-id="6115f-132">targetApps 操作</span><span class="sxs-lookup"><span data-stu-id="6115f-132">targetApps action</span></span>](../api/intune-shared-targetedmanagedappconfiguration-targetapps.md)|<span data-ttu-id="6115f-133">无</span><span class="sxs-lookup"><span data-stu-id="6115f-133">None</span></span>|<span data-ttu-id="6115f-134">尚未记录</span><span class="sxs-lookup"><span data-stu-id="6115f-134">Not yet documented</span></span>|
|<span data-ttu-id="6115f-135">**策略集**</span><span class="sxs-lookup"><span data-stu-id="6115f-135">**Policy Set**</span></span>|
|[<span data-ttu-id="6115f-136">hasPayloadLinks 操作</span><span class="sxs-lookup"><span data-stu-id="6115f-136">hasPayloadLinks action</span></span>](../api/intune-shared-targetedmanagedappconfiguration-haspayloadlinks.md)|<span data-ttu-id="6115f-137">[hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md)集合</span><span class="sxs-lookup"><span data-stu-id="6115f-137">[hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md) collection</span></span>|<span data-ttu-id="6115f-138">尚未记录</span><span class="sxs-lookup"><span data-stu-id="6115f-138">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="6115f-139">属性</span><span class="sxs-lookup"><span data-stu-id="6115f-139">Properties</span></span>
|<span data-ttu-id="6115f-140">属性</span><span class="sxs-lookup"><span data-stu-id="6115f-140">Property</span></span>|<span data-ttu-id="6115f-141">类型</span><span class="sxs-lookup"><span data-stu-id="6115f-141">Type</span></span>|<span data-ttu-id="6115f-142">说明</span><span class="sxs-lookup"><span data-stu-id="6115f-142">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6115f-143">id</span><span class="sxs-lookup"><span data-stu-id="6115f-143">id</span></span>|<span data-ttu-id="6115f-144">字符串</span><span class="sxs-lookup"><span data-stu-id="6115f-144">String</span></span>|<span data-ttu-id="6115f-145">实体的键。</span><span class="sxs-lookup"><span data-stu-id="6115f-145">Key of the entity.</span></span> <span data-ttu-id="6115f-146">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6115f-146">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="6115f-147">displayName</span><span class="sxs-lookup"><span data-stu-id="6115f-147">displayName</span></span>|<span data-ttu-id="6115f-148">字符串</span><span class="sxs-lookup"><span data-stu-id="6115f-148">String</span></span>|<span data-ttu-id="6115f-149">策略显示名称。</span><span class="sxs-lookup"><span data-stu-id="6115f-149">Policy display name.</span></span> <span data-ttu-id="6115f-150">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6115f-150">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="6115f-151">description</span><span class="sxs-lookup"><span data-stu-id="6115f-151">description</span></span>|<span data-ttu-id="6115f-152">String</span><span class="sxs-lookup"><span data-stu-id="6115f-152">String</span></span>|<span data-ttu-id="6115f-153">策略的说明。</span><span class="sxs-lookup"><span data-stu-id="6115f-153">The policy's description.</span></span> <span data-ttu-id="6115f-154">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6115f-154">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="6115f-155">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6115f-155">createdDateTime</span></span>|<span data-ttu-id="6115f-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6115f-156">DateTimeOffset</span></span>|<span data-ttu-id="6115f-157">创建策略的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="6115f-157">The date and time the policy was created.</span></span> <span data-ttu-id="6115f-158">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6115f-158">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="6115f-159">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6115f-159">lastModifiedDateTime</span></span>|<span data-ttu-id="6115f-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6115f-160">DateTimeOffset</span></span>|<span data-ttu-id="6115f-161">上次修改策略的时间。</span><span class="sxs-lookup"><span data-stu-id="6115f-161">Last time the policy was modified.</span></span> <span data-ttu-id="6115f-162">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6115f-162">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="6115f-163">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6115f-163">roleScopeTagIds</span></span>|<span data-ttu-id="6115f-164">String 集合</span><span class="sxs-lookup"><span data-stu-id="6115f-164">String collection</span></span>|<span data-ttu-id="6115f-165">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="6115f-165">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="6115f-166">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6115f-166">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="6115f-167">version</span><span class="sxs-lookup"><span data-stu-id="6115f-167">version</span></span>|<span data-ttu-id="6115f-168">String</span><span class="sxs-lookup"><span data-stu-id="6115f-168">String</span></span>|<span data-ttu-id="6115f-169">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="6115f-169">Version of the entity.</span></span> <span data-ttu-id="6115f-170">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6115f-170">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="6115f-171">customSettings</span><span class="sxs-lookup"><span data-stu-id="6115f-171">customSettings</span></span>|<span data-ttu-id="6115f-172">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6115f-172">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="6115f-173">要发送到配置范围确定的用户应用的一组字符串键和字符串值对，不由此服务更改。继承自 [ managedAppConfiguration ](../resources/intune-mam-managedappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6115f-173">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service Inherited from [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span></span>|
|<span data-ttu-id="6115f-174">deployedAppCount</span><span class="sxs-lookup"><span data-stu-id="6115f-174">deployedAppCount</span></span>|<span data-ttu-id="6115f-175">Int32</span><span class="sxs-lookup"><span data-stu-id="6115f-175">Int32</span></span>|<span data-ttu-id="6115f-176">当前策略部署到的应用的计数。</span><span class="sxs-lookup"><span data-stu-id="6115f-176">Count of apps to which the current policy is deployed.</span></span>|
|<span data-ttu-id="6115f-177">isAssigned</span><span class="sxs-lookup"><span data-stu-id="6115f-177">isAssigned</span></span>|<span data-ttu-id="6115f-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="6115f-178">Boolean</span></span>|<span data-ttu-id="6115f-179">指示策略是否部署到任何包含组。</span><span class="sxs-lookup"><span data-stu-id="6115f-179">Indicates if the policy is deployed to any inclusion groups or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6115f-180">关系</span><span class="sxs-lookup"><span data-stu-id="6115f-180">Relationships</span></span>
|<span data-ttu-id="6115f-181">关系</span><span class="sxs-lookup"><span data-stu-id="6115f-181">Relationship</span></span>|<span data-ttu-id="6115f-182">类型</span><span class="sxs-lookup"><span data-stu-id="6115f-182">Type</span></span>|<span data-ttu-id="6115f-183">说明</span><span class="sxs-lookup"><span data-stu-id="6115f-183">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6115f-184">**移动应用管理 (MAM)**</span><span class="sxs-lookup"><span data-stu-id="6115f-184">**Mobile app management (MAM)**</span></span>|
|<span data-ttu-id="6115f-185">apps</span><span class="sxs-lookup"><span data-stu-id="6115f-185">apps</span></span>|<span data-ttu-id="6115f-186">[managedMobileApp](../resources/intune-mam-managedmobileapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6115f-186">[managedMobileApp](../resources/intune-mam-managedmobileapp.md) collection</span></span>|<span data-ttu-id="6115f-187">策略部署到的应用的列表。</span><span class="sxs-lookup"><span data-stu-id="6115f-187">List of apps to which the policy is deployed.</span></span>|
|<span data-ttu-id="6115f-188">deploymentSummary</span><span class="sxs-lookup"><span data-stu-id="6115f-188">deploymentSummary</span></span>|[<span data-ttu-id="6115f-189">managedAppPolicyDeploymentSummary</span><span class="sxs-lookup"><span data-stu-id="6115f-189">managedAppPolicyDeploymentSummary</span></span>](../resources/intune-mam-managedapppolicydeploymentsummary.md)|<span data-ttu-id="6115f-190">配置的部署摘要的导航属性。</span><span class="sxs-lookup"><span data-stu-id="6115f-190">Navigation property to deployment summary of the configuration.</span></span>|
|<span data-ttu-id="6115f-191">assignments</span><span class="sxs-lookup"><span data-stu-id="6115f-191">assignments</span></span>|<span data-ttu-id="6115f-192">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6115f-192">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) collection</span></span>|<span data-ttu-id="6115f-193">策略部署到的包含组和排除组列表的导航属性。</span><span class="sxs-lookup"><span data-stu-id="6115f-193">Navigation property to list of inclusion and exclusion groups to which the policy is deployed.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6115f-194">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6115f-194">JSON Representation</span></span>
<span data-ttu-id="6115f-195">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6115f-195">Here is a JSON representation of the resource.</span></span>
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




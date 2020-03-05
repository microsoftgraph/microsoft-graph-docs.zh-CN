---
title: targetedManagedAppConfiguration 资源类型
description: 用于将一组自定义设置按原样提供给目标安全组中的所有用户的配置
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f15851191614c793eb50d4e8b7cdd25f3fe08d01
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523532"
---
# <a name="targetedmanagedappconfiguration-resource-type"></a><span data-ttu-id="34ee6-103">targetedManagedAppConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="34ee6-103">targetedManagedAppConfiguration resource type</span></span>

<span data-ttu-id="34ee6-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="34ee6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="34ee6-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="34ee6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="34ee6-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="34ee6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="34ee6-107">用于将一组自定义设置按原样提供给目标安全组中的所有用户的配置</span><span class="sxs-lookup"><span data-stu-id="34ee6-107">Configuration used to deliver a set of custom settings as-is to all users in the targeted security group</span></span>


<span data-ttu-id="34ee6-108">继承自 [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="34ee6-108">Inherits from [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="34ee6-109">方法</span><span class="sxs-lookup"><span data-stu-id="34ee6-109">Methods</span></span>
|<span data-ttu-id="34ee6-110">方法</span><span class="sxs-lookup"><span data-stu-id="34ee6-110">Method</span></span>|<span data-ttu-id="34ee6-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="34ee6-111">Return Type</span></span>|<span data-ttu-id="34ee6-112">说明</span><span class="sxs-lookup"><span data-stu-id="34ee6-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="34ee6-113">List targetedManagedAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="34ee6-113">List targetedManagedAppConfigurations</span></span>](../api/intune-shared-targetedmanagedappconfiguration-list.md)|<span data-ttu-id="34ee6-114">[targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="34ee6-114">[targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) collection</span></span>|<span data-ttu-id="34ee6-115">列出 [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="34ee6-115">List properties and relationships of the [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="34ee6-116">Get targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="34ee6-116">Get targetedManagedAppConfiguration</span></span>](../api/intune-shared-targetedmanagedappconfiguration-get.md)|[<span data-ttu-id="34ee6-117">targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="34ee6-117">targetedManagedAppConfiguration</span></span>](../resources/intune-shared-targetedmanagedappconfiguration.md)|<span data-ttu-id="34ee6-118">读取 [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="34ee6-118">Read properties and relationships of the [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) object.</span></span>|
|[<span data-ttu-id="34ee6-119">Create targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="34ee6-119">Create targetedManagedAppConfiguration</span></span>](../api/intune-shared-targetedmanagedappconfiguration-create.md)|[<span data-ttu-id="34ee6-120">targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="34ee6-120">targetedManagedAppConfiguration</span></span>](../resources/intune-shared-targetedmanagedappconfiguration.md)|<span data-ttu-id="34ee6-121">创建新的 [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="34ee6-121">Create a new [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) object.</span></span>|
|[<span data-ttu-id="34ee6-122">Delete targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="34ee6-122">Delete targetedManagedAppConfiguration</span></span>](../api/intune-shared-targetedmanagedappconfiguration-delete.md)|<span data-ttu-id="34ee6-123">无</span><span class="sxs-lookup"><span data-stu-id="34ee6-123">None</span></span>|<span data-ttu-id="34ee6-124">删除 [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="34ee6-124">Deletes a [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md).</span></span>|
|[<span data-ttu-id="34ee6-125">Update targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="34ee6-125">Update targetedManagedAppConfiguration</span></span>](../api/intune-shared-targetedmanagedappconfiguration-update.md)|[<span data-ttu-id="34ee6-126">targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="34ee6-126">targetedManagedAppConfiguration</span></span>](../resources/intune-shared-targetedmanagedappconfiguration.md)|<span data-ttu-id="34ee6-127">更新 [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="34ee6-127">Update the properties of a [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) object.</span></span>|
|<span data-ttu-id="34ee6-128">**移动应用管理 (MAM)**</span><span class="sxs-lookup"><span data-stu-id="34ee6-128">**Mobile app management (MAM)**</span></span>|
|[<span data-ttu-id="34ee6-129">分配操作</span><span class="sxs-lookup"><span data-stu-id="34ee6-129">assign action</span></span>](../api/intune-shared-targetedmanagedappconfiguration-assign.md)|<span data-ttu-id="34ee6-130">无</span><span class="sxs-lookup"><span data-stu-id="34ee6-130">None</span></span>|<span data-ttu-id="34ee6-131">尚未记录</span><span class="sxs-lookup"><span data-stu-id="34ee6-131">Not yet documented</span></span>|
|[<span data-ttu-id="34ee6-132">targetApps 操作</span><span class="sxs-lookup"><span data-stu-id="34ee6-132">targetApps action</span></span>](../api/intune-shared-targetedmanagedappconfiguration-targetapps.md)|<span data-ttu-id="34ee6-133">无</span><span class="sxs-lookup"><span data-stu-id="34ee6-133">None</span></span>|<span data-ttu-id="34ee6-134">尚未记录</span><span class="sxs-lookup"><span data-stu-id="34ee6-134">Not yet documented</span></span>|
|<span data-ttu-id="34ee6-135">**策略集**</span><span class="sxs-lookup"><span data-stu-id="34ee6-135">**Policy Set**</span></span>|
|[<span data-ttu-id="34ee6-136">hasPayloadLinks 操作</span><span class="sxs-lookup"><span data-stu-id="34ee6-136">hasPayloadLinks action</span></span>](../api/intune-shared-targetedmanagedappconfiguration-haspayloadlinks.md)|<span data-ttu-id="34ee6-137">[hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md)集合</span><span class="sxs-lookup"><span data-stu-id="34ee6-137">[hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md) collection</span></span>|<span data-ttu-id="34ee6-138">尚未记录</span><span class="sxs-lookup"><span data-stu-id="34ee6-138">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="34ee6-139">属性</span><span class="sxs-lookup"><span data-stu-id="34ee6-139">Properties</span></span>
|<span data-ttu-id="34ee6-140">属性</span><span class="sxs-lookup"><span data-stu-id="34ee6-140">Property</span></span>|<span data-ttu-id="34ee6-141">类型</span><span class="sxs-lookup"><span data-stu-id="34ee6-141">Type</span></span>|<span data-ttu-id="34ee6-142">说明</span><span class="sxs-lookup"><span data-stu-id="34ee6-142">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="34ee6-143">id</span><span class="sxs-lookup"><span data-stu-id="34ee6-143">id</span></span>|<span data-ttu-id="34ee6-144">字符串</span><span class="sxs-lookup"><span data-stu-id="34ee6-144">String</span></span>|<span data-ttu-id="34ee6-145">实体的键。</span><span class="sxs-lookup"><span data-stu-id="34ee6-145">Key of the entity.</span></span> <span data-ttu-id="34ee6-146">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="34ee6-146">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="34ee6-147">displayName</span><span class="sxs-lookup"><span data-stu-id="34ee6-147">displayName</span></span>|<span data-ttu-id="34ee6-148">字符串</span><span class="sxs-lookup"><span data-stu-id="34ee6-148">String</span></span>|<span data-ttu-id="34ee6-149">策略显示名称。</span><span class="sxs-lookup"><span data-stu-id="34ee6-149">Policy display name.</span></span> <span data-ttu-id="34ee6-150">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="34ee6-150">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="34ee6-151">说明</span><span class="sxs-lookup"><span data-stu-id="34ee6-151">description</span></span>|<span data-ttu-id="34ee6-152">String</span><span class="sxs-lookup"><span data-stu-id="34ee6-152">String</span></span>|<span data-ttu-id="34ee6-153">策略的说明。</span><span class="sxs-lookup"><span data-stu-id="34ee6-153">The policy's description.</span></span> <span data-ttu-id="34ee6-154">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="34ee6-154">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="34ee6-155">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="34ee6-155">createdDateTime</span></span>|<span data-ttu-id="34ee6-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="34ee6-156">DateTimeOffset</span></span>|<span data-ttu-id="34ee6-157">创建策略的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="34ee6-157">The date and time the policy was created.</span></span> <span data-ttu-id="34ee6-158">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="34ee6-158">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="34ee6-159">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="34ee6-159">lastModifiedDateTime</span></span>|<span data-ttu-id="34ee6-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="34ee6-160">DateTimeOffset</span></span>|<span data-ttu-id="34ee6-161">上次修改策略的时间。</span><span class="sxs-lookup"><span data-stu-id="34ee6-161">Last time the policy was modified.</span></span> <span data-ttu-id="34ee6-162">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="34ee6-162">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="34ee6-163">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="34ee6-163">roleScopeTagIds</span></span>|<span data-ttu-id="34ee6-164">String 集合</span><span class="sxs-lookup"><span data-stu-id="34ee6-164">String collection</span></span>|<span data-ttu-id="34ee6-165">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="34ee6-165">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="34ee6-166">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="34ee6-166">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="34ee6-167">version</span><span class="sxs-lookup"><span data-stu-id="34ee6-167">version</span></span>|<span data-ttu-id="34ee6-168">String</span><span class="sxs-lookup"><span data-stu-id="34ee6-168">String</span></span>|<span data-ttu-id="34ee6-169">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="34ee6-169">Version of the entity.</span></span> <span data-ttu-id="34ee6-170">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="34ee6-170">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="34ee6-171">customSettings</span><span class="sxs-lookup"><span data-stu-id="34ee6-171">customSettings</span></span>|<span data-ttu-id="34ee6-172">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="34ee6-172">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="34ee6-173">要发送到配置范围确定的用户应用的一组字符串键和字符串值对，不由此服务更改。继承自 [ managedAppConfiguration ](../resources/intune-mam-managedappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="34ee6-173">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service Inherited from [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span></span>|
|<span data-ttu-id="34ee6-174">deployedAppCount</span><span class="sxs-lookup"><span data-stu-id="34ee6-174">deployedAppCount</span></span>|<span data-ttu-id="34ee6-175">Int32</span><span class="sxs-lookup"><span data-stu-id="34ee6-175">Int32</span></span>|<span data-ttu-id="34ee6-176">当前策略部署到的应用的计数。</span><span class="sxs-lookup"><span data-stu-id="34ee6-176">Count of apps to which the current policy is deployed.</span></span>|
|<span data-ttu-id="34ee6-177">isAssigned</span><span class="sxs-lookup"><span data-stu-id="34ee6-177">isAssigned</span></span>|<span data-ttu-id="34ee6-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="34ee6-178">Boolean</span></span>|<span data-ttu-id="34ee6-179">指示策略是否部署到任何包含组。</span><span class="sxs-lookup"><span data-stu-id="34ee6-179">Indicates if the policy is deployed to any inclusion groups or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="34ee6-180">关系</span><span class="sxs-lookup"><span data-stu-id="34ee6-180">Relationships</span></span>
|<span data-ttu-id="34ee6-181">关系</span><span class="sxs-lookup"><span data-stu-id="34ee6-181">Relationship</span></span>|<span data-ttu-id="34ee6-182">类型</span><span class="sxs-lookup"><span data-stu-id="34ee6-182">Type</span></span>|<span data-ttu-id="34ee6-183">说明</span><span class="sxs-lookup"><span data-stu-id="34ee6-183">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="34ee6-184">**移动应用管理 (MAM)**</span><span class="sxs-lookup"><span data-stu-id="34ee6-184">**Mobile app management (MAM)**</span></span>|
|<span data-ttu-id="34ee6-185">apps</span><span class="sxs-lookup"><span data-stu-id="34ee6-185">apps</span></span>|<span data-ttu-id="34ee6-186">[managedMobileApp](../resources/intune-mam-managedmobileapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="34ee6-186">[managedMobileApp](../resources/intune-mam-managedmobileapp.md) collection</span></span>|<span data-ttu-id="34ee6-187">策略部署到的应用的列表。</span><span class="sxs-lookup"><span data-stu-id="34ee6-187">List of apps to which the policy is deployed.</span></span>|
|<span data-ttu-id="34ee6-188">deploymentSummary</span><span class="sxs-lookup"><span data-stu-id="34ee6-188">deploymentSummary</span></span>|[<span data-ttu-id="34ee6-189">managedAppPolicyDeploymentSummary</span><span class="sxs-lookup"><span data-stu-id="34ee6-189">managedAppPolicyDeploymentSummary</span></span>](../resources/intune-mam-managedapppolicydeploymentsummary.md)|<span data-ttu-id="34ee6-190">配置的部署摘要的导航属性。</span><span class="sxs-lookup"><span data-stu-id="34ee6-190">Navigation property to deployment summary of the configuration.</span></span>|
|<span data-ttu-id="34ee6-191">assignments</span><span class="sxs-lookup"><span data-stu-id="34ee6-191">assignments</span></span>|<span data-ttu-id="34ee6-192">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="34ee6-192">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) collection</span></span>|<span data-ttu-id="34ee6-193">策略部署到的包含组和排除组列表的导航属性。</span><span class="sxs-lookup"><span data-stu-id="34ee6-193">Navigation property to list of inclusion and exclusion groups to which the policy is deployed.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="34ee6-194">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="34ee6-194">JSON Representation</span></span>
<span data-ttu-id="34ee6-195">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="34ee6-195">Here is a JSON representation of the resource.</span></span>
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




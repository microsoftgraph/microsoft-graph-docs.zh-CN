---
title: targetedManagedAppConfiguration 资源类型
description: 用于将一组自定义设置按原样提供给目标安全组中的所有用户的配置
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 569bed8e1fd9811975f4d5093d59995fe6019f28
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37199911"
---
# <a name="targetedmanagedappconfiguration-resource-type"></a><span data-ttu-id="e9c45-103">targetedManagedAppConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="e9c45-103">targetedManagedAppConfiguration resource type</span></span>

> <span data-ttu-id="e9c45-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e9c45-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e9c45-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e9c45-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e9c45-106">用于将一组自定义设置按原样提供给目标安全组中的所有用户的配置</span><span class="sxs-lookup"><span data-stu-id="e9c45-106">Configuration used to deliver a set of custom settings as-is to all users in the targeted security group</span></span>


<span data-ttu-id="e9c45-107">继承自 [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e9c45-107">Inherits from [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="e9c45-108">方法</span><span class="sxs-lookup"><span data-stu-id="e9c45-108">Methods</span></span>
|<span data-ttu-id="e9c45-109">方法</span><span class="sxs-lookup"><span data-stu-id="e9c45-109">Method</span></span>|<span data-ttu-id="e9c45-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="e9c45-110">Return Type</span></span>|<span data-ttu-id="e9c45-111">说明</span><span class="sxs-lookup"><span data-stu-id="e9c45-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e9c45-112">List targetedManagedAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="e9c45-112">List targetedManagedAppConfigurations</span></span>](../api/intune-shared-targetedmanagedappconfiguration-list.md)|<span data-ttu-id="e9c45-113">[targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e9c45-113">[targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) collection</span></span>|<span data-ttu-id="e9c45-114">列出 [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e9c45-114">List properties and relationships of the [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="e9c45-115">Get targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="e9c45-115">Get targetedManagedAppConfiguration</span></span>](../api/intune-shared-targetedmanagedappconfiguration-get.md)|[<span data-ttu-id="e9c45-116">targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="e9c45-116">targetedManagedAppConfiguration</span></span>](../resources/intune-shared-targetedmanagedappconfiguration.md)|<span data-ttu-id="e9c45-117">读取 [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e9c45-117">Read properties and relationships of the [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) object.</span></span>|
|[<span data-ttu-id="e9c45-118">Create targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="e9c45-118">Create targetedManagedAppConfiguration</span></span>](../api/intune-shared-targetedmanagedappconfiguration-create.md)|[<span data-ttu-id="e9c45-119">targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="e9c45-119">targetedManagedAppConfiguration</span></span>](../resources/intune-shared-targetedmanagedappconfiguration.md)|<span data-ttu-id="e9c45-120">创建新的 [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e9c45-120">Create a new [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) object.</span></span>|
|[<span data-ttu-id="e9c45-121">Delete targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="e9c45-121">Delete targetedManagedAppConfiguration</span></span>](../api/intune-shared-targetedmanagedappconfiguration-delete.md)|<span data-ttu-id="e9c45-122">无</span><span class="sxs-lookup"><span data-stu-id="e9c45-122">None</span></span>|<span data-ttu-id="e9c45-123">删除 [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="e9c45-123">Deletes a [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md).</span></span>|
|[<span data-ttu-id="e9c45-124">Update targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="e9c45-124">Update targetedManagedAppConfiguration</span></span>](../api/intune-shared-targetedmanagedappconfiguration-update.md)|[<span data-ttu-id="e9c45-125">targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="e9c45-125">targetedManagedAppConfiguration</span></span>](../resources/intune-shared-targetedmanagedappconfiguration.md)|<span data-ttu-id="e9c45-126">更新 [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="e9c45-126">Update the properties of a [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) object.</span></span>|
|<span data-ttu-id="e9c45-127">**移动应用管理 (MAM)**</span><span class="sxs-lookup"><span data-stu-id="e9c45-127">**Mobile app management (MAM)**</span></span>|
|[<span data-ttu-id="e9c45-128">分配操作</span><span class="sxs-lookup"><span data-stu-id="e9c45-128">assign action</span></span>](../api/intune-shared-targetedmanagedappconfiguration-assign.md)|<span data-ttu-id="e9c45-129">无</span><span class="sxs-lookup"><span data-stu-id="e9c45-129">None</span></span>|<span data-ttu-id="e9c45-130">尚未记录</span><span class="sxs-lookup"><span data-stu-id="e9c45-130">Not yet documented</span></span>|
|[<span data-ttu-id="e9c45-131">targetApps 操作</span><span class="sxs-lookup"><span data-stu-id="e9c45-131">targetApps action</span></span>](../api/intune-shared-targetedmanagedappconfiguration-targetapps.md)|<span data-ttu-id="e9c45-132">无</span><span class="sxs-lookup"><span data-stu-id="e9c45-132">None</span></span>|<span data-ttu-id="e9c45-133">尚未记录</span><span class="sxs-lookup"><span data-stu-id="e9c45-133">Not yet documented</span></span>|
|<span data-ttu-id="e9c45-134">**策略集**</span><span class="sxs-lookup"><span data-stu-id="e9c45-134">**Policy Set**</span></span>|
|[<span data-ttu-id="e9c45-135">hasPayloadLinks 操作</span><span class="sxs-lookup"><span data-stu-id="e9c45-135">hasPayloadLinks action</span></span>](../api/intune-shared-targetedmanagedappconfiguration-haspayloadlinks.md)|<span data-ttu-id="e9c45-136">[hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md)集合</span><span class="sxs-lookup"><span data-stu-id="e9c45-136">[hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md) collection</span></span>|<span data-ttu-id="e9c45-137">尚未记录</span><span class="sxs-lookup"><span data-stu-id="e9c45-137">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="e9c45-138">属性</span><span class="sxs-lookup"><span data-stu-id="e9c45-138">Properties</span></span>
|<span data-ttu-id="e9c45-139">属性</span><span class="sxs-lookup"><span data-stu-id="e9c45-139">Property</span></span>|<span data-ttu-id="e9c45-140">类型</span><span class="sxs-lookup"><span data-stu-id="e9c45-140">Type</span></span>|<span data-ttu-id="e9c45-141">说明</span><span class="sxs-lookup"><span data-stu-id="e9c45-141">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e9c45-142">id</span><span class="sxs-lookup"><span data-stu-id="e9c45-142">id</span></span>|<span data-ttu-id="e9c45-143">字符串</span><span class="sxs-lookup"><span data-stu-id="e9c45-143">String</span></span>|<span data-ttu-id="e9c45-144">实体的键。</span><span class="sxs-lookup"><span data-stu-id="e9c45-144">Key of the entity.</span></span> <span data-ttu-id="e9c45-145">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="e9c45-145">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="e9c45-146">displayName</span><span class="sxs-lookup"><span data-stu-id="e9c45-146">displayName</span></span>|<span data-ttu-id="e9c45-147">字符串</span><span class="sxs-lookup"><span data-stu-id="e9c45-147">String</span></span>|<span data-ttu-id="e9c45-148">策略显示名称。</span><span class="sxs-lookup"><span data-stu-id="e9c45-148">Policy display name.</span></span> <span data-ttu-id="e9c45-149">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="e9c45-149">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="e9c45-150">说明</span><span class="sxs-lookup"><span data-stu-id="e9c45-150">description</span></span>|<span data-ttu-id="e9c45-151">String</span><span class="sxs-lookup"><span data-stu-id="e9c45-151">String</span></span>|<span data-ttu-id="e9c45-152">策略的说明。</span><span class="sxs-lookup"><span data-stu-id="e9c45-152">The policy's description.</span></span> <span data-ttu-id="e9c45-153">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="e9c45-153">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="e9c45-154">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e9c45-154">createdDateTime</span></span>|<span data-ttu-id="e9c45-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e9c45-155">DateTimeOffset</span></span>|<span data-ttu-id="e9c45-156">创建策略的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="e9c45-156">The date and time the policy was created.</span></span> <span data-ttu-id="e9c45-157">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="e9c45-157">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="e9c45-158">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e9c45-158">lastModifiedDateTime</span></span>|<span data-ttu-id="e9c45-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e9c45-159">DateTimeOffset</span></span>|<span data-ttu-id="e9c45-160">上次修改策略的时间。</span><span class="sxs-lookup"><span data-stu-id="e9c45-160">Last time the policy was modified.</span></span> <span data-ttu-id="e9c45-161">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="e9c45-161">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="e9c45-162">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e9c45-162">roleScopeTagIds</span></span>|<span data-ttu-id="e9c45-163">String collection</span><span class="sxs-lookup"><span data-stu-id="e9c45-163">String collection</span></span>|<span data-ttu-id="e9c45-164">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="e9c45-164">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="e9c45-165">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="e9c45-165">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="e9c45-166">version</span><span class="sxs-lookup"><span data-stu-id="e9c45-166">version</span></span>|<span data-ttu-id="e9c45-167">String</span><span class="sxs-lookup"><span data-stu-id="e9c45-167">String</span></span>|<span data-ttu-id="e9c45-168">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="e9c45-168">Version of the entity.</span></span> <span data-ttu-id="e9c45-169">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="e9c45-169">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="e9c45-170">customSettings</span><span class="sxs-lookup"><span data-stu-id="e9c45-170">customSettings</span></span>|<span data-ttu-id="e9c45-171">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e9c45-171">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="e9c45-172">要发送到配置范围确定的用户应用的一组字符串键和字符串值对，不由此服务更改。继承自 [ managedAppConfiguration ](../resources/intune-mam-managedappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e9c45-172">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service Inherited from [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span></span>|
|<span data-ttu-id="e9c45-173">deployedAppCount</span><span class="sxs-lookup"><span data-stu-id="e9c45-173">deployedAppCount</span></span>|<span data-ttu-id="e9c45-174">Int32</span><span class="sxs-lookup"><span data-stu-id="e9c45-174">Int32</span></span>|<span data-ttu-id="e9c45-175">当前策略部署到的应用的计数。</span><span class="sxs-lookup"><span data-stu-id="e9c45-175">Count of apps to which the current policy is deployed.</span></span>|
|<span data-ttu-id="e9c45-176">isAssigned</span><span class="sxs-lookup"><span data-stu-id="e9c45-176">isAssigned</span></span>|<span data-ttu-id="e9c45-177">Boolean</span><span class="sxs-lookup"><span data-stu-id="e9c45-177">Boolean</span></span>|<span data-ttu-id="e9c45-178">指示策略是否部署到任何包含组。</span><span class="sxs-lookup"><span data-stu-id="e9c45-178">Indicates if the policy is deployed to any inclusion groups or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e9c45-179">关系</span><span class="sxs-lookup"><span data-stu-id="e9c45-179">Relationships</span></span>
|<span data-ttu-id="e9c45-180">关系</span><span class="sxs-lookup"><span data-stu-id="e9c45-180">Relationship</span></span>|<span data-ttu-id="e9c45-181">类型</span><span class="sxs-lookup"><span data-stu-id="e9c45-181">Type</span></span>|<span data-ttu-id="e9c45-182">说明</span><span class="sxs-lookup"><span data-stu-id="e9c45-182">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e9c45-183">**移动应用管理 (MAM)**</span><span class="sxs-lookup"><span data-stu-id="e9c45-183">**Mobile app management (MAM)**</span></span>|
|<span data-ttu-id="e9c45-184">apps</span><span class="sxs-lookup"><span data-stu-id="e9c45-184">apps</span></span>|<span data-ttu-id="e9c45-185">[managedMobileApp](../resources/intune-mam-managedmobileapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e9c45-185">[managedMobileApp](../resources/intune-mam-managedmobileapp.md) collection</span></span>|<span data-ttu-id="e9c45-186">策略部署到的应用的列表。</span><span class="sxs-lookup"><span data-stu-id="e9c45-186">List of apps to which the policy is deployed.</span></span>|
|<span data-ttu-id="e9c45-187">deploymentSummary</span><span class="sxs-lookup"><span data-stu-id="e9c45-187">deploymentSummary</span></span>|[<span data-ttu-id="e9c45-188">managedAppPolicyDeploymentSummary</span><span class="sxs-lookup"><span data-stu-id="e9c45-188">managedAppPolicyDeploymentSummary</span></span>](../resources/intune-mam-managedapppolicydeploymentsummary.md)|<span data-ttu-id="e9c45-189">配置的部署摘要的导航属性。</span><span class="sxs-lookup"><span data-stu-id="e9c45-189">Navigation property to deployment summary of the configuration.</span></span>|
|<span data-ttu-id="e9c45-190">assignments</span><span class="sxs-lookup"><span data-stu-id="e9c45-190">assignments</span></span>|<span data-ttu-id="e9c45-191">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e9c45-191">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) collection</span></span>|<span data-ttu-id="e9c45-192">策略部署到的包含组和排除组列表的导航属性。</span><span class="sxs-lookup"><span data-stu-id="e9c45-192">Navigation property to list of inclusion and exclusion groups to which the policy is deployed.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e9c45-193">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e9c45-193">JSON Representation</span></span>
<span data-ttu-id="e9c45-194">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e9c45-194">Here is a JSON representation of the resource.</span></span>
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




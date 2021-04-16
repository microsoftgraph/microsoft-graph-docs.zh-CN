---
title: targetedManagedAppConfiguration 资源类型
description: 用于将一组自定义设置按原样提供给目标安全组中的所有用户的配置
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4d580e4eba2c8fbfa95a78024f82d5cc343881c8
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2021
ms.locfileid: "51868020"
---
# <a name="targetedmanagedappconfiguration-resource-type"></a><span data-ttu-id="cacef-103">targetedManagedAppConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="cacef-103">targetedManagedAppConfiguration resource type</span></span>

<span data-ttu-id="cacef-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cacef-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cacef-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="cacef-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cacef-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="cacef-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cacef-107">用于将一组自定义设置按原样提供给目标安全组中的所有用户的配置</span><span class="sxs-lookup"><span data-stu-id="cacef-107">Configuration used to deliver a set of custom settings as-is to all users in the targeted security group</span></span>


<span data-ttu-id="cacef-108">继承自 [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cacef-108">Inherits from [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="cacef-109">方法</span><span class="sxs-lookup"><span data-stu-id="cacef-109">Methods</span></span>
|<span data-ttu-id="cacef-110">方法</span><span class="sxs-lookup"><span data-stu-id="cacef-110">Method</span></span>|<span data-ttu-id="cacef-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="cacef-111">Return Type</span></span>|<span data-ttu-id="cacef-112">说明</span><span class="sxs-lookup"><span data-stu-id="cacef-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="cacef-113">List targetedManagedAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="cacef-113">List targetedManagedAppConfigurations</span></span>](../api/intune-shared-targetedmanagedappconfiguration-list.md)|<span data-ttu-id="cacef-114">[targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="cacef-114">[targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) collection</span></span>|<span data-ttu-id="cacef-115">列出 [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="cacef-115">List properties and relationships of the [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="cacef-116">Get targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="cacef-116">Get targetedManagedAppConfiguration</span></span>](../api/intune-shared-targetedmanagedappconfiguration-get.md)|[<span data-ttu-id="cacef-117">targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="cacef-117">targetedManagedAppConfiguration</span></span>](../resources/intune-shared-targetedmanagedappconfiguration.md)|<span data-ttu-id="cacef-118">读取 [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="cacef-118">Read properties and relationships of the [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) object.</span></span>|
|[<span data-ttu-id="cacef-119">Create targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="cacef-119">Create targetedManagedAppConfiguration</span></span>](../api/intune-shared-targetedmanagedappconfiguration-create.md)|[<span data-ttu-id="cacef-120">targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="cacef-120">targetedManagedAppConfiguration</span></span>](../resources/intune-shared-targetedmanagedappconfiguration.md)|<span data-ttu-id="cacef-121">创建新的 [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="cacef-121">Create a new [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) object.</span></span>|
|[<span data-ttu-id="cacef-122">Delete targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="cacef-122">Delete targetedManagedAppConfiguration</span></span>](../api/intune-shared-targetedmanagedappconfiguration-delete.md)|<span data-ttu-id="cacef-123">无</span><span class="sxs-lookup"><span data-stu-id="cacef-123">None</span></span>|<span data-ttu-id="cacef-124">删除 [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="cacef-124">Deletes a [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md).</span></span>|
|[<span data-ttu-id="cacef-125">Update targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="cacef-125">Update targetedManagedAppConfiguration</span></span>](../api/intune-shared-targetedmanagedappconfiguration-update.md)|[<span data-ttu-id="cacef-126">targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="cacef-126">targetedManagedAppConfiguration</span></span>](../resources/intune-shared-targetedmanagedappconfiguration.md)|<span data-ttu-id="cacef-127">更新 [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="cacef-127">Update the properties of a [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) object.</span></span>|
|<span data-ttu-id="cacef-128">**移动应用管理 (MAM)**</span><span class="sxs-lookup"><span data-stu-id="cacef-128">**Mobile app management (MAM)**</span></span>|
|[<span data-ttu-id="cacef-129">分配操作</span><span class="sxs-lookup"><span data-stu-id="cacef-129">assign action</span></span>](../api/intune-shared-targetedmanagedappconfiguration-assign.md)|<span data-ttu-id="cacef-130">无</span><span class="sxs-lookup"><span data-stu-id="cacef-130">None</span></span>|<span data-ttu-id="cacef-131">尚未记录</span><span class="sxs-lookup"><span data-stu-id="cacef-131">Not yet documented</span></span>|
|[<span data-ttu-id="cacef-132">targetApps 操作</span><span class="sxs-lookup"><span data-stu-id="cacef-132">targetApps action</span></span>](../api/intune-shared-targetedmanagedappconfiguration-targetapps.md)|<span data-ttu-id="cacef-133">无</span><span class="sxs-lookup"><span data-stu-id="cacef-133">None</span></span>|<span data-ttu-id="cacef-134">尚未记录</span><span class="sxs-lookup"><span data-stu-id="cacef-134">Not yet documented</span></span>|
|<span data-ttu-id="cacef-135">**策略集**</span><span class="sxs-lookup"><span data-stu-id="cacef-135">**Policy Set**</span></span>|
|[<span data-ttu-id="cacef-136">hasPayloadLinks 操作</span><span class="sxs-lookup"><span data-stu-id="cacef-136">hasPayloadLinks action</span></span>](../api/intune-shared-targetedmanagedappconfiguration-haspayloadlinks.md)|<span data-ttu-id="cacef-137">[hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="cacef-137">[hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md) collection</span></span>|<span data-ttu-id="cacef-138">尚未记录</span><span class="sxs-lookup"><span data-stu-id="cacef-138">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="cacef-139">属性</span><span class="sxs-lookup"><span data-stu-id="cacef-139">Properties</span></span>
|<span data-ttu-id="cacef-140">属性</span><span class="sxs-lookup"><span data-stu-id="cacef-140">Property</span></span>|<span data-ttu-id="cacef-141">类型</span><span class="sxs-lookup"><span data-stu-id="cacef-141">Type</span></span>|<span data-ttu-id="cacef-142">说明</span><span class="sxs-lookup"><span data-stu-id="cacef-142">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cacef-143">id</span><span class="sxs-lookup"><span data-stu-id="cacef-143">id</span></span>|<span data-ttu-id="cacef-144">String</span><span class="sxs-lookup"><span data-stu-id="cacef-144">String</span></span>|<span data-ttu-id="cacef-145">实体的键。</span><span class="sxs-lookup"><span data-stu-id="cacef-145">Key of the entity.</span></span> <span data-ttu-id="cacef-146">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="cacef-146">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="cacef-147">displayName</span><span class="sxs-lookup"><span data-stu-id="cacef-147">displayName</span></span>|<span data-ttu-id="cacef-148">String</span><span class="sxs-lookup"><span data-stu-id="cacef-148">String</span></span>|<span data-ttu-id="cacef-149">策略显示名称。</span><span class="sxs-lookup"><span data-stu-id="cacef-149">Policy display name.</span></span> <span data-ttu-id="cacef-150">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="cacef-150">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="cacef-151">说明</span><span class="sxs-lookup"><span data-stu-id="cacef-151">description</span></span>|<span data-ttu-id="cacef-152">String</span><span class="sxs-lookup"><span data-stu-id="cacef-152">String</span></span>|<span data-ttu-id="cacef-153">策略的说明。</span><span class="sxs-lookup"><span data-stu-id="cacef-153">The policy's description.</span></span> <span data-ttu-id="cacef-154">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="cacef-154">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="cacef-155">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cacef-155">createdDateTime</span></span>|<span data-ttu-id="cacef-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cacef-156">DateTimeOffset</span></span>|<span data-ttu-id="cacef-157">创建策略的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="cacef-157">The date and time the policy was created.</span></span> <span data-ttu-id="cacef-158">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="cacef-158">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="cacef-159">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cacef-159">lastModifiedDateTime</span></span>|<span data-ttu-id="cacef-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cacef-160">DateTimeOffset</span></span>|<span data-ttu-id="cacef-161">上次修改策略的时间。</span><span class="sxs-lookup"><span data-stu-id="cacef-161">Last time the policy was modified.</span></span> <span data-ttu-id="cacef-162">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="cacef-162">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="cacef-163">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="cacef-163">roleScopeTagIds</span></span>|<span data-ttu-id="cacef-164">String 集合</span><span class="sxs-lookup"><span data-stu-id="cacef-164">String collection</span></span>|<span data-ttu-id="cacef-165">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="cacef-165">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="cacef-166">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="cacef-166">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="cacef-167">version</span><span class="sxs-lookup"><span data-stu-id="cacef-167">version</span></span>|<span data-ttu-id="cacef-168">String</span><span class="sxs-lookup"><span data-stu-id="cacef-168">String</span></span>|<span data-ttu-id="cacef-169">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="cacef-169">Version of the entity.</span></span> <span data-ttu-id="cacef-170">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="cacef-170">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="cacef-171">customSettings</span><span class="sxs-lookup"><span data-stu-id="cacef-171">customSettings</span></span>|<span data-ttu-id="cacef-172">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="cacef-172">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="cacef-173">要发送到配置范围确定的用户应用的一组字符串键和字符串值对，不由此服务更改。继承自 [ managedAppConfiguration ](../resources/intune-mam-managedappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cacef-173">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service Inherited from [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span></span>|
|<span data-ttu-id="cacef-174">deployedAppCount</span><span class="sxs-lookup"><span data-stu-id="cacef-174">deployedAppCount</span></span>|<span data-ttu-id="cacef-175">Int32</span><span class="sxs-lookup"><span data-stu-id="cacef-175">Int32</span></span>|<span data-ttu-id="cacef-176">当前策略部署到的应用的计数。</span><span class="sxs-lookup"><span data-stu-id="cacef-176">Count of apps to which the current policy is deployed.</span></span>|
|<span data-ttu-id="cacef-177">isAssigned</span><span class="sxs-lookup"><span data-stu-id="cacef-177">isAssigned</span></span>|<span data-ttu-id="cacef-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="cacef-178">Boolean</span></span>|<span data-ttu-id="cacef-179">指示策略是否部署到任何包含组。</span><span class="sxs-lookup"><span data-stu-id="cacef-179">Indicates if the policy is deployed to any inclusion groups or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cacef-180">关系</span><span class="sxs-lookup"><span data-stu-id="cacef-180">Relationships</span></span>
|<span data-ttu-id="cacef-181">关系</span><span class="sxs-lookup"><span data-stu-id="cacef-181">Relationship</span></span>|<span data-ttu-id="cacef-182">类型</span><span class="sxs-lookup"><span data-stu-id="cacef-182">Type</span></span>|<span data-ttu-id="cacef-183">说明</span><span class="sxs-lookup"><span data-stu-id="cacef-183">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cacef-184">**移动应用管理 (MAM)**</span><span class="sxs-lookup"><span data-stu-id="cacef-184">**Mobile app management (MAM)**</span></span>|
|<span data-ttu-id="cacef-185">apps</span><span class="sxs-lookup"><span data-stu-id="cacef-185">apps</span></span>|<span data-ttu-id="cacef-186">[managedMobileApp](../resources/intune-mam-managedmobileapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="cacef-186">[managedMobileApp](../resources/intune-mam-managedmobileapp.md) collection</span></span>|<span data-ttu-id="cacef-187">策略部署到的应用的列表。</span><span class="sxs-lookup"><span data-stu-id="cacef-187">List of apps to which the policy is deployed.</span></span>|
|<span data-ttu-id="cacef-188">deploymentSummary</span><span class="sxs-lookup"><span data-stu-id="cacef-188">deploymentSummary</span></span>|[<span data-ttu-id="cacef-189">managedAppPolicyDeploymentSummary</span><span class="sxs-lookup"><span data-stu-id="cacef-189">managedAppPolicyDeploymentSummary</span></span>](../resources/intune-mam-managedapppolicydeploymentsummary.md)|<span data-ttu-id="cacef-190">配置的部署摘要的导航属性。</span><span class="sxs-lookup"><span data-stu-id="cacef-190">Navigation property to deployment summary of the configuration.</span></span>|
|<span data-ttu-id="cacef-191">assignments</span><span class="sxs-lookup"><span data-stu-id="cacef-191">assignments</span></span>|<span data-ttu-id="cacef-192">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="cacef-192">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) collection</span></span>|<span data-ttu-id="cacef-193">策略部署到的包含组和排除组列表的导航属性。</span><span class="sxs-lookup"><span data-stu-id="cacef-193">Navigation property to list of inclusion and exclusion groups to which the policy is deployed.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cacef-194">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cacef-194">JSON Representation</span></span>
<span data-ttu-id="cacef-195">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cacef-195">Here is a JSON representation of the resource.</span></span>
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





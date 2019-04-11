---
title: targetedManagedAppConfiguration 资源类型
description: 用于将一组自定义设置按原样提供给目标安全组中的所有用户的配置
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a293b112c0c418ed22322113ba948ed6db6c6133
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31790856"
---
# <a name="targetedmanagedappconfiguration-resource-type"></a><span data-ttu-id="455ad-103">targetedManagedAppConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="455ad-103">targetedManagedAppConfiguration resource type</span></span>

> <span data-ttu-id="455ad-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="455ad-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="455ad-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="455ad-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="455ad-106">用于将一组自定义设置按原样提供给目标安全组中的所有用户的配置</span><span class="sxs-lookup"><span data-stu-id="455ad-106">Configuration used to deliver a set of custom settings as-is to all users in the targeted security group</span></span>


<span data-ttu-id="455ad-107">继承自 [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="455ad-107">Inherits from [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="455ad-108">方法</span><span class="sxs-lookup"><span data-stu-id="455ad-108">Methods</span></span>
|<span data-ttu-id="455ad-109">方法</span><span class="sxs-lookup"><span data-stu-id="455ad-109">Method</span></span>|<span data-ttu-id="455ad-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="455ad-110">Return Type</span></span>|<span data-ttu-id="455ad-111">说明</span><span class="sxs-lookup"><span data-stu-id="455ad-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="455ad-112">列出 targetedManagedAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="455ad-112">List targetedManagedAppConfigurations</span></span>](../api/intune-mam-targetedmanagedappconfiguration-list.md)|<span data-ttu-id="455ad-113">[targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="455ad-113">[targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) collection</span></span>|<span data-ttu-id="455ad-114">列出 [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="455ad-114">List properties and relationships of the [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="455ad-115">获取 targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="455ad-115">Get targetedManagedAppConfiguration</span></span>](../api/intune-mam-targetedmanagedappconfiguration-get.md)|[<span data-ttu-id="455ad-116">targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="455ad-116">targetedManagedAppConfiguration</span></span>](../resources/intune-mam-targetedmanagedappconfiguration.md)|<span data-ttu-id="455ad-117">读取 [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="455ad-117">Read properties and relationships of the [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>|
|[<span data-ttu-id="455ad-118">创建 targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="455ad-118">Create targetedManagedAppConfiguration</span></span>](../api/intune-mam-targetedmanagedappconfiguration-create.md)|[<span data-ttu-id="455ad-119">targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="455ad-119">targetedManagedAppConfiguration</span></span>](../resources/intune-mam-targetedmanagedappconfiguration.md)|<span data-ttu-id="455ad-120">创建新的 [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="455ad-120">Create a new [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>|
|[<span data-ttu-id="455ad-121">删除 targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="455ad-121">Delete targetedManagedAppConfiguration</span></span>](../api/intune-mam-targetedmanagedappconfiguration-delete.md)|<span data-ttu-id="455ad-122">无</span><span class="sxs-lookup"><span data-stu-id="455ad-122">None</span></span>|<span data-ttu-id="455ad-123">删除 [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="455ad-123">Deletes a [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md).</span></span>|
|[<span data-ttu-id="455ad-124">更新 targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="455ad-124">Update targetedManagedAppConfiguration</span></span>](../api/intune-mam-targetedmanagedappconfiguration-update.md)|[<span data-ttu-id="455ad-125">targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="455ad-125">targetedManagedAppConfiguration</span></span>](../resources/intune-mam-targetedmanagedappconfiguration.md)|<span data-ttu-id="455ad-126">更新 [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="455ad-126">Update the properties of a [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>|
|[<span data-ttu-id="455ad-127">分配操作</span><span class="sxs-lookup"><span data-stu-id="455ad-127">assign action</span></span>](../api/intune-mam-targetedmanagedappconfiguration-assign.md)|<span data-ttu-id="455ad-128">无</span><span class="sxs-lookup"><span data-stu-id="455ad-128">None</span></span>|<span data-ttu-id="455ad-129">尚未记录</span><span class="sxs-lookup"><span data-stu-id="455ad-129">Not yet documented</span></span>|
|[<span data-ttu-id="455ad-130">targetApps 操作</span><span class="sxs-lookup"><span data-stu-id="455ad-130">targetApps action</span></span>](../api/intune-mam-targetedmanagedappconfiguration-targetapps.md)|<span data-ttu-id="455ad-131">无</span><span class="sxs-lookup"><span data-stu-id="455ad-131">None</span></span>|<span data-ttu-id="455ad-132">尚未记录</span><span class="sxs-lookup"><span data-stu-id="455ad-132">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="455ad-133">属性</span><span class="sxs-lookup"><span data-stu-id="455ad-133">Properties</span></span>
|<span data-ttu-id="455ad-134">属性</span><span class="sxs-lookup"><span data-stu-id="455ad-134">Property</span></span>|<span data-ttu-id="455ad-135">类型</span><span class="sxs-lookup"><span data-stu-id="455ad-135">Type</span></span>|<span data-ttu-id="455ad-136">说明</span><span class="sxs-lookup"><span data-stu-id="455ad-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="455ad-137">displayName</span><span class="sxs-lookup"><span data-stu-id="455ad-137">displayName</span></span>|<span data-ttu-id="455ad-138">String</span><span class="sxs-lookup"><span data-stu-id="455ad-138">String</span></span>|<span data-ttu-id="455ad-139">策略显示名称。</span><span class="sxs-lookup"><span data-stu-id="455ad-139">Policy display name.</span></span> <span data-ttu-id="455ad-140">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="455ad-140">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="455ad-141">description</span><span class="sxs-lookup"><span data-stu-id="455ad-141">description</span></span>|<span data-ttu-id="455ad-142">String</span><span class="sxs-lookup"><span data-stu-id="455ad-142">String</span></span>|<span data-ttu-id="455ad-143">策略的说明。</span><span class="sxs-lookup"><span data-stu-id="455ad-143">The policy's description.</span></span> <span data-ttu-id="455ad-144">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="455ad-144">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="455ad-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="455ad-145">createdDateTime</span></span>|<span data-ttu-id="455ad-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="455ad-146">DateTimeOffset</span></span>|<span data-ttu-id="455ad-147">创建策略的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="455ad-147">The date and time the policy was created.</span></span> <span data-ttu-id="455ad-148">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="455ad-148">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="455ad-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="455ad-149">lastModifiedDateTime</span></span>|<span data-ttu-id="455ad-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="455ad-150">DateTimeOffset</span></span>|<span data-ttu-id="455ad-151">上次修改策略的时间。</span><span class="sxs-lookup"><span data-stu-id="455ad-151">Last time the policy was modified.</span></span> <span data-ttu-id="455ad-152">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="455ad-152">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="455ad-153">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="455ad-153">roleScopeTagIds</span></span>|<span data-ttu-id="455ad-154">String 集合</span><span class="sxs-lookup"><span data-stu-id="455ad-154">String collection</span></span>|<span data-ttu-id="455ad-155">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="455ad-155">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="455ad-156">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="455ad-156">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="455ad-157">id</span><span class="sxs-lookup"><span data-stu-id="455ad-157">id</span></span>|<span data-ttu-id="455ad-158">String</span><span class="sxs-lookup"><span data-stu-id="455ad-158">String</span></span>|<span data-ttu-id="455ad-159">实体的键。</span><span class="sxs-lookup"><span data-stu-id="455ad-159">Key of the entity.</span></span> <span data-ttu-id="455ad-160">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="455ad-160">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="455ad-161">version</span><span class="sxs-lookup"><span data-stu-id="455ad-161">version</span></span>|<span data-ttu-id="455ad-162">String</span><span class="sxs-lookup"><span data-stu-id="455ad-162">String</span></span>|<span data-ttu-id="455ad-163">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="455ad-163">Version of the entity.</span></span> <span data-ttu-id="455ad-164">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="455ad-164">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="455ad-165">customSettings</span><span class="sxs-lookup"><span data-stu-id="455ad-165">customSettings</span></span>|<span data-ttu-id="455ad-166">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="455ad-166">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="455ad-167">要发送到配置范围确定的用户应用的一组字符串键和字符串值对，不由此服务更改。继承自 [ managedAppConfiguration ](../resources/intune-mam-managedappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="455ad-167">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service Inherited from [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span></span>|
|<span data-ttu-id="455ad-168">deployedAppCount</span><span class="sxs-lookup"><span data-stu-id="455ad-168">deployedAppCount</span></span>|<span data-ttu-id="455ad-169">Int32</span><span class="sxs-lookup"><span data-stu-id="455ad-169">Int32</span></span>|<span data-ttu-id="455ad-170">当前策略部署到的应用的计数。</span><span class="sxs-lookup"><span data-stu-id="455ad-170">Count of apps to which the current policy is deployed.</span></span>|
|<span data-ttu-id="455ad-171">isAssigned</span><span class="sxs-lookup"><span data-stu-id="455ad-171">isAssigned</span></span>|<span data-ttu-id="455ad-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="455ad-172">Boolean</span></span>|<span data-ttu-id="455ad-173">指示策略是否部署到任何包含组。</span><span class="sxs-lookup"><span data-stu-id="455ad-173">Indicates if the policy is deployed to any inclusion groups or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="455ad-174">关系</span><span class="sxs-lookup"><span data-stu-id="455ad-174">Relationships</span></span>
|<span data-ttu-id="455ad-175">关系</span><span class="sxs-lookup"><span data-stu-id="455ad-175">Relationship</span></span>|<span data-ttu-id="455ad-176">类型</span><span class="sxs-lookup"><span data-stu-id="455ad-176">Type</span></span>|<span data-ttu-id="455ad-177">说明</span><span class="sxs-lookup"><span data-stu-id="455ad-177">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="455ad-178">apps</span><span class="sxs-lookup"><span data-stu-id="455ad-178">apps</span></span>|<span data-ttu-id="455ad-179">[managedMobileApp](../resources/intune-mam-managedmobileapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="455ad-179">[managedMobileApp](../resources/intune-mam-managedmobileapp.md) collection</span></span>|<span data-ttu-id="455ad-180">策略部署到的应用的列表。</span><span class="sxs-lookup"><span data-stu-id="455ad-180">List of apps to which the policy is deployed.</span></span>|
|<span data-ttu-id="455ad-181">deploymentSummary</span><span class="sxs-lookup"><span data-stu-id="455ad-181">deploymentSummary</span></span>|[<span data-ttu-id="455ad-182">managedAppPolicyDeploymentSummary</span><span class="sxs-lookup"><span data-stu-id="455ad-182">managedAppPolicyDeploymentSummary</span></span>](../resources/intune-mam-managedapppolicydeploymentsummary.md)|<span data-ttu-id="455ad-183">配置的部署摘要的导航属性。</span><span class="sxs-lookup"><span data-stu-id="455ad-183">Navigation property to deployment summary of the configuration.</span></span>|
|<span data-ttu-id="455ad-184">assignments</span><span class="sxs-lookup"><span data-stu-id="455ad-184">assignments</span></span>|<span data-ttu-id="455ad-185">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="455ad-185">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) collection</span></span>|<span data-ttu-id="455ad-186">策略部署到的包含组和排除组列表的导航属性。</span><span class="sxs-lookup"><span data-stu-id="455ad-186">Navigation property to list of inclusion and exclusion groups to which the policy is deployed.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="455ad-187">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="455ad-187">JSON Representation</span></span>
<span data-ttu-id="455ad-188">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="455ad-188">Here is a JSON representation of the resource.</span></span>
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






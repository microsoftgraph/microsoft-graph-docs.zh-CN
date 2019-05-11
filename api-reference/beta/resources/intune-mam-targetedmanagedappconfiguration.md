---
title: targetedManagedAppConfiguration 资源类型
description: 用于将一组自定义设置按原样提供给目标安全组中的所有用户的配置
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 70a7d863b409d9447f42df49cd818787ab926c4f
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33940629"
---
# <a name="targetedmanagedappconfiguration-resource-type"></a><span data-ttu-id="9805b-103">targetedManagedAppConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="9805b-103">targetedManagedAppConfiguration resource type</span></span>

> <span data-ttu-id="9805b-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9805b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9805b-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9805b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9805b-106">用于将一组自定义设置按原样提供给目标安全组中的所有用户的配置</span><span class="sxs-lookup"><span data-stu-id="9805b-106">Configuration used to deliver a set of custom settings as-is to all users in the targeted security group</span></span>


<span data-ttu-id="9805b-107">继承自 [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9805b-107">Inherits from [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="9805b-108">方法</span><span class="sxs-lookup"><span data-stu-id="9805b-108">Methods</span></span>
|<span data-ttu-id="9805b-109">方法</span><span class="sxs-lookup"><span data-stu-id="9805b-109">Method</span></span>|<span data-ttu-id="9805b-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="9805b-110">Return Type</span></span>|<span data-ttu-id="9805b-111">说明</span><span class="sxs-lookup"><span data-stu-id="9805b-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="9805b-112">List targetedManagedAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="9805b-112">List targetedManagedAppConfigurations</span></span>](../api/intune-mam-targetedmanagedappconfiguration-list.md)|<span data-ttu-id="9805b-113">[targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9805b-113">[targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) collection</span></span>|<span data-ttu-id="9805b-114">列出 [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9805b-114">List properties and relationships of the [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="9805b-115">Get targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="9805b-115">Get targetedManagedAppConfiguration</span></span>](../api/intune-mam-targetedmanagedappconfiguration-get.md)|[<span data-ttu-id="9805b-116">targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="9805b-116">targetedManagedAppConfiguration</span></span>](../resources/intune-mam-targetedmanagedappconfiguration.md)|<span data-ttu-id="9805b-117">读取 [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9805b-117">Read properties and relationships of the [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>|
|[<span data-ttu-id="9805b-118">Create targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="9805b-118">Create targetedManagedAppConfiguration</span></span>](../api/intune-mam-targetedmanagedappconfiguration-create.md)|[<span data-ttu-id="9805b-119">targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="9805b-119">targetedManagedAppConfiguration</span></span>](../resources/intune-mam-targetedmanagedappconfiguration.md)|<span data-ttu-id="9805b-120">创建新的 [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9805b-120">Create a new [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>|
|[<span data-ttu-id="9805b-121">Delete targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="9805b-121">Delete targetedManagedAppConfiguration</span></span>](../api/intune-mam-targetedmanagedappconfiguration-delete.md)|<span data-ttu-id="9805b-122">无</span><span class="sxs-lookup"><span data-stu-id="9805b-122">None</span></span>|<span data-ttu-id="9805b-123">删除 [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="9805b-123">Deletes a [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md).</span></span>|
|[<span data-ttu-id="9805b-124">Update targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="9805b-124">Update targetedManagedAppConfiguration</span></span>](../api/intune-mam-targetedmanagedappconfiguration-update.md)|[<span data-ttu-id="9805b-125">targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="9805b-125">targetedManagedAppConfiguration</span></span>](../resources/intune-mam-targetedmanagedappconfiguration.md)|<span data-ttu-id="9805b-126">更新 [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="9805b-126">Update the properties of a [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>|
|[<span data-ttu-id="9805b-127">assign 操作</span><span class="sxs-lookup"><span data-stu-id="9805b-127">assign action</span></span>](../api/intune-mam-targetedmanagedappconfiguration-assign.md)|<span data-ttu-id="9805b-128">无</span><span class="sxs-lookup"><span data-stu-id="9805b-128">None</span></span>|<span data-ttu-id="9805b-129">尚未记录</span><span class="sxs-lookup"><span data-stu-id="9805b-129">Not yet documented</span></span>|
|[<span data-ttu-id="9805b-130">targetApps 操作</span><span class="sxs-lookup"><span data-stu-id="9805b-130">targetApps action</span></span>](../api/intune-mam-targetedmanagedappconfiguration-targetapps.md)|<span data-ttu-id="9805b-131">无</span><span class="sxs-lookup"><span data-stu-id="9805b-131">None</span></span>|<span data-ttu-id="9805b-132">尚未记录</span><span class="sxs-lookup"><span data-stu-id="9805b-132">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="9805b-133">属性</span><span class="sxs-lookup"><span data-stu-id="9805b-133">Properties</span></span>
|<span data-ttu-id="9805b-134">属性</span><span class="sxs-lookup"><span data-stu-id="9805b-134">Property</span></span>|<span data-ttu-id="9805b-135">类型</span><span class="sxs-lookup"><span data-stu-id="9805b-135">Type</span></span>|<span data-ttu-id="9805b-136">说明</span><span class="sxs-lookup"><span data-stu-id="9805b-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9805b-137">displayName</span><span class="sxs-lookup"><span data-stu-id="9805b-137">displayName</span></span>|<span data-ttu-id="9805b-138">字符串</span><span class="sxs-lookup"><span data-stu-id="9805b-138">String</span></span>|<span data-ttu-id="9805b-139">策略显示名称。</span><span class="sxs-lookup"><span data-stu-id="9805b-139">Policy display name.</span></span> <span data-ttu-id="9805b-140">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9805b-140">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="9805b-141">说明</span><span class="sxs-lookup"><span data-stu-id="9805b-141">description</span></span>|<span data-ttu-id="9805b-142">String</span><span class="sxs-lookup"><span data-stu-id="9805b-142">String</span></span>|<span data-ttu-id="9805b-143">策略的说明。</span><span class="sxs-lookup"><span data-stu-id="9805b-143">The policy's description.</span></span> <span data-ttu-id="9805b-144">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9805b-144">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="9805b-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9805b-145">createdDateTime</span></span>|<span data-ttu-id="9805b-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9805b-146">DateTimeOffset</span></span>|<span data-ttu-id="9805b-147">创建策略的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="9805b-147">The date and time the policy was created.</span></span> <span data-ttu-id="9805b-148">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9805b-148">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="9805b-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9805b-149">lastModifiedDateTime</span></span>|<span data-ttu-id="9805b-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9805b-150">DateTimeOffset</span></span>|<span data-ttu-id="9805b-151">上次修改策略的时间。</span><span class="sxs-lookup"><span data-stu-id="9805b-151">Last time the policy was modified.</span></span> <span data-ttu-id="9805b-152">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9805b-152">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="9805b-153">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="9805b-153">roleScopeTagIds</span></span>|<span data-ttu-id="9805b-154">String collection</span><span class="sxs-lookup"><span data-stu-id="9805b-154">String collection</span></span>|<span data-ttu-id="9805b-155">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="9805b-155">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="9805b-156">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9805b-156">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="9805b-157">id</span><span class="sxs-lookup"><span data-stu-id="9805b-157">id</span></span>|<span data-ttu-id="9805b-158">字符串</span><span class="sxs-lookup"><span data-stu-id="9805b-158">String</span></span>|<span data-ttu-id="9805b-159">实体的键。</span><span class="sxs-lookup"><span data-stu-id="9805b-159">Key of the entity.</span></span> <span data-ttu-id="9805b-160">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9805b-160">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="9805b-161">version</span><span class="sxs-lookup"><span data-stu-id="9805b-161">version</span></span>|<span data-ttu-id="9805b-162">String</span><span class="sxs-lookup"><span data-stu-id="9805b-162">String</span></span>|<span data-ttu-id="9805b-163">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="9805b-163">Version of the entity.</span></span> <span data-ttu-id="9805b-164">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9805b-164">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="9805b-165">customSettings</span><span class="sxs-lookup"><span data-stu-id="9805b-165">customSettings</span></span>|<span data-ttu-id="9805b-166">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9805b-166">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="9805b-167">要发送到配置范围确定的用户应用的一组字符串键和字符串值对，不由此服务更改。继承自 [ managedAppConfiguration ](../resources/intune-mam-managedappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9805b-167">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service Inherited from [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span></span>|
|<span data-ttu-id="9805b-168">deployedAppCount</span><span class="sxs-lookup"><span data-stu-id="9805b-168">deployedAppCount</span></span>|<span data-ttu-id="9805b-169">Int32</span><span class="sxs-lookup"><span data-stu-id="9805b-169">Int32</span></span>|<span data-ttu-id="9805b-170">当前策略部署到的应用的计数。</span><span class="sxs-lookup"><span data-stu-id="9805b-170">Count of apps to which the current policy is deployed.</span></span>|
|<span data-ttu-id="9805b-171">isAssigned</span><span class="sxs-lookup"><span data-stu-id="9805b-171">isAssigned</span></span>|<span data-ttu-id="9805b-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="9805b-172">Boolean</span></span>|<span data-ttu-id="9805b-173">指示策略是否部署到任何包含组。</span><span class="sxs-lookup"><span data-stu-id="9805b-173">Indicates if the policy is deployed to any inclusion groups or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9805b-174">关系</span><span class="sxs-lookup"><span data-stu-id="9805b-174">Relationships</span></span>
|<span data-ttu-id="9805b-175">关系</span><span class="sxs-lookup"><span data-stu-id="9805b-175">Relationship</span></span>|<span data-ttu-id="9805b-176">类型</span><span class="sxs-lookup"><span data-stu-id="9805b-176">Type</span></span>|<span data-ttu-id="9805b-177">说明</span><span class="sxs-lookup"><span data-stu-id="9805b-177">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9805b-178">apps</span><span class="sxs-lookup"><span data-stu-id="9805b-178">apps</span></span>|<span data-ttu-id="9805b-179">[managedMobileApp](../resources/intune-mam-managedmobileapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9805b-179">[managedMobileApp](../resources/intune-mam-managedmobileapp.md) collection</span></span>|<span data-ttu-id="9805b-180">策略部署到的应用的列表。</span><span class="sxs-lookup"><span data-stu-id="9805b-180">List of apps to which the policy is deployed.</span></span>|
|<span data-ttu-id="9805b-181">deploymentSummary</span><span class="sxs-lookup"><span data-stu-id="9805b-181">deploymentSummary</span></span>|[<span data-ttu-id="9805b-182">managedAppPolicyDeploymentSummary</span><span class="sxs-lookup"><span data-stu-id="9805b-182">managedAppPolicyDeploymentSummary</span></span>](../resources/intune-mam-managedapppolicydeploymentsummary.md)|<span data-ttu-id="9805b-183">配置的部署摘要的导航属性。</span><span class="sxs-lookup"><span data-stu-id="9805b-183">Navigation property to deployment summary of the configuration.</span></span>|
|<span data-ttu-id="9805b-184">assignments</span><span class="sxs-lookup"><span data-stu-id="9805b-184">assignments</span></span>|<span data-ttu-id="9805b-185">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9805b-185">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) collection</span></span>|<span data-ttu-id="9805b-186">策略部署到的包含组和排除组列表的导航属性。</span><span class="sxs-lookup"><span data-stu-id="9805b-186">Navigation property to list of inclusion and exclusion groups to which the policy is deployed.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9805b-187">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9805b-187">JSON Representation</span></span>
<span data-ttu-id="9805b-188">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9805b-188">Here is a JSON representation of the resource.</span></span>
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





---
title: targetedManagedAppConfiguration 资源类型
description: 用于将一组自定义设置按原样提供给目标安全组中的所有用户的配置
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6f3e04425dbde85b708379f4aea60a7240ff8b79
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37360473"
---
# <a name="targetedmanagedappconfiguration-resource-type"></a><span data-ttu-id="ebacb-103">targetedManagedAppConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="ebacb-103">targetedManagedAppConfiguration resource type</span></span>

> <span data-ttu-id="ebacb-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ebacb-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ebacb-105">用于将一组自定义设置按原样提供给目标安全组中的所有用户的配置</span><span class="sxs-lookup"><span data-stu-id="ebacb-105">Configuration used to deliver a set of custom settings as-is to all users in the targeted security group</span></span>


<span data-ttu-id="ebacb-106">继承自 [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ebacb-106">Inherits from [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="ebacb-107">方法</span><span class="sxs-lookup"><span data-stu-id="ebacb-107">Methods</span></span>
|<span data-ttu-id="ebacb-108">方法</span><span class="sxs-lookup"><span data-stu-id="ebacb-108">Method</span></span>|<span data-ttu-id="ebacb-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="ebacb-109">Return Type</span></span>|<span data-ttu-id="ebacb-110">说明</span><span class="sxs-lookup"><span data-stu-id="ebacb-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ebacb-111">List targetedManagedAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="ebacb-111">List targetedManagedAppConfigurations</span></span>](../api/intune-mam-targetedmanagedappconfiguration-list.md)|<span data-ttu-id="ebacb-112">[targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ebacb-112">[targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) collection</span></span>|<span data-ttu-id="ebacb-113">列出 [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ebacb-113">List properties and relationships of the [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="ebacb-114">Get targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="ebacb-114">Get targetedManagedAppConfiguration</span></span>](../api/intune-mam-targetedmanagedappconfiguration-get.md)|[<span data-ttu-id="ebacb-115">targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="ebacb-115">targetedManagedAppConfiguration</span></span>](../resources/intune-mam-targetedmanagedappconfiguration.md)|<span data-ttu-id="ebacb-116">读取 [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ebacb-116">Read properties and relationships of the [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>|
|[<span data-ttu-id="ebacb-117">Create targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="ebacb-117">Create targetedManagedAppConfiguration</span></span>](../api/intune-mam-targetedmanagedappconfiguration-create.md)|[<span data-ttu-id="ebacb-118">targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="ebacb-118">targetedManagedAppConfiguration</span></span>](../resources/intune-mam-targetedmanagedappconfiguration.md)|<span data-ttu-id="ebacb-119">创建新的 [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ebacb-119">Create a new [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>|
|[<span data-ttu-id="ebacb-120">Delete targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="ebacb-120">Delete targetedManagedAppConfiguration</span></span>](../api/intune-mam-targetedmanagedappconfiguration-delete.md)|<span data-ttu-id="ebacb-121">无</span><span class="sxs-lookup"><span data-stu-id="ebacb-121">None</span></span>|<span data-ttu-id="ebacb-122">删除 [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="ebacb-122">Deletes a [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md).</span></span>|
|[<span data-ttu-id="ebacb-123">Update targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="ebacb-123">Update targetedManagedAppConfiguration</span></span>](../api/intune-mam-targetedmanagedappconfiguration-update.md)|[<span data-ttu-id="ebacb-124">targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="ebacb-124">targetedManagedAppConfiguration</span></span>](../resources/intune-mam-targetedmanagedappconfiguration.md)|<span data-ttu-id="ebacb-125">更新 [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="ebacb-125">Update the properties of a [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>|
|[<span data-ttu-id="ebacb-126">assign 操作</span><span class="sxs-lookup"><span data-stu-id="ebacb-126">assign action</span></span>](../api/intune-mam-targetedmanagedappconfiguration-assign.md)|<span data-ttu-id="ebacb-127">无</span><span class="sxs-lookup"><span data-stu-id="ebacb-127">None</span></span>|<span data-ttu-id="ebacb-128">尚未记录</span><span class="sxs-lookup"><span data-stu-id="ebacb-128">Not yet documented</span></span>|
|[<span data-ttu-id="ebacb-129">targetApps 操作</span><span class="sxs-lookup"><span data-stu-id="ebacb-129">targetApps action</span></span>](../api/intune-mam-targetedmanagedappconfiguration-targetapps.md)|<span data-ttu-id="ebacb-130">无</span><span class="sxs-lookup"><span data-stu-id="ebacb-130">None</span></span>|<span data-ttu-id="ebacb-131">尚未记录</span><span class="sxs-lookup"><span data-stu-id="ebacb-131">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="ebacb-132">属性</span><span class="sxs-lookup"><span data-stu-id="ebacb-132">Properties</span></span>
|<span data-ttu-id="ebacb-133">属性</span><span class="sxs-lookup"><span data-stu-id="ebacb-133">Property</span></span>|<span data-ttu-id="ebacb-134">类型</span><span class="sxs-lookup"><span data-stu-id="ebacb-134">Type</span></span>|<span data-ttu-id="ebacb-135">说明</span><span class="sxs-lookup"><span data-stu-id="ebacb-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ebacb-136">displayName</span><span class="sxs-lookup"><span data-stu-id="ebacb-136">displayName</span></span>|<span data-ttu-id="ebacb-137">字符串</span><span class="sxs-lookup"><span data-stu-id="ebacb-137">String</span></span>|<span data-ttu-id="ebacb-138">策略显示名称。</span><span class="sxs-lookup"><span data-stu-id="ebacb-138">Policy display name.</span></span> <span data-ttu-id="ebacb-139">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="ebacb-139">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="ebacb-140">说明</span><span class="sxs-lookup"><span data-stu-id="ebacb-140">description</span></span>|<span data-ttu-id="ebacb-141">String</span><span class="sxs-lookup"><span data-stu-id="ebacb-141">String</span></span>|<span data-ttu-id="ebacb-142">策略的说明。</span><span class="sxs-lookup"><span data-stu-id="ebacb-142">The policy's description.</span></span> <span data-ttu-id="ebacb-143">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="ebacb-143">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="ebacb-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ebacb-144">createdDateTime</span></span>|<span data-ttu-id="ebacb-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ebacb-145">DateTimeOffset</span></span>|<span data-ttu-id="ebacb-146">创建策略的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="ebacb-146">The date and time the policy was created.</span></span> <span data-ttu-id="ebacb-147">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="ebacb-147">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="ebacb-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ebacb-148">lastModifiedDateTime</span></span>|<span data-ttu-id="ebacb-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ebacb-149">DateTimeOffset</span></span>|<span data-ttu-id="ebacb-150">上次修改策略的时间。</span><span class="sxs-lookup"><span data-stu-id="ebacb-150">Last time the policy was modified.</span></span> <span data-ttu-id="ebacb-151">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="ebacb-151">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="ebacb-152">id</span><span class="sxs-lookup"><span data-stu-id="ebacb-152">id</span></span>|<span data-ttu-id="ebacb-153">字符串</span><span class="sxs-lookup"><span data-stu-id="ebacb-153">String</span></span>|<span data-ttu-id="ebacb-154">实体的键。</span><span class="sxs-lookup"><span data-stu-id="ebacb-154">Key of the entity.</span></span> <span data-ttu-id="ebacb-155">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="ebacb-155">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="ebacb-156">version</span><span class="sxs-lookup"><span data-stu-id="ebacb-156">version</span></span>|<span data-ttu-id="ebacb-157">String</span><span class="sxs-lookup"><span data-stu-id="ebacb-157">String</span></span>|<span data-ttu-id="ebacb-158">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="ebacb-158">Version of the entity.</span></span> <span data-ttu-id="ebacb-159">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="ebacb-159">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="ebacb-160">customSettings</span><span class="sxs-lookup"><span data-stu-id="ebacb-160">customSettings</span></span>|<span data-ttu-id="ebacb-161">[keyValuePair](../resources/intune-mam-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ebacb-161">[keyValuePair](../resources/intune-mam-keyvaluepair.md) collection</span></span>|<span data-ttu-id="ebacb-162">要发送到配置范围确定的用户应用的一组字符串键和字符串值对，不由此服务更改。继承自 [ managedAppConfiguration ](../resources/intune-mam-managedappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ebacb-162">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service Inherited from [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span></span>|
|<span data-ttu-id="ebacb-163">deployedAppCount</span><span class="sxs-lookup"><span data-stu-id="ebacb-163">deployedAppCount</span></span>|<span data-ttu-id="ebacb-164">Int32</span><span class="sxs-lookup"><span data-stu-id="ebacb-164">Int32</span></span>|<span data-ttu-id="ebacb-165">当前策略部署到的应用的计数。</span><span class="sxs-lookup"><span data-stu-id="ebacb-165">Count of apps to which the current policy is deployed.</span></span>|
|<span data-ttu-id="ebacb-166">isAssigned</span><span class="sxs-lookup"><span data-stu-id="ebacb-166">isAssigned</span></span>|<span data-ttu-id="ebacb-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="ebacb-167">Boolean</span></span>|<span data-ttu-id="ebacb-168">指示策略是否部署到任何包含组。</span><span class="sxs-lookup"><span data-stu-id="ebacb-168">Indicates if the policy is deployed to any inclusion groups or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ebacb-169">关系</span><span class="sxs-lookup"><span data-stu-id="ebacb-169">Relationships</span></span>
|<span data-ttu-id="ebacb-170">关系</span><span class="sxs-lookup"><span data-stu-id="ebacb-170">Relationship</span></span>|<span data-ttu-id="ebacb-171">类型</span><span class="sxs-lookup"><span data-stu-id="ebacb-171">Type</span></span>|<span data-ttu-id="ebacb-172">说明</span><span class="sxs-lookup"><span data-stu-id="ebacb-172">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ebacb-173">apps</span><span class="sxs-lookup"><span data-stu-id="ebacb-173">apps</span></span>|<span data-ttu-id="ebacb-174">[managedMobileApp](../resources/intune-mam-managedmobileapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ebacb-174">[managedMobileApp](../resources/intune-mam-managedmobileapp.md) collection</span></span>|<span data-ttu-id="ebacb-175">策略部署到的应用的列表。</span><span class="sxs-lookup"><span data-stu-id="ebacb-175">List of apps to which the policy is deployed.</span></span>|
|<span data-ttu-id="ebacb-176">deploymentSummary</span><span class="sxs-lookup"><span data-stu-id="ebacb-176">deploymentSummary</span></span>|[<span data-ttu-id="ebacb-177">managedAppPolicyDeploymentSummary</span><span class="sxs-lookup"><span data-stu-id="ebacb-177">managedAppPolicyDeploymentSummary</span></span>](../resources/intune-mam-managedapppolicydeploymentsummary.md)|<span data-ttu-id="ebacb-178">配置的部署摘要的导航属性。</span><span class="sxs-lookup"><span data-stu-id="ebacb-178">Navigation property to deployment summary of the configuration.</span></span>|
|<span data-ttu-id="ebacb-179">assignments</span><span class="sxs-lookup"><span data-stu-id="ebacb-179">assignments</span></span>|<span data-ttu-id="ebacb-180">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ebacb-180">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) collection</span></span>|<span data-ttu-id="ebacb-181">策略部署到的包含组和排除组列表的导航属性。</span><span class="sxs-lookup"><span data-stu-id="ebacb-181">Navigation property to list of inclusion and exclusion groups to which the policy is deployed.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ebacb-182">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ebacb-182">JSON Representation</span></span>
<span data-ttu-id="ebacb-183">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ebacb-183">Here is a JSON representation of the resource.</span></span>
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





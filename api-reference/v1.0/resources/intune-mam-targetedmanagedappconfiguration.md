---
title: targetedManagedAppConfiguration 资源类型
description: 用于将一组自定义设置按原样提供给目标安全组中的所有用户的配置
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a39026b86a9c63012ba1d30090cd8f34b6bfb0ef
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52751641"
---
# <a name="targetedmanagedappconfiguration-resource-type"></a><span data-ttu-id="bc55e-103">targetedManagedAppConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="bc55e-103">targetedManagedAppConfiguration resource type</span></span>

<span data-ttu-id="bc55e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bc55e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bc55e-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="bc55e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bc55e-106">用于将一组自定义设置按原样提供给目标安全组中的所有用户的配置</span><span class="sxs-lookup"><span data-stu-id="bc55e-106">Configuration used to deliver a set of custom settings as-is to all users in the targeted security group</span></span>


<span data-ttu-id="bc55e-107">继承自 [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bc55e-107">Inherits from [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="bc55e-108">Methods</span><span class="sxs-lookup"><span data-stu-id="bc55e-108">Methods</span></span>
|<span data-ttu-id="bc55e-109">方法</span><span class="sxs-lookup"><span data-stu-id="bc55e-109">Method</span></span>|<span data-ttu-id="bc55e-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="bc55e-110">Return Type</span></span>|<span data-ttu-id="bc55e-111">Description</span><span class="sxs-lookup"><span data-stu-id="bc55e-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="bc55e-112">List targetedManagedAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="bc55e-112">List targetedManagedAppConfigurations</span></span>](../api/intune-mam-targetedmanagedappconfiguration-list.md)|<span data-ttu-id="bc55e-113">[targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="bc55e-113">[targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) collection</span></span>|<span data-ttu-id="bc55e-114">列出 [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="bc55e-114">List properties and relationships of the [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="bc55e-115">Get targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="bc55e-115">Get targetedManagedAppConfiguration</span></span>](../api/intune-mam-targetedmanagedappconfiguration-get.md)|[<span data-ttu-id="bc55e-116">targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="bc55e-116">targetedManagedAppConfiguration</span></span>](../resources/intune-mam-targetedmanagedappconfiguration.md)|<span data-ttu-id="bc55e-117">读取 [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="bc55e-117">Read properties and relationships of the [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>|
|[<span data-ttu-id="bc55e-118">Create targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="bc55e-118">Create targetedManagedAppConfiguration</span></span>](../api/intune-mam-targetedmanagedappconfiguration-create.md)|[<span data-ttu-id="bc55e-119">targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="bc55e-119">targetedManagedAppConfiguration</span></span>](../resources/intune-mam-targetedmanagedappconfiguration.md)|<span data-ttu-id="bc55e-120">创建新的 [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="bc55e-120">Create a new [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>|
|[<span data-ttu-id="bc55e-121">Delete targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="bc55e-121">Delete targetedManagedAppConfiguration</span></span>](../api/intune-mam-targetedmanagedappconfiguration-delete.md)|<span data-ttu-id="bc55e-122">无</span><span class="sxs-lookup"><span data-stu-id="bc55e-122">None</span></span>|<span data-ttu-id="bc55e-123">删除 [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="bc55e-123">Deletes a [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md).</span></span>|
|[<span data-ttu-id="bc55e-124">Update targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="bc55e-124">Update targetedManagedAppConfiguration</span></span>](../api/intune-mam-targetedmanagedappconfiguration-update.md)|[<span data-ttu-id="bc55e-125">targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="bc55e-125">targetedManagedAppConfiguration</span></span>](../resources/intune-mam-targetedmanagedappconfiguration.md)|<span data-ttu-id="bc55e-126">更新 [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="bc55e-126">Update the properties of a [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>|
|[<span data-ttu-id="bc55e-127">assign 操作</span><span class="sxs-lookup"><span data-stu-id="bc55e-127">assign action</span></span>](../api/intune-mam-targetedmanagedappconfiguration-assign.md)|<span data-ttu-id="bc55e-128">无</span><span class="sxs-lookup"><span data-stu-id="bc55e-128">None</span></span>|<span data-ttu-id="bc55e-129">尚未记录</span><span class="sxs-lookup"><span data-stu-id="bc55e-129">Not yet documented</span></span>|
|[<span data-ttu-id="bc55e-130">targetApps 操作</span><span class="sxs-lookup"><span data-stu-id="bc55e-130">targetApps action</span></span>](../api/intune-mam-targetedmanagedappconfiguration-targetapps.md)|<span data-ttu-id="bc55e-131">无</span><span class="sxs-lookup"><span data-stu-id="bc55e-131">None</span></span>|<span data-ttu-id="bc55e-132">尚未记录</span><span class="sxs-lookup"><span data-stu-id="bc55e-132">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="bc55e-133">属性</span><span class="sxs-lookup"><span data-stu-id="bc55e-133">Properties</span></span>
|<span data-ttu-id="bc55e-134">属性</span><span class="sxs-lookup"><span data-stu-id="bc55e-134">Property</span></span>|<span data-ttu-id="bc55e-135">类型</span><span class="sxs-lookup"><span data-stu-id="bc55e-135">Type</span></span>|<span data-ttu-id="bc55e-136">说明</span><span class="sxs-lookup"><span data-stu-id="bc55e-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bc55e-137">displayName</span><span class="sxs-lookup"><span data-stu-id="bc55e-137">displayName</span></span>|<span data-ttu-id="bc55e-138">String</span><span class="sxs-lookup"><span data-stu-id="bc55e-138">String</span></span>|<span data-ttu-id="bc55e-139">策略显示名称。</span><span class="sxs-lookup"><span data-stu-id="bc55e-139">Policy display name.</span></span> <span data-ttu-id="bc55e-140">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="bc55e-140">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="bc55e-141">说明</span><span class="sxs-lookup"><span data-stu-id="bc55e-141">description</span></span>|<span data-ttu-id="bc55e-142">String</span><span class="sxs-lookup"><span data-stu-id="bc55e-142">String</span></span>|<span data-ttu-id="bc55e-143">策略的说明。</span><span class="sxs-lookup"><span data-stu-id="bc55e-143">The policy's description.</span></span> <span data-ttu-id="bc55e-144">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="bc55e-144">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="bc55e-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bc55e-145">createdDateTime</span></span>|<span data-ttu-id="bc55e-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bc55e-146">DateTimeOffset</span></span>|<span data-ttu-id="bc55e-147">创建策略的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="bc55e-147">The date and time the policy was created.</span></span> <span data-ttu-id="bc55e-148">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="bc55e-148">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="bc55e-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bc55e-149">lastModifiedDateTime</span></span>|<span data-ttu-id="bc55e-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bc55e-150">DateTimeOffset</span></span>|<span data-ttu-id="bc55e-151">上次修改策略的时间。</span><span class="sxs-lookup"><span data-stu-id="bc55e-151">Last time the policy was modified.</span></span> <span data-ttu-id="bc55e-152">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="bc55e-152">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="bc55e-153">id</span><span class="sxs-lookup"><span data-stu-id="bc55e-153">id</span></span>|<span data-ttu-id="bc55e-154">String</span><span class="sxs-lookup"><span data-stu-id="bc55e-154">String</span></span>|<span data-ttu-id="bc55e-155">实体的键。</span><span class="sxs-lookup"><span data-stu-id="bc55e-155">Key of the entity.</span></span> <span data-ttu-id="bc55e-156">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="bc55e-156">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="bc55e-157">version</span><span class="sxs-lookup"><span data-stu-id="bc55e-157">version</span></span>|<span data-ttu-id="bc55e-158">String</span><span class="sxs-lookup"><span data-stu-id="bc55e-158">String</span></span>|<span data-ttu-id="bc55e-159">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="bc55e-159">Version of the entity.</span></span> <span data-ttu-id="bc55e-160">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="bc55e-160">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="bc55e-161">customSettings</span><span class="sxs-lookup"><span data-stu-id="bc55e-161">customSettings</span></span>|<span data-ttu-id="bc55e-162">[keyValuePair](../resources/intune-mam-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="bc55e-162">[keyValuePair](../resources/intune-mam-keyvaluepair.md) collection</span></span>|<span data-ttu-id="bc55e-163">要发送到配置范围确定的用户应用的一组字符串键和字符串值对，不由此服务更改。继承自 [ managedAppConfiguration ](../resources/intune-mam-managedappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bc55e-163">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service Inherited from [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span></span>|
|<span data-ttu-id="bc55e-164">deployedAppCount</span><span class="sxs-lookup"><span data-stu-id="bc55e-164">deployedAppCount</span></span>|<span data-ttu-id="bc55e-165">Int32</span><span class="sxs-lookup"><span data-stu-id="bc55e-165">Int32</span></span>|<span data-ttu-id="bc55e-166">当前策略部署到的应用的计数。</span><span class="sxs-lookup"><span data-stu-id="bc55e-166">Count of apps to which the current policy is deployed.</span></span>|
|<span data-ttu-id="bc55e-167">isAssigned</span><span class="sxs-lookup"><span data-stu-id="bc55e-167">isAssigned</span></span>|<span data-ttu-id="bc55e-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc55e-168">Boolean</span></span>|<span data-ttu-id="bc55e-169">指示策略是否部署到任何包含组。</span><span class="sxs-lookup"><span data-stu-id="bc55e-169">Indicates if the policy is deployed to any inclusion groups or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bc55e-170">关系</span><span class="sxs-lookup"><span data-stu-id="bc55e-170">Relationships</span></span>
|<span data-ttu-id="bc55e-171">关系</span><span class="sxs-lookup"><span data-stu-id="bc55e-171">Relationship</span></span>|<span data-ttu-id="bc55e-172">类型</span><span class="sxs-lookup"><span data-stu-id="bc55e-172">Type</span></span>|<span data-ttu-id="bc55e-173">说明</span><span class="sxs-lookup"><span data-stu-id="bc55e-173">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bc55e-174">apps</span><span class="sxs-lookup"><span data-stu-id="bc55e-174">apps</span></span>|<span data-ttu-id="bc55e-175">[managedMobileApp](../resources/intune-mam-managedmobileapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="bc55e-175">[managedMobileApp](../resources/intune-mam-managedmobileapp.md) collection</span></span>|<span data-ttu-id="bc55e-176">策略部署到的应用的列表。</span><span class="sxs-lookup"><span data-stu-id="bc55e-176">List of apps to which the policy is deployed.</span></span>|
|<span data-ttu-id="bc55e-177">deploymentSummary</span><span class="sxs-lookup"><span data-stu-id="bc55e-177">deploymentSummary</span></span>|[<span data-ttu-id="bc55e-178">managedAppPolicyDeploymentSummary</span><span class="sxs-lookup"><span data-stu-id="bc55e-178">managedAppPolicyDeploymentSummary</span></span>](../resources/intune-mam-managedapppolicydeploymentsummary.md)|<span data-ttu-id="bc55e-179">配置的部署摘要的导航属性。</span><span class="sxs-lookup"><span data-stu-id="bc55e-179">Navigation property to deployment summary of the configuration.</span></span>|
|<span data-ttu-id="bc55e-180">assignments</span><span class="sxs-lookup"><span data-stu-id="bc55e-180">assignments</span></span>|<span data-ttu-id="bc55e-181">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="bc55e-181">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) collection</span></span>|<span data-ttu-id="bc55e-182">策略部署到的包含组和排除组列表的导航属性。</span><span class="sxs-lookup"><span data-stu-id="bc55e-182">Navigation property to list of inclusion and exclusion groups to which the policy is deployed.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bc55e-183">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bc55e-183">JSON Representation</span></span>
<span data-ttu-id="bc55e-184">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bc55e-184">Here is a JSON representation of the resource.</span></span>
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





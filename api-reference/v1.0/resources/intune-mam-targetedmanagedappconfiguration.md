---
title: targetedManagedAppConfiguration 资源类型
description: 用于将一组自定义设置按原样提供给目标安全组中的所有用户的配置
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5d650cbfc96c3382671fec8d92e88c92200adaa8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48048342"
---
# <a name="targetedmanagedappconfiguration-resource-type"></a><span data-ttu-id="c88f7-103">targetedManagedAppConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="c88f7-103">targetedManagedAppConfiguration resource type</span></span>

<span data-ttu-id="c88f7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c88f7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c88f7-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c88f7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c88f7-106">用于将一组自定义设置按原样提供给目标安全组中的所有用户的配置</span><span class="sxs-lookup"><span data-stu-id="c88f7-106">Configuration used to deliver a set of custom settings as-is to all users in the targeted security group</span></span>


<span data-ttu-id="c88f7-107">继承自 [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c88f7-107">Inherits from [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="c88f7-108">方法</span><span class="sxs-lookup"><span data-stu-id="c88f7-108">Methods</span></span>
|<span data-ttu-id="c88f7-109">方法</span><span class="sxs-lookup"><span data-stu-id="c88f7-109">Method</span></span>|<span data-ttu-id="c88f7-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="c88f7-110">Return Type</span></span>|<span data-ttu-id="c88f7-111">说明</span><span class="sxs-lookup"><span data-stu-id="c88f7-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c88f7-112">List targetedManagedAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="c88f7-112">List targetedManagedAppConfigurations</span></span>](../api/intune-mam-targetedmanagedappconfiguration-list.md)|<span data-ttu-id="c88f7-113">[targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c88f7-113">[targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) collection</span></span>|<span data-ttu-id="c88f7-114">列出 [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c88f7-114">List properties and relationships of the [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="c88f7-115">Get targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="c88f7-115">Get targetedManagedAppConfiguration</span></span>](../api/intune-mam-targetedmanagedappconfiguration-get.md)|[<span data-ttu-id="c88f7-116">targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="c88f7-116">targetedManagedAppConfiguration</span></span>](../resources/intune-mam-targetedmanagedappconfiguration.md)|<span data-ttu-id="c88f7-117">读取 [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c88f7-117">Read properties and relationships of the [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>|
|[<span data-ttu-id="c88f7-118">Create targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="c88f7-118">Create targetedManagedAppConfiguration</span></span>](../api/intune-mam-targetedmanagedappconfiguration-create.md)|[<span data-ttu-id="c88f7-119">targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="c88f7-119">targetedManagedAppConfiguration</span></span>](../resources/intune-mam-targetedmanagedappconfiguration.md)|<span data-ttu-id="c88f7-120">创建新的 [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c88f7-120">Create a new [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>|
|[<span data-ttu-id="c88f7-121">Delete targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="c88f7-121">Delete targetedManagedAppConfiguration</span></span>](../api/intune-mam-targetedmanagedappconfiguration-delete.md)|<span data-ttu-id="c88f7-122">无</span><span class="sxs-lookup"><span data-stu-id="c88f7-122">None</span></span>|<span data-ttu-id="c88f7-123">删除 [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="c88f7-123">Deletes a [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md).</span></span>|
|[<span data-ttu-id="c88f7-124">Update targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="c88f7-124">Update targetedManagedAppConfiguration</span></span>](../api/intune-mam-targetedmanagedappconfiguration-update.md)|[<span data-ttu-id="c88f7-125">targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="c88f7-125">targetedManagedAppConfiguration</span></span>](../resources/intune-mam-targetedmanagedappconfiguration.md)|<span data-ttu-id="c88f7-126">更新 [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="c88f7-126">Update the properties of a [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>|
|[<span data-ttu-id="c88f7-127">assign 操作</span><span class="sxs-lookup"><span data-stu-id="c88f7-127">assign action</span></span>](../api/intune-mam-targetedmanagedappconfiguration-assign.md)|<span data-ttu-id="c88f7-128">无</span><span class="sxs-lookup"><span data-stu-id="c88f7-128">None</span></span>|<span data-ttu-id="c88f7-129">尚未记录</span><span class="sxs-lookup"><span data-stu-id="c88f7-129">Not yet documented</span></span>|
|[<span data-ttu-id="c88f7-130">targetApps 操作</span><span class="sxs-lookup"><span data-stu-id="c88f7-130">targetApps action</span></span>](../api/intune-mam-targetedmanagedappconfiguration-targetapps.md)|<span data-ttu-id="c88f7-131">无</span><span class="sxs-lookup"><span data-stu-id="c88f7-131">None</span></span>|<span data-ttu-id="c88f7-132">尚未记录</span><span class="sxs-lookup"><span data-stu-id="c88f7-132">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="c88f7-133">属性</span><span class="sxs-lookup"><span data-stu-id="c88f7-133">Properties</span></span>
|<span data-ttu-id="c88f7-134">属性</span><span class="sxs-lookup"><span data-stu-id="c88f7-134">Property</span></span>|<span data-ttu-id="c88f7-135">类型</span><span class="sxs-lookup"><span data-stu-id="c88f7-135">Type</span></span>|<span data-ttu-id="c88f7-136">说明</span><span class="sxs-lookup"><span data-stu-id="c88f7-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c88f7-137">displayName</span><span class="sxs-lookup"><span data-stu-id="c88f7-137">displayName</span></span>|<span data-ttu-id="c88f7-138">String</span><span class="sxs-lookup"><span data-stu-id="c88f7-138">String</span></span>|<span data-ttu-id="c88f7-139">策略显示名称。</span><span class="sxs-lookup"><span data-stu-id="c88f7-139">Policy display name.</span></span> <span data-ttu-id="c88f7-140">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="c88f7-140">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="c88f7-141">description</span><span class="sxs-lookup"><span data-stu-id="c88f7-141">description</span></span>|<span data-ttu-id="c88f7-142">String</span><span class="sxs-lookup"><span data-stu-id="c88f7-142">String</span></span>|<span data-ttu-id="c88f7-143">策略的说明。</span><span class="sxs-lookup"><span data-stu-id="c88f7-143">The policy's description.</span></span> <span data-ttu-id="c88f7-144">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="c88f7-144">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="c88f7-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c88f7-145">createdDateTime</span></span>|<span data-ttu-id="c88f7-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c88f7-146">DateTimeOffset</span></span>|<span data-ttu-id="c88f7-147">创建策略的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="c88f7-147">The date and time the policy was created.</span></span> <span data-ttu-id="c88f7-148">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="c88f7-148">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="c88f7-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c88f7-149">lastModifiedDateTime</span></span>|<span data-ttu-id="c88f7-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c88f7-150">DateTimeOffset</span></span>|<span data-ttu-id="c88f7-151">上次修改策略的时间。</span><span class="sxs-lookup"><span data-stu-id="c88f7-151">Last time the policy was modified.</span></span> <span data-ttu-id="c88f7-152">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="c88f7-152">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="c88f7-153">id</span><span class="sxs-lookup"><span data-stu-id="c88f7-153">id</span></span>|<span data-ttu-id="c88f7-154">String</span><span class="sxs-lookup"><span data-stu-id="c88f7-154">String</span></span>|<span data-ttu-id="c88f7-155">实体的键。</span><span class="sxs-lookup"><span data-stu-id="c88f7-155">Key of the entity.</span></span> <span data-ttu-id="c88f7-156">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="c88f7-156">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="c88f7-157">version</span><span class="sxs-lookup"><span data-stu-id="c88f7-157">version</span></span>|<span data-ttu-id="c88f7-158">String</span><span class="sxs-lookup"><span data-stu-id="c88f7-158">String</span></span>|<span data-ttu-id="c88f7-159">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="c88f7-159">Version of the entity.</span></span> <span data-ttu-id="c88f7-160">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="c88f7-160">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="c88f7-161">customSettings</span><span class="sxs-lookup"><span data-stu-id="c88f7-161">customSettings</span></span>|<span data-ttu-id="c88f7-162">[keyValuePair](../resources/intune-mam-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c88f7-162">[keyValuePair](../resources/intune-mam-keyvaluepair.md) collection</span></span>|<span data-ttu-id="c88f7-163">要发送到配置范围确定的用户应用的一组字符串键和字符串值对，不由此服务更改。继承自 [ managedAppConfiguration ](../resources/intune-mam-managedappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c88f7-163">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service Inherited from [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span></span>|
|<span data-ttu-id="c88f7-164">deployedAppCount</span><span class="sxs-lookup"><span data-stu-id="c88f7-164">deployedAppCount</span></span>|<span data-ttu-id="c88f7-165">Int32</span><span class="sxs-lookup"><span data-stu-id="c88f7-165">Int32</span></span>|<span data-ttu-id="c88f7-166">当前策略部署到的应用的计数。</span><span class="sxs-lookup"><span data-stu-id="c88f7-166">Count of apps to which the current policy is deployed.</span></span>|
|<span data-ttu-id="c88f7-167">isAssigned</span><span class="sxs-lookup"><span data-stu-id="c88f7-167">isAssigned</span></span>|<span data-ttu-id="c88f7-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="c88f7-168">Boolean</span></span>|<span data-ttu-id="c88f7-169">指示策略是否部署到任何包含组。</span><span class="sxs-lookup"><span data-stu-id="c88f7-169">Indicates if the policy is deployed to any inclusion groups or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c88f7-170">关系</span><span class="sxs-lookup"><span data-stu-id="c88f7-170">Relationships</span></span>
|<span data-ttu-id="c88f7-171">关系</span><span class="sxs-lookup"><span data-stu-id="c88f7-171">Relationship</span></span>|<span data-ttu-id="c88f7-172">类型</span><span class="sxs-lookup"><span data-stu-id="c88f7-172">Type</span></span>|<span data-ttu-id="c88f7-173">说明</span><span class="sxs-lookup"><span data-stu-id="c88f7-173">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c88f7-174">apps</span><span class="sxs-lookup"><span data-stu-id="c88f7-174">apps</span></span>|<span data-ttu-id="c88f7-175">[managedMobileApp](../resources/intune-mam-managedmobileapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c88f7-175">[managedMobileApp](../resources/intune-mam-managedmobileapp.md) collection</span></span>|<span data-ttu-id="c88f7-176">策略部署到的应用的列表。</span><span class="sxs-lookup"><span data-stu-id="c88f7-176">List of apps to which the policy is deployed.</span></span>|
|<span data-ttu-id="c88f7-177">deploymentSummary</span><span class="sxs-lookup"><span data-stu-id="c88f7-177">deploymentSummary</span></span>|[<span data-ttu-id="c88f7-178">managedAppPolicyDeploymentSummary</span><span class="sxs-lookup"><span data-stu-id="c88f7-178">managedAppPolicyDeploymentSummary</span></span>](../resources/intune-mam-managedapppolicydeploymentsummary.md)|<span data-ttu-id="c88f7-179">配置的部署摘要的导航属性。</span><span class="sxs-lookup"><span data-stu-id="c88f7-179">Navigation property to deployment summary of the configuration.</span></span>|
|<span data-ttu-id="c88f7-180">assignments</span><span class="sxs-lookup"><span data-stu-id="c88f7-180">assignments</span></span>|<span data-ttu-id="c88f7-181">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c88f7-181">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) collection</span></span>|<span data-ttu-id="c88f7-182">策略部署到的包含组和排除组列表的导航属性。</span><span class="sxs-lookup"><span data-stu-id="c88f7-182">Navigation property to list of inclusion and exclusion groups to which the policy is deployed.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c88f7-183">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c88f7-183">JSON Representation</span></span>
<span data-ttu-id="c88f7-184">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c88f7-184">Here is a JSON representation of the resource.</span></span>
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










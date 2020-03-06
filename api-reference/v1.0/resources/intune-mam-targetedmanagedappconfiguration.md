---
title: targetedManagedAppConfiguration 资源类型
description: 用于将一组自定义设置按原样提供给目标安全组中的所有用户的配置
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b366be38543619ceee45990f822412ae4c26d83a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533354"
---
# <a name="targetedmanagedappconfiguration-resource-type"></a><span data-ttu-id="237aa-103">targetedManagedAppConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="237aa-103">targetedManagedAppConfiguration resource type</span></span>

<span data-ttu-id="237aa-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="237aa-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="237aa-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="237aa-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="237aa-106">用于将一组自定义设置按原样提供给目标安全组中的所有用户的配置</span><span class="sxs-lookup"><span data-stu-id="237aa-106">Configuration used to deliver a set of custom settings as-is to all users in the targeted security group</span></span>


<span data-ttu-id="237aa-107">继承自 [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="237aa-107">Inherits from [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="237aa-108">Methods</span><span class="sxs-lookup"><span data-stu-id="237aa-108">Methods</span></span>
|<span data-ttu-id="237aa-109">方法</span><span class="sxs-lookup"><span data-stu-id="237aa-109">Method</span></span>|<span data-ttu-id="237aa-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="237aa-110">Return Type</span></span>|<span data-ttu-id="237aa-111">说明</span><span class="sxs-lookup"><span data-stu-id="237aa-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="237aa-112">List targetedManagedAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="237aa-112">List targetedManagedAppConfigurations</span></span>](../api/intune-mam-targetedmanagedappconfiguration-list.md)|<span data-ttu-id="237aa-113">[targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="237aa-113">[targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) collection</span></span>|<span data-ttu-id="237aa-114">列出 [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="237aa-114">List properties and relationships of the [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="237aa-115">Get targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="237aa-115">Get targetedManagedAppConfiguration</span></span>](../api/intune-mam-targetedmanagedappconfiguration-get.md)|[<span data-ttu-id="237aa-116">targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="237aa-116">targetedManagedAppConfiguration</span></span>](../resources/intune-mam-targetedmanagedappconfiguration.md)|<span data-ttu-id="237aa-117">读取 [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="237aa-117">Read properties and relationships of the [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>|
|[<span data-ttu-id="237aa-118">Create targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="237aa-118">Create targetedManagedAppConfiguration</span></span>](../api/intune-mam-targetedmanagedappconfiguration-create.md)|[<span data-ttu-id="237aa-119">targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="237aa-119">targetedManagedAppConfiguration</span></span>](../resources/intune-mam-targetedmanagedappconfiguration.md)|<span data-ttu-id="237aa-120">创建新的 [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="237aa-120">Create a new [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>|
|[<span data-ttu-id="237aa-121">Delete targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="237aa-121">Delete targetedManagedAppConfiguration</span></span>](../api/intune-mam-targetedmanagedappconfiguration-delete.md)|<span data-ttu-id="237aa-122">无</span><span class="sxs-lookup"><span data-stu-id="237aa-122">None</span></span>|<span data-ttu-id="237aa-123">删除 [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="237aa-123">Deletes a [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md).</span></span>|
|[<span data-ttu-id="237aa-124">Update targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="237aa-124">Update targetedManagedAppConfiguration</span></span>](../api/intune-mam-targetedmanagedappconfiguration-update.md)|[<span data-ttu-id="237aa-125">targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="237aa-125">targetedManagedAppConfiguration</span></span>](../resources/intune-mam-targetedmanagedappconfiguration.md)|<span data-ttu-id="237aa-126">更新 [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="237aa-126">Update the properties of a [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>|
|[<span data-ttu-id="237aa-127">assign 操作</span><span class="sxs-lookup"><span data-stu-id="237aa-127">assign action</span></span>](../api/intune-mam-targetedmanagedappconfiguration-assign.md)|<span data-ttu-id="237aa-128">无</span><span class="sxs-lookup"><span data-stu-id="237aa-128">None</span></span>|<span data-ttu-id="237aa-129">尚未记录</span><span class="sxs-lookup"><span data-stu-id="237aa-129">Not yet documented</span></span>|
|[<span data-ttu-id="237aa-130">targetApps 操作</span><span class="sxs-lookup"><span data-stu-id="237aa-130">targetApps action</span></span>](../api/intune-mam-targetedmanagedappconfiguration-targetapps.md)|<span data-ttu-id="237aa-131">无</span><span class="sxs-lookup"><span data-stu-id="237aa-131">None</span></span>|<span data-ttu-id="237aa-132">尚未记录</span><span class="sxs-lookup"><span data-stu-id="237aa-132">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="237aa-133">属性</span><span class="sxs-lookup"><span data-stu-id="237aa-133">Properties</span></span>
|<span data-ttu-id="237aa-134">属性</span><span class="sxs-lookup"><span data-stu-id="237aa-134">Property</span></span>|<span data-ttu-id="237aa-135">类型</span><span class="sxs-lookup"><span data-stu-id="237aa-135">Type</span></span>|<span data-ttu-id="237aa-136">说明</span><span class="sxs-lookup"><span data-stu-id="237aa-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="237aa-137">displayName</span><span class="sxs-lookup"><span data-stu-id="237aa-137">displayName</span></span>|<span data-ttu-id="237aa-138">字符串</span><span class="sxs-lookup"><span data-stu-id="237aa-138">String</span></span>|<span data-ttu-id="237aa-139">策略显示名称。</span><span class="sxs-lookup"><span data-stu-id="237aa-139">Policy display name.</span></span> <span data-ttu-id="237aa-140">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="237aa-140">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="237aa-141">说明</span><span class="sxs-lookup"><span data-stu-id="237aa-141">description</span></span>|<span data-ttu-id="237aa-142">String</span><span class="sxs-lookup"><span data-stu-id="237aa-142">String</span></span>|<span data-ttu-id="237aa-143">策略的说明。</span><span class="sxs-lookup"><span data-stu-id="237aa-143">The policy's description.</span></span> <span data-ttu-id="237aa-144">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="237aa-144">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="237aa-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="237aa-145">createdDateTime</span></span>|<span data-ttu-id="237aa-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="237aa-146">DateTimeOffset</span></span>|<span data-ttu-id="237aa-147">创建策略的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="237aa-147">The date and time the policy was created.</span></span> <span data-ttu-id="237aa-148">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="237aa-148">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="237aa-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="237aa-149">lastModifiedDateTime</span></span>|<span data-ttu-id="237aa-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="237aa-150">DateTimeOffset</span></span>|<span data-ttu-id="237aa-151">上次修改策略的时间。</span><span class="sxs-lookup"><span data-stu-id="237aa-151">Last time the policy was modified.</span></span> <span data-ttu-id="237aa-152">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="237aa-152">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="237aa-153">id</span><span class="sxs-lookup"><span data-stu-id="237aa-153">id</span></span>|<span data-ttu-id="237aa-154">字符串</span><span class="sxs-lookup"><span data-stu-id="237aa-154">String</span></span>|<span data-ttu-id="237aa-155">实体的键。</span><span class="sxs-lookup"><span data-stu-id="237aa-155">Key of the entity.</span></span> <span data-ttu-id="237aa-156">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="237aa-156">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="237aa-157">version</span><span class="sxs-lookup"><span data-stu-id="237aa-157">version</span></span>|<span data-ttu-id="237aa-158">String</span><span class="sxs-lookup"><span data-stu-id="237aa-158">String</span></span>|<span data-ttu-id="237aa-159">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="237aa-159">Version of the entity.</span></span> <span data-ttu-id="237aa-160">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="237aa-160">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="237aa-161">customSettings</span><span class="sxs-lookup"><span data-stu-id="237aa-161">customSettings</span></span>|<span data-ttu-id="237aa-162">[keyValuePair](../resources/intune-mam-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="237aa-162">[keyValuePair](../resources/intune-mam-keyvaluepair.md) collection</span></span>|<span data-ttu-id="237aa-163">要发送到配置范围确定的用户应用的一组字符串键和字符串值对，不由此服务更改。继承自 [ managedAppConfiguration ](../resources/intune-mam-managedappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="237aa-163">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service Inherited from [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span></span>|
|<span data-ttu-id="237aa-164">deployedAppCount</span><span class="sxs-lookup"><span data-stu-id="237aa-164">deployedAppCount</span></span>|<span data-ttu-id="237aa-165">Int32</span><span class="sxs-lookup"><span data-stu-id="237aa-165">Int32</span></span>|<span data-ttu-id="237aa-166">当前策略部署到的应用的计数。</span><span class="sxs-lookup"><span data-stu-id="237aa-166">Count of apps to which the current policy is deployed.</span></span>|
|<span data-ttu-id="237aa-167">isAssigned</span><span class="sxs-lookup"><span data-stu-id="237aa-167">isAssigned</span></span>|<span data-ttu-id="237aa-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="237aa-168">Boolean</span></span>|<span data-ttu-id="237aa-169">指示策略是否部署到任何包含组。</span><span class="sxs-lookup"><span data-stu-id="237aa-169">Indicates if the policy is deployed to any inclusion groups or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="237aa-170">关系</span><span class="sxs-lookup"><span data-stu-id="237aa-170">Relationships</span></span>
|<span data-ttu-id="237aa-171">关系</span><span class="sxs-lookup"><span data-stu-id="237aa-171">Relationship</span></span>|<span data-ttu-id="237aa-172">类型</span><span class="sxs-lookup"><span data-stu-id="237aa-172">Type</span></span>|<span data-ttu-id="237aa-173">说明</span><span class="sxs-lookup"><span data-stu-id="237aa-173">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="237aa-174">apps</span><span class="sxs-lookup"><span data-stu-id="237aa-174">apps</span></span>|<span data-ttu-id="237aa-175">[managedMobileApp](../resources/intune-mam-managedmobileapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="237aa-175">[managedMobileApp](../resources/intune-mam-managedmobileapp.md) collection</span></span>|<span data-ttu-id="237aa-176">策略部署到的应用的列表。</span><span class="sxs-lookup"><span data-stu-id="237aa-176">List of apps to which the policy is deployed.</span></span>|
|<span data-ttu-id="237aa-177">deploymentSummary</span><span class="sxs-lookup"><span data-stu-id="237aa-177">deploymentSummary</span></span>|[<span data-ttu-id="237aa-178">managedAppPolicyDeploymentSummary</span><span class="sxs-lookup"><span data-stu-id="237aa-178">managedAppPolicyDeploymentSummary</span></span>](../resources/intune-mam-managedapppolicydeploymentsummary.md)|<span data-ttu-id="237aa-179">配置的部署摘要的导航属性。</span><span class="sxs-lookup"><span data-stu-id="237aa-179">Navigation property to deployment summary of the configuration.</span></span>|
|<span data-ttu-id="237aa-180">assignments</span><span class="sxs-lookup"><span data-stu-id="237aa-180">assignments</span></span>|<span data-ttu-id="237aa-181">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="237aa-181">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) collection</span></span>|<span data-ttu-id="237aa-182">策略部署到的包含组和排除组列表的导航属性。</span><span class="sxs-lookup"><span data-stu-id="237aa-182">Navigation property to list of inclusion and exclusion groups to which the policy is deployed.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="237aa-183">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="237aa-183">JSON Representation</span></span>
<span data-ttu-id="237aa-184">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="237aa-184">Here is a JSON representation of the resource.</span></span>
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





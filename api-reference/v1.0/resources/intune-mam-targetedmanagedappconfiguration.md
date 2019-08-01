---
title: targetedManagedAppConfiguration 资源类型
description: 用于将一组自定义设置按原样提供给目标安全组中的所有用户的配置
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a3e1b8ac4c3db947268bd050cbd698527c8d38b9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36037812"
---
# <a name="targetedmanagedappconfiguration-resource-type"></a><span data-ttu-id="88c32-103">targetedManagedAppConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="88c32-103">targetedManagedAppConfiguration resource type</span></span>

> <span data-ttu-id="88c32-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="88c32-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="88c32-105">用于将一组自定义设置按原样提供给目标安全组中的所有用户的配置</span><span class="sxs-lookup"><span data-stu-id="88c32-105">Configuration used to deliver a set of custom settings as-is to all users in the targeted security group</span></span>


<span data-ttu-id="88c32-106">继承自 [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="88c32-106">Inherits from [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="88c32-107">方法</span><span class="sxs-lookup"><span data-stu-id="88c32-107">Methods</span></span>
|<span data-ttu-id="88c32-108">方法</span><span class="sxs-lookup"><span data-stu-id="88c32-108">Method</span></span>|<span data-ttu-id="88c32-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="88c32-109">Return Type</span></span>|<span data-ttu-id="88c32-110">说明</span><span class="sxs-lookup"><span data-stu-id="88c32-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="88c32-111">List targetedManagedAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="88c32-111">List targetedManagedAppConfigurations</span></span>](../api/intune-mam-targetedmanagedappconfiguration-list.md)|<span data-ttu-id="88c32-112">[targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="88c32-112">[targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) collection</span></span>|<span data-ttu-id="88c32-113">列出 [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="88c32-113">List properties and relationships of the [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="88c32-114">Get targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="88c32-114">Get targetedManagedAppConfiguration</span></span>](../api/intune-mam-targetedmanagedappconfiguration-get.md)|[<span data-ttu-id="88c32-115">targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="88c32-115">targetedManagedAppConfiguration</span></span>](../resources/intune-mam-targetedmanagedappconfiguration.md)|<span data-ttu-id="88c32-116">读取 [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="88c32-116">Read properties and relationships of the [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>|
|[<span data-ttu-id="88c32-117">Create targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="88c32-117">Create targetedManagedAppConfiguration</span></span>](../api/intune-mam-targetedmanagedappconfiguration-create.md)|[<span data-ttu-id="88c32-118">targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="88c32-118">targetedManagedAppConfiguration</span></span>](../resources/intune-mam-targetedmanagedappconfiguration.md)|<span data-ttu-id="88c32-119">创建新的 [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="88c32-119">Create a new [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>|
|[<span data-ttu-id="88c32-120">Delete targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="88c32-120">Delete targetedManagedAppConfiguration</span></span>](../api/intune-mam-targetedmanagedappconfiguration-delete.md)|<span data-ttu-id="88c32-121">无</span><span class="sxs-lookup"><span data-stu-id="88c32-121">None</span></span>|<span data-ttu-id="88c32-122">删除 [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="88c32-122">Deletes a [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md).</span></span>|
|[<span data-ttu-id="88c32-123">Update targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="88c32-123">Update targetedManagedAppConfiguration</span></span>](../api/intune-mam-targetedmanagedappconfiguration-update.md)|[<span data-ttu-id="88c32-124">targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="88c32-124">targetedManagedAppConfiguration</span></span>](../resources/intune-mam-targetedmanagedappconfiguration.md)|<span data-ttu-id="88c32-125">更新 [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="88c32-125">Update the properties of a [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>|
|[<span data-ttu-id="88c32-126">assign 操作</span><span class="sxs-lookup"><span data-stu-id="88c32-126">assign action</span></span>](../api/intune-mam-targetedmanagedappconfiguration-assign.md)|<span data-ttu-id="88c32-127">无</span><span class="sxs-lookup"><span data-stu-id="88c32-127">None</span></span>|<span data-ttu-id="88c32-128">尚未记录</span><span class="sxs-lookup"><span data-stu-id="88c32-128">Not yet documented</span></span>|
|[<span data-ttu-id="88c32-129">targetApps 操作</span><span class="sxs-lookup"><span data-stu-id="88c32-129">targetApps action</span></span>](../api/intune-mam-targetedmanagedappconfiguration-targetapps.md)|<span data-ttu-id="88c32-130">无</span><span class="sxs-lookup"><span data-stu-id="88c32-130">None</span></span>|<span data-ttu-id="88c32-131">尚未记录</span><span class="sxs-lookup"><span data-stu-id="88c32-131">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="88c32-132">属性</span><span class="sxs-lookup"><span data-stu-id="88c32-132">Properties</span></span>
|<span data-ttu-id="88c32-133">属性</span><span class="sxs-lookup"><span data-stu-id="88c32-133">Property</span></span>|<span data-ttu-id="88c32-134">类型</span><span class="sxs-lookup"><span data-stu-id="88c32-134">Type</span></span>|<span data-ttu-id="88c32-135">说明</span><span class="sxs-lookup"><span data-stu-id="88c32-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="88c32-136">displayName</span><span class="sxs-lookup"><span data-stu-id="88c32-136">displayName</span></span>|<span data-ttu-id="88c32-137">字符串</span><span class="sxs-lookup"><span data-stu-id="88c32-137">String</span></span>|<span data-ttu-id="88c32-138">策略显示名称。</span><span class="sxs-lookup"><span data-stu-id="88c32-138">Policy display name.</span></span> <span data-ttu-id="88c32-139">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="88c32-139">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="88c32-140">说明</span><span class="sxs-lookup"><span data-stu-id="88c32-140">description</span></span>|<span data-ttu-id="88c32-141">String</span><span class="sxs-lookup"><span data-stu-id="88c32-141">String</span></span>|<span data-ttu-id="88c32-142">策略的说明。</span><span class="sxs-lookup"><span data-stu-id="88c32-142">The policy's description.</span></span> <span data-ttu-id="88c32-143">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="88c32-143">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="88c32-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="88c32-144">createdDateTime</span></span>|<span data-ttu-id="88c32-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="88c32-145">DateTimeOffset</span></span>|<span data-ttu-id="88c32-146">创建策略的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="88c32-146">The date and time the policy was created.</span></span> <span data-ttu-id="88c32-147">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="88c32-147">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="88c32-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="88c32-148">lastModifiedDateTime</span></span>|<span data-ttu-id="88c32-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="88c32-149">DateTimeOffset</span></span>|<span data-ttu-id="88c32-150">上次修改策略的时间。</span><span class="sxs-lookup"><span data-stu-id="88c32-150">Last time the policy was modified.</span></span> <span data-ttu-id="88c32-151">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="88c32-151">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="88c32-152">id</span><span class="sxs-lookup"><span data-stu-id="88c32-152">id</span></span>|<span data-ttu-id="88c32-153">字符串</span><span class="sxs-lookup"><span data-stu-id="88c32-153">String</span></span>|<span data-ttu-id="88c32-154">实体的键。</span><span class="sxs-lookup"><span data-stu-id="88c32-154">Key of the entity.</span></span> <span data-ttu-id="88c32-155">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="88c32-155">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="88c32-156">version</span><span class="sxs-lookup"><span data-stu-id="88c32-156">version</span></span>|<span data-ttu-id="88c32-157">String</span><span class="sxs-lookup"><span data-stu-id="88c32-157">String</span></span>|<span data-ttu-id="88c32-158">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="88c32-158">Version of the entity.</span></span> <span data-ttu-id="88c32-159">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="88c32-159">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="88c32-160">customSettings</span><span class="sxs-lookup"><span data-stu-id="88c32-160">customSettings</span></span>|<span data-ttu-id="88c32-161">[keyValuePair](../resources/intune-mam-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="88c32-161">[keyValuePair](../resources/intune-mam-keyvaluepair.md) collection</span></span>|<span data-ttu-id="88c32-162">要发送到配置范围确定的用户应用的一组字符串键和字符串值对，不由此服务更改。继承自 [ managedAppConfiguration ](../resources/intune-mam-managedappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="88c32-162">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service Inherited from [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span></span>|
|<span data-ttu-id="88c32-163">deployedAppCount</span><span class="sxs-lookup"><span data-stu-id="88c32-163">deployedAppCount</span></span>|<span data-ttu-id="88c32-164">Int32</span><span class="sxs-lookup"><span data-stu-id="88c32-164">Int32</span></span>|<span data-ttu-id="88c32-165">当前策略部署到的应用的计数。</span><span class="sxs-lookup"><span data-stu-id="88c32-165">Count of apps to which the current policy is deployed.</span></span>|
|<span data-ttu-id="88c32-166">isAssigned</span><span class="sxs-lookup"><span data-stu-id="88c32-166">isAssigned</span></span>|<span data-ttu-id="88c32-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="88c32-167">Boolean</span></span>|<span data-ttu-id="88c32-168">指示策略是否部署到任何包含组。</span><span class="sxs-lookup"><span data-stu-id="88c32-168">Indicates if the policy is deployed to any inclusion groups or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="88c32-169">关系</span><span class="sxs-lookup"><span data-stu-id="88c32-169">Relationships</span></span>
|<span data-ttu-id="88c32-170">关系</span><span class="sxs-lookup"><span data-stu-id="88c32-170">Relationship</span></span>|<span data-ttu-id="88c32-171">类型</span><span class="sxs-lookup"><span data-stu-id="88c32-171">Type</span></span>|<span data-ttu-id="88c32-172">说明</span><span class="sxs-lookup"><span data-stu-id="88c32-172">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="88c32-173">apps</span><span class="sxs-lookup"><span data-stu-id="88c32-173">apps</span></span>|<span data-ttu-id="88c32-174">[managedMobileApp](../resources/intune-mam-managedmobileapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="88c32-174">[managedMobileApp](../resources/intune-mam-managedmobileapp.md) collection</span></span>|<span data-ttu-id="88c32-175">策略部署到的应用的列表。</span><span class="sxs-lookup"><span data-stu-id="88c32-175">List of apps to which the policy is deployed.</span></span>|
|<span data-ttu-id="88c32-176">deploymentSummary</span><span class="sxs-lookup"><span data-stu-id="88c32-176">deploymentSummary</span></span>|[<span data-ttu-id="88c32-177">managedAppPolicyDeploymentSummary</span><span class="sxs-lookup"><span data-stu-id="88c32-177">managedAppPolicyDeploymentSummary</span></span>](../resources/intune-mam-managedapppolicydeploymentsummary.md)|<span data-ttu-id="88c32-178">配置的部署摘要的导航属性。</span><span class="sxs-lookup"><span data-stu-id="88c32-178">Navigation property to deployment summary of the configuration.</span></span>|
|<span data-ttu-id="88c32-179">assignments</span><span class="sxs-lookup"><span data-stu-id="88c32-179">assignments</span></span>|<span data-ttu-id="88c32-180">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="88c32-180">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) collection</span></span>|<span data-ttu-id="88c32-181">策略部署到的包含组和排除组列表的导航属性。</span><span class="sxs-lookup"><span data-stu-id="88c32-181">Navigation property to list of inclusion and exclusion groups to which the policy is deployed.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="88c32-182">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="88c32-182">JSON Representation</span></span>
<span data-ttu-id="88c32-183">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="88c32-183">Here is a JSON representation of the resource.</span></span>
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




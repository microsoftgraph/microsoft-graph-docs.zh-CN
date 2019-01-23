---
title: targetedManagedAppConfiguration 资源类型
description: 用于将一组自定义设置按原样提供给目标安全组中的所有用户的配置
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 41a8ad1e246b977a853ec9ae16b8485894862b0e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29420925"
---
# <a name="targetedmanagedappconfiguration-resource-type"></a><span data-ttu-id="deba2-103">targetedManagedAppConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="deba2-103">targetedManagedAppConfiguration resource type</span></span>

> <span data-ttu-id="deba2-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="deba2-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="deba2-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="deba2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="deba2-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="deba2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="deba2-107">用于将一组自定义设置按原样提供给目标安全组中的所有用户的配置</span><span class="sxs-lookup"><span data-stu-id="deba2-107">Configuration used to deliver a set of custom settings as-is to all users in the targeted security group</span></span>


<span data-ttu-id="deba2-108">继承自 [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="deba2-108">Inherits from [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="deba2-109">方法</span><span class="sxs-lookup"><span data-stu-id="deba2-109">Methods</span></span>
|<span data-ttu-id="deba2-110">方法</span><span class="sxs-lookup"><span data-stu-id="deba2-110">Method</span></span>|<span data-ttu-id="deba2-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="deba2-111">Return Type</span></span>|<span data-ttu-id="deba2-112">说明</span><span class="sxs-lookup"><span data-stu-id="deba2-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="deba2-113">List targetedManagedAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="deba2-113">List targetedManagedAppConfigurations</span></span>](../api/intune-mam-targetedmanagedappconfiguration-list.md)|<span data-ttu-id="deba2-114">[targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="deba2-114">[targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) collection</span></span>|<span data-ttu-id="deba2-115">列出 [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="deba2-115">List properties and relationships of the [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="deba2-116">Get targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="deba2-116">Get targetedManagedAppConfiguration</span></span>](../api/intune-mam-targetedmanagedappconfiguration-get.md)|[<span data-ttu-id="deba2-117">targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="deba2-117">targetedManagedAppConfiguration</span></span>](../resources/intune-mam-targetedmanagedappconfiguration.md)|<span data-ttu-id="deba2-118">读取 [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="deba2-118">Read properties and relationships of the [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>|
|[<span data-ttu-id="deba2-119">Create targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="deba2-119">Create targetedManagedAppConfiguration</span></span>](../api/intune-mam-targetedmanagedappconfiguration-create.md)|[<span data-ttu-id="deba2-120">targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="deba2-120">targetedManagedAppConfiguration</span></span>](../resources/intune-mam-targetedmanagedappconfiguration.md)|<span data-ttu-id="deba2-121">创建新的 [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="deba2-121">Create a new [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>|
|[<span data-ttu-id="deba2-122">Delete targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="deba2-122">Delete targetedManagedAppConfiguration</span></span>](../api/intune-mam-targetedmanagedappconfiguration-delete.md)|<span data-ttu-id="deba2-123">无</span><span class="sxs-lookup"><span data-stu-id="deba2-123">None</span></span>|<span data-ttu-id="deba2-124">删除 [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="deba2-124">Deletes a [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md).</span></span>|
|[<span data-ttu-id="deba2-125">Update targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="deba2-125">Update targetedManagedAppConfiguration</span></span>](../api/intune-mam-targetedmanagedappconfiguration-update.md)|[<span data-ttu-id="deba2-126">targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="deba2-126">targetedManagedAppConfiguration</span></span>](../resources/intune-mam-targetedmanagedappconfiguration.md)|<span data-ttu-id="deba2-127">更新 [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="deba2-127">Update the properties of a [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>|
|[<span data-ttu-id="deba2-128">assign 操作</span><span class="sxs-lookup"><span data-stu-id="deba2-128">assign action</span></span>](../api/intune-mam-targetedmanagedappconfiguration-assign.md)|<span data-ttu-id="deba2-129">无</span><span class="sxs-lookup"><span data-stu-id="deba2-129">None</span></span>|<span data-ttu-id="deba2-130">尚未记录</span><span class="sxs-lookup"><span data-stu-id="deba2-130">Not yet documented</span></span>|
|[<span data-ttu-id="deba2-131">targetApps 操作</span><span class="sxs-lookup"><span data-stu-id="deba2-131">targetApps action</span></span>](../api/intune-mam-targetedmanagedappconfiguration-targetapps.md)|<span data-ttu-id="deba2-132">无</span><span class="sxs-lookup"><span data-stu-id="deba2-132">None</span></span>|<span data-ttu-id="deba2-133">尚未记录</span><span class="sxs-lookup"><span data-stu-id="deba2-133">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="deba2-134">属性</span><span class="sxs-lookup"><span data-stu-id="deba2-134">Properties</span></span>
|<span data-ttu-id="deba2-135">属性</span><span class="sxs-lookup"><span data-stu-id="deba2-135">Property</span></span>|<span data-ttu-id="deba2-136">类型</span><span class="sxs-lookup"><span data-stu-id="deba2-136">Type</span></span>|<span data-ttu-id="deba2-137">说明</span><span class="sxs-lookup"><span data-stu-id="deba2-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="deba2-138">displayName</span><span class="sxs-lookup"><span data-stu-id="deba2-138">displayName</span></span>|<span data-ttu-id="deba2-139">String</span><span class="sxs-lookup"><span data-stu-id="deba2-139">String</span></span>|<span data-ttu-id="deba2-140">策略显示名称。</span><span class="sxs-lookup"><span data-stu-id="deba2-140">Policy display name.</span></span> <span data-ttu-id="deba2-141">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="deba2-141">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="deba2-142">description</span><span class="sxs-lookup"><span data-stu-id="deba2-142">description</span></span>|<span data-ttu-id="deba2-143">String</span><span class="sxs-lookup"><span data-stu-id="deba2-143">String</span></span>|<span data-ttu-id="deba2-144">策略的说明。</span><span class="sxs-lookup"><span data-stu-id="deba2-144">The policy's description.</span></span> <span data-ttu-id="deba2-145">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="deba2-145">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="deba2-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="deba2-146">createdDateTime</span></span>|<span data-ttu-id="deba2-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="deba2-147">DateTimeOffset</span></span>|<span data-ttu-id="deba2-148">创建策略的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="deba2-148">The date and time the policy was created.</span></span> <span data-ttu-id="deba2-149">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="deba2-149">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="deba2-150">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="deba2-150">lastModifiedDateTime</span></span>|<span data-ttu-id="deba2-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="deba2-151">DateTimeOffset</span></span>|<span data-ttu-id="deba2-152">上次修改策略的时间。</span><span class="sxs-lookup"><span data-stu-id="deba2-152">Last time the policy was modified.</span></span> <span data-ttu-id="deba2-153">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="deba2-153">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="deba2-154">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="deba2-154">roleScopeTagIds</span></span>|<span data-ttu-id="deba2-155">String 集合</span><span class="sxs-lookup"><span data-stu-id="deba2-155">String collection</span></span>|<span data-ttu-id="deba2-156">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="deba2-156">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="deba2-157">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="deba2-157">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="deba2-158">id</span><span class="sxs-lookup"><span data-stu-id="deba2-158">id</span></span>|<span data-ttu-id="deba2-159">String</span><span class="sxs-lookup"><span data-stu-id="deba2-159">String</span></span>|<span data-ttu-id="deba2-160">实体的键。</span><span class="sxs-lookup"><span data-stu-id="deba2-160">Key of the entity.</span></span> <span data-ttu-id="deba2-161">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="deba2-161">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="deba2-162">version</span><span class="sxs-lookup"><span data-stu-id="deba2-162">version</span></span>|<span data-ttu-id="deba2-163">String</span><span class="sxs-lookup"><span data-stu-id="deba2-163">String</span></span>|<span data-ttu-id="deba2-164">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="deba2-164">Version of the entity.</span></span> <span data-ttu-id="deba2-165">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="deba2-165">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="deba2-166">customSettings</span><span class="sxs-lookup"><span data-stu-id="deba2-166">customSettings</span></span>|<span data-ttu-id="deba2-167">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="deba2-167">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="deba2-168">要发送到配置范围确定的用户应用的一组字符串键和字符串值对，不由此服务更改。继承自 [ managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="deba2-168">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service Inherited from [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span></span>|
|<span data-ttu-id="deba2-169">deployedAppCount</span><span class="sxs-lookup"><span data-stu-id="deba2-169">deployedAppCount</span></span>|<span data-ttu-id="deba2-170">Int32</span><span class="sxs-lookup"><span data-stu-id="deba2-170">Int32</span></span>|<span data-ttu-id="deba2-171">当前策略部署到的应用的计数。</span><span class="sxs-lookup"><span data-stu-id="deba2-171">Count of apps to which the current policy is deployed.</span></span>|
|<span data-ttu-id="deba2-172">isAssigned</span><span class="sxs-lookup"><span data-stu-id="deba2-172">isAssigned</span></span>|<span data-ttu-id="deba2-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="deba2-173">Boolean</span></span>|<span data-ttu-id="deba2-174">指示策略是否部署到任何包含组。</span><span class="sxs-lookup"><span data-stu-id="deba2-174">Indicates if the policy is deployed to any inclusion groups or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="deba2-175">关系</span><span class="sxs-lookup"><span data-stu-id="deba2-175">Relationships</span></span>
|<span data-ttu-id="deba2-176">关系</span><span class="sxs-lookup"><span data-stu-id="deba2-176">Relationship</span></span>|<span data-ttu-id="deba2-177">类型</span><span class="sxs-lookup"><span data-stu-id="deba2-177">Type</span></span>|<span data-ttu-id="deba2-178">说明</span><span class="sxs-lookup"><span data-stu-id="deba2-178">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="deba2-179">apps</span><span class="sxs-lookup"><span data-stu-id="deba2-179">apps</span></span>|<span data-ttu-id="deba2-180">[managedMobileApp](../resources/intune-mam-managedmobileapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="deba2-180">[managedMobileApp](../resources/intune-mam-managedmobileapp.md) collection</span></span>|<span data-ttu-id="deba2-181">策略部署到的应用的列表。</span><span class="sxs-lookup"><span data-stu-id="deba2-181">List of apps to which the policy is deployed.</span></span>|
|<span data-ttu-id="deba2-182">deploymentSummary</span><span class="sxs-lookup"><span data-stu-id="deba2-182">deploymentSummary</span></span>|[<span data-ttu-id="deba2-183">managedAppPolicyDeploymentSummary</span><span class="sxs-lookup"><span data-stu-id="deba2-183">managedAppPolicyDeploymentSummary</span></span>](../resources/intune-mam-managedapppolicydeploymentsummary.md)|<span data-ttu-id="deba2-184">配置的部署摘要的导航属性。</span><span class="sxs-lookup"><span data-stu-id="deba2-184">Navigation property to deployment summary of the configuration.</span></span>|
|<span data-ttu-id="deba2-185">assignments</span><span class="sxs-lookup"><span data-stu-id="deba2-185">assignments</span></span>|<span data-ttu-id="deba2-186">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="deba2-186">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) collection</span></span>|<span data-ttu-id="deba2-187">策略部署到的包含组和排除组列表的导航属性。</span><span class="sxs-lookup"><span data-stu-id="deba2-187">Navigation property to list of inclusion and exclusion groups to which the policy is deployed.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="deba2-188">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="deba2-188">JSON Representation</span></span>
<span data-ttu-id="deba2-189">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="deba2-189">Here is a JSON representation of the resource.</span></span>
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





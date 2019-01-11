---
title: targetedManagedAppConfiguration 资源类型
description: 用于将一组自定义设置按原样提供给目标安全组中的所有用户的配置
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: e12d51b0925ad2412e86c0bbb1b6b3992204659c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27879322"
---
# <a name="targetedmanagedappconfiguration-resource-type"></a><span data-ttu-id="39ba6-103">targetedManagedAppConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="39ba6-103">targetedManagedAppConfiguration resource type</span></span>

> <span data-ttu-id="39ba6-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="39ba6-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="39ba6-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="39ba6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="39ba6-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="39ba6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="39ba6-107">用于将一组自定义设置按原样提供给目标安全组中的所有用户的配置</span><span class="sxs-lookup"><span data-stu-id="39ba6-107">Configuration used to deliver a set of custom settings as-is to all users in the targeted security group</span></span>

<span data-ttu-id="39ba6-108">继承自 [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="39ba6-108">Inherits from [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="39ba6-109">方法</span><span class="sxs-lookup"><span data-stu-id="39ba6-109">Methods</span></span>
|<span data-ttu-id="39ba6-110">方法</span><span class="sxs-lookup"><span data-stu-id="39ba6-110">Method</span></span>|<span data-ttu-id="39ba6-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="39ba6-111">Return Type</span></span>|<span data-ttu-id="39ba6-112">说明</span><span class="sxs-lookup"><span data-stu-id="39ba6-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="39ba6-113">List targetedManagedAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="39ba6-113">List targetedManagedAppConfigurations</span></span>](../api/intune-mam-targetedmanagedappconfiguration-list.md)|<span data-ttu-id="39ba6-114">[targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="39ba6-114">[targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) collection</span></span>|<span data-ttu-id="39ba6-115">列出 [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="39ba6-115">List properties and relationships of the [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="39ba6-116">Get targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="39ba6-116">Get targetedManagedAppConfiguration</span></span>](../api/intune-mam-targetedmanagedappconfiguration-get.md)|[<span data-ttu-id="39ba6-117">targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="39ba6-117">targetedManagedAppConfiguration</span></span>](../resources/intune-mam-targetedmanagedappconfiguration.md)|<span data-ttu-id="39ba6-118">读取 [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="39ba6-118">Read properties and relationships of the [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>|
|[<span data-ttu-id="39ba6-119">Create targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="39ba6-119">Create targetedManagedAppConfiguration</span></span>](../api/intune-mam-targetedmanagedappconfiguration-create.md)|[<span data-ttu-id="39ba6-120">targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="39ba6-120">targetedManagedAppConfiguration</span></span>](../resources/intune-mam-targetedmanagedappconfiguration.md)|<span data-ttu-id="39ba6-121">创建新的 [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="39ba6-121">Create a new [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>|
|[<span data-ttu-id="39ba6-122">Delete targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="39ba6-122">Delete targetedManagedAppConfiguration</span></span>](../api/intune-mam-targetedmanagedappconfiguration-delete.md)|<span data-ttu-id="39ba6-123">无</span><span class="sxs-lookup"><span data-stu-id="39ba6-123">None</span></span>|<span data-ttu-id="39ba6-124">删除 [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="39ba6-124">Deletes a [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md).</span></span>|
|[<span data-ttu-id="39ba6-125">Update targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="39ba6-125">Update targetedManagedAppConfiguration</span></span>](../api/intune-mam-targetedmanagedappconfiguration-update.md)|[<span data-ttu-id="39ba6-126">targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="39ba6-126">targetedManagedAppConfiguration</span></span>](../resources/intune-mam-targetedmanagedappconfiguration.md)|<span data-ttu-id="39ba6-127">更新 [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="39ba6-127">Update the properties of a [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>|
|[<span data-ttu-id="39ba6-128">assign 操作</span><span class="sxs-lookup"><span data-stu-id="39ba6-128">assign action</span></span>](../api/intune-mam-targetedmanagedappconfiguration-assign.md)|<span data-ttu-id="39ba6-129">无</span><span class="sxs-lookup"><span data-stu-id="39ba6-129">None</span></span>|<span data-ttu-id="39ba6-130">尚未记录</span><span class="sxs-lookup"><span data-stu-id="39ba6-130">Not yet documented</span></span>|
|[<span data-ttu-id="39ba6-131">targetApps 操作</span><span class="sxs-lookup"><span data-stu-id="39ba6-131">targetApps action</span></span>](../api/intune-mam-targetedmanagedappconfiguration-targetapps.md)|<span data-ttu-id="39ba6-132">无</span><span class="sxs-lookup"><span data-stu-id="39ba6-132">None</span></span>|<span data-ttu-id="39ba6-133">尚未记录</span><span class="sxs-lookup"><span data-stu-id="39ba6-133">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="39ba6-134">属性</span><span class="sxs-lookup"><span data-stu-id="39ba6-134">Properties</span></span>
|<span data-ttu-id="39ba6-135">属性</span><span class="sxs-lookup"><span data-stu-id="39ba6-135">Property</span></span>|<span data-ttu-id="39ba6-136">类型</span><span class="sxs-lookup"><span data-stu-id="39ba6-136">Type</span></span>|<span data-ttu-id="39ba6-137">说明</span><span class="sxs-lookup"><span data-stu-id="39ba6-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="39ba6-138">displayName</span><span class="sxs-lookup"><span data-stu-id="39ba6-138">displayName</span></span>|<span data-ttu-id="39ba6-139">String</span><span class="sxs-lookup"><span data-stu-id="39ba6-139">String</span></span>|<span data-ttu-id="39ba6-140">策略显示名称。</span><span class="sxs-lookup"><span data-stu-id="39ba6-140">Policy display name.</span></span> <span data-ttu-id="39ba6-141">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="39ba6-141">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="39ba6-142">description</span><span class="sxs-lookup"><span data-stu-id="39ba6-142">description</span></span>|<span data-ttu-id="39ba6-143">String</span><span class="sxs-lookup"><span data-stu-id="39ba6-143">String</span></span>|<span data-ttu-id="39ba6-144">策略的说明。</span><span class="sxs-lookup"><span data-stu-id="39ba6-144">The policy's description.</span></span> <span data-ttu-id="39ba6-145">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="39ba6-145">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="39ba6-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="39ba6-146">createdDateTime</span></span>|<span data-ttu-id="39ba6-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="39ba6-147">DateTimeOffset</span></span>|<span data-ttu-id="39ba6-148">创建策略的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="39ba6-148">The date and time the policy was created.</span></span> <span data-ttu-id="39ba6-149">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="39ba6-149">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="39ba6-150">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="39ba6-150">lastModifiedDateTime</span></span>|<span data-ttu-id="39ba6-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="39ba6-151">DateTimeOffset</span></span>|<span data-ttu-id="39ba6-152">上次修改策略的时间。</span><span class="sxs-lookup"><span data-stu-id="39ba6-152">Last time the policy was modified.</span></span> <span data-ttu-id="39ba6-153">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="39ba6-153">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="39ba6-154">id</span><span class="sxs-lookup"><span data-stu-id="39ba6-154">id</span></span>|<span data-ttu-id="39ba6-155">String</span><span class="sxs-lookup"><span data-stu-id="39ba6-155">String</span></span>|<span data-ttu-id="39ba6-156">实体的键。</span><span class="sxs-lookup"><span data-stu-id="39ba6-156">Key of the entity.</span></span> <span data-ttu-id="39ba6-157">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="39ba6-157">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="39ba6-158">version</span><span class="sxs-lookup"><span data-stu-id="39ba6-158">version</span></span>|<span data-ttu-id="39ba6-159">String</span><span class="sxs-lookup"><span data-stu-id="39ba6-159">String</span></span>|<span data-ttu-id="39ba6-160">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="39ba6-160">Version of the entity.</span></span> <span data-ttu-id="39ba6-161">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="39ba6-161">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="39ba6-162">customSettings</span><span class="sxs-lookup"><span data-stu-id="39ba6-162">customSettings</span></span>|<span data-ttu-id="39ba6-163">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="39ba6-163">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="39ba6-164">要发送到配置范围确定的用户应用的一组字符串键和字符串值对，不由此服务更改。继承自 [ managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="39ba6-164">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service Inherited from [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span></span>|
|<span data-ttu-id="39ba6-165">deployedAppCount</span><span class="sxs-lookup"><span data-stu-id="39ba6-165">deployedAppCount</span></span>|<span data-ttu-id="39ba6-166">Int32</span><span class="sxs-lookup"><span data-stu-id="39ba6-166">Int32</span></span>|<span data-ttu-id="39ba6-167">当前策略部署到的应用的计数。</span><span class="sxs-lookup"><span data-stu-id="39ba6-167">Count of apps to which the current policy is deployed.</span></span>|
|<span data-ttu-id="39ba6-168">isAssigned</span><span class="sxs-lookup"><span data-stu-id="39ba6-168">isAssigned</span></span>|<span data-ttu-id="39ba6-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="39ba6-169">Boolean</span></span>|<span data-ttu-id="39ba6-170">指示策略是否部署到任何包含组。</span><span class="sxs-lookup"><span data-stu-id="39ba6-170">Indicates if the policy is deployed to any inclusion groups or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="39ba6-171">关系</span><span class="sxs-lookup"><span data-stu-id="39ba6-171">Relationships</span></span>
|<span data-ttu-id="39ba6-172">关系</span><span class="sxs-lookup"><span data-stu-id="39ba6-172">Relationship</span></span>|<span data-ttu-id="39ba6-173">类型</span><span class="sxs-lookup"><span data-stu-id="39ba6-173">Type</span></span>|<span data-ttu-id="39ba6-174">说明</span><span class="sxs-lookup"><span data-stu-id="39ba6-174">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="39ba6-175">apps</span><span class="sxs-lookup"><span data-stu-id="39ba6-175">apps</span></span>|<span data-ttu-id="39ba6-176">[managedMobileApp](../resources/intune-mam-managedmobileapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="39ba6-176">[managedMobileApp](../resources/intune-mam-managedmobileapp.md) collection</span></span>|<span data-ttu-id="39ba6-177">策略部署到的应用的列表。</span><span class="sxs-lookup"><span data-stu-id="39ba6-177">List of apps to which the policy is deployed.</span></span>|
|<span data-ttu-id="39ba6-178">deploymentSummary</span><span class="sxs-lookup"><span data-stu-id="39ba6-178">deploymentSummary</span></span>|[<span data-ttu-id="39ba6-179">managedAppPolicyDeploymentSummary</span><span class="sxs-lookup"><span data-stu-id="39ba6-179">managedAppPolicyDeploymentSummary</span></span>](../resources/intune-mam-managedapppolicydeploymentsummary.md)|<span data-ttu-id="39ba6-180">配置的部署摘要的导航属性。</span><span class="sxs-lookup"><span data-stu-id="39ba6-180">Navigation property to deployment summary of the configuration.</span></span>|
|<span data-ttu-id="39ba6-181">assignments</span><span class="sxs-lookup"><span data-stu-id="39ba6-181">assignments</span></span>|<span data-ttu-id="39ba6-182">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="39ba6-182">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) collection</span></span>|<span data-ttu-id="39ba6-183">策略部署到的包含组和排除组列表的导航属性。</span><span class="sxs-lookup"><span data-stu-id="39ba6-183">Navigation property to list of inclusion and exclusion groups to which the policy is deployed.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="39ba6-184">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="39ba6-184">JSON Representation</span></span>
<span data-ttu-id="39ba6-185">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="39ba6-185">Here is a JSON representation of the resource.</span></span>
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






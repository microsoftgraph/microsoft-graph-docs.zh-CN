---
title: targetedManagedAppConfiguration 资源类型
description: 用于将一组自定义设置按原样提供给目标安全组中的所有用户的配置
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f622aa6a4baac6eb301981b0413c199cf0e14136
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27913140"
---
# <a name="targetedmanagedappconfiguration-resource-type"></a><span data-ttu-id="176a0-103">targetedManagedAppConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="176a0-103">targetedManagedAppConfiguration resource type</span></span>

> <span data-ttu-id="176a0-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="176a0-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="176a0-105">用于将一组自定义设置按原样提供给目标安全组中的所有用户的配置</span><span class="sxs-lookup"><span data-stu-id="176a0-105">Configuration used to deliver a set of custom settings as-is to all users in the targeted security group</span></span>

<span data-ttu-id="176a0-106">继承自 [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="176a0-106">Inherits from [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="176a0-107">方法</span><span class="sxs-lookup"><span data-stu-id="176a0-107">Methods</span></span>
|<span data-ttu-id="176a0-108">方法</span><span class="sxs-lookup"><span data-stu-id="176a0-108">Method</span></span>|<span data-ttu-id="176a0-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="176a0-109">Return Type</span></span>|<span data-ttu-id="176a0-110">说明</span><span class="sxs-lookup"><span data-stu-id="176a0-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="176a0-111">List targetedManagedAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="176a0-111">List targetedManagedAppConfigurations</span></span>](../api/intune-mam-targetedmanagedappconfiguration-list.md)|<span data-ttu-id="176a0-112">[targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="176a0-112">[targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) collection</span></span>|<span data-ttu-id="176a0-113">列出 [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="176a0-113">List properties and relationships of the [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="176a0-114">Get targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="176a0-114">Get targetedManagedAppConfiguration</span></span>](../api/intune-mam-targetedmanagedappconfiguration-get.md)|[<span data-ttu-id="176a0-115">targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="176a0-115">targetedManagedAppConfiguration</span></span>](../resources/intune-mam-targetedmanagedappconfiguration.md)|<span data-ttu-id="176a0-116">读取 [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="176a0-116">Read properties and relationships of the [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>|
|[<span data-ttu-id="176a0-117">Create targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="176a0-117">Create targetedManagedAppConfiguration</span></span>](../api/intune-mam-targetedmanagedappconfiguration-create.md)|[<span data-ttu-id="176a0-118">targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="176a0-118">targetedManagedAppConfiguration</span></span>](../resources/intune-mam-targetedmanagedappconfiguration.md)|<span data-ttu-id="176a0-119">创建新的 [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="176a0-119">Create a new [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>|
|[<span data-ttu-id="176a0-120">Delete targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="176a0-120">Delete targetedManagedAppConfiguration</span></span>](../api/intune-mam-targetedmanagedappconfiguration-delete.md)|<span data-ttu-id="176a0-121">无</span><span class="sxs-lookup"><span data-stu-id="176a0-121">None</span></span>|<span data-ttu-id="176a0-122">删除 [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="176a0-122">Deletes a [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md).</span></span>|
|[<span data-ttu-id="176a0-123">Update targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="176a0-123">Update targetedManagedAppConfiguration</span></span>](../api/intune-mam-targetedmanagedappconfiguration-update.md)|[<span data-ttu-id="176a0-124">targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="176a0-124">targetedManagedAppConfiguration</span></span>](../resources/intune-mam-targetedmanagedappconfiguration.md)|<span data-ttu-id="176a0-125">更新 [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="176a0-125">Update the properties of a [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>|
|[<span data-ttu-id="176a0-126">assign 操作</span><span class="sxs-lookup"><span data-stu-id="176a0-126">assign action</span></span>](../api/intune-mam-targetedmanagedappconfiguration-assign.md)|<span data-ttu-id="176a0-127">无</span><span class="sxs-lookup"><span data-stu-id="176a0-127">None</span></span>|<span data-ttu-id="176a0-128">尚未记录</span><span class="sxs-lookup"><span data-stu-id="176a0-128">Not yet documented</span></span>|
|[<span data-ttu-id="176a0-129">targetApps 操作</span><span class="sxs-lookup"><span data-stu-id="176a0-129">targetApps action</span></span>](../api/intune-mam-targetedmanagedappconfiguration-targetapps.md)|<span data-ttu-id="176a0-130">无</span><span class="sxs-lookup"><span data-stu-id="176a0-130">None</span></span>|<span data-ttu-id="176a0-131">尚未记录</span><span class="sxs-lookup"><span data-stu-id="176a0-131">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="176a0-132">属性</span><span class="sxs-lookup"><span data-stu-id="176a0-132">Properties</span></span>
|<span data-ttu-id="176a0-133">属性</span><span class="sxs-lookup"><span data-stu-id="176a0-133">Property</span></span>|<span data-ttu-id="176a0-134">类型</span><span class="sxs-lookup"><span data-stu-id="176a0-134">Type</span></span>|<span data-ttu-id="176a0-135">说明</span><span class="sxs-lookup"><span data-stu-id="176a0-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="176a0-136">displayName</span><span class="sxs-lookup"><span data-stu-id="176a0-136">displayName</span></span>|<span data-ttu-id="176a0-137">String</span><span class="sxs-lookup"><span data-stu-id="176a0-137">String</span></span>|<span data-ttu-id="176a0-138">策略显示名称。</span><span class="sxs-lookup"><span data-stu-id="176a0-138">Policy display name.</span></span> <span data-ttu-id="176a0-139">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="176a0-139">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="176a0-140">description</span><span class="sxs-lookup"><span data-stu-id="176a0-140">description</span></span>|<span data-ttu-id="176a0-141">String</span><span class="sxs-lookup"><span data-stu-id="176a0-141">String</span></span>|<span data-ttu-id="176a0-142">策略的说明。</span><span class="sxs-lookup"><span data-stu-id="176a0-142">The policy's description.</span></span> <span data-ttu-id="176a0-143">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="176a0-143">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="176a0-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="176a0-144">createdDateTime</span></span>|<span data-ttu-id="176a0-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="176a0-145">DateTimeOffset</span></span>|<span data-ttu-id="176a0-146">创建策略的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="176a0-146">The date and time the policy was created.</span></span> <span data-ttu-id="176a0-147">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="176a0-147">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="176a0-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="176a0-148">lastModifiedDateTime</span></span>|<span data-ttu-id="176a0-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="176a0-149">DateTimeOffset</span></span>|<span data-ttu-id="176a0-150">上次修改策略的时间。</span><span class="sxs-lookup"><span data-stu-id="176a0-150">Last time the policy was modified.</span></span> <span data-ttu-id="176a0-151">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="176a0-151">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="176a0-152">id</span><span class="sxs-lookup"><span data-stu-id="176a0-152">id</span></span>|<span data-ttu-id="176a0-153">String</span><span class="sxs-lookup"><span data-stu-id="176a0-153">String</span></span>|<span data-ttu-id="176a0-154">实体的键。</span><span class="sxs-lookup"><span data-stu-id="176a0-154">Key of the entity.</span></span> <span data-ttu-id="176a0-155">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="176a0-155">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="176a0-156">version</span><span class="sxs-lookup"><span data-stu-id="176a0-156">version</span></span>|<span data-ttu-id="176a0-157">String</span><span class="sxs-lookup"><span data-stu-id="176a0-157">String</span></span>|<span data-ttu-id="176a0-158">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="176a0-158">Version of the entity.</span></span> <span data-ttu-id="176a0-159">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="176a0-159">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="176a0-160">customSettings</span><span class="sxs-lookup"><span data-stu-id="176a0-160">customSettings</span></span>|<span data-ttu-id="176a0-161">[keyValuePair](../resources/intune-mam-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="176a0-161">[keyValuePair](../resources/intune-mam-keyvaluepair.md) collection</span></span>|<span data-ttu-id="176a0-162">要发送到配置范围确定的用户应用的一组字符串键和字符串值对，不由此服务更改。继承自 [ managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="176a0-162">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service Inherited from [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span></span>|
|<span data-ttu-id="176a0-163">deployedAppCount</span><span class="sxs-lookup"><span data-stu-id="176a0-163">deployedAppCount</span></span>|<span data-ttu-id="176a0-164">Int32</span><span class="sxs-lookup"><span data-stu-id="176a0-164">Int32</span></span>|<span data-ttu-id="176a0-165">当前策略部署到的应用的计数。</span><span class="sxs-lookup"><span data-stu-id="176a0-165">Count of apps to which the current policy is deployed.</span></span>|
|<span data-ttu-id="176a0-166">isAssigned</span><span class="sxs-lookup"><span data-stu-id="176a0-166">isAssigned</span></span>|<span data-ttu-id="176a0-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="176a0-167">Boolean</span></span>|<span data-ttu-id="176a0-168">指示策略是否部署到任何包含组。</span><span class="sxs-lookup"><span data-stu-id="176a0-168">Indicates if the policy is deployed to any inclusion groups or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="176a0-169">关系</span><span class="sxs-lookup"><span data-stu-id="176a0-169">Relationships</span></span>
|<span data-ttu-id="176a0-170">关系</span><span class="sxs-lookup"><span data-stu-id="176a0-170">Relationship</span></span>|<span data-ttu-id="176a0-171">类型</span><span class="sxs-lookup"><span data-stu-id="176a0-171">Type</span></span>|<span data-ttu-id="176a0-172">说明</span><span class="sxs-lookup"><span data-stu-id="176a0-172">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="176a0-173">apps</span><span class="sxs-lookup"><span data-stu-id="176a0-173">apps</span></span>|<span data-ttu-id="176a0-174">[managedMobileApp](../resources/intune-mam-managedmobileapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="176a0-174">[managedMobileApp](../resources/intune-mam-managedmobileapp.md) collection</span></span>|<span data-ttu-id="176a0-175">策略部署到的应用的列表。</span><span class="sxs-lookup"><span data-stu-id="176a0-175">List of apps to which the policy is deployed.</span></span>|
|<span data-ttu-id="176a0-176">deploymentSummary</span><span class="sxs-lookup"><span data-stu-id="176a0-176">deploymentSummary</span></span>|[<span data-ttu-id="176a0-177">managedAppPolicyDeploymentSummary</span><span class="sxs-lookup"><span data-stu-id="176a0-177">managedAppPolicyDeploymentSummary</span></span>](../resources/intune-mam-managedapppolicydeploymentsummary.md)|<span data-ttu-id="176a0-178">配置的部署摘要的导航属性。</span><span class="sxs-lookup"><span data-stu-id="176a0-178">Navigation property to deployment summary of the configuration.</span></span>|
|<span data-ttu-id="176a0-179">assignments</span><span class="sxs-lookup"><span data-stu-id="176a0-179">assignments</span></span>|<span data-ttu-id="176a0-180">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="176a0-180">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) collection</span></span>|<span data-ttu-id="176a0-181">策略部署到的包含组和排除组列表的导航属性。</span><span class="sxs-lookup"><span data-stu-id="176a0-181">Navigation property to list of inclusion and exclusion groups to which the policy is deployed.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="176a0-182">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="176a0-182">JSON Representation</span></span>
<span data-ttu-id="176a0-183">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="176a0-183">Here is a JSON representation of the resource.</span></span>
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




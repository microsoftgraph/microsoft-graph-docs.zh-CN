---
title: targetedManagedAppConfiguration 资源类型
description: 用于将一组自定义设置按原样提供给目标安全组中的所有用户的配置
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 771265d8fef141e6803e22d594da90d47a7c7742
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27961783"
---
# <a name="targetedmanagedappconfiguration-resource-type"></a><span data-ttu-id="d8448-103">targetedManagedAppConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="d8448-103">targetedManagedAppConfiguration resource type</span></span>

> <span data-ttu-id="d8448-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="d8448-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d8448-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d8448-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d8448-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="d8448-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d8448-107">用于将一组自定义设置按原样提供给目标安全组中的所有用户的配置</span><span class="sxs-lookup"><span data-stu-id="d8448-107">Configuration used to deliver a set of custom settings as-is to all users in the targeted security group</span></span>

<span data-ttu-id="d8448-108">继承自 [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d8448-108">Inherits from [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="d8448-109">方法</span><span class="sxs-lookup"><span data-stu-id="d8448-109">Methods</span></span>
|<span data-ttu-id="d8448-110">方法</span><span class="sxs-lookup"><span data-stu-id="d8448-110">Method</span></span>|<span data-ttu-id="d8448-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="d8448-111">Return Type</span></span>|<span data-ttu-id="d8448-112">说明</span><span class="sxs-lookup"><span data-stu-id="d8448-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d8448-113">List targetedManagedAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="d8448-113">List targetedManagedAppConfigurations</span></span>](../api/intune-mam-targetedmanagedappconfiguration-list.md)|<span data-ttu-id="d8448-114">[targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d8448-114">[targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) collection</span></span>|<span data-ttu-id="d8448-115">列出 [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d8448-115">List properties and relationships of the [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="d8448-116">Get targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="d8448-116">Get targetedManagedAppConfiguration</span></span>](../api/intune-mam-targetedmanagedappconfiguration-get.md)|[<span data-ttu-id="d8448-117">targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="d8448-117">targetedManagedAppConfiguration</span></span>](../resources/intune-mam-targetedmanagedappconfiguration.md)|<span data-ttu-id="d8448-118">读取 [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d8448-118">Read properties and relationships of the [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>|
|[<span data-ttu-id="d8448-119">Create targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="d8448-119">Create targetedManagedAppConfiguration</span></span>](../api/intune-mam-targetedmanagedappconfiguration-create.md)|[<span data-ttu-id="d8448-120">targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="d8448-120">targetedManagedAppConfiguration</span></span>](../resources/intune-mam-targetedmanagedappconfiguration.md)|<span data-ttu-id="d8448-121">创建新的 [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d8448-121">Create a new [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>|
|[<span data-ttu-id="d8448-122">Delete targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="d8448-122">Delete targetedManagedAppConfiguration</span></span>](../api/intune-mam-targetedmanagedappconfiguration-delete.md)|<span data-ttu-id="d8448-123">无</span><span class="sxs-lookup"><span data-stu-id="d8448-123">None</span></span>|<span data-ttu-id="d8448-124">删除 [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="d8448-124">Deletes a [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md).</span></span>|
|[<span data-ttu-id="d8448-125">Update targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="d8448-125">Update targetedManagedAppConfiguration</span></span>](../api/intune-mam-targetedmanagedappconfiguration-update.md)|[<span data-ttu-id="d8448-126">targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="d8448-126">targetedManagedAppConfiguration</span></span>](../resources/intune-mam-targetedmanagedappconfiguration.md)|<span data-ttu-id="d8448-127">更新 [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d8448-127">Update the properties of a [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>|
|[<span data-ttu-id="d8448-128">assign 操作</span><span class="sxs-lookup"><span data-stu-id="d8448-128">assign action</span></span>](../api/intune-mam-targetedmanagedappconfiguration-assign.md)|<span data-ttu-id="d8448-129">无</span><span class="sxs-lookup"><span data-stu-id="d8448-129">None</span></span>|<span data-ttu-id="d8448-130">尚未记录</span><span class="sxs-lookup"><span data-stu-id="d8448-130">Not yet documented</span></span>|
|[<span data-ttu-id="d8448-131">targetApps 操作</span><span class="sxs-lookup"><span data-stu-id="d8448-131">targetApps action</span></span>](../api/intune-mam-targetedmanagedappconfiguration-targetapps.md)|<span data-ttu-id="d8448-132">无</span><span class="sxs-lookup"><span data-stu-id="d8448-132">None</span></span>|<span data-ttu-id="d8448-133">尚未记录</span><span class="sxs-lookup"><span data-stu-id="d8448-133">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="d8448-134">属性</span><span class="sxs-lookup"><span data-stu-id="d8448-134">Properties</span></span>
|<span data-ttu-id="d8448-135">属性</span><span class="sxs-lookup"><span data-stu-id="d8448-135">Property</span></span>|<span data-ttu-id="d8448-136">类型</span><span class="sxs-lookup"><span data-stu-id="d8448-136">Type</span></span>|<span data-ttu-id="d8448-137">说明</span><span class="sxs-lookup"><span data-stu-id="d8448-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d8448-138">displayName</span><span class="sxs-lookup"><span data-stu-id="d8448-138">displayName</span></span>|<span data-ttu-id="d8448-139">String</span><span class="sxs-lookup"><span data-stu-id="d8448-139">String</span></span>|<span data-ttu-id="d8448-140">策略显示名称。</span><span class="sxs-lookup"><span data-stu-id="d8448-140">Policy display name.</span></span> <span data-ttu-id="d8448-141">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="d8448-141">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="d8448-142">description</span><span class="sxs-lookup"><span data-stu-id="d8448-142">description</span></span>|<span data-ttu-id="d8448-143">String</span><span class="sxs-lookup"><span data-stu-id="d8448-143">String</span></span>|<span data-ttu-id="d8448-144">策略的说明。</span><span class="sxs-lookup"><span data-stu-id="d8448-144">The policy's description.</span></span> <span data-ttu-id="d8448-145">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="d8448-145">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="d8448-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d8448-146">createdDateTime</span></span>|<span data-ttu-id="d8448-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d8448-147">DateTimeOffset</span></span>|<span data-ttu-id="d8448-148">创建策略的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="d8448-148">The date and time the policy was created.</span></span> <span data-ttu-id="d8448-149">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="d8448-149">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="d8448-150">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d8448-150">lastModifiedDateTime</span></span>|<span data-ttu-id="d8448-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d8448-151">DateTimeOffset</span></span>|<span data-ttu-id="d8448-152">上次修改策略的时间。</span><span class="sxs-lookup"><span data-stu-id="d8448-152">Last time the policy was modified.</span></span> <span data-ttu-id="d8448-153">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="d8448-153">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="d8448-154">id</span><span class="sxs-lookup"><span data-stu-id="d8448-154">id</span></span>|<span data-ttu-id="d8448-155">String</span><span class="sxs-lookup"><span data-stu-id="d8448-155">String</span></span>|<span data-ttu-id="d8448-156">实体的键。</span><span class="sxs-lookup"><span data-stu-id="d8448-156">Key of the entity.</span></span> <span data-ttu-id="d8448-157">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="d8448-157">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="d8448-158">version</span><span class="sxs-lookup"><span data-stu-id="d8448-158">version</span></span>|<span data-ttu-id="d8448-159">String</span><span class="sxs-lookup"><span data-stu-id="d8448-159">String</span></span>|<span data-ttu-id="d8448-160">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="d8448-160">Version of the entity.</span></span> <span data-ttu-id="d8448-161">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="d8448-161">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="d8448-162">customSettings</span><span class="sxs-lookup"><span data-stu-id="d8448-162">customSettings</span></span>|<span data-ttu-id="d8448-163">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d8448-163">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="d8448-164">要发送到配置范围确定的用户应用的一组字符串键和字符串值对，不由此服务更改。继承自 [ managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d8448-164">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service Inherited from [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span></span>|
|<span data-ttu-id="d8448-165">deployedAppCount</span><span class="sxs-lookup"><span data-stu-id="d8448-165">deployedAppCount</span></span>|<span data-ttu-id="d8448-166">Int32</span><span class="sxs-lookup"><span data-stu-id="d8448-166">Int32</span></span>|<span data-ttu-id="d8448-167">当前策略部署到的应用的计数。</span><span class="sxs-lookup"><span data-stu-id="d8448-167">Count of apps to which the current policy is deployed.</span></span>|
|<span data-ttu-id="d8448-168">isAssigned</span><span class="sxs-lookup"><span data-stu-id="d8448-168">isAssigned</span></span>|<span data-ttu-id="d8448-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8448-169">Boolean</span></span>|<span data-ttu-id="d8448-170">指示策略是否部署到任何包含组。</span><span class="sxs-lookup"><span data-stu-id="d8448-170">Indicates if the policy is deployed to any inclusion groups or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d8448-171">关系</span><span class="sxs-lookup"><span data-stu-id="d8448-171">Relationships</span></span>
|<span data-ttu-id="d8448-172">关系</span><span class="sxs-lookup"><span data-stu-id="d8448-172">Relationship</span></span>|<span data-ttu-id="d8448-173">类型</span><span class="sxs-lookup"><span data-stu-id="d8448-173">Type</span></span>|<span data-ttu-id="d8448-174">说明</span><span class="sxs-lookup"><span data-stu-id="d8448-174">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d8448-175">apps</span><span class="sxs-lookup"><span data-stu-id="d8448-175">apps</span></span>|<span data-ttu-id="d8448-176">[managedMobileApp](../resources/intune-mam-managedmobileapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d8448-176">[managedMobileApp](../resources/intune-mam-managedmobileapp.md) collection</span></span>|<span data-ttu-id="d8448-177">策略部署到的应用的列表。</span><span class="sxs-lookup"><span data-stu-id="d8448-177">List of apps to which the policy is deployed.</span></span>|
|<span data-ttu-id="d8448-178">deploymentSummary</span><span class="sxs-lookup"><span data-stu-id="d8448-178">deploymentSummary</span></span>|[<span data-ttu-id="d8448-179">managedAppPolicyDeploymentSummary</span><span class="sxs-lookup"><span data-stu-id="d8448-179">managedAppPolicyDeploymentSummary</span></span>](../resources/intune-mam-managedapppolicydeploymentsummary.md)|<span data-ttu-id="d8448-180">配置的部署摘要的导航属性。</span><span class="sxs-lookup"><span data-stu-id="d8448-180">Navigation property to deployment summary of the configuration.</span></span>|
|<span data-ttu-id="d8448-181">assignments</span><span class="sxs-lookup"><span data-stu-id="d8448-181">assignments</span></span>|<span data-ttu-id="d8448-182">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d8448-182">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) collection</span></span>|<span data-ttu-id="d8448-183">策略部署到的包含组和排除组列表的导航属性。</span><span class="sxs-lookup"><span data-stu-id="d8448-183">Navigation property to list of inclusion and exclusion groups to which the policy is deployed.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d8448-184">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d8448-184">JSON Representation</span></span>
<span data-ttu-id="d8448-185">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d8448-185">Here is a JSON representation of the resource.</span></span>
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






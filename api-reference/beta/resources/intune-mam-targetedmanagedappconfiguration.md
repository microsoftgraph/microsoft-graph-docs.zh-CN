---
title: targetedManagedAppConfiguration 资源类型
description: 用于将一组自定义设置按原样提供给目标安全组中的所有用户的配置
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4fc64145d1c821360984656450dc82cc7e44efeb
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36010852"
---
# <a name="targetedmanagedappconfiguration-resource-type"></a><span data-ttu-id="12436-103">targetedManagedAppConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="12436-103">targetedManagedAppConfiguration resource type</span></span>

> <span data-ttu-id="12436-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="12436-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="12436-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="12436-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="12436-106">用于将一组自定义设置按原样提供给目标安全组中的所有用户的配置</span><span class="sxs-lookup"><span data-stu-id="12436-106">Configuration used to deliver a set of custom settings as-is to all users in the targeted security group</span></span>


<span data-ttu-id="12436-107">继承自 [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="12436-107">Inherits from [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="12436-108">方法</span><span class="sxs-lookup"><span data-stu-id="12436-108">Methods</span></span>
|<span data-ttu-id="12436-109">方法</span><span class="sxs-lookup"><span data-stu-id="12436-109">Method</span></span>|<span data-ttu-id="12436-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="12436-110">Return Type</span></span>|<span data-ttu-id="12436-111">说明</span><span class="sxs-lookup"><span data-stu-id="12436-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="12436-112">List targetedManagedAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="12436-112">List targetedManagedAppConfigurations</span></span>](../api/intune-mam-targetedmanagedappconfiguration-list.md)|<span data-ttu-id="12436-113">[targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="12436-113">[targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) collection</span></span>|<span data-ttu-id="12436-114">列出 [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="12436-114">List properties and relationships of the [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="12436-115">Get targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="12436-115">Get targetedManagedAppConfiguration</span></span>](../api/intune-mam-targetedmanagedappconfiguration-get.md)|[<span data-ttu-id="12436-116">targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="12436-116">targetedManagedAppConfiguration</span></span>](../resources/intune-mam-targetedmanagedappconfiguration.md)|<span data-ttu-id="12436-117">读取 [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="12436-117">Read properties and relationships of the [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>|
|[<span data-ttu-id="12436-118">Create targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="12436-118">Create targetedManagedAppConfiguration</span></span>](../api/intune-mam-targetedmanagedappconfiguration-create.md)|[<span data-ttu-id="12436-119">targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="12436-119">targetedManagedAppConfiguration</span></span>](../resources/intune-mam-targetedmanagedappconfiguration.md)|<span data-ttu-id="12436-120">创建新的 [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="12436-120">Create a new [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>|
|[<span data-ttu-id="12436-121">Delete targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="12436-121">Delete targetedManagedAppConfiguration</span></span>](../api/intune-mam-targetedmanagedappconfiguration-delete.md)|<span data-ttu-id="12436-122">无</span><span class="sxs-lookup"><span data-stu-id="12436-122">None</span></span>|<span data-ttu-id="12436-123">删除 [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="12436-123">Deletes a [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md).</span></span>|
|[<span data-ttu-id="12436-124">Update targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="12436-124">Update targetedManagedAppConfiguration</span></span>](../api/intune-mam-targetedmanagedappconfiguration-update.md)|[<span data-ttu-id="12436-125">targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="12436-125">targetedManagedAppConfiguration</span></span>](../resources/intune-mam-targetedmanagedappconfiguration.md)|<span data-ttu-id="12436-126">更新 [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="12436-126">Update the properties of a [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>|
|[<span data-ttu-id="12436-127">assign 操作</span><span class="sxs-lookup"><span data-stu-id="12436-127">assign action</span></span>](../api/intune-mam-targetedmanagedappconfiguration-assign.md)|<span data-ttu-id="12436-128">无</span><span class="sxs-lookup"><span data-stu-id="12436-128">None</span></span>|<span data-ttu-id="12436-129">尚未记录</span><span class="sxs-lookup"><span data-stu-id="12436-129">Not yet documented</span></span>|
|[<span data-ttu-id="12436-130">targetApps 操作</span><span class="sxs-lookup"><span data-stu-id="12436-130">targetApps action</span></span>](../api/intune-mam-targetedmanagedappconfiguration-targetapps.md)|<span data-ttu-id="12436-131">无</span><span class="sxs-lookup"><span data-stu-id="12436-131">None</span></span>|<span data-ttu-id="12436-132">尚未记录</span><span class="sxs-lookup"><span data-stu-id="12436-132">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="12436-133">属性</span><span class="sxs-lookup"><span data-stu-id="12436-133">Properties</span></span>
|<span data-ttu-id="12436-134">属性</span><span class="sxs-lookup"><span data-stu-id="12436-134">Property</span></span>|<span data-ttu-id="12436-135">类型</span><span class="sxs-lookup"><span data-stu-id="12436-135">Type</span></span>|<span data-ttu-id="12436-136">说明</span><span class="sxs-lookup"><span data-stu-id="12436-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="12436-137">displayName</span><span class="sxs-lookup"><span data-stu-id="12436-137">displayName</span></span>|<span data-ttu-id="12436-138">字符串</span><span class="sxs-lookup"><span data-stu-id="12436-138">String</span></span>|<span data-ttu-id="12436-139">策略显示名称。</span><span class="sxs-lookup"><span data-stu-id="12436-139">Policy display name.</span></span> <span data-ttu-id="12436-140">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="12436-140">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="12436-141">说明</span><span class="sxs-lookup"><span data-stu-id="12436-141">description</span></span>|<span data-ttu-id="12436-142">String</span><span class="sxs-lookup"><span data-stu-id="12436-142">String</span></span>|<span data-ttu-id="12436-143">策略的说明。</span><span class="sxs-lookup"><span data-stu-id="12436-143">The policy's description.</span></span> <span data-ttu-id="12436-144">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="12436-144">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="12436-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="12436-145">createdDateTime</span></span>|<span data-ttu-id="12436-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="12436-146">DateTimeOffset</span></span>|<span data-ttu-id="12436-147">创建策略的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="12436-147">The date and time the policy was created.</span></span> <span data-ttu-id="12436-148">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="12436-148">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="12436-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="12436-149">lastModifiedDateTime</span></span>|<span data-ttu-id="12436-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="12436-150">DateTimeOffset</span></span>|<span data-ttu-id="12436-151">上次修改策略的时间。</span><span class="sxs-lookup"><span data-stu-id="12436-151">Last time the policy was modified.</span></span> <span data-ttu-id="12436-152">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="12436-152">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="12436-153">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="12436-153">roleScopeTagIds</span></span>|<span data-ttu-id="12436-154">String collection</span><span class="sxs-lookup"><span data-stu-id="12436-154">String collection</span></span>|<span data-ttu-id="12436-155">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="12436-155">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="12436-156">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="12436-156">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="12436-157">id</span><span class="sxs-lookup"><span data-stu-id="12436-157">id</span></span>|<span data-ttu-id="12436-158">字符串</span><span class="sxs-lookup"><span data-stu-id="12436-158">String</span></span>|<span data-ttu-id="12436-159">实体的键。</span><span class="sxs-lookup"><span data-stu-id="12436-159">Key of the entity.</span></span> <span data-ttu-id="12436-160">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="12436-160">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="12436-161">version</span><span class="sxs-lookup"><span data-stu-id="12436-161">version</span></span>|<span data-ttu-id="12436-162">String</span><span class="sxs-lookup"><span data-stu-id="12436-162">String</span></span>|<span data-ttu-id="12436-163">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="12436-163">Version of the entity.</span></span> <span data-ttu-id="12436-164">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="12436-164">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="12436-165">customSettings</span><span class="sxs-lookup"><span data-stu-id="12436-165">customSettings</span></span>|<span data-ttu-id="12436-166">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="12436-166">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="12436-167">要发送到配置范围确定的用户应用的一组字符串键和字符串值对，不由此服务更改。继承自 [ managedAppConfiguration ](../resources/intune-mam-managedappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="12436-167">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service Inherited from [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span></span>|
|<span data-ttu-id="12436-168">deployedAppCount</span><span class="sxs-lookup"><span data-stu-id="12436-168">deployedAppCount</span></span>|<span data-ttu-id="12436-169">Int32</span><span class="sxs-lookup"><span data-stu-id="12436-169">Int32</span></span>|<span data-ttu-id="12436-170">当前策略部署到的应用的计数。</span><span class="sxs-lookup"><span data-stu-id="12436-170">Count of apps to which the current policy is deployed.</span></span>|
|<span data-ttu-id="12436-171">isAssigned</span><span class="sxs-lookup"><span data-stu-id="12436-171">isAssigned</span></span>|<span data-ttu-id="12436-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="12436-172">Boolean</span></span>|<span data-ttu-id="12436-173">指示策略是否部署到任何包含组。</span><span class="sxs-lookup"><span data-stu-id="12436-173">Indicates if the policy is deployed to any inclusion groups or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="12436-174">关系</span><span class="sxs-lookup"><span data-stu-id="12436-174">Relationships</span></span>
|<span data-ttu-id="12436-175">关系</span><span class="sxs-lookup"><span data-stu-id="12436-175">Relationship</span></span>|<span data-ttu-id="12436-176">类型</span><span class="sxs-lookup"><span data-stu-id="12436-176">Type</span></span>|<span data-ttu-id="12436-177">说明</span><span class="sxs-lookup"><span data-stu-id="12436-177">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="12436-178">apps</span><span class="sxs-lookup"><span data-stu-id="12436-178">apps</span></span>|<span data-ttu-id="12436-179">[managedMobileApp](../resources/intune-mam-managedmobileapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="12436-179">[managedMobileApp](../resources/intune-mam-managedmobileapp.md) collection</span></span>|<span data-ttu-id="12436-180">策略部署到的应用的列表。</span><span class="sxs-lookup"><span data-stu-id="12436-180">List of apps to which the policy is deployed.</span></span>|
|<span data-ttu-id="12436-181">deploymentSummary</span><span class="sxs-lookup"><span data-stu-id="12436-181">deploymentSummary</span></span>|[<span data-ttu-id="12436-182">managedAppPolicyDeploymentSummary</span><span class="sxs-lookup"><span data-stu-id="12436-182">managedAppPolicyDeploymentSummary</span></span>](../resources/intune-mam-managedapppolicydeploymentsummary.md)|<span data-ttu-id="12436-183">配置的部署摘要的导航属性。</span><span class="sxs-lookup"><span data-stu-id="12436-183">Navigation property to deployment summary of the configuration.</span></span>|
|<span data-ttu-id="12436-184">assignments</span><span class="sxs-lookup"><span data-stu-id="12436-184">assignments</span></span>|<span data-ttu-id="12436-185">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="12436-185">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) collection</span></span>|<span data-ttu-id="12436-186">策略部署到的包含组和排除组列表的导航属性。</span><span class="sxs-lookup"><span data-stu-id="12436-186">Navigation property to list of inclusion and exclusion groups to which the policy is deployed.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="12436-187">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="12436-187">JSON Representation</span></span>
<span data-ttu-id="12436-188">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="12436-188">Here is a JSON representation of the resource.</span></span>
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






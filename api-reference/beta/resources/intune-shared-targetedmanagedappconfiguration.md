---
title: targetedManagedAppConfiguration 资源类型
description: 用于将一组自定义设置按原样提供给目标安全组中的所有用户的配置
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4b02a254598e0adb9622999f4eb3fe03a63a3ba6
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49255810"
---
# <a name="targetedmanagedappconfiguration-resource-type"></a><span data-ttu-id="b121a-103">targetedManagedAppConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="b121a-103">targetedManagedAppConfiguration resource type</span></span>

<span data-ttu-id="b121a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b121a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b121a-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b121a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b121a-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b121a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b121a-107">用于将一组自定义设置按原样提供给目标安全组中的所有用户的配置</span><span class="sxs-lookup"><span data-stu-id="b121a-107">Configuration used to deliver a set of custom settings as-is to all users in the targeted security group</span></span>


<span data-ttu-id="b121a-108">继承自 [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b121a-108">Inherits from [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="b121a-109">方法</span><span class="sxs-lookup"><span data-stu-id="b121a-109">Methods</span></span>
|<span data-ttu-id="b121a-110">方法</span><span class="sxs-lookup"><span data-stu-id="b121a-110">Method</span></span>|<span data-ttu-id="b121a-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="b121a-111">Return Type</span></span>|<span data-ttu-id="b121a-112">说明</span><span class="sxs-lookup"><span data-stu-id="b121a-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b121a-113">List targetedManagedAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="b121a-113">List targetedManagedAppConfigurations</span></span>](../api/intune-shared-targetedmanagedappconfiguration-list.md)|<span data-ttu-id="b121a-114">[targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b121a-114">[targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) collection</span></span>|<span data-ttu-id="b121a-115">列出 [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b121a-115">List properties and relationships of the [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="b121a-116">Get targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="b121a-116">Get targetedManagedAppConfiguration</span></span>](../api/intune-shared-targetedmanagedappconfiguration-get.md)|[<span data-ttu-id="b121a-117">targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="b121a-117">targetedManagedAppConfiguration</span></span>](../resources/intune-shared-targetedmanagedappconfiguration.md)|<span data-ttu-id="b121a-118">读取 [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b121a-118">Read properties and relationships of the [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) object.</span></span>|
|[<span data-ttu-id="b121a-119">Create targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="b121a-119">Create targetedManagedAppConfiguration</span></span>](../api/intune-shared-targetedmanagedappconfiguration-create.md)|[<span data-ttu-id="b121a-120">targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="b121a-120">targetedManagedAppConfiguration</span></span>](../resources/intune-shared-targetedmanagedappconfiguration.md)|<span data-ttu-id="b121a-121">创建新的 [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b121a-121">Create a new [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) object.</span></span>|
|[<span data-ttu-id="b121a-122">Delete targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="b121a-122">Delete targetedManagedAppConfiguration</span></span>](../api/intune-shared-targetedmanagedappconfiguration-delete.md)|<span data-ttu-id="b121a-123">无</span><span class="sxs-lookup"><span data-stu-id="b121a-123">None</span></span>|<span data-ttu-id="b121a-124">删除 [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="b121a-124">Deletes a [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md).</span></span>|
|[<span data-ttu-id="b121a-125">Update targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="b121a-125">Update targetedManagedAppConfiguration</span></span>](../api/intune-shared-targetedmanagedappconfiguration-update.md)|[<span data-ttu-id="b121a-126">targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="b121a-126">targetedManagedAppConfiguration</span></span>](../resources/intune-shared-targetedmanagedappconfiguration.md)|<span data-ttu-id="b121a-127">更新 [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b121a-127">Update the properties of a [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) object.</span></span>|
|<span data-ttu-id="b121a-128">**移动应用管理 (MAM)**</span><span class="sxs-lookup"><span data-stu-id="b121a-128">**Mobile app management (MAM)**</span></span>|
|[<span data-ttu-id="b121a-129">分配操作</span><span class="sxs-lookup"><span data-stu-id="b121a-129">assign action</span></span>](../api/intune-shared-targetedmanagedappconfiguration-assign.md)|<span data-ttu-id="b121a-130">无</span><span class="sxs-lookup"><span data-stu-id="b121a-130">None</span></span>|<span data-ttu-id="b121a-131">尚未记录</span><span class="sxs-lookup"><span data-stu-id="b121a-131">Not yet documented</span></span>|
|[<span data-ttu-id="b121a-132">targetApps 操作</span><span class="sxs-lookup"><span data-stu-id="b121a-132">targetApps action</span></span>](../api/intune-shared-targetedmanagedappconfiguration-targetapps.md)|<span data-ttu-id="b121a-133">无</span><span class="sxs-lookup"><span data-stu-id="b121a-133">None</span></span>|<span data-ttu-id="b121a-134">尚未记录</span><span class="sxs-lookup"><span data-stu-id="b121a-134">Not yet documented</span></span>|
|<span data-ttu-id="b121a-135">**策略集**</span><span class="sxs-lookup"><span data-stu-id="b121a-135">**Policy Set**</span></span>|
|[<span data-ttu-id="b121a-136">hasPayloadLinks 操作</span><span class="sxs-lookup"><span data-stu-id="b121a-136">hasPayloadLinks action</span></span>](../api/intune-shared-targetedmanagedappconfiguration-haspayloadlinks.md)|<span data-ttu-id="b121a-137">[hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b121a-137">[hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md) collection</span></span>|<span data-ttu-id="b121a-138">尚未记录</span><span class="sxs-lookup"><span data-stu-id="b121a-138">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="b121a-139">属性</span><span class="sxs-lookup"><span data-stu-id="b121a-139">Properties</span></span>
|<span data-ttu-id="b121a-140">属性</span><span class="sxs-lookup"><span data-stu-id="b121a-140">Property</span></span>|<span data-ttu-id="b121a-141">类型</span><span class="sxs-lookup"><span data-stu-id="b121a-141">Type</span></span>|<span data-ttu-id="b121a-142">说明</span><span class="sxs-lookup"><span data-stu-id="b121a-142">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b121a-143">id</span><span class="sxs-lookup"><span data-stu-id="b121a-143">id</span></span>|<span data-ttu-id="b121a-144">String</span><span class="sxs-lookup"><span data-stu-id="b121a-144">String</span></span>|<span data-ttu-id="b121a-145">实体的键。</span><span class="sxs-lookup"><span data-stu-id="b121a-145">Key of the entity.</span></span> <span data-ttu-id="b121a-146">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="b121a-146">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="b121a-147">displayName</span><span class="sxs-lookup"><span data-stu-id="b121a-147">displayName</span></span>|<span data-ttu-id="b121a-148">String</span><span class="sxs-lookup"><span data-stu-id="b121a-148">String</span></span>|<span data-ttu-id="b121a-149">策略显示名称。</span><span class="sxs-lookup"><span data-stu-id="b121a-149">Policy display name.</span></span> <span data-ttu-id="b121a-150">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="b121a-150">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="b121a-151">description</span><span class="sxs-lookup"><span data-stu-id="b121a-151">description</span></span>|<span data-ttu-id="b121a-152">String</span><span class="sxs-lookup"><span data-stu-id="b121a-152">String</span></span>|<span data-ttu-id="b121a-153">策略的说明。</span><span class="sxs-lookup"><span data-stu-id="b121a-153">The policy's description.</span></span> <span data-ttu-id="b121a-154">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="b121a-154">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="b121a-155">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b121a-155">createdDateTime</span></span>|<span data-ttu-id="b121a-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b121a-156">DateTimeOffset</span></span>|<span data-ttu-id="b121a-157">创建策略的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="b121a-157">The date and time the policy was created.</span></span> <span data-ttu-id="b121a-158">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="b121a-158">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="b121a-159">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b121a-159">lastModifiedDateTime</span></span>|<span data-ttu-id="b121a-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b121a-160">DateTimeOffset</span></span>|<span data-ttu-id="b121a-161">上次修改策略的时间。</span><span class="sxs-lookup"><span data-stu-id="b121a-161">Last time the policy was modified.</span></span> <span data-ttu-id="b121a-162">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="b121a-162">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="b121a-163">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b121a-163">roleScopeTagIds</span></span>|<span data-ttu-id="b121a-164">String 集合</span><span class="sxs-lookup"><span data-stu-id="b121a-164">String collection</span></span>|<span data-ttu-id="b121a-165">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="b121a-165">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="b121a-166">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="b121a-166">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="b121a-167">version</span><span class="sxs-lookup"><span data-stu-id="b121a-167">version</span></span>|<span data-ttu-id="b121a-168">String</span><span class="sxs-lookup"><span data-stu-id="b121a-168">String</span></span>|<span data-ttu-id="b121a-169">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="b121a-169">Version of the entity.</span></span> <span data-ttu-id="b121a-170">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="b121a-170">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="b121a-171">customSettings</span><span class="sxs-lookup"><span data-stu-id="b121a-171">customSettings</span></span>|<span data-ttu-id="b121a-172">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b121a-172">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="b121a-173">要发送到配置范围确定的用户应用的一组字符串键和字符串值对，不由此服务更改。继承自 [ managedAppConfiguration ](../resources/intune-mam-managedappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b121a-173">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service Inherited from [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span></span>|
|<span data-ttu-id="b121a-174">deployedAppCount</span><span class="sxs-lookup"><span data-stu-id="b121a-174">deployedAppCount</span></span>|<span data-ttu-id="b121a-175">Int32</span><span class="sxs-lookup"><span data-stu-id="b121a-175">Int32</span></span>|<span data-ttu-id="b121a-176">当前策略部署到的应用的计数。</span><span class="sxs-lookup"><span data-stu-id="b121a-176">Count of apps to which the current policy is deployed.</span></span>|
|<span data-ttu-id="b121a-177">isAssigned</span><span class="sxs-lookup"><span data-stu-id="b121a-177">isAssigned</span></span>|<span data-ttu-id="b121a-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="b121a-178">Boolean</span></span>|<span data-ttu-id="b121a-179">指示策略是否部署到任何包含组。</span><span class="sxs-lookup"><span data-stu-id="b121a-179">Indicates if the policy is deployed to any inclusion groups or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b121a-180">关系</span><span class="sxs-lookup"><span data-stu-id="b121a-180">Relationships</span></span>
|<span data-ttu-id="b121a-181">关系</span><span class="sxs-lookup"><span data-stu-id="b121a-181">Relationship</span></span>|<span data-ttu-id="b121a-182">类型</span><span class="sxs-lookup"><span data-stu-id="b121a-182">Type</span></span>|<span data-ttu-id="b121a-183">描述</span><span class="sxs-lookup"><span data-stu-id="b121a-183">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b121a-184">**移动应用管理 (MAM)**</span><span class="sxs-lookup"><span data-stu-id="b121a-184">**Mobile app management (MAM)**</span></span>|
|<span data-ttu-id="b121a-185">apps</span><span class="sxs-lookup"><span data-stu-id="b121a-185">apps</span></span>|<span data-ttu-id="b121a-186">[managedMobileApp](../resources/intune-mam-managedmobileapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b121a-186">[managedMobileApp](../resources/intune-mam-managedmobileapp.md) collection</span></span>|<span data-ttu-id="b121a-187">策略部署到的应用的列表。</span><span class="sxs-lookup"><span data-stu-id="b121a-187">List of apps to which the policy is deployed.</span></span>|
|<span data-ttu-id="b121a-188">deploymentSummary</span><span class="sxs-lookup"><span data-stu-id="b121a-188">deploymentSummary</span></span>|[<span data-ttu-id="b121a-189">managedAppPolicyDeploymentSummary</span><span class="sxs-lookup"><span data-stu-id="b121a-189">managedAppPolicyDeploymentSummary</span></span>](../resources/intune-mam-managedapppolicydeploymentsummary.md)|<span data-ttu-id="b121a-190">配置的部署摘要的导航属性。</span><span class="sxs-lookup"><span data-stu-id="b121a-190">Navigation property to deployment summary of the configuration.</span></span>|
|<span data-ttu-id="b121a-191">assignments</span><span class="sxs-lookup"><span data-stu-id="b121a-191">assignments</span></span>|<span data-ttu-id="b121a-192">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b121a-192">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) collection</span></span>|<span data-ttu-id="b121a-193">策略部署到的包含组和排除组列表的导航属性。</span><span class="sxs-lookup"><span data-stu-id="b121a-193">Navigation property to list of inclusion and exclusion groups to which the policy is deployed.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b121a-194">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b121a-194">JSON Representation</span></span>
<span data-ttu-id="b121a-195">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b121a-195">Here is a JSON representation of the resource.</span></span>
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





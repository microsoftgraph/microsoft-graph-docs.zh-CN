---
title: officeClientConfiguration 资源类型
description: Office 客户端配置。
localization_priority: Normal
author: dougeby
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7dfe98bae90f0534c915577f3195d27e3071a4b0
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43465276"
---
# <a name="officeclientconfiguration-resource-type"></a><span data-ttu-id="3058e-103">officeClientConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="3058e-103">officeClientConfiguration resource type</span></span>

<span data-ttu-id="3058e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3058e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3058e-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3058e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3058e-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3058e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3058e-107">Office 客户端配置。</span><span class="sxs-lookup"><span data-stu-id="3058e-107">Office Client Configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="3058e-108">方法</span><span class="sxs-lookup"><span data-stu-id="3058e-108">Methods</span></span>
|<span data-ttu-id="3058e-109">方法</span><span class="sxs-lookup"><span data-stu-id="3058e-109">Method</span></span>|<span data-ttu-id="3058e-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="3058e-110">Return Type</span></span>|<span data-ttu-id="3058e-111">说明</span><span class="sxs-lookup"><span data-stu-id="3058e-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="3058e-112">列出 officeClientConfigurations</span><span class="sxs-lookup"><span data-stu-id="3058e-112">List officeClientConfigurations</span></span>](../api/intune-cirrus-officeclientconfiguration-list.md)|<span data-ttu-id="3058e-113">[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)集合</span><span class="sxs-lookup"><span data-stu-id="3058e-113">[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) collection</span></span>|<span data-ttu-id="3058e-114">列出[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="3058e-114">List properties and relationships of the [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="3058e-115">获取 officeClientConfiguration</span><span class="sxs-lookup"><span data-stu-id="3058e-115">Get officeClientConfiguration</span></span>](../api/intune-cirrus-officeclientconfiguration-get.md)|[<span data-ttu-id="3058e-116">officeClientConfiguration</span><span class="sxs-lookup"><span data-stu-id="3058e-116">officeClientConfiguration</span></span>](../resources/intune-cirrus-officeclientconfiguration.md)|<span data-ttu-id="3058e-117">读取[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="3058e-117">Read properties and relationships of the [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) object.</span></span>|
|[<span data-ttu-id="3058e-118">分配操作</span><span class="sxs-lookup"><span data-stu-id="3058e-118">assign action</span></span>](../api/intune-cirrus-officeclientconfiguration-assign.md)|<span data-ttu-id="3058e-119">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="3058e-119">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) collection</span></span>|<span data-ttu-id="3058e-120">替换策略的所有目标组。</span><span class="sxs-lookup"><span data-stu-id="3058e-120">Replace all targeted groups for a policy.</span></span>|
|[<span data-ttu-id="3058e-121">updatePriorities 操作</span><span class="sxs-lookup"><span data-stu-id="3058e-121">updatePriorities action</span></span>](../api/intune-cirrus-officeclientconfiguration-updatepriorities.md)|<span data-ttu-id="3058e-122">无</span><span class="sxs-lookup"><span data-stu-id="3058e-122">None</span></span>|<span data-ttu-id="3058e-123">更新策略优先级。</span><span class="sxs-lookup"><span data-stu-id="3058e-123">Update policy priorities.</span></span>|

## <a name="properties"></a><span data-ttu-id="3058e-124">属性</span><span class="sxs-lookup"><span data-stu-id="3058e-124">Properties</span></span>
|<span data-ttu-id="3058e-125">属性</span><span class="sxs-lookup"><span data-stu-id="3058e-125">Property</span></span>|<span data-ttu-id="3058e-126">类型</span><span class="sxs-lookup"><span data-stu-id="3058e-126">Type</span></span>|<span data-ttu-id="3058e-127">说明</span><span class="sxs-lookup"><span data-stu-id="3058e-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3058e-128">id</span><span class="sxs-lookup"><span data-stu-id="3058e-128">id</span></span>|<span data-ttu-id="3058e-129">字符串</span><span class="sxs-lookup"><span data-stu-id="3058e-129">String</span></span>|<span data-ttu-id="3058e-130">Office 客户端配置策略的 Id。</span><span class="sxs-lookup"><span data-stu-id="3058e-130">Id of the office client configuration policy.</span></span>|
|<span data-ttu-id="3058e-131">userPreferencePayload</span><span class="sxs-lookup"><span data-stu-id="3058e-131">userPreferencePayload</span></span>|<span data-ttu-id="3058e-132">Stream</span><span class="sxs-lookup"><span data-stu-id="3058e-132">Stream</span></span>|<span data-ttu-id="3058e-133">首选项设置 JSON string 二进制格式，则用户可以重写这些值。</span><span class="sxs-lookup"><span data-stu-id="3058e-133">Preference settings JSON string in binary format, these values can be overridden by the user.</span></span>|
|<span data-ttu-id="3058e-134">policyPayload</span><span class="sxs-lookup"><span data-stu-id="3058e-134">policyPayload</span></span>|<span data-ttu-id="3058e-135">Stream</span><span class="sxs-lookup"><span data-stu-id="3058e-135">Stream</span></span>|<span data-ttu-id="3058e-136">策略设置 JSON string 二进制格式，用户不能更改这些值。</span><span class="sxs-lookup"><span data-stu-id="3058e-136">Policy settings JSON string in binary format, these values cannot be changed by the user.</span></span>|
|<span data-ttu-id="3058e-137">description</span><span class="sxs-lookup"><span data-stu-id="3058e-137">description</span></span>|<span data-ttu-id="3058e-138">String</span><span class="sxs-lookup"><span data-stu-id="3058e-138">String</span></span>|<span data-ttu-id="3058e-139">尚未记录</span><span class="sxs-lookup"><span data-stu-id="3058e-139">Not yet documented</span></span>|
|<span data-ttu-id="3058e-140">displayName</span><span class="sxs-lookup"><span data-stu-id="3058e-140">displayName</span></span>|<span data-ttu-id="3058e-141">String</span><span class="sxs-lookup"><span data-stu-id="3058e-141">String</span></span>|<span data-ttu-id="3058e-142">管理员提供的 office 客户端配置策略的说明。</span><span class="sxs-lookup"><span data-stu-id="3058e-142">Admin provided description of the office client configuration policy.</span></span>|
|<span data-ttu-id="3058e-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3058e-143">lastModifiedDateTime</span></span>|<span data-ttu-id="3058e-144">日期时间</span><span class="sxs-lookup"><span data-stu-id="3058e-144">DateTime</span></span>|<span data-ttu-id="3058e-145">策略的上次修改日期时间戳。</span><span class="sxs-lookup"><span data-stu-id="3058e-145">Last modified datetime stamp of the policy.</span></span>|
|<span data-ttu-id="3058e-146">priority</span><span class="sxs-lookup"><span data-stu-id="3058e-146">priority</span></span>|<span data-ttu-id="3058e-147">Int32</span><span class="sxs-lookup"><span data-stu-id="3058e-147">Int32</span></span>|<span data-ttu-id="3058e-148">对于租户下的每个策略，优先级值应为唯一值，并将用于冲突解决，较低值意味着优先级较高。</span><span class="sxs-lookup"><span data-stu-id="3058e-148">Priority value should be unique value for each policy under a tenant and will be used for conflict resolution, lower values mean priority is high.</span></span>|
|<span data-ttu-id="3058e-149">userCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="3058e-149">userCheckinSummary</span></span>|[<span data-ttu-id="3058e-150">officeUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="3058e-150">officeUserCheckinSummary</span></span>](../resources/intune-cirrus-officeusercheckinsummary.md)|<span data-ttu-id="3058e-151">策略的用户签入摘要。</span><span class="sxs-lookup"><span data-stu-id="3058e-151">User check-in summary for the policy.</span></span>|
|<span data-ttu-id="3058e-152">checkinStatuses</span><span class="sxs-lookup"><span data-stu-id="3058e-152">checkinStatuses</span></span>|<span data-ttu-id="3058e-153">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md)集合</span><span class="sxs-lookup"><span data-stu-id="3058e-153">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) collection</span></span>|<span data-ttu-id="3058e-154">Office 客户端签入状态的列表。</span><span class="sxs-lookup"><span data-stu-id="3058e-154">List of office Client check-in status.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3058e-155">关系</span><span class="sxs-lookup"><span data-stu-id="3058e-155">Relationships</span></span>
|<span data-ttu-id="3058e-156">关系</span><span class="sxs-lookup"><span data-stu-id="3058e-156">Relationship</span></span>|<span data-ttu-id="3058e-157">类型</span><span class="sxs-lookup"><span data-stu-id="3058e-157">Type</span></span>|<span data-ttu-id="3058e-158">说明</span><span class="sxs-lookup"><span data-stu-id="3058e-158">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3058e-159">assignments</span><span class="sxs-lookup"><span data-stu-id="3058e-159">assignments</span></span>|<span data-ttu-id="3058e-160">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="3058e-160">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) collection</span></span>|<span data-ttu-id="3058e-161">策略的组分配列表。</span><span class="sxs-lookup"><span data-stu-id="3058e-161">The list of group assignments for the policy.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3058e-162">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3058e-162">JSON Representation</span></span>
<span data-ttu-id="3058e-163">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3058e-163">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.officeClientConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.officeClientConfiguration",
  "id": "String (identifier)",
  "userPreferencePayload": "<Unknown Primitive Type Edm.Stream>",
  "policyPayload": "<Unknown Primitive Type Edm.Stream>",
  "description": "String",
  "displayName": "String",
  "priority": 1024,
  "userCheckinSummary": {
    "@odata.type": "microsoft.graph.officeUserCheckinSummary",
    "succeededUserCount": 1024,
    "failedUserCount": 1024
  },
  "checkinStatuses": [
    {
      "@odata.type": "microsoft.graph.officeClientCheckinStatus",
      "userPrincipalName": "String",
      "deviceName": "String",
      "devicePlatform": "String",
      "devicePlatformVersion": "String",
      "wasSuccessful": true,
      "userId": "String",
      "checkinDateTime": "String (timestamp)",
      "errorMessage": "String",
      "appliedPolicies": [
        "String"
      ]
    }
  ]
}
```




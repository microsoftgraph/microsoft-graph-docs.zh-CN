---
title: officeClientConfiguration 资源类型
description: Office 客户端配置。
localization_priority: Normal
author: rolyon
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3688503cf19d8cebe51b4afe7abd1563257f9192
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36004757"
---
# <a name="officeclientconfiguration-resource-type"></a><span data-ttu-id="ae5a6-103">officeClientConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="ae5a6-103">officeClientConfiguration resource type</span></span>

> <span data-ttu-id="ae5a6-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ae5a6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ae5a6-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ae5a6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ae5a6-106">Office 客户端配置。</span><span class="sxs-lookup"><span data-stu-id="ae5a6-106">Office Client Configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="ae5a6-107">方法</span><span class="sxs-lookup"><span data-stu-id="ae5a6-107">Methods</span></span>
|<span data-ttu-id="ae5a6-108">方法</span><span class="sxs-lookup"><span data-stu-id="ae5a6-108">Method</span></span>|<span data-ttu-id="ae5a6-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="ae5a6-109">Return Type</span></span>|<span data-ttu-id="ae5a6-110">说明</span><span class="sxs-lookup"><span data-stu-id="ae5a6-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ae5a6-111">列出 officeClientConfigurations</span><span class="sxs-lookup"><span data-stu-id="ae5a6-111">List officeClientConfigurations</span></span>](../api/intune-cirrus-officeclientconfiguration-list.md)|<span data-ttu-id="ae5a6-112">[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)集合</span><span class="sxs-lookup"><span data-stu-id="ae5a6-112">[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) collection</span></span>|<span data-ttu-id="ae5a6-113">列出[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ae5a6-113">List properties and relationships of the [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="ae5a6-114">获取 officeClientConfiguration</span><span class="sxs-lookup"><span data-stu-id="ae5a6-114">Get officeClientConfiguration</span></span>](../api/intune-cirrus-officeclientconfiguration-get.md)|[<span data-ttu-id="ae5a6-115">officeClientConfiguration</span><span class="sxs-lookup"><span data-stu-id="ae5a6-115">officeClientConfiguration</span></span>](../resources/intune-cirrus-officeclientconfiguration.md)|<span data-ttu-id="ae5a6-116">读取[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ae5a6-116">Read properties and relationships of the [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) object.</span></span>|
|[<span data-ttu-id="ae5a6-117">分配操作</span><span class="sxs-lookup"><span data-stu-id="ae5a6-117">assign action</span></span>](../api/intune-cirrus-officeclientconfiguration-assign.md)|<span data-ttu-id="ae5a6-118">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="ae5a6-118">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) collection</span></span>|<span data-ttu-id="ae5a6-119">替换策略的所有目标组。</span><span class="sxs-lookup"><span data-stu-id="ae5a6-119">Replace all targeted groups for a policy.</span></span>|
|[<span data-ttu-id="ae5a6-120">updatePriorities 操作</span><span class="sxs-lookup"><span data-stu-id="ae5a6-120">updatePriorities action</span></span>](../api/intune-cirrus-officeclientconfiguration-updatepriorities.md)|<span data-ttu-id="ae5a6-121">无</span><span class="sxs-lookup"><span data-stu-id="ae5a6-121">None</span></span>|<span data-ttu-id="ae5a6-122">更新策略优先级。</span><span class="sxs-lookup"><span data-stu-id="ae5a6-122">Update policy priorities.</span></span>|

## <a name="properties"></a><span data-ttu-id="ae5a6-123">属性</span><span class="sxs-lookup"><span data-stu-id="ae5a6-123">Properties</span></span>
|<span data-ttu-id="ae5a6-124">属性</span><span class="sxs-lookup"><span data-stu-id="ae5a6-124">Property</span></span>|<span data-ttu-id="ae5a6-125">类型</span><span class="sxs-lookup"><span data-stu-id="ae5a6-125">Type</span></span>|<span data-ttu-id="ae5a6-126">说明</span><span class="sxs-lookup"><span data-stu-id="ae5a6-126">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ae5a6-127">id</span><span class="sxs-lookup"><span data-stu-id="ae5a6-127">id</span></span>|<span data-ttu-id="ae5a6-128">字符串</span><span class="sxs-lookup"><span data-stu-id="ae5a6-128">String</span></span>|<span data-ttu-id="ae5a6-129">Office 客户端配置策略的 Id。</span><span class="sxs-lookup"><span data-stu-id="ae5a6-129">Id of the office client configuration policy.</span></span>|
|<span data-ttu-id="ae5a6-130">userPreferencePayload</span><span class="sxs-lookup"><span data-stu-id="ae5a6-130">userPreferencePayload</span></span>|<span data-ttu-id="ae5a6-131">流</span><span class="sxs-lookup"><span data-stu-id="ae5a6-131">Stream</span></span>|<span data-ttu-id="ae5a6-132">首选项设置 JSON string 二进制格式, 则用户可以重写这些值。</span><span class="sxs-lookup"><span data-stu-id="ae5a6-132">Preference settings JSON string in binary format, these values can be overridden by the user.</span></span>|
|<span data-ttu-id="ae5a6-133">policyPayload</span><span class="sxs-lookup"><span data-stu-id="ae5a6-133">policyPayload</span></span>|<span data-ttu-id="ae5a6-134">流</span><span class="sxs-lookup"><span data-stu-id="ae5a6-134">Stream</span></span>|<span data-ttu-id="ae5a6-135">策略设置 JSON string 二进制格式, 用户不能更改这些值。</span><span class="sxs-lookup"><span data-stu-id="ae5a6-135">Policy settings JSON string in binary format, these values cannot be changed by the user.</span></span>|
|<span data-ttu-id="ae5a6-136">说明</span><span class="sxs-lookup"><span data-stu-id="ae5a6-136">description</span></span>|<span data-ttu-id="ae5a6-137">String</span><span class="sxs-lookup"><span data-stu-id="ae5a6-137">String</span></span>|<span data-ttu-id="ae5a6-138">尚未记录</span><span class="sxs-lookup"><span data-stu-id="ae5a6-138">Not yet documented</span></span>|
|<span data-ttu-id="ae5a6-139">displayName</span><span class="sxs-lookup"><span data-stu-id="ae5a6-139">displayName</span></span>|<span data-ttu-id="ae5a6-140">String</span><span class="sxs-lookup"><span data-stu-id="ae5a6-140">String</span></span>|<span data-ttu-id="ae5a6-141">管理员提供的 office 客户端配置策略的说明。</span><span class="sxs-lookup"><span data-stu-id="ae5a6-141">Admin provided description of the office client configuration policy.</span></span>|
|<span data-ttu-id="ae5a6-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ae5a6-142">lastModifiedDateTime</span></span>|<span data-ttu-id="ae5a6-143">日期时间</span><span class="sxs-lookup"><span data-stu-id="ae5a6-143">DateTime</span></span>|<span data-ttu-id="ae5a6-144">策略的上次修改日期时间戳。</span><span class="sxs-lookup"><span data-stu-id="ae5a6-144">Last modified datetime stamp of the policy.</span></span>|
|<span data-ttu-id="ae5a6-145">priority</span><span class="sxs-lookup"><span data-stu-id="ae5a6-145">priority</span></span>|<span data-ttu-id="ae5a6-146">Int32</span><span class="sxs-lookup"><span data-stu-id="ae5a6-146">Int32</span></span>|<span data-ttu-id="ae5a6-147">对于租户下的每个策略, 优先级值应为唯一值, 并将用于冲突解决, 较低值意味着优先级较高。</span><span class="sxs-lookup"><span data-stu-id="ae5a6-147">Priority value should be unique value for each policy under a tenant and will be used for conflict resolution, lower values mean priority is high.</span></span>|
|<span data-ttu-id="ae5a6-148">userCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="ae5a6-148">userCheckinSummary</span></span>|[<span data-ttu-id="ae5a6-149">officeUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="ae5a6-149">officeUserCheckinSummary</span></span>](../resources/intune-cirrus-officeusercheckinsummary.md)|<span data-ttu-id="ae5a6-150">策略的用户签入摘要。</span><span class="sxs-lookup"><span data-stu-id="ae5a6-150">User check-in summary for the policy.</span></span>|
|<span data-ttu-id="ae5a6-151">checkinStatuses</span><span class="sxs-lookup"><span data-stu-id="ae5a6-151">checkinStatuses</span></span>|<span data-ttu-id="ae5a6-152">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md)集合</span><span class="sxs-lookup"><span data-stu-id="ae5a6-152">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) collection</span></span>|<span data-ttu-id="ae5a6-153">Office 客户端签入状态的列表。</span><span class="sxs-lookup"><span data-stu-id="ae5a6-153">List of office Client check-in status.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ae5a6-154">关系</span><span class="sxs-lookup"><span data-stu-id="ae5a6-154">Relationships</span></span>
|<span data-ttu-id="ae5a6-155">关系</span><span class="sxs-lookup"><span data-stu-id="ae5a6-155">Relationship</span></span>|<span data-ttu-id="ae5a6-156">类型</span><span class="sxs-lookup"><span data-stu-id="ae5a6-156">Type</span></span>|<span data-ttu-id="ae5a6-157">说明</span><span class="sxs-lookup"><span data-stu-id="ae5a6-157">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ae5a6-158">assignments</span><span class="sxs-lookup"><span data-stu-id="ae5a6-158">assignments</span></span>|<span data-ttu-id="ae5a6-159">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="ae5a6-159">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) collection</span></span>|<span data-ttu-id="ae5a6-160">策略的组分配列表。</span><span class="sxs-lookup"><span data-stu-id="ae5a6-160">The list of group assignments for the policy.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ae5a6-161">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ae5a6-161">JSON Representation</span></span>
<span data-ttu-id="ae5a6-162">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ae5a6-162">Here is a JSON representation of the resource.</span></span>
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




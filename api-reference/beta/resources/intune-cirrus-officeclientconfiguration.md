---
title: officeClientConfiguration 资源类型
description: Office 客户端配置。
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 87351ed868a1f46ff769882fea4e12da25aed16e
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48693995"
---
# <a name="officeclientconfiguration-resource-type"></a><span data-ttu-id="dc042-103">officeClientConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="dc042-103">officeClientConfiguration resource type</span></span>

<span data-ttu-id="dc042-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dc042-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dc042-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="dc042-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dc042-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="dc042-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dc042-107">Office 客户端配置。</span><span class="sxs-lookup"><span data-stu-id="dc042-107">Office Client Configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="dc042-108">Methods</span><span class="sxs-lookup"><span data-stu-id="dc042-108">Methods</span></span>
|<span data-ttu-id="dc042-109">方法</span><span class="sxs-lookup"><span data-stu-id="dc042-109">Method</span></span>|<span data-ttu-id="dc042-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="dc042-110">Return Type</span></span>|<span data-ttu-id="dc042-111">说明</span><span class="sxs-lookup"><span data-stu-id="dc042-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="dc042-112">列出 officeClientConfigurations</span><span class="sxs-lookup"><span data-stu-id="dc042-112">List officeClientConfigurations</span></span>](../api/intune-cirrus-officeclientconfiguration-list.md)|<span data-ttu-id="dc042-113">[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="dc042-113">[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) collection</span></span>|<span data-ttu-id="dc042-114">列出 [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="dc042-114">List properties and relationships of the [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="dc042-115">获取 officeClientConfiguration</span><span class="sxs-lookup"><span data-stu-id="dc042-115">Get officeClientConfiguration</span></span>](../api/intune-cirrus-officeclientconfiguration-get.md)|[<span data-ttu-id="dc042-116">officeClientConfiguration</span><span class="sxs-lookup"><span data-stu-id="dc042-116">officeClientConfiguration</span></span>](../resources/intune-cirrus-officeclientconfiguration.md)|<span data-ttu-id="dc042-117">读取 [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="dc042-117">Read properties and relationships of the [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) object.</span></span>|
|[<span data-ttu-id="dc042-118">分配操作</span><span class="sxs-lookup"><span data-stu-id="dc042-118">assign action</span></span>](../api/intune-cirrus-officeclientconfiguration-assign.md)|<span data-ttu-id="dc042-119">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="dc042-119">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) collection</span></span>|<span data-ttu-id="dc042-120">替换策略的所有目标组。</span><span class="sxs-lookup"><span data-stu-id="dc042-120">Replace all targeted groups for a policy.</span></span>|
|[<span data-ttu-id="dc042-121">updatePriorities 操作</span><span class="sxs-lookup"><span data-stu-id="dc042-121">updatePriorities action</span></span>](../api/intune-cirrus-officeclientconfiguration-updatepriorities.md)|<span data-ttu-id="dc042-122">无</span><span class="sxs-lookup"><span data-stu-id="dc042-122">None</span></span>|<span data-ttu-id="dc042-123">更新策略优先级。</span><span class="sxs-lookup"><span data-stu-id="dc042-123">Update policy priorities.</span></span>|

## <a name="properties"></a><span data-ttu-id="dc042-124">属性</span><span class="sxs-lookup"><span data-stu-id="dc042-124">Properties</span></span>
|<span data-ttu-id="dc042-125">属性</span><span class="sxs-lookup"><span data-stu-id="dc042-125">Property</span></span>|<span data-ttu-id="dc042-126">类型</span><span class="sxs-lookup"><span data-stu-id="dc042-126">Type</span></span>|<span data-ttu-id="dc042-127">说明</span><span class="sxs-lookup"><span data-stu-id="dc042-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dc042-128">id</span><span class="sxs-lookup"><span data-stu-id="dc042-128">id</span></span>|<span data-ttu-id="dc042-129">String</span><span class="sxs-lookup"><span data-stu-id="dc042-129">String</span></span>|<span data-ttu-id="dc042-130">Office 客户端配置策略的 Id。</span><span class="sxs-lookup"><span data-stu-id="dc042-130">Id of the office client configuration policy.</span></span>|
|<span data-ttu-id="dc042-131">userPreferencePayload</span><span class="sxs-lookup"><span data-stu-id="dc042-131">userPreferencePayload</span></span>|<span data-ttu-id="dc042-132">Stream</span><span class="sxs-lookup"><span data-stu-id="dc042-132">Stream</span></span>|<span data-ttu-id="dc042-133">首选项设置 JSON string 二进制格式，则用户可以重写这些值。</span><span class="sxs-lookup"><span data-stu-id="dc042-133">Preference settings JSON string in binary format, these values can be overridden by the user.</span></span>|
|<span data-ttu-id="dc042-134">policyPayload</span><span class="sxs-lookup"><span data-stu-id="dc042-134">policyPayload</span></span>|<span data-ttu-id="dc042-135">Stream</span><span class="sxs-lookup"><span data-stu-id="dc042-135">Stream</span></span>|<span data-ttu-id="dc042-136">策略设置 JSON string 二进制格式，用户不能更改这些值。</span><span class="sxs-lookup"><span data-stu-id="dc042-136">Policy settings JSON string in binary format, these values cannot be changed by the user.</span></span>|
|<span data-ttu-id="dc042-137">说明</span><span class="sxs-lookup"><span data-stu-id="dc042-137">description</span></span>|<span data-ttu-id="dc042-138">String</span><span class="sxs-lookup"><span data-stu-id="dc042-138">String</span></span>|<span data-ttu-id="dc042-139">尚未记录</span><span class="sxs-lookup"><span data-stu-id="dc042-139">Not yet documented</span></span>|
|<span data-ttu-id="dc042-140">displayName</span><span class="sxs-lookup"><span data-stu-id="dc042-140">displayName</span></span>|<span data-ttu-id="dc042-141">String</span><span class="sxs-lookup"><span data-stu-id="dc042-141">String</span></span>|<span data-ttu-id="dc042-142">管理员提供的 office 客户端配置策略的说明。</span><span class="sxs-lookup"><span data-stu-id="dc042-142">Admin provided description of the office client configuration policy.</span></span>|
|<span data-ttu-id="dc042-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="dc042-143">lastModifiedDateTime</span></span>|<span data-ttu-id="dc042-144">日期时间</span><span class="sxs-lookup"><span data-stu-id="dc042-144">DateTime</span></span>|<span data-ttu-id="dc042-145">策略的上次修改日期时间戳。</span><span class="sxs-lookup"><span data-stu-id="dc042-145">Last modified datetime stamp of the policy.</span></span>|
|<span data-ttu-id="dc042-146">priority</span><span class="sxs-lookup"><span data-stu-id="dc042-146">priority</span></span>|<span data-ttu-id="dc042-147">Int32</span><span class="sxs-lookup"><span data-stu-id="dc042-147">Int32</span></span>|<span data-ttu-id="dc042-148">对于租户下的每个策略，优先级值应为唯一值，并将用于冲突解决，较低值意味着优先级较高。</span><span class="sxs-lookup"><span data-stu-id="dc042-148">Priority value should be unique value for each policy under a tenant and will be used for conflict resolution, lower values mean priority is high.</span></span>|
|<span data-ttu-id="dc042-149">userCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="dc042-149">userCheckinSummary</span></span>|[<span data-ttu-id="dc042-150">officeUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="dc042-150">officeUserCheckinSummary</span></span>](../resources/intune-cirrus-officeusercheckinsummary.md)|<span data-ttu-id="dc042-151">策略的用户签入摘要。</span><span class="sxs-lookup"><span data-stu-id="dc042-151">User check-in summary for the policy.</span></span>|
|<span data-ttu-id="dc042-152">checkinStatuses</span><span class="sxs-lookup"><span data-stu-id="dc042-152">checkinStatuses</span></span>|<span data-ttu-id="dc042-153">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="dc042-153">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) collection</span></span>|<span data-ttu-id="dc042-154">Office 客户端签入状态的列表。</span><span class="sxs-lookup"><span data-stu-id="dc042-154">List of office Client check-in status.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dc042-155">关系</span><span class="sxs-lookup"><span data-stu-id="dc042-155">Relationships</span></span>
|<span data-ttu-id="dc042-156">关系</span><span class="sxs-lookup"><span data-stu-id="dc042-156">Relationship</span></span>|<span data-ttu-id="dc042-157">类型</span><span class="sxs-lookup"><span data-stu-id="dc042-157">Type</span></span>|<span data-ttu-id="dc042-158">说明</span><span class="sxs-lookup"><span data-stu-id="dc042-158">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dc042-159">assignments</span><span class="sxs-lookup"><span data-stu-id="dc042-159">assignments</span></span>|<span data-ttu-id="dc042-160">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="dc042-160">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) collection</span></span>|<span data-ttu-id="dc042-161">策略的组分配列表。</span><span class="sxs-lookup"><span data-stu-id="dc042-161">The list of group assignments for the policy.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="dc042-162">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="dc042-162">JSON Representation</span></span>
<span data-ttu-id="dc042-163">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dc042-163">Here is a JSON representation of the resource.</span></span>
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






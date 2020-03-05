---
title: officeClientConfiguration 资源类型
description: Office 客户端配置。
localization_priority: Normal
author: rolyon
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6fabc35866aafbbb4052ce5eab3f0de977ec6adb
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42488535"
---
# <a name="officeclientconfiguration-resource-type"></a><span data-ttu-id="97c6a-103">officeClientConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="97c6a-103">officeClientConfiguration resource type</span></span>

<span data-ttu-id="97c6a-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="97c6a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="97c6a-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="97c6a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="97c6a-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="97c6a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="97c6a-107">Office 客户端配置。</span><span class="sxs-lookup"><span data-stu-id="97c6a-107">Office Client Configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="97c6a-108">方法</span><span class="sxs-lookup"><span data-stu-id="97c6a-108">Methods</span></span>
|<span data-ttu-id="97c6a-109">方法</span><span class="sxs-lookup"><span data-stu-id="97c6a-109">Method</span></span>|<span data-ttu-id="97c6a-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="97c6a-110">Return Type</span></span>|<span data-ttu-id="97c6a-111">说明</span><span class="sxs-lookup"><span data-stu-id="97c6a-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="97c6a-112">列出 officeClientConfigurations</span><span class="sxs-lookup"><span data-stu-id="97c6a-112">List officeClientConfigurations</span></span>](../api/intune-cirrus-officeclientconfiguration-list.md)|<span data-ttu-id="97c6a-113">[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)集合</span><span class="sxs-lookup"><span data-stu-id="97c6a-113">[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) collection</span></span>|<span data-ttu-id="97c6a-114">列出[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="97c6a-114">List properties and relationships of the [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="97c6a-115">获取 officeClientConfiguration</span><span class="sxs-lookup"><span data-stu-id="97c6a-115">Get officeClientConfiguration</span></span>](../api/intune-cirrus-officeclientconfiguration-get.md)|[<span data-ttu-id="97c6a-116">officeClientConfiguration</span><span class="sxs-lookup"><span data-stu-id="97c6a-116">officeClientConfiguration</span></span>](../resources/intune-cirrus-officeclientconfiguration.md)|<span data-ttu-id="97c6a-117">读取[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="97c6a-117">Read properties and relationships of the [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) object.</span></span>|
|[<span data-ttu-id="97c6a-118">分配操作</span><span class="sxs-lookup"><span data-stu-id="97c6a-118">assign action</span></span>](../api/intune-cirrus-officeclientconfiguration-assign.md)|<span data-ttu-id="97c6a-119">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="97c6a-119">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) collection</span></span>|<span data-ttu-id="97c6a-120">替换策略的所有目标组。</span><span class="sxs-lookup"><span data-stu-id="97c6a-120">Replace all targeted groups for a policy.</span></span>|
|[<span data-ttu-id="97c6a-121">updatePriorities 操作</span><span class="sxs-lookup"><span data-stu-id="97c6a-121">updatePriorities action</span></span>](../api/intune-cirrus-officeclientconfiguration-updatepriorities.md)|<span data-ttu-id="97c6a-122">无</span><span class="sxs-lookup"><span data-stu-id="97c6a-122">None</span></span>|<span data-ttu-id="97c6a-123">更新策略优先级。</span><span class="sxs-lookup"><span data-stu-id="97c6a-123">Update policy priorities.</span></span>|

## <a name="properties"></a><span data-ttu-id="97c6a-124">属性</span><span class="sxs-lookup"><span data-stu-id="97c6a-124">Properties</span></span>
|<span data-ttu-id="97c6a-125">属性</span><span class="sxs-lookup"><span data-stu-id="97c6a-125">Property</span></span>|<span data-ttu-id="97c6a-126">类型</span><span class="sxs-lookup"><span data-stu-id="97c6a-126">Type</span></span>|<span data-ttu-id="97c6a-127">说明</span><span class="sxs-lookup"><span data-stu-id="97c6a-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="97c6a-128">id</span><span class="sxs-lookup"><span data-stu-id="97c6a-128">id</span></span>|<span data-ttu-id="97c6a-129">字符串</span><span class="sxs-lookup"><span data-stu-id="97c6a-129">String</span></span>|<span data-ttu-id="97c6a-130">Office 客户端配置策略的 Id。</span><span class="sxs-lookup"><span data-stu-id="97c6a-130">Id of the office client configuration policy.</span></span>|
|<span data-ttu-id="97c6a-131">userPreferencePayload</span><span class="sxs-lookup"><span data-stu-id="97c6a-131">userPreferencePayload</span></span>|<span data-ttu-id="97c6a-132">Stream</span><span class="sxs-lookup"><span data-stu-id="97c6a-132">Stream</span></span>|<span data-ttu-id="97c6a-133">首选项设置 JSON string 二进制格式，则用户可以重写这些值。</span><span class="sxs-lookup"><span data-stu-id="97c6a-133">Preference settings JSON string in binary format, these values can be overridden by the user.</span></span>|
|<span data-ttu-id="97c6a-134">policyPayload</span><span class="sxs-lookup"><span data-stu-id="97c6a-134">policyPayload</span></span>|<span data-ttu-id="97c6a-135">Stream</span><span class="sxs-lookup"><span data-stu-id="97c6a-135">Stream</span></span>|<span data-ttu-id="97c6a-136">策略设置 JSON string 二进制格式，用户不能更改这些值。</span><span class="sxs-lookup"><span data-stu-id="97c6a-136">Policy settings JSON string in binary format, these values cannot be changed by the user.</span></span>|
|<span data-ttu-id="97c6a-137">说明</span><span class="sxs-lookup"><span data-stu-id="97c6a-137">description</span></span>|<span data-ttu-id="97c6a-138">String</span><span class="sxs-lookup"><span data-stu-id="97c6a-138">String</span></span>|<span data-ttu-id="97c6a-139">尚未记录</span><span class="sxs-lookup"><span data-stu-id="97c6a-139">Not yet documented</span></span>|
|<span data-ttu-id="97c6a-140">displayName</span><span class="sxs-lookup"><span data-stu-id="97c6a-140">displayName</span></span>|<span data-ttu-id="97c6a-141">String</span><span class="sxs-lookup"><span data-stu-id="97c6a-141">String</span></span>|<span data-ttu-id="97c6a-142">管理员提供的 office 客户端配置策略的说明。</span><span class="sxs-lookup"><span data-stu-id="97c6a-142">Admin provided description of the office client configuration policy.</span></span>|
|<span data-ttu-id="97c6a-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="97c6a-143">lastModifiedDateTime</span></span>|<span data-ttu-id="97c6a-144">日期时间</span><span class="sxs-lookup"><span data-stu-id="97c6a-144">DateTime</span></span>|<span data-ttu-id="97c6a-145">策略的上次修改日期时间戳。</span><span class="sxs-lookup"><span data-stu-id="97c6a-145">Last modified datetime stamp of the policy.</span></span>|
|<span data-ttu-id="97c6a-146">priority</span><span class="sxs-lookup"><span data-stu-id="97c6a-146">priority</span></span>|<span data-ttu-id="97c6a-147">Int32</span><span class="sxs-lookup"><span data-stu-id="97c6a-147">Int32</span></span>|<span data-ttu-id="97c6a-148">对于租户下的每个策略，优先级值应为唯一值，并将用于冲突解决，较低值意味着优先级较高。</span><span class="sxs-lookup"><span data-stu-id="97c6a-148">Priority value should be unique value for each policy under a tenant and will be used for conflict resolution, lower values mean priority is high.</span></span>|
|<span data-ttu-id="97c6a-149">userCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="97c6a-149">userCheckinSummary</span></span>|[<span data-ttu-id="97c6a-150">officeUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="97c6a-150">officeUserCheckinSummary</span></span>](../resources/intune-cirrus-officeusercheckinsummary.md)|<span data-ttu-id="97c6a-151">策略的用户签入摘要。</span><span class="sxs-lookup"><span data-stu-id="97c6a-151">User check-in summary for the policy.</span></span>|
|<span data-ttu-id="97c6a-152">checkinStatuses</span><span class="sxs-lookup"><span data-stu-id="97c6a-152">checkinStatuses</span></span>|<span data-ttu-id="97c6a-153">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md)集合</span><span class="sxs-lookup"><span data-stu-id="97c6a-153">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) collection</span></span>|<span data-ttu-id="97c6a-154">Office 客户端签入状态的列表。</span><span class="sxs-lookup"><span data-stu-id="97c6a-154">List of office Client check-in status.</span></span>|

## <a name="relationships"></a><span data-ttu-id="97c6a-155">关系</span><span class="sxs-lookup"><span data-stu-id="97c6a-155">Relationships</span></span>
|<span data-ttu-id="97c6a-156">关系</span><span class="sxs-lookup"><span data-stu-id="97c6a-156">Relationship</span></span>|<span data-ttu-id="97c6a-157">类型</span><span class="sxs-lookup"><span data-stu-id="97c6a-157">Type</span></span>|<span data-ttu-id="97c6a-158">说明</span><span class="sxs-lookup"><span data-stu-id="97c6a-158">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="97c6a-159">assignments</span><span class="sxs-lookup"><span data-stu-id="97c6a-159">assignments</span></span>|<span data-ttu-id="97c6a-160">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="97c6a-160">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) collection</span></span>|<span data-ttu-id="97c6a-161">策略的组分配列表。</span><span class="sxs-lookup"><span data-stu-id="97c6a-161">The list of group assignments for the policy.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="97c6a-162">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="97c6a-162">JSON Representation</span></span>
<span data-ttu-id="97c6a-163">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="97c6a-163">Here is a JSON representation of the resource.</span></span>
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




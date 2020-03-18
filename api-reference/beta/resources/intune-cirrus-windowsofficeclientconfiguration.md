---
title: windowsOfficeClientConfiguration 资源类型
description: 描述 Windows 的 office 策略设置的实体。
localization_priority: Normal
author: davidmu1
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 705555ff285420c4aa9d43ee57034026e9043785
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42797288"
---
# <a name="windowsofficeclientconfiguration-resource-type"></a><span data-ttu-id="13f28-103">windowsOfficeClientConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="13f28-103">windowsOfficeClientConfiguration resource type</span></span>

> <span data-ttu-id="13f28-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="13f28-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="13f28-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="13f28-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="13f28-106">描述 Windows 的 office 策略设置的实体。</span><span class="sxs-lookup"><span data-stu-id="13f28-106">Entity that describes office policy settings for Windows.</span></span>

<span data-ttu-id="13f28-107">继承自[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="13f28-107">Inherits from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="13f28-108">方法</span><span class="sxs-lookup"><span data-stu-id="13f28-108">Methods</span></span>
|<span data-ttu-id="13f28-109">方法</span><span class="sxs-lookup"><span data-stu-id="13f28-109">Method</span></span>|<span data-ttu-id="13f28-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="13f28-110">Return Type</span></span>|<span data-ttu-id="13f28-111">说明</span><span class="sxs-lookup"><span data-stu-id="13f28-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="13f28-112">列出 windowsOfficeClientConfigurations</span><span class="sxs-lookup"><span data-stu-id="13f28-112">List windowsOfficeClientConfigurations</span></span>](../api/intune-cirrus-windowsofficeclientconfiguration-list.md)|<span data-ttu-id="13f28-113">[windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md)集合</span><span class="sxs-lookup"><span data-stu-id="13f28-113">[windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) collection</span></span>|<span data-ttu-id="13f28-114">列出[windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="13f28-114">List properties and relationships of the [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="13f28-115">获取 windowsOfficeClientConfiguration</span><span class="sxs-lookup"><span data-stu-id="13f28-115">Get windowsOfficeClientConfiguration</span></span>](../api/intune-cirrus-windowsofficeclientconfiguration-get.md)|[<span data-ttu-id="13f28-116">windowsOfficeClientConfiguration</span><span class="sxs-lookup"><span data-stu-id="13f28-116">windowsOfficeClientConfiguration</span></span>](../resources/intune-cirrus-windowsofficeclientconfiguration.md)|<span data-ttu-id="13f28-117">读取[windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="13f28-117">Read properties and relationships of the [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) object.</span></span>|
|[<span data-ttu-id="13f28-118">创建 windowsOfficeClientConfiguration</span><span class="sxs-lookup"><span data-stu-id="13f28-118">Create windowsOfficeClientConfiguration</span></span>](../api/intune-cirrus-windowsofficeclientconfiguration-create.md)|[<span data-ttu-id="13f28-119">windowsOfficeClientConfiguration</span><span class="sxs-lookup"><span data-stu-id="13f28-119">windowsOfficeClientConfiguration</span></span>](../resources/intune-cirrus-windowsofficeclientconfiguration.md)|<span data-ttu-id="13f28-120">创建新的[windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="13f28-120">Create a new [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) object.</span></span>|
|[<span data-ttu-id="13f28-121">删除 windowsOfficeClientConfiguration</span><span class="sxs-lookup"><span data-stu-id="13f28-121">Delete windowsOfficeClientConfiguration</span></span>](../api/intune-cirrus-windowsofficeclientconfiguration-delete.md)|<span data-ttu-id="13f28-122">None</span><span class="sxs-lookup"><span data-stu-id="13f28-122">None</span></span>|<span data-ttu-id="13f28-123">删除[windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="13f28-123">Deletes a [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md).</span></span>|
|[<span data-ttu-id="13f28-124">更新 windowsOfficeClientConfiguration</span><span class="sxs-lookup"><span data-stu-id="13f28-124">Update windowsOfficeClientConfiguration</span></span>](../api/intune-cirrus-windowsofficeclientconfiguration-update.md)|[<span data-ttu-id="13f28-125">windowsOfficeClientConfiguration</span><span class="sxs-lookup"><span data-stu-id="13f28-125">windowsOfficeClientConfiguration</span></span>](../resources/intune-cirrus-windowsofficeclientconfiguration.md)|<span data-ttu-id="13f28-126">更新[windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="13f28-126">Update the properties of a [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="13f28-127">属性</span><span class="sxs-lookup"><span data-stu-id="13f28-127">Properties</span></span>
|<span data-ttu-id="13f28-128">属性</span><span class="sxs-lookup"><span data-stu-id="13f28-128">Property</span></span>|<span data-ttu-id="13f28-129">类型</span><span class="sxs-lookup"><span data-stu-id="13f28-129">Type</span></span>|<span data-ttu-id="13f28-130">说明</span><span class="sxs-lookup"><span data-stu-id="13f28-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="13f28-131">id</span><span class="sxs-lookup"><span data-stu-id="13f28-131">id</span></span>|<span data-ttu-id="13f28-132">字符串</span><span class="sxs-lookup"><span data-stu-id="13f28-132">String</span></span>|<span data-ttu-id="13f28-133">Office 客户端配置策略的 Id。</span><span class="sxs-lookup"><span data-stu-id="13f28-133">Id of the office client configuration policy.</span></span> <span data-ttu-id="13f28-134">继承自[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="13f28-134">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="13f28-135">userPreferencePayload</span><span class="sxs-lookup"><span data-stu-id="13f28-135">userPreferencePayload</span></span>|<span data-ttu-id="13f28-136">Stream</span><span class="sxs-lookup"><span data-stu-id="13f28-136">Stream</span></span>|<span data-ttu-id="13f28-137">首选项设置 JSON string 二进制格式，则用户可以重写这些值。</span><span class="sxs-lookup"><span data-stu-id="13f28-137">Preference settings JSON string in binary format, these values can be overridden by the user.</span></span> <span data-ttu-id="13f28-138">继承自[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="13f28-138">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="13f28-139">policyPayload</span><span class="sxs-lookup"><span data-stu-id="13f28-139">policyPayload</span></span>|<span data-ttu-id="13f28-140">Stream</span><span class="sxs-lookup"><span data-stu-id="13f28-140">Stream</span></span>|<span data-ttu-id="13f28-141">策略设置 JSON string 二进制格式，用户不能更改这些值。</span><span class="sxs-lookup"><span data-stu-id="13f28-141">Policy settings JSON string in binary format, these values cannot be changed by the user.</span></span> <span data-ttu-id="13f28-142">继承自[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="13f28-142">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="13f28-143">说明</span><span class="sxs-lookup"><span data-stu-id="13f28-143">description</span></span>|<span data-ttu-id="13f28-144">String</span><span class="sxs-lookup"><span data-stu-id="13f28-144">String</span></span>|<span data-ttu-id="13f28-145">管理员提供的 office 客户端配置策略的说明。</span><span class="sxs-lookup"><span data-stu-id="13f28-145">Admin provided description of the office client configuration policy.</span></span> <span data-ttu-id="13f28-146">继承自[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="13f28-146">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="13f28-147">displayName</span><span class="sxs-lookup"><span data-stu-id="13f28-147">displayName</span></span>|<span data-ttu-id="13f28-148">String</span><span class="sxs-lookup"><span data-stu-id="13f28-148">String</span></span>|<span data-ttu-id="13f28-149">管理员提供的 office 客户端配置策略的名称。</span><span class="sxs-lookup"><span data-stu-id="13f28-149">Admin provided name of the office client configuration policy.</span></span> <span data-ttu-id="13f28-150">继承自[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="13f28-150">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="13f28-151">priority</span><span class="sxs-lookup"><span data-stu-id="13f28-151">priority</span></span>|<span data-ttu-id="13f28-152">Int32</span><span class="sxs-lookup"><span data-stu-id="13f28-152">Int32</span></span>|<span data-ttu-id="13f28-153">对于租户下的每个策略，优先级值应为唯一值，并将用于冲突解决，较低值意味着优先级较高。</span><span class="sxs-lookup"><span data-stu-id="13f28-153">Priority value should be unique value for each policy under a tenant and will be used for conflict resolution, lower values mean priority is high.</span></span> <span data-ttu-id="13f28-154">继承自[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="13f28-154">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="13f28-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="13f28-155">lastModifiedDateTime</span></span>|<span data-ttu-id="13f28-156">日期时间</span><span class="sxs-lookup"><span data-stu-id="13f28-156">DateTime</span></span>|<span data-ttu-id="13f28-157">策略的上次修改日期时间戳。</span><span class="sxs-lookup"><span data-stu-id="13f28-157">Last modified datetime stamp of the policy.</span></span> <span data-ttu-id="13f28-158">继承自[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="13f28-158">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="13f28-159">userCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="13f28-159">userCheckinSummary</span></span>|[<span data-ttu-id="13f28-160">officeUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="13f28-160">officeUserCheckinSummary</span></span>](../resources/intune-cirrus-officeusercheckinsummary.md)|<span data-ttu-id="13f28-161">策略的用户签入摘要。</span><span class="sxs-lookup"><span data-stu-id="13f28-161">User check-in summary for the policy.</span></span> <span data-ttu-id="13f28-162">继承自[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="13f28-162">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="13f28-163">checkinStatuses</span><span class="sxs-lookup"><span data-stu-id="13f28-163">checkinStatuses</span></span>|<span data-ttu-id="13f28-164">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md)集合</span><span class="sxs-lookup"><span data-stu-id="13f28-164">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) collection</span></span>|<span data-ttu-id="13f28-165">Office 客户端签入状态的列表。</span><span class="sxs-lookup"><span data-stu-id="13f28-165">List of office Client check-in status.</span></span> <span data-ttu-id="13f28-166">继承自[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="13f28-166">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="13f28-167">关系</span><span class="sxs-lookup"><span data-stu-id="13f28-167">Relationships</span></span>
|<span data-ttu-id="13f28-168">关系</span><span class="sxs-lookup"><span data-stu-id="13f28-168">Relationship</span></span>|<span data-ttu-id="13f28-169">类型</span><span class="sxs-lookup"><span data-stu-id="13f28-169">Type</span></span>|<span data-ttu-id="13f28-170">说明</span><span class="sxs-lookup"><span data-stu-id="13f28-170">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="13f28-171">assignments</span><span class="sxs-lookup"><span data-stu-id="13f28-171">assignments</span></span>|<span data-ttu-id="13f28-172">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="13f28-172">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) collection</span></span>|<span data-ttu-id="13f28-173">策略的组分配列表。</span><span class="sxs-lookup"><span data-stu-id="13f28-173">The list of group assignments for the policy.</span></span> <span data-ttu-id="13f28-174">继承自[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="13f28-174">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="13f28-175">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="13f28-175">JSON Representation</span></span>
<span data-ttu-id="13f28-176">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="13f28-176">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsOfficeClientConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsOfficeClientConfiguration",
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




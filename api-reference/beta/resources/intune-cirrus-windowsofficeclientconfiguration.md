---
title: windowsOfficeClientConfiguration 资源类型
description: 介绍用于 Windows 的 office 策略设置的实体。
ms.openlocfilehash: 5e1a3281ec6b970765c81ecfd238026d71066c59
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27043831"
---
# <a name="windowsofficeclientconfiguration-resource-type"></a><span data-ttu-id="8bbc2-103">windowsOfficeClientConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="8bbc2-103">windowsOfficeClientConfiguration resource type</span></span>

> <span data-ttu-id="8bbc2-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="8bbc2-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8bbc2-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="8bbc2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8bbc2-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="8bbc2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8bbc2-107">介绍用于 Windows 的 office 策略设置的实体。</span><span class="sxs-lookup"><span data-stu-id="8bbc2-107">Entity that describes office policy settings for Windows.</span></span>

<span data-ttu-id="8bbc2-108">继承自[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8bbc2-108">Inherits from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="8bbc2-109">方法</span><span class="sxs-lookup"><span data-stu-id="8bbc2-109">Methods</span></span>
|<span data-ttu-id="8bbc2-110">方法</span><span class="sxs-lookup"><span data-stu-id="8bbc2-110">Method</span></span>|<span data-ttu-id="8bbc2-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="8bbc2-111">Return Type</span></span>|<span data-ttu-id="8bbc2-112">说明</span><span class="sxs-lookup"><span data-stu-id="8bbc2-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="8bbc2-113">列表 windowsOfficeClientConfigurations</span><span class="sxs-lookup"><span data-stu-id="8bbc2-113">List windowsOfficeClientConfigurations</span></span>](../api/intune-cirrus-windowsofficeclientconfiguration-list.md)|<span data-ttu-id="8bbc2-114">[windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md)集合</span><span class="sxs-lookup"><span data-stu-id="8bbc2-114">[windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) collection</span></span>|<span data-ttu-id="8bbc2-115">列出属性和[windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md)对象之间的关系。</span><span class="sxs-lookup"><span data-stu-id="8bbc2-115">List properties and relationships of the [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="8bbc2-116">获取 windowsOfficeClientConfiguration</span><span class="sxs-lookup"><span data-stu-id="8bbc2-116">Get windowsOfficeClientConfiguration</span></span>](../api/intune-cirrus-windowsofficeclientconfiguration-get.md)|[<span data-ttu-id="8bbc2-117">windowsOfficeClientConfiguration</span><span class="sxs-lookup"><span data-stu-id="8bbc2-117">windowsOfficeClientConfiguration</span></span>](../resources/intune-cirrus-windowsofficeclientconfiguration.md)|<span data-ttu-id="8bbc2-118">读取属性和[windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="8bbc2-118">Read properties and relationships of the [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) object.</span></span>|
|[<span data-ttu-id="8bbc2-119">创建 windowsOfficeClientConfiguration</span><span class="sxs-lookup"><span data-stu-id="8bbc2-119">Create windowsOfficeClientConfiguration</span></span>](../api/intune-cirrus-windowsofficeclientconfiguration-create.md)|[<span data-ttu-id="8bbc2-120">windowsOfficeClientConfiguration</span><span class="sxs-lookup"><span data-stu-id="8bbc2-120">windowsOfficeClientConfiguration</span></span>](../resources/intune-cirrus-windowsofficeclientconfiguration.md)|<span data-ttu-id="8bbc2-121">创建新的[windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="8bbc2-121">Create a new [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) object.</span></span>|
|[<span data-ttu-id="8bbc2-122">删除 windowsOfficeClientConfiguration</span><span class="sxs-lookup"><span data-stu-id="8bbc2-122">Delete windowsOfficeClientConfiguration</span></span>](../api/intune-cirrus-windowsofficeclientconfiguration-delete.md)|<span data-ttu-id="8bbc2-123">无</span><span class="sxs-lookup"><span data-stu-id="8bbc2-123">None</span></span>|<span data-ttu-id="8bbc2-124">删除[windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="8bbc2-124">Deletes a [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md).</span></span>|
|[<span data-ttu-id="8bbc2-125">更新 windowsOfficeClientConfiguration</span><span class="sxs-lookup"><span data-stu-id="8bbc2-125">Update windowsOfficeClientConfiguration</span></span>](../api/intune-cirrus-windowsofficeclientconfiguration-update.md)|[<span data-ttu-id="8bbc2-126">windowsOfficeClientConfiguration</span><span class="sxs-lookup"><span data-stu-id="8bbc2-126">windowsOfficeClientConfiguration</span></span>](../resources/intune-cirrus-windowsofficeclientconfiguration.md)|<span data-ttu-id="8bbc2-127">更新[windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="8bbc2-127">Update the properties of a [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="8bbc2-128">属性</span><span class="sxs-lookup"><span data-stu-id="8bbc2-128">Properties</span></span>
|<span data-ttu-id="8bbc2-129">属性</span><span class="sxs-lookup"><span data-stu-id="8bbc2-129">Property</span></span>|<span data-ttu-id="8bbc2-130">类型</span><span class="sxs-lookup"><span data-stu-id="8bbc2-130">Type</span></span>|<span data-ttu-id="8bbc2-131">说明</span><span class="sxs-lookup"><span data-stu-id="8bbc2-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8bbc2-132">id</span><span class="sxs-lookup"><span data-stu-id="8bbc2-132">id</span></span>|<span data-ttu-id="8bbc2-133">字符串</span><span class="sxs-lookup"><span data-stu-id="8bbc2-133">String</span></span>|<span data-ttu-id="8bbc2-134">Office 客户端配置策略的 id。</span><span class="sxs-lookup"><span data-stu-id="8bbc2-134">Id of the office client configuration policy.</span></span> <span data-ttu-id="8bbc2-135">继承自[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8bbc2-135">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="8bbc2-136">userPreferencePayload</span><span class="sxs-lookup"><span data-stu-id="8bbc2-136">userPreferencePayload</span></span>|<span data-ttu-id="8bbc2-137">Stream</span><span class="sxs-lookup"><span data-stu-id="8bbc2-137">Stream</span></span>|<span data-ttu-id="8bbc2-138">首选项设置为 JSON 字符串以二进制格式，用户可以重写这些值。</span><span class="sxs-lookup"><span data-stu-id="8bbc2-138">Preference settings JSON string in binary format, these values can be overridden by the user.</span></span> <span data-ttu-id="8bbc2-139">继承自[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8bbc2-139">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="8bbc2-140">policyPayload</span><span class="sxs-lookup"><span data-stu-id="8bbc2-140">policyPayload</span></span>|<span data-ttu-id="8bbc2-141">Stream</span><span class="sxs-lookup"><span data-stu-id="8bbc2-141">Stream</span></span>|<span data-ttu-id="8bbc2-142">策略设置 JSON 字符串以二进制格式，不能由用户更改这些值。</span><span class="sxs-lookup"><span data-stu-id="8bbc2-142">Policy settings JSON string in binary format, these values cannot be changed by the user.</span></span> <span data-ttu-id="8bbc2-143">继承自[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8bbc2-143">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="8bbc2-144">说明</span><span class="sxs-lookup"><span data-stu-id="8bbc2-144">description</span></span>|<span data-ttu-id="8bbc2-145">字符串</span><span class="sxs-lookup"><span data-stu-id="8bbc2-145">String</span></span>|<span data-ttu-id="8bbc2-146">管理员提供的 office 客户端的说明配置策略。</span><span class="sxs-lookup"><span data-stu-id="8bbc2-146">Admin provided description of the office client configuration policy.</span></span> <span data-ttu-id="8bbc2-147">继承自[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8bbc2-147">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="8bbc2-148">displayName</span><span class="sxs-lookup"><span data-stu-id="8bbc2-148">displayName</span></span>|<span data-ttu-id="8bbc2-149">字符串</span><span class="sxs-lookup"><span data-stu-id="8bbc2-149">String</span></span>|<span data-ttu-id="8bbc2-150">管理员提供的 office 客户端配置策略的名称。</span><span class="sxs-lookup"><span data-stu-id="8bbc2-150">Admin provided name of the office client configuration policy.</span></span> <span data-ttu-id="8bbc2-151">继承自[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8bbc2-151">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="8bbc2-152">priority</span><span class="sxs-lookup"><span data-stu-id="8bbc2-152">priority</span></span>|<span data-ttu-id="8bbc2-153">Int32</span><span class="sxs-lookup"><span data-stu-id="8bbc2-153">Int32</span></span>|<span data-ttu-id="8bbc2-154">优先级值应为每个策略下租户的唯一值并将用于指定在冲突解决，较低值意味着很高的优先级。</span><span class="sxs-lookup"><span data-stu-id="8bbc2-154">Priority value should be unique value for each policy under a tenant and will be used for conflict resolution, lower values mean priority is high.</span></span> <span data-ttu-id="8bbc2-155">继承自[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8bbc2-155">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="8bbc2-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8bbc2-156">lastModifiedDateTime</span></span>|<span data-ttu-id="8bbc2-157">DateTime</span><span class="sxs-lookup"><span data-stu-id="8bbc2-157">DateTime</span></span>|<span data-ttu-id="8bbc2-158">上次修改日期时间戳的策略。</span><span class="sxs-lookup"><span data-stu-id="8bbc2-158">Last modified datetime stamp of the policy.</span></span> <span data-ttu-id="8bbc2-159">继承自[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8bbc2-159">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="8bbc2-160">userCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="8bbc2-160">userCheckinSummary</span></span>|[<span data-ttu-id="8bbc2-161">officeUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="8bbc2-161">officeUserCheckinSummary</span></span>](../resources/intune-cirrus-officeusercheckinsummary.md)|<span data-ttu-id="8bbc2-162">用户签入的摘要策略。</span><span class="sxs-lookup"><span data-stu-id="8bbc2-162">User check-in summary for the policy.</span></span> <span data-ttu-id="8bbc2-163">继承自[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8bbc2-163">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="8bbc2-164">checkinStatuses</span><span class="sxs-lookup"><span data-stu-id="8bbc2-164">checkinStatuses</span></span>|<span data-ttu-id="8bbc2-165">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md)集合</span><span class="sxs-lookup"><span data-stu-id="8bbc2-165">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) collection</span></span>|<span data-ttu-id="8bbc2-166">Office 客户端中签入状态的列表。</span><span class="sxs-lookup"><span data-stu-id="8bbc2-166">List of office Client check-in status.</span></span> <span data-ttu-id="8bbc2-167">继承自[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8bbc2-167">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="8bbc2-168">Relationships</span><span class="sxs-lookup"><span data-stu-id="8bbc2-168">Relationships</span></span>
|<span data-ttu-id="8bbc2-169">关系</span><span class="sxs-lookup"><span data-stu-id="8bbc2-169">Relationship</span></span>|<span data-ttu-id="8bbc2-170">类型</span><span class="sxs-lookup"><span data-stu-id="8bbc2-170">Type</span></span>|<span data-ttu-id="8bbc2-171">说明</span><span class="sxs-lookup"><span data-stu-id="8bbc2-171">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8bbc2-172">assignments</span><span class="sxs-lookup"><span data-stu-id="8bbc2-172">assignments</span></span>|<span data-ttu-id="8bbc2-173">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="8bbc2-173">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) collection</span></span>|<span data-ttu-id="8bbc2-174">组策略的工作分配列表。</span><span class="sxs-lookup"><span data-stu-id="8bbc2-174">The list of group assignments for the policy.</span></span> <span data-ttu-id="8bbc2-175">继承自[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8bbc2-175">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8bbc2-176">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8bbc2-176">JSON Representation</span></span>
<span data-ttu-id="8bbc2-177">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8bbc2-177">Here is a JSON representation of the resource.</span></span>
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




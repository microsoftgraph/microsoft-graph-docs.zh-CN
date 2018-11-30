---
title: officeClientConfiguration 资源类型
description: Office 客户端配置。
ms.openlocfilehash: de510d7a57c10d1f74a3e58856afb9233243ec17
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27044439"
---
# <a name="officeclientconfiguration-resource-type"></a><span data-ttu-id="1b326-103">officeClientConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="1b326-103">officeClientConfiguration resource type</span></span>

> <span data-ttu-id="1b326-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="1b326-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1b326-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="1b326-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1b326-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="1b326-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1b326-107">Office 客户端配置。</span><span class="sxs-lookup"><span data-stu-id="1b326-107">Office Client Configuration.</span></span>
## <a name="methods"></a><span data-ttu-id="1b326-108">方法</span><span class="sxs-lookup"><span data-stu-id="1b326-108">Methods</span></span>
|<span data-ttu-id="1b326-109">方法</span><span class="sxs-lookup"><span data-stu-id="1b326-109">Method</span></span>|<span data-ttu-id="1b326-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="1b326-110">Return Type</span></span>|<span data-ttu-id="1b326-111">说明</span><span class="sxs-lookup"><span data-stu-id="1b326-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="1b326-112">列表 officeClientConfigurations</span><span class="sxs-lookup"><span data-stu-id="1b326-112">List officeClientConfigurations</span></span>](../api/intune-cirrus-officeclientconfiguration-list.md)|<span data-ttu-id="1b326-113">[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)集合</span><span class="sxs-lookup"><span data-stu-id="1b326-113">[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) collection</span></span>|<span data-ttu-id="1b326-114">列出属性和[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)对象之间的关系。</span><span class="sxs-lookup"><span data-stu-id="1b326-114">List properties and relationships of the [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="1b326-115">获取 officeClientConfiguration</span><span class="sxs-lookup"><span data-stu-id="1b326-115">Get officeClientConfiguration</span></span>](../api/intune-cirrus-officeclientconfiguration-get.md)|[<span data-ttu-id="1b326-116">officeClientConfiguration</span><span class="sxs-lookup"><span data-stu-id="1b326-116">officeClientConfiguration</span></span>](../resources/intune-cirrus-officeclientconfiguration.md)|<span data-ttu-id="1b326-117">读取属性和[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="1b326-117">Read properties and relationships of the [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) object.</span></span>|
|[<span data-ttu-id="1b326-118">assign 操作</span><span class="sxs-lookup"><span data-stu-id="1b326-118">assign action</span></span>](../api/intune-cirrus-officeclientconfiguration-assign.md)|<span data-ttu-id="1b326-119">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="1b326-119">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) collection</span></span>|<span data-ttu-id="1b326-120">更换所有目标的组策略。</span><span class="sxs-lookup"><span data-stu-id="1b326-120">Replace all targeted groups for a policy.</span></span>|
|[<span data-ttu-id="1b326-121">updatePriorities 操作</span><span class="sxs-lookup"><span data-stu-id="1b326-121">updatePriorities action</span></span>](../api/intune-cirrus-officeclientconfiguration-updatepriorities.md)|<span data-ttu-id="1b326-122">无</span><span class="sxs-lookup"><span data-stu-id="1b326-122">None</span></span>|<span data-ttu-id="1b326-123">更新策略优先级。</span><span class="sxs-lookup"><span data-stu-id="1b326-123">Update policy priorities.</span></span>|

## <a name="properties"></a><span data-ttu-id="1b326-124">属性</span><span class="sxs-lookup"><span data-stu-id="1b326-124">Properties</span></span>
|<span data-ttu-id="1b326-125">属性</span><span class="sxs-lookup"><span data-stu-id="1b326-125">Property</span></span>|<span data-ttu-id="1b326-126">类型</span><span class="sxs-lookup"><span data-stu-id="1b326-126">Type</span></span>|<span data-ttu-id="1b326-127">说明</span><span class="sxs-lookup"><span data-stu-id="1b326-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1b326-128">id</span><span class="sxs-lookup"><span data-stu-id="1b326-128">id</span></span>|<span data-ttu-id="1b326-129">字符串</span><span class="sxs-lookup"><span data-stu-id="1b326-129">String</span></span>|<span data-ttu-id="1b326-130">Office 客户端配置策略的 id。</span><span class="sxs-lookup"><span data-stu-id="1b326-130">Id of the office client configuration policy.</span></span>|
|<span data-ttu-id="1b326-131">userPreferencePayload</span><span class="sxs-lookup"><span data-stu-id="1b326-131">userPreferencePayload</span></span>|<span data-ttu-id="1b326-132">Stream</span><span class="sxs-lookup"><span data-stu-id="1b326-132">Stream</span></span>|<span data-ttu-id="1b326-133">首选项设置为 JSON 字符串以二进制格式，用户可以重写这些值。</span><span class="sxs-lookup"><span data-stu-id="1b326-133">Preference settings JSON string in binary format, these values can be overridden by the user.</span></span>|
|<span data-ttu-id="1b326-134">policyPayload</span><span class="sxs-lookup"><span data-stu-id="1b326-134">policyPayload</span></span>|<span data-ttu-id="1b326-135">Stream</span><span class="sxs-lookup"><span data-stu-id="1b326-135">Stream</span></span>|<span data-ttu-id="1b326-136">策略设置 JSON 字符串以二进制格式，不能由用户更改这些值。</span><span class="sxs-lookup"><span data-stu-id="1b326-136">Policy settings JSON string in binary format, these values cannot be changed by the user.</span></span>|
|<span data-ttu-id="1b326-137">说明</span><span class="sxs-lookup"><span data-stu-id="1b326-137">description</span></span>|<span data-ttu-id="1b326-138">字符串</span><span class="sxs-lookup"><span data-stu-id="1b326-138">String</span></span>|<span data-ttu-id="1b326-139">尚未记录</span><span class="sxs-lookup"><span data-stu-id="1b326-139">Not yet documented</span></span>|
|<span data-ttu-id="1b326-140">displayName</span><span class="sxs-lookup"><span data-stu-id="1b326-140">displayName</span></span>|<span data-ttu-id="1b326-141">字符串</span><span class="sxs-lookup"><span data-stu-id="1b326-141">String</span></span>|<span data-ttu-id="1b326-142">管理员提供的 office 客户端的说明配置策略。</span><span class="sxs-lookup"><span data-stu-id="1b326-142">Admin provided description of the office client configuration policy.</span></span>|
|<span data-ttu-id="1b326-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1b326-143">lastModifiedDateTime</span></span>|<span data-ttu-id="1b326-144">DateTime</span><span class="sxs-lookup"><span data-stu-id="1b326-144">DateTime</span></span>|<span data-ttu-id="1b326-145">上次修改日期时间戳的策略。</span><span class="sxs-lookup"><span data-stu-id="1b326-145">Last modified datetime stamp of the policy.</span></span>|
|<span data-ttu-id="1b326-146">priority</span><span class="sxs-lookup"><span data-stu-id="1b326-146">priority</span></span>|<span data-ttu-id="1b326-147">Int32</span><span class="sxs-lookup"><span data-stu-id="1b326-147">Int32</span></span>|<span data-ttu-id="1b326-148">优先级值应为每个策略下租户的唯一值并将用于指定在冲突解决，较低值意味着很高的优先级。</span><span class="sxs-lookup"><span data-stu-id="1b326-148">Priority value should be unique value for each policy under a tenant and will be used for conflict resolution, lower values mean priority is high.</span></span>|
|<span data-ttu-id="1b326-149">userCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="1b326-149">userCheckinSummary</span></span>|[<span data-ttu-id="1b326-150">officeUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="1b326-150">officeUserCheckinSummary</span></span>](../resources/intune-cirrus-officeusercheckinsummary.md)|<span data-ttu-id="1b326-151">用户签入的摘要策略。</span><span class="sxs-lookup"><span data-stu-id="1b326-151">User check-in summary for the policy.</span></span>|
|<span data-ttu-id="1b326-152">checkinStatuses</span><span class="sxs-lookup"><span data-stu-id="1b326-152">checkinStatuses</span></span>|<span data-ttu-id="1b326-153">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md)集合</span><span class="sxs-lookup"><span data-stu-id="1b326-153">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) collection</span></span>|<span data-ttu-id="1b326-154">Office 客户端中签入状态的列表。</span><span class="sxs-lookup"><span data-stu-id="1b326-154">List of office Client check-in status.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1b326-155">Relationships</span><span class="sxs-lookup"><span data-stu-id="1b326-155">Relationships</span></span>
|<span data-ttu-id="1b326-156">关系</span><span class="sxs-lookup"><span data-stu-id="1b326-156">Relationship</span></span>|<span data-ttu-id="1b326-157">类型</span><span class="sxs-lookup"><span data-stu-id="1b326-157">Type</span></span>|<span data-ttu-id="1b326-158">说明</span><span class="sxs-lookup"><span data-stu-id="1b326-158">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1b326-159">assignments</span><span class="sxs-lookup"><span data-stu-id="1b326-159">assignments</span></span>|<span data-ttu-id="1b326-160">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="1b326-160">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) collection</span></span>|<span data-ttu-id="1b326-161">组策略的工作分配列表。</span><span class="sxs-lookup"><span data-stu-id="1b326-161">The list of group assignments for the policy.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1b326-162">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1b326-162">JSON Representation</span></span>
<span data-ttu-id="1b326-163">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1b326-163">Here is a JSON representation of the resource.</span></span>
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




---
title: managedDeviceMobileAppConfigurationUserSummary 资源类型
description: 包含 MDM 移动应用配置用户状态摘要的属性、继承属性和操作。
localization_priority: Normal
ms.openlocfilehash: 7b409e81e1fe82237d739dc5e8b75ce42e74a783
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27805416"
---
# <a name="manageddevicemobileappconfigurationusersummary-resource-type"></a><span data-ttu-id="1aa46-103">managedDeviceMobileAppConfigurationUserSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="1aa46-103">managedDeviceMobileAppConfigurationUserSummary resource type</span></span>

> <span data-ttu-id="1aa46-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="1aa46-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1aa46-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="1aa46-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1aa46-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="1aa46-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1aa46-107">包含 MDM 移动应用配置用户状态摘要的属性、继承属性和操作。</span><span class="sxs-lookup"><span data-stu-id="1aa46-107">Contains properties, inherited properties and actions for an MDM mobile app configuration user status summary.</span></span>
## <a name="methods"></a><span data-ttu-id="1aa46-108">方法</span><span class="sxs-lookup"><span data-stu-id="1aa46-108">Methods</span></span>
|<span data-ttu-id="1aa46-109">方法</span><span class="sxs-lookup"><span data-stu-id="1aa46-109">Method</span></span>|<span data-ttu-id="1aa46-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="1aa46-110">Return Type</span></span>|<span data-ttu-id="1aa46-111">说明</span><span class="sxs-lookup"><span data-stu-id="1aa46-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="1aa46-112">获取 managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="1aa46-112">Get managedDeviceMobileAppConfigurationUserSummary</span></span>](../api/intune-apps-manageddevicemobileappconfigurationusersummary-get.md)|[<span data-ttu-id="1aa46-113">managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="1aa46-113">managedDeviceMobileAppConfigurationUserSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md)|<span data-ttu-id="1aa46-114">读取 [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="1aa46-114">Read properties and relationships of the [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) object.</span></span>|
|[<span data-ttu-id="1aa46-115">更新 managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="1aa46-115">Update managedDeviceMobileAppConfigurationUserSummary</span></span>](../api/intune-apps-manageddevicemobileappconfigurationusersummary-update.md)|[<span data-ttu-id="1aa46-116">managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="1aa46-116">managedDeviceMobileAppConfigurationUserSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md)|<span data-ttu-id="1aa46-117">更新 [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="1aa46-117">Update the properties of a [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="1aa46-118">属性</span><span class="sxs-lookup"><span data-stu-id="1aa46-118">Properties</span></span>
|<span data-ttu-id="1aa46-119">属性</span><span class="sxs-lookup"><span data-stu-id="1aa46-119">Property</span></span>|<span data-ttu-id="1aa46-120">类型</span><span class="sxs-lookup"><span data-stu-id="1aa46-120">Type</span></span>|<span data-ttu-id="1aa46-121">说明</span><span class="sxs-lookup"><span data-stu-id="1aa46-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1aa46-122">id</span><span class="sxs-lookup"><span data-stu-id="1aa46-122">id</span></span>|<span data-ttu-id="1aa46-123">String</span><span class="sxs-lookup"><span data-stu-id="1aa46-123">String</span></span>|<span data-ttu-id="1aa46-124">实体的键。</span><span class="sxs-lookup"><span data-stu-id="1aa46-124">Key of the entity.</span></span>|
|<span data-ttu-id="1aa46-125">pendingCount</span><span class="sxs-lookup"><span data-stu-id="1aa46-125">pendingCount</span></span>|<span data-ttu-id="1aa46-126">Int32</span><span class="sxs-lookup"><span data-stu-id="1aa46-126">Int32</span></span>|<span data-ttu-id="1aa46-127">待定用户的数量</span><span class="sxs-lookup"><span data-stu-id="1aa46-127">Number of pending Users</span></span>|
|<span data-ttu-id="1aa46-128">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="1aa46-128">notApplicableCount</span></span>|<span data-ttu-id="1aa46-129">Int32</span><span class="sxs-lookup"><span data-stu-id="1aa46-129">Int32</span></span>|<span data-ttu-id="1aa46-130">不适用的用户数</span><span class="sxs-lookup"><span data-stu-id="1aa46-130">Number of not applicable users</span></span>|
|<span data-ttu-id="1aa46-131">successCount</span><span class="sxs-lookup"><span data-stu-id="1aa46-131">successCount</span></span>|<span data-ttu-id="1aa46-132">Int32</span><span class="sxs-lookup"><span data-stu-id="1aa46-132">Int32</span></span>|<span data-ttu-id="1aa46-133">成功用户的数量</span><span class="sxs-lookup"><span data-stu-id="1aa46-133">Number of succeeded Users</span></span>|
|<span data-ttu-id="1aa46-134">errorCount</span><span class="sxs-lookup"><span data-stu-id="1aa46-134">errorCount</span></span>|<span data-ttu-id="1aa46-135">Int32</span><span class="sxs-lookup"><span data-stu-id="1aa46-135">Int32</span></span>|<span data-ttu-id="1aa46-136">错误用户的数量</span><span class="sxs-lookup"><span data-stu-id="1aa46-136">Number of error Users</span></span>|
|<span data-ttu-id="1aa46-137">failedCount</span><span class="sxs-lookup"><span data-stu-id="1aa46-137">failedCount</span></span>|<span data-ttu-id="1aa46-138">Int32</span><span class="sxs-lookup"><span data-stu-id="1aa46-138">Int32</span></span>|<span data-ttu-id="1aa46-139">失败用户的数量</span><span class="sxs-lookup"><span data-stu-id="1aa46-139">Number of failed Users</span></span>|
|<span data-ttu-id="1aa46-140">conflictCount</span><span class="sxs-lookup"><span data-stu-id="1aa46-140">conflictCount</span></span>|<span data-ttu-id="1aa46-141">Int32</span><span class="sxs-lookup"><span data-stu-id="1aa46-141">Int32</span></span>|<span data-ttu-id="1aa46-142">存在冲突的用户数</span><span class="sxs-lookup"><span data-stu-id="1aa46-142">Number of users in conflict</span></span>|
|<span data-ttu-id="1aa46-143">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="1aa46-143">lastUpdateDateTime</span></span>|<span data-ttu-id="1aa46-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1aa46-144">DateTimeOffset</span></span>|<span data-ttu-id="1aa46-145">上次更新时间</span><span class="sxs-lookup"><span data-stu-id="1aa46-145">Last update time</span></span>|
|<span data-ttu-id="1aa46-146">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="1aa46-146">configurationVersion</span></span>|<span data-ttu-id="1aa46-147">Int32</span><span class="sxs-lookup"><span data-stu-id="1aa46-147">Int32</span></span>|<span data-ttu-id="1aa46-148">用于此概述的策略版本</span><span class="sxs-lookup"><span data-stu-id="1aa46-148">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="1aa46-149">关系</span><span class="sxs-lookup"><span data-stu-id="1aa46-149">Relationships</span></span>
<span data-ttu-id="1aa46-150">无</span><span class="sxs-lookup"><span data-stu-id="1aa46-150">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="1aa46-151">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1aa46-151">JSON Representation</span></span>
<span data-ttu-id="1aa46-152">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1aa46-152">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDeviceMobileAppConfigurationUserSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationUserSummary",
  "id": "String (identifier)",
  "pendingCount": 1024,
  "notApplicableCount": 1024,
  "successCount": 1024,
  "errorCount": 1024,
  "failedCount": 1024,
  "conflictCount": 1024,
  "lastUpdateDateTime": "String (timestamp)",
  "configurationVersion": 1024
}
```






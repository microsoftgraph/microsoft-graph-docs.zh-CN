---
title: managedDeviceMobileAppConfigurationUserSummary 资源类型
description: 包含 MDM 移动应用配置用户状态摘要的属性、继承属性和操作。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 34f6d8254e743f4a294d2351c291631d2ae65a51
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399869"
---
# <a name="manageddevicemobileappconfigurationusersummary-resource-type"></a><span data-ttu-id="be980-103">managedDeviceMobileAppConfigurationUserSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="be980-103">managedDeviceMobileAppConfigurationUserSummary resource type</span></span>

> <span data-ttu-id="be980-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="be980-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="be980-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="be980-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="be980-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="be980-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="be980-107">包含 MDM 移动应用配置用户状态摘要的属性、继承属性和操作。</span><span class="sxs-lookup"><span data-stu-id="be980-107">Contains properties, inherited properties and actions for an MDM mobile app configuration user status summary.</span></span>

## <a name="methods"></a><span data-ttu-id="be980-108">方法</span><span class="sxs-lookup"><span data-stu-id="be980-108">Methods</span></span>
|<span data-ttu-id="be980-109">方法</span><span class="sxs-lookup"><span data-stu-id="be980-109">Method</span></span>|<span data-ttu-id="be980-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="be980-110">Return Type</span></span>|<span data-ttu-id="be980-111">说明</span><span class="sxs-lookup"><span data-stu-id="be980-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="be980-112">获取 managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="be980-112">Get managedDeviceMobileAppConfigurationUserSummary</span></span>](../api/intune-apps-manageddevicemobileappconfigurationusersummary-get.md)|[<span data-ttu-id="be980-113">managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="be980-113">managedDeviceMobileAppConfigurationUserSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md)|<span data-ttu-id="be980-114">读取 [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="be980-114">Read properties and relationships of the [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) object.</span></span>|
|[<span data-ttu-id="be980-115">更新 managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="be980-115">Update managedDeviceMobileAppConfigurationUserSummary</span></span>](../api/intune-apps-manageddevicemobileappconfigurationusersummary-update.md)|[<span data-ttu-id="be980-116">managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="be980-116">managedDeviceMobileAppConfigurationUserSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md)|<span data-ttu-id="be980-117">更新 [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="be980-117">Update the properties of a [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="be980-118">属性</span><span class="sxs-lookup"><span data-stu-id="be980-118">Properties</span></span>
|<span data-ttu-id="be980-119">属性</span><span class="sxs-lookup"><span data-stu-id="be980-119">Property</span></span>|<span data-ttu-id="be980-120">类型</span><span class="sxs-lookup"><span data-stu-id="be980-120">Type</span></span>|<span data-ttu-id="be980-121">说明</span><span class="sxs-lookup"><span data-stu-id="be980-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="be980-122">id</span><span class="sxs-lookup"><span data-stu-id="be980-122">id</span></span>|<span data-ttu-id="be980-123">String</span><span class="sxs-lookup"><span data-stu-id="be980-123">String</span></span>|<span data-ttu-id="be980-124">实体的键。</span><span class="sxs-lookup"><span data-stu-id="be980-124">Key of the entity.</span></span>|
|<span data-ttu-id="be980-125">pendingCount</span><span class="sxs-lookup"><span data-stu-id="be980-125">pendingCount</span></span>|<span data-ttu-id="be980-126">Int32</span><span class="sxs-lookup"><span data-stu-id="be980-126">Int32</span></span>|<span data-ttu-id="be980-127">待定用户的数量</span><span class="sxs-lookup"><span data-stu-id="be980-127">Number of pending Users</span></span>|
|<span data-ttu-id="be980-128">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="be980-128">notApplicableCount</span></span>|<span data-ttu-id="be980-129">Int32</span><span class="sxs-lookup"><span data-stu-id="be980-129">Int32</span></span>|<span data-ttu-id="be980-130">不适用的用户数</span><span class="sxs-lookup"><span data-stu-id="be980-130">Number of not applicable users</span></span>|
|<span data-ttu-id="be980-131">successCount</span><span class="sxs-lookup"><span data-stu-id="be980-131">successCount</span></span>|<span data-ttu-id="be980-132">Int32</span><span class="sxs-lookup"><span data-stu-id="be980-132">Int32</span></span>|<span data-ttu-id="be980-133">成功用户的数量</span><span class="sxs-lookup"><span data-stu-id="be980-133">Number of succeeded Users</span></span>|
|<span data-ttu-id="be980-134">errorCount</span><span class="sxs-lookup"><span data-stu-id="be980-134">errorCount</span></span>|<span data-ttu-id="be980-135">Int32</span><span class="sxs-lookup"><span data-stu-id="be980-135">Int32</span></span>|<span data-ttu-id="be980-136">错误用户的数量</span><span class="sxs-lookup"><span data-stu-id="be980-136">Number of error Users</span></span>|
|<span data-ttu-id="be980-137">failedCount</span><span class="sxs-lookup"><span data-stu-id="be980-137">failedCount</span></span>|<span data-ttu-id="be980-138">Int32</span><span class="sxs-lookup"><span data-stu-id="be980-138">Int32</span></span>|<span data-ttu-id="be980-139">失败用户的数量</span><span class="sxs-lookup"><span data-stu-id="be980-139">Number of failed Users</span></span>|
|<span data-ttu-id="be980-140">conflictCount</span><span class="sxs-lookup"><span data-stu-id="be980-140">conflictCount</span></span>|<span data-ttu-id="be980-141">Int32</span><span class="sxs-lookup"><span data-stu-id="be980-141">Int32</span></span>|<span data-ttu-id="be980-142">存在冲突的用户数</span><span class="sxs-lookup"><span data-stu-id="be980-142">Number of users in conflict</span></span>|
|<span data-ttu-id="be980-143">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="be980-143">lastUpdateDateTime</span></span>|<span data-ttu-id="be980-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="be980-144">DateTimeOffset</span></span>|<span data-ttu-id="be980-145">上次更新时间</span><span class="sxs-lookup"><span data-stu-id="be980-145">Last update time</span></span>|
|<span data-ttu-id="be980-146">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="be980-146">configurationVersion</span></span>|<span data-ttu-id="be980-147">Int32</span><span class="sxs-lookup"><span data-stu-id="be980-147">Int32</span></span>|<span data-ttu-id="be980-148">用于此概述的策略版本</span><span class="sxs-lookup"><span data-stu-id="be980-148">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="be980-149">关系</span><span class="sxs-lookup"><span data-stu-id="be980-149">Relationships</span></span>
<span data-ttu-id="be980-150">无</span><span class="sxs-lookup"><span data-stu-id="be980-150">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="be980-151">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="be980-151">JSON Representation</span></span>
<span data-ttu-id="be980-152">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="be980-152">Here is a JSON representation of the resource.</span></span>
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





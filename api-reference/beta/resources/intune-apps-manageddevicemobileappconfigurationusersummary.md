---
title: managedDeviceMobileAppConfigurationUserSummary 资源类型
description: 包含 MDM 移动应用配置用户状态摘要的属性、继承属性和操作。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c135f63675dc6fb8cf4105578aa20ec8634c2ced
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42797921"
---
# <a name="manageddevicemobileappconfigurationusersummary-resource-type"></a><span data-ttu-id="28545-103">managedDeviceMobileAppConfigurationUserSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="28545-103">managedDeviceMobileAppConfigurationUserSummary resource type</span></span>

> <span data-ttu-id="28545-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="28545-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="28545-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="28545-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="28545-106">包含 MDM 移动应用配置用户状态摘要的属性、继承属性和操作。</span><span class="sxs-lookup"><span data-stu-id="28545-106">Contains properties, inherited properties and actions for an MDM mobile app configuration user status summary.</span></span>

## <a name="methods"></a><span data-ttu-id="28545-107">方法</span><span class="sxs-lookup"><span data-stu-id="28545-107">Methods</span></span>
|<span data-ttu-id="28545-108">方法</span><span class="sxs-lookup"><span data-stu-id="28545-108">Method</span></span>|<span data-ttu-id="28545-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="28545-109">Return Type</span></span>|<span data-ttu-id="28545-110">说明</span><span class="sxs-lookup"><span data-stu-id="28545-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="28545-111">获取 managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="28545-111">Get managedDeviceMobileAppConfigurationUserSummary</span></span>](../api/intune-apps-manageddevicemobileappconfigurationusersummary-get.md)|[<span data-ttu-id="28545-112">managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="28545-112">managedDeviceMobileAppConfigurationUserSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md)|<span data-ttu-id="28545-113">读取 [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="28545-113">Read properties and relationships of the [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) object.</span></span>|
|[<span data-ttu-id="28545-114">更新 managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="28545-114">Update managedDeviceMobileAppConfigurationUserSummary</span></span>](../api/intune-apps-manageddevicemobileappconfigurationusersummary-update.md)|[<span data-ttu-id="28545-115">managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="28545-115">managedDeviceMobileAppConfigurationUserSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md)|<span data-ttu-id="28545-116">更新 [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="28545-116">Update the properties of a [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="28545-117">属性</span><span class="sxs-lookup"><span data-stu-id="28545-117">Properties</span></span>
|<span data-ttu-id="28545-118">属性</span><span class="sxs-lookup"><span data-stu-id="28545-118">Property</span></span>|<span data-ttu-id="28545-119">类型</span><span class="sxs-lookup"><span data-stu-id="28545-119">Type</span></span>|<span data-ttu-id="28545-120">说明</span><span class="sxs-lookup"><span data-stu-id="28545-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="28545-121">id</span><span class="sxs-lookup"><span data-stu-id="28545-121">id</span></span>|<span data-ttu-id="28545-122">String</span><span class="sxs-lookup"><span data-stu-id="28545-122">String</span></span>|<span data-ttu-id="28545-123">实体的键。</span><span class="sxs-lookup"><span data-stu-id="28545-123">Key of the entity.</span></span>|
|<span data-ttu-id="28545-124">pendingCount</span><span class="sxs-lookup"><span data-stu-id="28545-124">pendingCount</span></span>|<span data-ttu-id="28545-125">Int32</span><span class="sxs-lookup"><span data-stu-id="28545-125">Int32</span></span>|<span data-ttu-id="28545-126">待定用户的数量</span><span class="sxs-lookup"><span data-stu-id="28545-126">Number of pending Users</span></span>|
|<span data-ttu-id="28545-127">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="28545-127">notApplicableCount</span></span>|<span data-ttu-id="28545-128">Int32</span><span class="sxs-lookup"><span data-stu-id="28545-128">Int32</span></span>|<span data-ttu-id="28545-129">不适用的用户数</span><span class="sxs-lookup"><span data-stu-id="28545-129">Number of not applicable users</span></span>|
|<span data-ttu-id="28545-130">successCount</span><span class="sxs-lookup"><span data-stu-id="28545-130">successCount</span></span>|<span data-ttu-id="28545-131">Int32</span><span class="sxs-lookup"><span data-stu-id="28545-131">Int32</span></span>|<span data-ttu-id="28545-132">成功用户的数量</span><span class="sxs-lookup"><span data-stu-id="28545-132">Number of succeeded Users</span></span>|
|<span data-ttu-id="28545-133">errorCount</span><span class="sxs-lookup"><span data-stu-id="28545-133">errorCount</span></span>|<span data-ttu-id="28545-134">Int32</span><span class="sxs-lookup"><span data-stu-id="28545-134">Int32</span></span>|<span data-ttu-id="28545-135">错误用户的数量</span><span class="sxs-lookup"><span data-stu-id="28545-135">Number of error Users</span></span>|
|<span data-ttu-id="28545-136">failedCount</span><span class="sxs-lookup"><span data-stu-id="28545-136">failedCount</span></span>|<span data-ttu-id="28545-137">Int32</span><span class="sxs-lookup"><span data-stu-id="28545-137">Int32</span></span>|<span data-ttu-id="28545-138">失败用户的数量</span><span class="sxs-lookup"><span data-stu-id="28545-138">Number of failed Users</span></span>|
|<span data-ttu-id="28545-139">conflictCount</span><span class="sxs-lookup"><span data-stu-id="28545-139">conflictCount</span></span>|<span data-ttu-id="28545-140">Int32</span><span class="sxs-lookup"><span data-stu-id="28545-140">Int32</span></span>|<span data-ttu-id="28545-141">发生冲突的用户数</span><span class="sxs-lookup"><span data-stu-id="28545-141">Number of users in conflict</span></span>|
|<span data-ttu-id="28545-142">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="28545-142">lastUpdateDateTime</span></span>|<span data-ttu-id="28545-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="28545-143">DateTimeOffset</span></span>|<span data-ttu-id="28545-144">上次更新时间</span><span class="sxs-lookup"><span data-stu-id="28545-144">Last update time</span></span>|
|<span data-ttu-id="28545-145">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="28545-145">configurationVersion</span></span>|<span data-ttu-id="28545-146">Int32</span><span class="sxs-lookup"><span data-stu-id="28545-146">Int32</span></span>|<span data-ttu-id="28545-147">用于此概述的策略版本</span><span class="sxs-lookup"><span data-stu-id="28545-147">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="28545-148">关系</span><span class="sxs-lookup"><span data-stu-id="28545-148">Relationships</span></span>
<span data-ttu-id="28545-149">无</span><span class="sxs-lookup"><span data-stu-id="28545-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="28545-150">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="28545-150">JSON Representation</span></span>
<span data-ttu-id="28545-151">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="28545-151">Here is a JSON representation of the resource.</span></span>
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




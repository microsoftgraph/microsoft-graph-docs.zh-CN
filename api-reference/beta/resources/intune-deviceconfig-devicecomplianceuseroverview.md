---
title: deviceComplianceUserOverview 资源类型
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 112b366f9678d092b0a59699d9a9931376819eca
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30173421"
---
# <a name="devicecomplianceuseroverview-resource-type"></a><span data-ttu-id="66c08-103">deviceComplianceUserOverview 资源类型</span><span class="sxs-lookup"><span data-stu-id="66c08-103">deviceComplianceUserOverview resource type</span></span>

> <span data-ttu-id="66c08-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="66c08-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="66c08-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="66c08-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="66c08-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="66c08-106">Not yet documented</span></span>

## <a name="methods"></a><span data-ttu-id="66c08-107">方法</span><span class="sxs-lookup"><span data-stu-id="66c08-107">Methods</span></span>
|<span data-ttu-id="66c08-108">方法</span><span class="sxs-lookup"><span data-stu-id="66c08-108">Method</span></span>|<span data-ttu-id="66c08-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="66c08-109">Return Type</span></span>|<span data-ttu-id="66c08-110">说明</span><span class="sxs-lookup"><span data-stu-id="66c08-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="66c08-111">获取 deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="66c08-111">Get deviceComplianceUserOverview</span></span>](../api/intune-deviceconfig-devicecomplianceuseroverview-get.md)|[<span data-ttu-id="66c08-112">deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="66c08-112">deviceComplianceUserOverview</span></span>](../resources/intune-deviceconfig-devicecomplianceuseroverview.md)|<span data-ttu-id="66c08-113">读取 [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="66c08-113">Read properties and relationships of the [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object.</span></span>|
|[<span data-ttu-id="66c08-114">更新 deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="66c08-114">Update deviceComplianceUserOverview</span></span>](../api/intune-deviceconfig-devicecomplianceuseroverview-update.md)|[<span data-ttu-id="66c08-115">deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="66c08-115">deviceComplianceUserOverview</span></span>](../resources/intune-deviceconfig-devicecomplianceuseroverview.md)|<span data-ttu-id="66c08-116">更新 [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="66c08-116">Update the properties of a [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="66c08-117">属性</span><span class="sxs-lookup"><span data-stu-id="66c08-117">Properties</span></span>
|<span data-ttu-id="66c08-118">属性</span><span class="sxs-lookup"><span data-stu-id="66c08-118">Property</span></span>|<span data-ttu-id="66c08-119">类型</span><span class="sxs-lookup"><span data-stu-id="66c08-119">Type</span></span>|<span data-ttu-id="66c08-120">说明</span><span class="sxs-lookup"><span data-stu-id="66c08-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="66c08-121">id</span><span class="sxs-lookup"><span data-stu-id="66c08-121">id</span></span>|<span data-ttu-id="66c08-122">String</span><span class="sxs-lookup"><span data-stu-id="66c08-122">String</span></span>|<span data-ttu-id="66c08-123">实体的键。</span><span class="sxs-lookup"><span data-stu-id="66c08-123">Key of the entity.</span></span>|
|<span data-ttu-id="66c08-124">pendingCount</span><span class="sxs-lookup"><span data-stu-id="66c08-124">pendingCount</span></span>|<span data-ttu-id="66c08-125">Int32</span><span class="sxs-lookup"><span data-stu-id="66c08-125">Int32</span></span>|<span data-ttu-id="66c08-126">待定用户的数量</span><span class="sxs-lookup"><span data-stu-id="66c08-126">Number of pending Users</span></span>|
|<span data-ttu-id="66c08-127">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="66c08-127">notApplicableCount</span></span>|<span data-ttu-id="66c08-128">Int32</span><span class="sxs-lookup"><span data-stu-id="66c08-128">Int32</span></span>|<span data-ttu-id="66c08-129">不适用的用户数</span><span class="sxs-lookup"><span data-stu-id="66c08-129">Number of not applicable users</span></span>|
|<span data-ttu-id="66c08-130">successCount</span><span class="sxs-lookup"><span data-stu-id="66c08-130">successCount</span></span>|<span data-ttu-id="66c08-131">Int32</span><span class="sxs-lookup"><span data-stu-id="66c08-131">Int32</span></span>|<span data-ttu-id="66c08-132">成功用户的数量</span><span class="sxs-lookup"><span data-stu-id="66c08-132">Number of succeeded Users</span></span>|
|<span data-ttu-id="66c08-133">errorCount</span><span class="sxs-lookup"><span data-stu-id="66c08-133">errorCount</span></span>|<span data-ttu-id="66c08-134">Int32</span><span class="sxs-lookup"><span data-stu-id="66c08-134">Int32</span></span>|<span data-ttu-id="66c08-135">错误用户的数量</span><span class="sxs-lookup"><span data-stu-id="66c08-135">Number of error Users</span></span>|
|<span data-ttu-id="66c08-136">failedCount</span><span class="sxs-lookup"><span data-stu-id="66c08-136">failedCount</span></span>|<span data-ttu-id="66c08-137">Int32</span><span class="sxs-lookup"><span data-stu-id="66c08-137">Int32</span></span>|<span data-ttu-id="66c08-138">失败用户的数量</span><span class="sxs-lookup"><span data-stu-id="66c08-138">Number of failed Users</span></span>|
|<span data-ttu-id="66c08-139">conflictCount</span><span class="sxs-lookup"><span data-stu-id="66c08-139">conflictCount</span></span>|<span data-ttu-id="66c08-140">Int32</span><span class="sxs-lookup"><span data-stu-id="66c08-140">Int32</span></span>|<span data-ttu-id="66c08-141">发生冲突的用户数</span><span class="sxs-lookup"><span data-stu-id="66c08-141">Number of users in conflict</span></span>|
|<span data-ttu-id="66c08-142">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="66c08-142">lastUpdateDateTime</span></span>|<span data-ttu-id="66c08-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="66c08-143">DateTimeOffset</span></span>|<span data-ttu-id="66c08-144">上次更新时间</span><span class="sxs-lookup"><span data-stu-id="66c08-144">Last update time</span></span>|
|<span data-ttu-id="66c08-145">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="66c08-145">configurationVersion</span></span>|<span data-ttu-id="66c08-146">Int32</span><span class="sxs-lookup"><span data-stu-id="66c08-146">Int32</span></span>|<span data-ttu-id="66c08-147">用于此概述的策略版本</span><span class="sxs-lookup"><span data-stu-id="66c08-147">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="66c08-148">关系</span><span class="sxs-lookup"><span data-stu-id="66c08-148">Relationships</span></span>
<span data-ttu-id="66c08-149">无</span><span class="sxs-lookup"><span data-stu-id="66c08-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="66c08-150">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="66c08-150">JSON Representation</span></span>
<span data-ttu-id="66c08-151">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="66c08-151">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceComplianceUserOverview"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComplianceUserOverview",
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





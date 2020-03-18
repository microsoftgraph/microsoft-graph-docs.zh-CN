---
title: deviceComplianceUserOverview 资源类型
description: 尚未记录
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 73ebad2f4facc08d2552db80682eb2f1a2376951
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42793294"
---
# <a name="devicecomplianceuseroverview-resource-type"></a><span data-ttu-id="ba9cc-103">deviceComplianceUserOverview 资源类型</span><span class="sxs-lookup"><span data-stu-id="ba9cc-103">deviceComplianceUserOverview resource type</span></span>

> <span data-ttu-id="ba9cc-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ba9cc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ba9cc-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ba9cc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ba9cc-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="ba9cc-106">Not yet documented</span></span>

## <a name="methods"></a><span data-ttu-id="ba9cc-107">方法</span><span class="sxs-lookup"><span data-stu-id="ba9cc-107">Methods</span></span>
|<span data-ttu-id="ba9cc-108">方法</span><span class="sxs-lookup"><span data-stu-id="ba9cc-108">Method</span></span>|<span data-ttu-id="ba9cc-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="ba9cc-109">Return Type</span></span>|<span data-ttu-id="ba9cc-110">说明</span><span class="sxs-lookup"><span data-stu-id="ba9cc-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ba9cc-111">获取 deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="ba9cc-111">Get deviceComplianceUserOverview</span></span>](../api/intune-deviceconfig-devicecomplianceuseroverview-get.md)|[<span data-ttu-id="ba9cc-112">deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="ba9cc-112">deviceComplianceUserOverview</span></span>](../resources/intune-deviceconfig-devicecomplianceuseroverview.md)|<span data-ttu-id="ba9cc-113">读取 [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ba9cc-113">Read properties and relationships of the [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object.</span></span>|
|[<span data-ttu-id="ba9cc-114">更新 deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="ba9cc-114">Update deviceComplianceUserOverview</span></span>](../api/intune-deviceconfig-devicecomplianceuseroverview-update.md)|[<span data-ttu-id="ba9cc-115">deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="ba9cc-115">deviceComplianceUserOverview</span></span>](../resources/intune-deviceconfig-devicecomplianceuseroverview.md)|<span data-ttu-id="ba9cc-116">更新 [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="ba9cc-116">Update the properties of a [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ba9cc-117">属性</span><span class="sxs-lookup"><span data-stu-id="ba9cc-117">Properties</span></span>
|<span data-ttu-id="ba9cc-118">属性</span><span class="sxs-lookup"><span data-stu-id="ba9cc-118">Property</span></span>|<span data-ttu-id="ba9cc-119">类型</span><span class="sxs-lookup"><span data-stu-id="ba9cc-119">Type</span></span>|<span data-ttu-id="ba9cc-120">说明</span><span class="sxs-lookup"><span data-stu-id="ba9cc-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ba9cc-121">id</span><span class="sxs-lookup"><span data-stu-id="ba9cc-121">id</span></span>|<span data-ttu-id="ba9cc-122">String</span><span class="sxs-lookup"><span data-stu-id="ba9cc-122">String</span></span>|<span data-ttu-id="ba9cc-123">实体的键。</span><span class="sxs-lookup"><span data-stu-id="ba9cc-123">Key of the entity.</span></span>|
|<span data-ttu-id="ba9cc-124">pendingCount</span><span class="sxs-lookup"><span data-stu-id="ba9cc-124">pendingCount</span></span>|<span data-ttu-id="ba9cc-125">Int32</span><span class="sxs-lookup"><span data-stu-id="ba9cc-125">Int32</span></span>|<span data-ttu-id="ba9cc-126">待定用户的数量</span><span class="sxs-lookup"><span data-stu-id="ba9cc-126">Number of pending Users</span></span>|
|<span data-ttu-id="ba9cc-127">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="ba9cc-127">notApplicableCount</span></span>|<span data-ttu-id="ba9cc-128">Int32</span><span class="sxs-lookup"><span data-stu-id="ba9cc-128">Int32</span></span>|<span data-ttu-id="ba9cc-129">不适用的用户数</span><span class="sxs-lookup"><span data-stu-id="ba9cc-129">Number of not applicable users</span></span>|
|<span data-ttu-id="ba9cc-130">successCount</span><span class="sxs-lookup"><span data-stu-id="ba9cc-130">successCount</span></span>|<span data-ttu-id="ba9cc-131">Int32</span><span class="sxs-lookup"><span data-stu-id="ba9cc-131">Int32</span></span>|<span data-ttu-id="ba9cc-132">成功用户的数量</span><span class="sxs-lookup"><span data-stu-id="ba9cc-132">Number of succeeded Users</span></span>|
|<span data-ttu-id="ba9cc-133">errorCount</span><span class="sxs-lookup"><span data-stu-id="ba9cc-133">errorCount</span></span>|<span data-ttu-id="ba9cc-134">Int32</span><span class="sxs-lookup"><span data-stu-id="ba9cc-134">Int32</span></span>|<span data-ttu-id="ba9cc-135">错误用户的数量</span><span class="sxs-lookup"><span data-stu-id="ba9cc-135">Number of error Users</span></span>|
|<span data-ttu-id="ba9cc-136">failedCount</span><span class="sxs-lookup"><span data-stu-id="ba9cc-136">failedCount</span></span>|<span data-ttu-id="ba9cc-137">Int32</span><span class="sxs-lookup"><span data-stu-id="ba9cc-137">Int32</span></span>|<span data-ttu-id="ba9cc-138">失败用户的数量</span><span class="sxs-lookup"><span data-stu-id="ba9cc-138">Number of failed Users</span></span>|
|<span data-ttu-id="ba9cc-139">conflictCount</span><span class="sxs-lookup"><span data-stu-id="ba9cc-139">conflictCount</span></span>|<span data-ttu-id="ba9cc-140">Int32</span><span class="sxs-lookup"><span data-stu-id="ba9cc-140">Int32</span></span>|<span data-ttu-id="ba9cc-141">发生冲突的用户数</span><span class="sxs-lookup"><span data-stu-id="ba9cc-141">Number of users in conflict</span></span>|
|<span data-ttu-id="ba9cc-142">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="ba9cc-142">lastUpdateDateTime</span></span>|<span data-ttu-id="ba9cc-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ba9cc-143">DateTimeOffset</span></span>|<span data-ttu-id="ba9cc-144">上次更新时间</span><span class="sxs-lookup"><span data-stu-id="ba9cc-144">Last update time</span></span>|
|<span data-ttu-id="ba9cc-145">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="ba9cc-145">configurationVersion</span></span>|<span data-ttu-id="ba9cc-146">Int32</span><span class="sxs-lookup"><span data-stu-id="ba9cc-146">Int32</span></span>|<span data-ttu-id="ba9cc-147">用于此概述的策略版本</span><span class="sxs-lookup"><span data-stu-id="ba9cc-147">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="ba9cc-148">关系</span><span class="sxs-lookup"><span data-stu-id="ba9cc-148">Relationships</span></span>
<span data-ttu-id="ba9cc-149">无</span><span class="sxs-lookup"><span data-stu-id="ba9cc-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ba9cc-150">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ba9cc-150">JSON Representation</span></span>
<span data-ttu-id="ba9cc-151">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ba9cc-151">Here is a JSON representation of the resource.</span></span>
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




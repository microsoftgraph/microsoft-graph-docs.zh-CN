---
title: deviceComplianceUserOverview 资源类型
description: 尚未记录
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 93c36baaefaad86e60e975f7ba70c21247902925
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37359500"
---
# <a name="devicecomplianceuseroverview-resource-type"></a><span data-ttu-id="f3b41-103">deviceComplianceUserOverview 资源类型</span><span class="sxs-lookup"><span data-stu-id="f3b41-103">deviceComplianceUserOverview resource type</span></span>

> <span data-ttu-id="f3b41-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f3b41-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f3b41-105">尚未记录</span><span class="sxs-lookup"><span data-stu-id="f3b41-105">Not yet documented</span></span>

## <a name="methods"></a><span data-ttu-id="f3b41-106">方法</span><span class="sxs-lookup"><span data-stu-id="f3b41-106">Methods</span></span>
|<span data-ttu-id="f3b41-107">方法</span><span class="sxs-lookup"><span data-stu-id="f3b41-107">Method</span></span>|<span data-ttu-id="f3b41-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="f3b41-108">Return Type</span></span>|<span data-ttu-id="f3b41-109">说明</span><span class="sxs-lookup"><span data-stu-id="f3b41-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f3b41-110">获取 deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="f3b41-110">Get deviceComplianceUserOverview</span></span>](../api/intune-deviceconfig-devicecomplianceuseroverview-get.md)|[<span data-ttu-id="f3b41-111">deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="f3b41-111">deviceComplianceUserOverview</span></span>](../resources/intune-deviceconfig-devicecomplianceuseroverview.md)|<span data-ttu-id="f3b41-112">读取 [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f3b41-112">Read properties and relationships of the [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object.</span></span>|
|[<span data-ttu-id="f3b41-113">更新 deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="f3b41-113">Update deviceComplianceUserOverview</span></span>](../api/intune-deviceconfig-devicecomplianceuseroverview-update.md)|[<span data-ttu-id="f3b41-114">deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="f3b41-114">deviceComplianceUserOverview</span></span>](../resources/intune-deviceconfig-devicecomplianceuseroverview.md)|<span data-ttu-id="f3b41-115">更新 [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="f3b41-115">Update the properties of a [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="f3b41-116">属性</span><span class="sxs-lookup"><span data-stu-id="f3b41-116">Properties</span></span>
|<span data-ttu-id="f3b41-117">属性</span><span class="sxs-lookup"><span data-stu-id="f3b41-117">Property</span></span>|<span data-ttu-id="f3b41-118">类型</span><span class="sxs-lookup"><span data-stu-id="f3b41-118">Type</span></span>|<span data-ttu-id="f3b41-119">说明</span><span class="sxs-lookup"><span data-stu-id="f3b41-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f3b41-120">id</span><span class="sxs-lookup"><span data-stu-id="f3b41-120">id</span></span>|<span data-ttu-id="f3b41-121">String</span><span class="sxs-lookup"><span data-stu-id="f3b41-121">String</span></span>|<span data-ttu-id="f3b41-122">实体的键。</span><span class="sxs-lookup"><span data-stu-id="f3b41-122">Key of the entity.</span></span>|
|<span data-ttu-id="f3b41-123">pendingCount</span><span class="sxs-lookup"><span data-stu-id="f3b41-123">pendingCount</span></span>|<span data-ttu-id="f3b41-124">Int32</span><span class="sxs-lookup"><span data-stu-id="f3b41-124">Int32</span></span>|<span data-ttu-id="f3b41-125">待定用户的数量</span><span class="sxs-lookup"><span data-stu-id="f3b41-125">Number of pending Users</span></span>|
|<span data-ttu-id="f3b41-126">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="f3b41-126">notApplicableCount</span></span>|<span data-ttu-id="f3b41-127">Int32</span><span class="sxs-lookup"><span data-stu-id="f3b41-127">Int32</span></span>|<span data-ttu-id="f3b41-128">不适用的用户数</span><span class="sxs-lookup"><span data-stu-id="f3b41-128">Number of not applicable users</span></span>|
|<span data-ttu-id="f3b41-129">successCount</span><span class="sxs-lookup"><span data-stu-id="f3b41-129">successCount</span></span>|<span data-ttu-id="f3b41-130">Int32</span><span class="sxs-lookup"><span data-stu-id="f3b41-130">Int32</span></span>|<span data-ttu-id="f3b41-131">成功用户的数量</span><span class="sxs-lookup"><span data-stu-id="f3b41-131">Number of succeeded Users</span></span>|
|<span data-ttu-id="f3b41-132">errorCount</span><span class="sxs-lookup"><span data-stu-id="f3b41-132">errorCount</span></span>|<span data-ttu-id="f3b41-133">Int32</span><span class="sxs-lookup"><span data-stu-id="f3b41-133">Int32</span></span>|<span data-ttu-id="f3b41-134">错误用户的数量</span><span class="sxs-lookup"><span data-stu-id="f3b41-134">Number of error Users</span></span>|
|<span data-ttu-id="f3b41-135">failedCount</span><span class="sxs-lookup"><span data-stu-id="f3b41-135">failedCount</span></span>|<span data-ttu-id="f3b41-136">Int32</span><span class="sxs-lookup"><span data-stu-id="f3b41-136">Int32</span></span>|<span data-ttu-id="f3b41-137">失败用户的数量</span><span class="sxs-lookup"><span data-stu-id="f3b41-137">Number of failed Users</span></span>|
|<span data-ttu-id="f3b41-138">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="f3b41-138">lastUpdateDateTime</span></span>|<span data-ttu-id="f3b41-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f3b41-139">DateTimeOffset</span></span>|<span data-ttu-id="f3b41-140">上次更新时间</span><span class="sxs-lookup"><span data-stu-id="f3b41-140">Last update time</span></span>|
|<span data-ttu-id="f3b41-141">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="f3b41-141">configurationVersion</span></span>|<span data-ttu-id="f3b41-142">Int32</span><span class="sxs-lookup"><span data-stu-id="f3b41-142">Int32</span></span>|<span data-ttu-id="f3b41-143">用于此概述的策略版本</span><span class="sxs-lookup"><span data-stu-id="f3b41-143">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="f3b41-144">关系</span><span class="sxs-lookup"><span data-stu-id="f3b41-144">Relationships</span></span>
<span data-ttu-id="f3b41-145">无</span><span class="sxs-lookup"><span data-stu-id="f3b41-145">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f3b41-146">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f3b41-146">JSON Representation</span></span>
<span data-ttu-id="f3b41-147">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f3b41-147">Here is a JSON representation of the resource.</span></span>
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
  "lastUpdateDateTime": "String (timestamp)",
  "configurationVersion": 1024
}
```





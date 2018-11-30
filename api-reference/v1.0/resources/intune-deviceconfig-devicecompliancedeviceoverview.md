---
title: deviceComplianceDeviceOverview 资源类型
description: 尚未记录
ms.openlocfilehash: 3d4a52274e3cc68fbf98f0950ad2bda3ed04b265
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27011385"
---
# <a name="devicecompliancedeviceoverview-resource-type"></a><span data-ttu-id="30f1d-103">deviceComplianceDeviceOverview 资源类型</span><span class="sxs-lookup"><span data-stu-id="30f1d-103">deviceComplianceDeviceOverview resource type</span></span>

> <span data-ttu-id="30f1d-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="30f1d-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="30f1d-105">尚未记录</span><span class="sxs-lookup"><span data-stu-id="30f1d-105">Not yet documented</span></span>
## <a name="methods"></a><span data-ttu-id="30f1d-106">方法</span><span class="sxs-lookup"><span data-stu-id="30f1d-106">Methods</span></span>
|<span data-ttu-id="30f1d-107">方法</span><span class="sxs-lookup"><span data-stu-id="30f1d-107">Method</span></span>|<span data-ttu-id="30f1d-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="30f1d-108">Return Type</span></span>|<span data-ttu-id="30f1d-109">说明</span><span class="sxs-lookup"><span data-stu-id="30f1d-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="30f1d-110">获取 deviceComplianceDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="30f1d-110">Get deviceComplianceDeviceOverview</span></span>](../api/intune-deviceconfig-devicecompliancedeviceoverview-get.md)|[<span data-ttu-id="30f1d-111">deviceComplianceDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="30f1d-111">deviceComplianceDeviceOverview</span></span>](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md)|<span data-ttu-id="30f1d-112">读取 [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="30f1d-112">Read properties and relationships of the [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) object.</span></span>|
|[<span data-ttu-id="30f1d-113">更新 deviceComplianceDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="30f1d-113">Update deviceComplianceDeviceOverview</span></span>](../api/intune-deviceconfig-devicecompliancedeviceoverview-update.md)|[<span data-ttu-id="30f1d-114">deviceComplianceDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="30f1d-114">deviceComplianceDeviceOverview</span></span>](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md)|<span data-ttu-id="30f1d-115">更新 [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="30f1d-115">Update the properties of a [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="30f1d-116">属性</span><span class="sxs-lookup"><span data-stu-id="30f1d-116">Properties</span></span>
|<span data-ttu-id="30f1d-117">属性</span><span class="sxs-lookup"><span data-stu-id="30f1d-117">Property</span></span>|<span data-ttu-id="30f1d-118">类型</span><span class="sxs-lookup"><span data-stu-id="30f1d-118">Type</span></span>|<span data-ttu-id="30f1d-119">说明</span><span class="sxs-lookup"><span data-stu-id="30f1d-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="30f1d-120">id</span><span class="sxs-lookup"><span data-stu-id="30f1d-120">id</span></span>|<span data-ttu-id="30f1d-121">String</span><span class="sxs-lookup"><span data-stu-id="30f1d-121">String</span></span>|<span data-ttu-id="30f1d-122">实体的键。</span><span class="sxs-lookup"><span data-stu-id="30f1d-122">Key of the entity.</span></span>|
|<span data-ttu-id="30f1d-123">pendingCount</span><span class="sxs-lookup"><span data-stu-id="30f1d-123">pendingCount</span></span>|<span data-ttu-id="30f1d-124">Int32</span><span class="sxs-lookup"><span data-stu-id="30f1d-124">Int32</span></span>|<span data-ttu-id="30f1d-125">挂起设备的数量</span><span class="sxs-lookup"><span data-stu-id="30f1d-125">Number of pending devices</span></span>|
|<span data-ttu-id="30f1d-126">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="30f1d-126">notApplicableCount</span></span>|<span data-ttu-id="30f1d-127">Int32</span><span class="sxs-lookup"><span data-stu-id="30f1d-127">Int32</span></span>|<span data-ttu-id="30f1d-128">不适用设备的数量</span><span class="sxs-lookup"><span data-stu-id="30f1d-128">Number of not applicable devices</span></span>|
|<span data-ttu-id="30f1d-129">successCount</span><span class="sxs-lookup"><span data-stu-id="30f1d-129">successCount</span></span>|<span data-ttu-id="30f1d-130">Int32</span><span class="sxs-lookup"><span data-stu-id="30f1d-130">Int32</span></span>|<span data-ttu-id="30f1d-131">成功设备的数量</span><span class="sxs-lookup"><span data-stu-id="30f1d-131">Number of succeeded devices</span></span>|
|<span data-ttu-id="30f1d-132">errorCount</span><span class="sxs-lookup"><span data-stu-id="30f1d-132">errorCount</span></span>|<span data-ttu-id="30f1d-133">Int32</span><span class="sxs-lookup"><span data-stu-id="30f1d-133">Int32</span></span>|<span data-ttu-id="30f1d-134">错误设备的数量</span><span class="sxs-lookup"><span data-stu-id="30f1d-134">Number of error devices</span></span>|
|<span data-ttu-id="30f1d-135">failedCount</span><span class="sxs-lookup"><span data-stu-id="30f1d-135">failedCount</span></span>|<span data-ttu-id="30f1d-136">Int32</span><span class="sxs-lookup"><span data-stu-id="30f1d-136">Int32</span></span>|<span data-ttu-id="30f1d-137">失败设备的数量</span><span class="sxs-lookup"><span data-stu-id="30f1d-137">Number of failed devices</span></span>|
|<span data-ttu-id="30f1d-138">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="30f1d-138">lastUpdateDateTime</span></span>|<span data-ttu-id="30f1d-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="30f1d-139">DateTimeOffset</span></span>|<span data-ttu-id="30f1d-140">上次更新时间</span><span class="sxs-lookup"><span data-stu-id="30f1d-140">Last update time</span></span>|
|<span data-ttu-id="30f1d-141">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="30f1d-141">configurationVersion</span></span>|<span data-ttu-id="30f1d-142">Int32</span><span class="sxs-lookup"><span data-stu-id="30f1d-142">Int32</span></span>|<span data-ttu-id="30f1d-143">用于此概述的策略版本</span><span class="sxs-lookup"><span data-stu-id="30f1d-143">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="30f1d-144">关系</span><span class="sxs-lookup"><span data-stu-id="30f1d-144">Relationships</span></span>
<span data-ttu-id="30f1d-145">无</span><span class="sxs-lookup"><span data-stu-id="30f1d-145">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="30f1d-146">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="30f1d-146">JSON Representation</span></span>
<span data-ttu-id="30f1d-147">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="30f1d-147">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceComplianceDeviceOverview"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComplianceDeviceOverview",
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




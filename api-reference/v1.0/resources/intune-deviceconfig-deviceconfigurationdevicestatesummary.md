---
title: deviceConfigurationDeviceStateSummary 资源类型
description: 尚未记录
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: bcc2f390402ddcf48b772c5905956a9e11195a56
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37359549"
---
# <a name="deviceconfigurationdevicestatesummary-resource-type"></a><span data-ttu-id="c045f-103">deviceConfigurationDeviceStateSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="c045f-103">deviceConfigurationDeviceStateSummary resource type</span></span>

> <span data-ttu-id="c045f-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c045f-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c045f-105">尚未记录</span><span class="sxs-lookup"><span data-stu-id="c045f-105">Not yet documented</span></span>

## <a name="methods"></a><span data-ttu-id="c045f-106">方法</span><span class="sxs-lookup"><span data-stu-id="c045f-106">Methods</span></span>
|<span data-ttu-id="c045f-107">方法</span><span class="sxs-lookup"><span data-stu-id="c045f-107">Method</span></span>|<span data-ttu-id="c045f-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="c045f-108">Return Type</span></span>|<span data-ttu-id="c045f-109">说明</span><span class="sxs-lookup"><span data-stu-id="c045f-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c045f-110">获取 deviceConfigurationDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="c045f-110">Get deviceConfigurationDeviceStateSummary</span></span>](../api/intune-deviceconfig-deviceconfigurationdevicestatesummary-get.md)|[<span data-ttu-id="c045f-111">deviceConfigurationDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="c045f-111">deviceConfigurationDeviceStateSummary</span></span>](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md)|<span data-ttu-id="c045f-112">读取 [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c045f-112">Read properties and relationships of the [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object.</span></span>|
|[<span data-ttu-id="c045f-113">更新 deviceConfigurationDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="c045f-113">Update deviceConfigurationDeviceStateSummary</span></span>](../api/intune-deviceconfig-deviceconfigurationdevicestatesummary-update.md)|[<span data-ttu-id="c045f-114">deviceConfigurationDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="c045f-114">deviceConfigurationDeviceStateSummary</span></span>](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md)|<span data-ttu-id="c045f-115">更新 [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="c045f-115">Update the properties of a [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c045f-116">属性</span><span class="sxs-lookup"><span data-stu-id="c045f-116">Properties</span></span>
|<span data-ttu-id="c045f-117">属性</span><span class="sxs-lookup"><span data-stu-id="c045f-117">Property</span></span>|<span data-ttu-id="c045f-118">类型</span><span class="sxs-lookup"><span data-stu-id="c045f-118">Type</span></span>|<span data-ttu-id="c045f-119">说明</span><span class="sxs-lookup"><span data-stu-id="c045f-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c045f-120">id</span><span class="sxs-lookup"><span data-stu-id="c045f-120">id</span></span>|<span data-ttu-id="c045f-121">String</span><span class="sxs-lookup"><span data-stu-id="c045f-121">String</span></span>|<span data-ttu-id="c045f-122">实体的键。</span><span class="sxs-lookup"><span data-stu-id="c045f-122">Key of the entity.</span></span>|
|<span data-ttu-id="c045f-123">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c045f-123">unknownDeviceCount</span></span>|<span data-ttu-id="c045f-124">Int32</span><span class="sxs-lookup"><span data-stu-id="c045f-124">Int32</span></span>|<span data-ttu-id="c045f-125">未知设备的数量</span><span class="sxs-lookup"><span data-stu-id="c045f-125">Number of unknown devices</span></span>|
|<span data-ttu-id="c045f-126">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c045f-126">notApplicableDeviceCount</span></span>|<span data-ttu-id="c045f-127">Int32</span><span class="sxs-lookup"><span data-stu-id="c045f-127">Int32</span></span>|<span data-ttu-id="c045f-128">不适用设备的数量</span><span class="sxs-lookup"><span data-stu-id="c045f-128">Number of not applicable devices</span></span>|
|<span data-ttu-id="c045f-129">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c045f-129">compliantDeviceCount</span></span>|<span data-ttu-id="c045f-130">Int32</span><span class="sxs-lookup"><span data-stu-id="c045f-130">Int32</span></span>|<span data-ttu-id="c045f-131">兼容设备的数量</span><span class="sxs-lookup"><span data-stu-id="c045f-131">Number of compliant devices</span></span>|
|<span data-ttu-id="c045f-132">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c045f-132">remediatedDeviceCount</span></span>|<span data-ttu-id="c045f-133">Int32</span><span class="sxs-lookup"><span data-stu-id="c045f-133">Int32</span></span>|<span data-ttu-id="c045f-134">已修复设备的数量</span><span class="sxs-lookup"><span data-stu-id="c045f-134">Number of remediated devices</span></span>|
|<span data-ttu-id="c045f-135">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c045f-135">nonCompliantDeviceCount</span></span>|<span data-ttu-id="c045f-136">Int32</span><span class="sxs-lookup"><span data-stu-id="c045f-136">Int32</span></span>|<span data-ttu-id="c045f-137">不兼容设备的数量</span><span class="sxs-lookup"><span data-stu-id="c045f-137">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="c045f-138">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c045f-138">errorDeviceCount</span></span>|<span data-ttu-id="c045f-139">Int32</span><span class="sxs-lookup"><span data-stu-id="c045f-139">Int32</span></span>|<span data-ttu-id="c045f-140">错误设备的数量</span><span class="sxs-lookup"><span data-stu-id="c045f-140">Number of error devices</span></span>|
|<span data-ttu-id="c045f-141">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c045f-141">conflictDeviceCount</span></span>|<span data-ttu-id="c045f-142">Int32</span><span class="sxs-lookup"><span data-stu-id="c045f-142">Int32</span></span>|<span data-ttu-id="c045f-143">冲突设备的数量</span><span class="sxs-lookup"><span data-stu-id="c045f-143">Number of conflict devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="c045f-144">关系</span><span class="sxs-lookup"><span data-stu-id="c045f-144">Relationships</span></span>
<span data-ttu-id="c045f-145">无</span><span class="sxs-lookup"><span data-stu-id="c045f-145">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c045f-146">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c045f-146">JSON Representation</span></span>
<span data-ttu-id="c045f-147">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c045f-147">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceConfigurationDeviceStateSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceStateSummary",
  "id": "String (identifier)",
  "unknownDeviceCount": 1024,
  "notApplicableDeviceCount": 1024,
  "compliantDeviceCount": 1024,
  "remediatedDeviceCount": 1024,
  "nonCompliantDeviceCount": 1024,
  "errorDeviceCount": 1024,
  "conflictDeviceCount": 1024
}
```





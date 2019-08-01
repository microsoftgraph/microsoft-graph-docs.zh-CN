---
title: deviceConfigurationDeviceStateSummary 资源类型
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c34a95ceb54cbdd37ca935793e4a9007b20cc6be
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36031652"
---
# <a name="deviceconfigurationdevicestatesummary-resource-type"></a><span data-ttu-id="74979-103">deviceConfigurationDeviceStateSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="74979-103">deviceConfigurationDeviceStateSummary resource type</span></span>

> <span data-ttu-id="74979-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="74979-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="74979-105">尚未记录</span><span class="sxs-lookup"><span data-stu-id="74979-105">Not yet documented</span></span>

## <a name="methods"></a><span data-ttu-id="74979-106">方法</span><span class="sxs-lookup"><span data-stu-id="74979-106">Methods</span></span>
|<span data-ttu-id="74979-107">方法</span><span class="sxs-lookup"><span data-stu-id="74979-107">Method</span></span>|<span data-ttu-id="74979-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="74979-108">Return Type</span></span>|<span data-ttu-id="74979-109">说明</span><span class="sxs-lookup"><span data-stu-id="74979-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="74979-110">获取 deviceConfigurationDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="74979-110">Get deviceConfigurationDeviceStateSummary</span></span>](../api/intune-deviceconfig-deviceconfigurationdevicestatesummary-get.md)|[<span data-ttu-id="74979-111">deviceConfigurationDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="74979-111">deviceConfigurationDeviceStateSummary</span></span>](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md)|<span data-ttu-id="74979-112">读取 [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="74979-112">Read properties and relationships of the [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object.</span></span>|
|[<span data-ttu-id="74979-113">更新 deviceConfigurationDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="74979-113">Update deviceConfigurationDeviceStateSummary</span></span>](../api/intune-deviceconfig-deviceconfigurationdevicestatesummary-update.md)|[<span data-ttu-id="74979-114">deviceConfigurationDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="74979-114">deviceConfigurationDeviceStateSummary</span></span>](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md)|<span data-ttu-id="74979-115">更新 [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="74979-115">Update the properties of a [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="74979-116">属性</span><span class="sxs-lookup"><span data-stu-id="74979-116">Properties</span></span>
|<span data-ttu-id="74979-117">属性</span><span class="sxs-lookup"><span data-stu-id="74979-117">Property</span></span>|<span data-ttu-id="74979-118">类型</span><span class="sxs-lookup"><span data-stu-id="74979-118">Type</span></span>|<span data-ttu-id="74979-119">说明</span><span class="sxs-lookup"><span data-stu-id="74979-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="74979-120">id</span><span class="sxs-lookup"><span data-stu-id="74979-120">id</span></span>|<span data-ttu-id="74979-121">String</span><span class="sxs-lookup"><span data-stu-id="74979-121">String</span></span>|<span data-ttu-id="74979-122">实体的键。</span><span class="sxs-lookup"><span data-stu-id="74979-122">Key of the entity.</span></span>|
|<span data-ttu-id="74979-123">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="74979-123">unknownDeviceCount</span></span>|<span data-ttu-id="74979-124">Int32</span><span class="sxs-lookup"><span data-stu-id="74979-124">Int32</span></span>|<span data-ttu-id="74979-125">未知设备的数量</span><span class="sxs-lookup"><span data-stu-id="74979-125">Number of unknown devices</span></span>|
|<span data-ttu-id="74979-126">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="74979-126">notApplicableDeviceCount</span></span>|<span data-ttu-id="74979-127">Int32</span><span class="sxs-lookup"><span data-stu-id="74979-127">Int32</span></span>|<span data-ttu-id="74979-128">不适用设备的数量</span><span class="sxs-lookup"><span data-stu-id="74979-128">Number of not applicable devices</span></span>|
|<span data-ttu-id="74979-129">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="74979-129">compliantDeviceCount</span></span>|<span data-ttu-id="74979-130">Int32</span><span class="sxs-lookup"><span data-stu-id="74979-130">Int32</span></span>|<span data-ttu-id="74979-131">兼容设备的数量</span><span class="sxs-lookup"><span data-stu-id="74979-131">Number of compliant devices</span></span>|
|<span data-ttu-id="74979-132">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="74979-132">remediatedDeviceCount</span></span>|<span data-ttu-id="74979-133">Int32</span><span class="sxs-lookup"><span data-stu-id="74979-133">Int32</span></span>|<span data-ttu-id="74979-134">已修复设备的数量</span><span class="sxs-lookup"><span data-stu-id="74979-134">Number of remediated devices</span></span>|
|<span data-ttu-id="74979-135">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="74979-135">nonCompliantDeviceCount</span></span>|<span data-ttu-id="74979-136">Int32</span><span class="sxs-lookup"><span data-stu-id="74979-136">Int32</span></span>|<span data-ttu-id="74979-137">不兼容设备的数量</span><span class="sxs-lookup"><span data-stu-id="74979-137">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="74979-138">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="74979-138">errorDeviceCount</span></span>|<span data-ttu-id="74979-139">Int32</span><span class="sxs-lookup"><span data-stu-id="74979-139">Int32</span></span>|<span data-ttu-id="74979-140">错误设备的数量</span><span class="sxs-lookup"><span data-stu-id="74979-140">Number of error devices</span></span>|
|<span data-ttu-id="74979-141">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="74979-141">conflictDeviceCount</span></span>|<span data-ttu-id="74979-142">Int32</span><span class="sxs-lookup"><span data-stu-id="74979-142">Int32</span></span>|<span data-ttu-id="74979-143">冲突设备的数量</span><span class="sxs-lookup"><span data-stu-id="74979-143">Number of conflict devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="74979-144">关系</span><span class="sxs-lookup"><span data-stu-id="74979-144">Relationships</span></span>
<span data-ttu-id="74979-145">无</span><span class="sxs-lookup"><span data-stu-id="74979-145">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="74979-146">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="74979-146">JSON Representation</span></span>
<span data-ttu-id="74979-147">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="74979-147">Here is a JSON representation of the resource.</span></span>
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




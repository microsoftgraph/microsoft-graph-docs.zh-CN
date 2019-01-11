---
title: deviceConfigurationDeviceStateSummary 资源类型
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 24da8858e899b8781763cccb22306a6a219848b6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27820158"
---
# <a name="deviceconfigurationdevicestatesummary-resource-type"></a><span data-ttu-id="bd251-103">deviceConfigurationDeviceStateSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="bd251-103">deviceConfigurationDeviceStateSummary resource type</span></span>

> <span data-ttu-id="bd251-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="bd251-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bd251-105">尚未记录</span><span class="sxs-lookup"><span data-stu-id="bd251-105">Not yet documented</span></span>
## <a name="methods"></a><span data-ttu-id="bd251-106">方法</span><span class="sxs-lookup"><span data-stu-id="bd251-106">Methods</span></span>
|<span data-ttu-id="bd251-107">方法</span><span class="sxs-lookup"><span data-stu-id="bd251-107">Method</span></span>|<span data-ttu-id="bd251-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="bd251-108">Return Type</span></span>|<span data-ttu-id="bd251-109">说明</span><span class="sxs-lookup"><span data-stu-id="bd251-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="bd251-110">获取 deviceConfigurationDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="bd251-110">Get deviceConfigurationDeviceStateSummary</span></span>](../api/intune-deviceconfig-deviceconfigurationdevicestatesummary-get.md)|[<span data-ttu-id="bd251-111">deviceConfigurationDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="bd251-111">deviceConfigurationDeviceStateSummary</span></span>](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md)|<span data-ttu-id="bd251-112">读取 [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="bd251-112">Read properties and relationships of the [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object.</span></span>|
|[<span data-ttu-id="bd251-113">更新 deviceConfigurationDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="bd251-113">Update deviceConfigurationDeviceStateSummary</span></span>](../api/intune-deviceconfig-deviceconfigurationdevicestatesummary-update.md)|[<span data-ttu-id="bd251-114">deviceConfigurationDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="bd251-114">deviceConfigurationDeviceStateSummary</span></span>](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md)|<span data-ttu-id="bd251-115">更新 [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="bd251-115">Update the properties of a [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="bd251-116">属性</span><span class="sxs-lookup"><span data-stu-id="bd251-116">Properties</span></span>
|<span data-ttu-id="bd251-117">属性</span><span class="sxs-lookup"><span data-stu-id="bd251-117">Property</span></span>|<span data-ttu-id="bd251-118">类型</span><span class="sxs-lookup"><span data-stu-id="bd251-118">Type</span></span>|<span data-ttu-id="bd251-119">说明</span><span class="sxs-lookup"><span data-stu-id="bd251-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bd251-120">id</span><span class="sxs-lookup"><span data-stu-id="bd251-120">id</span></span>|<span data-ttu-id="bd251-121">String</span><span class="sxs-lookup"><span data-stu-id="bd251-121">String</span></span>|<span data-ttu-id="bd251-122">实体的键。</span><span class="sxs-lookup"><span data-stu-id="bd251-122">Key of the entity.</span></span>|
|<span data-ttu-id="bd251-123">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="bd251-123">unknownDeviceCount</span></span>|<span data-ttu-id="bd251-124">Int32</span><span class="sxs-lookup"><span data-stu-id="bd251-124">Int32</span></span>|<span data-ttu-id="bd251-125">未知设备的数量</span><span class="sxs-lookup"><span data-stu-id="bd251-125">Number of unknown devices</span></span>|
|<span data-ttu-id="bd251-126">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="bd251-126">notApplicableDeviceCount</span></span>|<span data-ttu-id="bd251-127">Int32</span><span class="sxs-lookup"><span data-stu-id="bd251-127">Int32</span></span>|<span data-ttu-id="bd251-128">不适用设备的数量</span><span class="sxs-lookup"><span data-stu-id="bd251-128">Number of not applicable devices</span></span>|
|<span data-ttu-id="bd251-129">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="bd251-129">compliantDeviceCount</span></span>|<span data-ttu-id="bd251-130">Int32</span><span class="sxs-lookup"><span data-stu-id="bd251-130">Int32</span></span>|<span data-ttu-id="bd251-131">兼容设备的数量</span><span class="sxs-lookup"><span data-stu-id="bd251-131">Number of compliant devices</span></span>|
|<span data-ttu-id="bd251-132">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="bd251-132">remediatedDeviceCount</span></span>|<span data-ttu-id="bd251-133">Int32</span><span class="sxs-lookup"><span data-stu-id="bd251-133">Int32</span></span>|<span data-ttu-id="bd251-134">已修复设备的数量</span><span class="sxs-lookup"><span data-stu-id="bd251-134">Number of remediated devices</span></span>|
|<span data-ttu-id="bd251-135">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="bd251-135">nonCompliantDeviceCount</span></span>|<span data-ttu-id="bd251-136">Int32</span><span class="sxs-lookup"><span data-stu-id="bd251-136">Int32</span></span>|<span data-ttu-id="bd251-137">不兼容设备的数量</span><span class="sxs-lookup"><span data-stu-id="bd251-137">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="bd251-138">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="bd251-138">errorDeviceCount</span></span>|<span data-ttu-id="bd251-139">Int32</span><span class="sxs-lookup"><span data-stu-id="bd251-139">Int32</span></span>|<span data-ttu-id="bd251-140">错误设备的数量</span><span class="sxs-lookup"><span data-stu-id="bd251-140">Number of error devices</span></span>|
|<span data-ttu-id="bd251-141">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="bd251-141">conflictDeviceCount</span></span>|<span data-ttu-id="bd251-142">Int32</span><span class="sxs-lookup"><span data-stu-id="bd251-142">Int32</span></span>|<span data-ttu-id="bd251-143">冲突设备的数量</span><span class="sxs-lookup"><span data-stu-id="bd251-143">Number of conflict devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="bd251-144">关系</span><span class="sxs-lookup"><span data-stu-id="bd251-144">Relationships</span></span>
<span data-ttu-id="bd251-145">无</span><span class="sxs-lookup"><span data-stu-id="bd251-145">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="bd251-146">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bd251-146">JSON Representation</span></span>
<span data-ttu-id="bd251-147">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bd251-147">Here is a JSON representation of the resource.</span></span>
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




---
title: locateDeviceActionResult 资源类型
description: 查找设备操作结果
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 98f61377675154034a4a839bdb990717f03d4c2c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48091136"
---
# <a name="locatedeviceactionresult-resource-type"></a><span data-ttu-id="db94d-103">locateDeviceActionResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="db94d-103">locateDeviceActionResult resource type</span></span>

<span data-ttu-id="db94d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="db94d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="db94d-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="db94d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="db94d-106">查找设备操作结果</span><span class="sxs-lookup"><span data-stu-id="db94d-106">Locate device action result</span></span>


<span data-ttu-id="db94d-107">继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="db94d-107">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="db94d-108">属性</span><span class="sxs-lookup"><span data-stu-id="db94d-108">Properties</span></span>
|<span data-ttu-id="db94d-109">属性</span><span class="sxs-lookup"><span data-stu-id="db94d-109">Property</span></span>|<span data-ttu-id="db94d-110">类型</span><span class="sxs-lookup"><span data-stu-id="db94d-110">Type</span></span>|<span data-ttu-id="db94d-111">说明</span><span class="sxs-lookup"><span data-stu-id="db94d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="db94d-112">actionName</span><span class="sxs-lookup"><span data-stu-id="db94d-112">actionName</span></span>|<span data-ttu-id="db94d-113">String</span><span class="sxs-lookup"><span data-stu-id="db94d-113">String</span></span>|<span data-ttu-id="db94d-114">操作名称 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="db94d-114">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="db94d-115">actionState</span><span class="sxs-lookup"><span data-stu-id="db94d-115">actionState</span></span>|[<span data-ttu-id="db94d-116">actionState</span><span class="sxs-lookup"><span data-stu-id="db94d-116">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="db94d-117">继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)的操作的状态。</span><span class="sxs-lookup"><span data-stu-id="db94d-117">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="db94d-118">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed` 或 `notSupported`。</span><span class="sxs-lookup"><span data-stu-id="db94d-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="db94d-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="db94d-119">startDateTime</span></span>|<span data-ttu-id="db94d-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="db94d-120">DateTimeOffset</span></span>|<span data-ttu-id="db94d-121">操作启动的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="db94d-121">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="db94d-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="db94d-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="db94d-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="db94d-123">DateTimeOffset</span></span>|<span data-ttu-id="db94d-124">操作状态上次更新的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="db94d-124">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="db94d-125">deviceLocation</span><span class="sxs-lookup"><span data-stu-id="db94d-125">deviceLocation</span></span>|[<span data-ttu-id="db94d-126">deviceGeoLocation</span><span class="sxs-lookup"><span data-stu-id="db94d-126">deviceGeoLocation</span></span>](../resources/intune-devices-devicegeolocation.md)|<span data-ttu-id="db94d-127">设备位置</span><span class="sxs-lookup"><span data-stu-id="db94d-127">device location</span></span>|

## <a name="relationships"></a><span data-ttu-id="db94d-128">关系</span><span class="sxs-lookup"><span data-stu-id="db94d-128">Relationships</span></span>
<span data-ttu-id="db94d-129">无</span><span class="sxs-lookup"><span data-stu-id="db94d-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="db94d-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="db94d-130">JSON Representation</span></span>
<span data-ttu-id="db94d-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="db94d-131">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.locateDeviceActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.locateDeviceActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "deviceLocation": {
    "@odata.type": "microsoft.graph.deviceGeoLocation",
    "lastCollectedDateTime": "String (timestamp)",
    "longitude": "<Unknown Primitive Type Edm.Double>",
    "latitude": "<Unknown Primitive Type Edm.Double>",
    "altitude": "<Unknown Primitive Type Edm.Double>",
    "horizontalAccuracy": "<Unknown Primitive Type Edm.Double>",
    "verticalAccuracy": "<Unknown Primitive Type Edm.Double>",
    "heading": "<Unknown Primitive Type Edm.Double>",
    "speed": "<Unknown Primitive Type Edm.Double>"
  }
}
```










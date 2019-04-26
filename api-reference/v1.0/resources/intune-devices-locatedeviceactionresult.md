---
title: locateDeviceActionResult 资源类型
description: 查找设备操作结果
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c335ac49bcf053e58381f7c1111caf5ae70cb0fd
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32570360"
---
# <a name="locatedeviceactionresult-resource-type"></a><span data-ttu-id="b79f9-103">locateDeviceActionResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="b79f9-103">locateDeviceActionResult resource type</span></span>

> <span data-ttu-id="b79f9-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b79f9-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b79f9-105">查找设备操作结果</span><span class="sxs-lookup"><span data-stu-id="b79f9-105">Locate device action result</span></span>


<span data-ttu-id="b79f9-106">继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="b79f9-106">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b79f9-107">属性</span><span class="sxs-lookup"><span data-stu-id="b79f9-107">Properties</span></span>
|<span data-ttu-id="b79f9-108">属性</span><span class="sxs-lookup"><span data-stu-id="b79f9-108">Property</span></span>|<span data-ttu-id="b79f9-109">类型</span><span class="sxs-lookup"><span data-stu-id="b79f9-109">Type</span></span>|<span data-ttu-id="b79f9-110">说明</span><span class="sxs-lookup"><span data-stu-id="b79f9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b79f9-111">actionName</span><span class="sxs-lookup"><span data-stu-id="b79f9-111">actionName</span></span>|<span data-ttu-id="b79f9-112">String</span><span class="sxs-lookup"><span data-stu-id="b79f9-112">String</span></span>|<span data-ttu-id="b79f9-113">操作名称 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="b79f9-113">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="b79f9-114">actionState</span><span class="sxs-lookup"><span data-stu-id="b79f9-114">actionState</span></span>|[<span data-ttu-id="b79f9-115">actionState</span><span class="sxs-lookup"><span data-stu-id="b79f9-115">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="b79f9-116">继承自[deviceActionResult](../resources/intune-devices-deviceactionresult.md)的操作的状态。</span><span class="sxs-lookup"><span data-stu-id="b79f9-116">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="b79f9-117">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed` 或 `notSupported`。</span><span class="sxs-lookup"><span data-stu-id="b79f9-117">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="b79f9-118">startDateTime</span><span class="sxs-lookup"><span data-stu-id="b79f9-118">startDateTime</span></span>|<span data-ttu-id="b79f9-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b79f9-119">DateTimeOffset</span></span>|<span data-ttu-id="b79f9-120">操作启动的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="b79f9-120">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="b79f9-121">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="b79f9-121">lastUpdatedDateTime</span></span>|<span data-ttu-id="b79f9-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b79f9-122">DateTimeOffset</span></span>|<span data-ttu-id="b79f9-123">操作状态上次更新的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="b79f9-123">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="b79f9-124">deviceLocation</span><span class="sxs-lookup"><span data-stu-id="b79f9-124">deviceLocation</span></span>|[<span data-ttu-id="b79f9-125">deviceGeoLocation</span><span class="sxs-lookup"><span data-stu-id="b79f9-125">deviceGeoLocation</span></span>](../resources/intune-devices-devicegeolocation.md)|<span data-ttu-id="b79f9-126">设备位置</span><span class="sxs-lookup"><span data-stu-id="b79f9-126">device location</span></span>|

## <a name="relationships"></a><span data-ttu-id="b79f9-127">关系</span><span class="sxs-lookup"><span data-stu-id="b79f9-127">Relationships</span></span>
<span data-ttu-id="b79f9-128">无</span><span class="sxs-lookup"><span data-stu-id="b79f9-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b79f9-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b79f9-129">JSON Representation</span></span>
<span data-ttu-id="b79f9-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b79f9-130">Here is a JSON representation of the resource.</span></span>
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




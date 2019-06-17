---
title: locateDeviceActionResult 资源类型
description: 查找设备操作结果
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 588296ad2243e326f855221d217e63fdc01f9cb8
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34995145"
---
# <a name="locatedeviceactionresult-resource-type"></a><span data-ttu-id="e6810-103">locateDeviceActionResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="e6810-103">locateDeviceActionResult resource type</span></span>

> <span data-ttu-id="e6810-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e6810-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e6810-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e6810-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e6810-106">查找设备操作结果</span><span class="sxs-lookup"><span data-stu-id="e6810-106">Locate device action result</span></span>


<span data-ttu-id="e6810-107">继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="e6810-107">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e6810-108">属性</span><span class="sxs-lookup"><span data-stu-id="e6810-108">Properties</span></span>
|<span data-ttu-id="e6810-109">属性</span><span class="sxs-lookup"><span data-stu-id="e6810-109">Property</span></span>|<span data-ttu-id="e6810-110">类型</span><span class="sxs-lookup"><span data-stu-id="e6810-110">Type</span></span>|<span data-ttu-id="e6810-111">说明</span><span class="sxs-lookup"><span data-stu-id="e6810-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e6810-112">actionName</span><span class="sxs-lookup"><span data-stu-id="e6810-112">actionName</span></span>|<span data-ttu-id="e6810-113">String</span><span class="sxs-lookup"><span data-stu-id="e6810-113">String</span></span>|<span data-ttu-id="e6810-114">操作名称 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="e6810-114">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="e6810-115">actionState</span><span class="sxs-lookup"><span data-stu-id="e6810-115">actionState</span></span>|[<span data-ttu-id="e6810-116">actionState</span><span class="sxs-lookup"><span data-stu-id="e6810-116">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="e6810-117">继承自[deviceActionResult](../resources/intune-devices-deviceactionresult.md)的操作的状态。</span><span class="sxs-lookup"><span data-stu-id="e6810-117">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="e6810-118">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed` 或 `notSupported`。</span><span class="sxs-lookup"><span data-stu-id="e6810-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="e6810-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="e6810-119">startDateTime</span></span>|<span data-ttu-id="e6810-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e6810-120">DateTimeOffset</span></span>|<span data-ttu-id="e6810-121">操作启动的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="e6810-121">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="e6810-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="e6810-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="e6810-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e6810-123">DateTimeOffset</span></span>|<span data-ttu-id="e6810-124">操作状态上次更新的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="e6810-124">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="e6810-125">deviceLocation</span><span class="sxs-lookup"><span data-stu-id="e6810-125">deviceLocation</span></span>|[<span data-ttu-id="e6810-126">deviceGeoLocation</span><span class="sxs-lookup"><span data-stu-id="e6810-126">deviceGeoLocation</span></span>](../resources/intune-devices-devicegeolocation.md)|<span data-ttu-id="e6810-127">设备位置</span><span class="sxs-lookup"><span data-stu-id="e6810-127">device location</span></span>|

## <a name="relationships"></a><span data-ttu-id="e6810-128">关系</span><span class="sxs-lookup"><span data-stu-id="e6810-128">Relationships</span></span>
<span data-ttu-id="e6810-129">无</span><span class="sxs-lookup"><span data-stu-id="e6810-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e6810-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e6810-130">JSON Representation</span></span>
<span data-ttu-id="e6810-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e6810-131">Here is a JSON representation of the resource.</span></span>
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
    "lastCollectedDateTimeUtc": "String (timestamp)",
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






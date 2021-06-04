---
title: locateDeviceActionResult 资源类型
description: 查找设备操作结果
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0fc2fa997d56fffd673964a1d387b175bfef2ba1
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52754558"
---
# <a name="locatedeviceactionresult-resource-type"></a><span data-ttu-id="098b5-103">locateDeviceActionResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="098b5-103">locateDeviceActionResult resource type</span></span>

<span data-ttu-id="098b5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="098b5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="098b5-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="098b5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="098b5-106">查找设备操作结果</span><span class="sxs-lookup"><span data-stu-id="098b5-106">Locate device action result</span></span>


<span data-ttu-id="098b5-107">继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="098b5-107">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="098b5-108">属性</span><span class="sxs-lookup"><span data-stu-id="098b5-108">Properties</span></span>
|<span data-ttu-id="098b5-109">属性</span><span class="sxs-lookup"><span data-stu-id="098b5-109">Property</span></span>|<span data-ttu-id="098b5-110">类型</span><span class="sxs-lookup"><span data-stu-id="098b5-110">Type</span></span>|<span data-ttu-id="098b5-111">Description</span><span class="sxs-lookup"><span data-stu-id="098b5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="098b5-112">actionName</span><span class="sxs-lookup"><span data-stu-id="098b5-112">actionName</span></span>|<span data-ttu-id="098b5-113">String</span><span class="sxs-lookup"><span data-stu-id="098b5-113">String</span></span>|<span data-ttu-id="098b5-114">操作名称 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="098b5-114">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="098b5-115">actionState</span><span class="sxs-lookup"><span data-stu-id="098b5-115">actionState</span></span>|[<span data-ttu-id="098b5-116">actionState</span><span class="sxs-lookup"><span data-stu-id="098b5-116">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="098b5-117">操作的状态 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)。</span><span class="sxs-lookup"><span data-stu-id="098b5-117">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="098b5-118">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed` 或 `notSupported`。</span><span class="sxs-lookup"><span data-stu-id="098b5-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="098b5-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="098b5-119">startDateTime</span></span>|<span data-ttu-id="098b5-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="098b5-120">DateTimeOffset</span></span>|<span data-ttu-id="098b5-121">操作启动的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="098b5-121">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="098b5-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="098b5-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="098b5-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="098b5-123">DateTimeOffset</span></span>|<span data-ttu-id="098b5-124">操作状态上次更新的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="098b5-124">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="098b5-125">deviceLocation</span><span class="sxs-lookup"><span data-stu-id="098b5-125">deviceLocation</span></span>|[<span data-ttu-id="098b5-126">deviceGeoLocation</span><span class="sxs-lookup"><span data-stu-id="098b5-126">deviceGeoLocation</span></span>](../resources/intune-devices-devicegeolocation.md)|<span data-ttu-id="098b5-127">设备位置</span><span class="sxs-lookup"><span data-stu-id="098b5-127">device location</span></span>|

## <a name="relationships"></a><span data-ttu-id="098b5-128">关系</span><span class="sxs-lookup"><span data-stu-id="098b5-128">Relationships</span></span>
<span data-ttu-id="098b5-129">无</span><span class="sxs-lookup"><span data-stu-id="098b5-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="098b5-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="098b5-130">JSON Representation</span></span>
<span data-ttu-id="098b5-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="098b5-131">Here is a JSON representation of the resource.</span></span>
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
    "longitude": "4.2",
    "latitude": "4.2",
    "altitude": "4.2",
    "horizontalAccuracy": "4.2",
    "verticalAccuracy": "4.2",
    "heading": "4.2",
    "speed": "4.2"
  }
}
```





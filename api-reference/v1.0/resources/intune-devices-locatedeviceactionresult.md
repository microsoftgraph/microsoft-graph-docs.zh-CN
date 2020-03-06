---
title: locateDeviceActionResult 资源类型
description: 查找设备操作结果
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 821b02b887289dc96b2644938360fb4ab0a67f9e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533261"
---
# <a name="locatedeviceactionresult-resource-type"></a><span data-ttu-id="2bdfa-103">locateDeviceActionResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="2bdfa-103">locateDeviceActionResult resource type</span></span>

<span data-ttu-id="2bdfa-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2bdfa-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2bdfa-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2bdfa-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2bdfa-106">查找设备操作结果</span><span class="sxs-lookup"><span data-stu-id="2bdfa-106">Locate device action result</span></span>


<span data-ttu-id="2bdfa-107">继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="2bdfa-107">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="2bdfa-108">属性</span><span class="sxs-lookup"><span data-stu-id="2bdfa-108">Properties</span></span>
|<span data-ttu-id="2bdfa-109">属性</span><span class="sxs-lookup"><span data-stu-id="2bdfa-109">Property</span></span>|<span data-ttu-id="2bdfa-110">类型</span><span class="sxs-lookup"><span data-stu-id="2bdfa-110">Type</span></span>|<span data-ttu-id="2bdfa-111">说明</span><span class="sxs-lookup"><span data-stu-id="2bdfa-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2bdfa-112">actionName</span><span class="sxs-lookup"><span data-stu-id="2bdfa-112">actionName</span></span>|<span data-ttu-id="2bdfa-113">String</span><span class="sxs-lookup"><span data-stu-id="2bdfa-113">String</span></span>|<span data-ttu-id="2bdfa-114">操作名称 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="2bdfa-114">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="2bdfa-115">actionState</span><span class="sxs-lookup"><span data-stu-id="2bdfa-115">actionState</span></span>|[<span data-ttu-id="2bdfa-116">actionState</span><span class="sxs-lookup"><span data-stu-id="2bdfa-116">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="2bdfa-117">继承自[deviceActionResult](../resources/intune-devices-deviceactionresult.md)的操作的状态。</span><span class="sxs-lookup"><span data-stu-id="2bdfa-117">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="2bdfa-118">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed` 或 `notSupported`。</span><span class="sxs-lookup"><span data-stu-id="2bdfa-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="2bdfa-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="2bdfa-119">startDateTime</span></span>|<span data-ttu-id="2bdfa-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2bdfa-120">DateTimeOffset</span></span>|<span data-ttu-id="2bdfa-121">操作启动的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="2bdfa-121">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="2bdfa-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="2bdfa-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="2bdfa-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2bdfa-123">DateTimeOffset</span></span>|<span data-ttu-id="2bdfa-124">操作状态上次更新的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="2bdfa-124">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="2bdfa-125">deviceLocation</span><span class="sxs-lookup"><span data-stu-id="2bdfa-125">deviceLocation</span></span>|[<span data-ttu-id="2bdfa-126">deviceGeoLocation</span><span class="sxs-lookup"><span data-stu-id="2bdfa-126">deviceGeoLocation</span></span>](../resources/intune-devices-devicegeolocation.md)|<span data-ttu-id="2bdfa-127">设备位置</span><span class="sxs-lookup"><span data-stu-id="2bdfa-127">device location</span></span>|

## <a name="relationships"></a><span data-ttu-id="2bdfa-128">关系</span><span class="sxs-lookup"><span data-stu-id="2bdfa-128">Relationships</span></span>
<span data-ttu-id="2bdfa-129">无</span><span class="sxs-lookup"><span data-stu-id="2bdfa-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2bdfa-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2bdfa-130">JSON Representation</span></span>
<span data-ttu-id="2bdfa-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2bdfa-131">Here is a JSON representation of the resource.</span></span>
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





---
title: locateDeviceActionResult 资源类型
description: 查找设备操作结果
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 682b2267369a80b3d2cb37d17dd1b2aafdef1f63
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29416886"
---
# <a name="locatedeviceactionresult-resource-type"></a><span data-ttu-id="592a6-103">locateDeviceActionResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="592a6-103">locateDeviceActionResult resource type</span></span>

> <span data-ttu-id="592a6-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="592a6-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="592a6-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="592a6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="592a6-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="592a6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="592a6-107">查找设备操作结果</span><span class="sxs-lookup"><span data-stu-id="592a6-107">Locate device action result</span></span>


<span data-ttu-id="592a6-108">继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="592a6-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="592a6-109">属性</span><span class="sxs-lookup"><span data-stu-id="592a6-109">Properties</span></span>
|<span data-ttu-id="592a6-110">属性</span><span class="sxs-lookup"><span data-stu-id="592a6-110">Property</span></span>|<span data-ttu-id="592a6-111">类型</span><span class="sxs-lookup"><span data-stu-id="592a6-111">Type</span></span>|<span data-ttu-id="592a6-112">说明</span><span class="sxs-lookup"><span data-stu-id="592a6-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="592a6-113">actionName</span><span class="sxs-lookup"><span data-stu-id="592a6-113">actionName</span></span>|<span data-ttu-id="592a6-114">String</span><span class="sxs-lookup"><span data-stu-id="592a6-114">String</span></span>|<span data-ttu-id="592a6-115">操作名称 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="592a6-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="592a6-116">actionState</span><span class="sxs-lookup"><span data-stu-id="592a6-116">actionState</span></span>|[<span data-ttu-id="592a6-117">actionState</span><span class="sxs-lookup"><span data-stu-id="592a6-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="592a6-118">从[deviceActionResult](../resources/intune-devices-deviceactionresult.md)继承操作的状态。</span><span class="sxs-lookup"><span data-stu-id="592a6-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="592a6-119">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported`。</span><span class="sxs-lookup"><span data-stu-id="592a6-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="592a6-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="592a6-120">startDateTime</span></span>|<span data-ttu-id="592a6-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="592a6-121">DateTimeOffset</span></span>|<span data-ttu-id="592a6-122">启动操作的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="592a6-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="592a6-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="592a6-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="592a6-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="592a6-124">DateTimeOffset</span></span>|<span data-ttu-id="592a6-125">操作状态上次更新的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="592a6-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="592a6-126">deviceLocation</span><span class="sxs-lookup"><span data-stu-id="592a6-126">deviceLocation</span></span>|[<span data-ttu-id="592a6-127">deviceGeoLocation</span><span class="sxs-lookup"><span data-stu-id="592a6-127">deviceGeoLocation</span></span>](../resources/intune-devices-devicegeolocation.md)|<span data-ttu-id="592a6-128">设备位置</span><span class="sxs-lookup"><span data-stu-id="592a6-128">device location</span></span>|

## <a name="relationships"></a><span data-ttu-id="592a6-129">关系</span><span class="sxs-lookup"><span data-stu-id="592a6-129">Relationships</span></span>
<span data-ttu-id="592a6-130">无</span><span class="sxs-lookup"><span data-stu-id="592a6-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="592a6-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="592a6-131">JSON Representation</span></span>
<span data-ttu-id="592a6-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="592a6-132">Here is a JSON representation of the resource.</span></span>
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





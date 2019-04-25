---
title: locateDeviceActionResult 资源类型
description: 查找设备操作结果
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f38422c419d4f50901cbc015b82ca51c470ddfe4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32522200"
---
# <a name="locatedeviceactionresult-resource-type"></a><span data-ttu-id="44a0b-103">locateDeviceActionResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="44a0b-103">locateDeviceActionResult resource type</span></span>

> <span data-ttu-id="44a0b-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="44a0b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="44a0b-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="44a0b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="44a0b-106">查找设备操作结果</span><span class="sxs-lookup"><span data-stu-id="44a0b-106">Locate device action result</span></span>


<span data-ttu-id="44a0b-107">继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="44a0b-107">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="44a0b-108">属性</span><span class="sxs-lookup"><span data-stu-id="44a0b-108">Properties</span></span>
|<span data-ttu-id="44a0b-109">属性</span><span class="sxs-lookup"><span data-stu-id="44a0b-109">Property</span></span>|<span data-ttu-id="44a0b-110">类型</span><span class="sxs-lookup"><span data-stu-id="44a0b-110">Type</span></span>|<span data-ttu-id="44a0b-111">说明</span><span class="sxs-lookup"><span data-stu-id="44a0b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="44a0b-112">actionName</span><span class="sxs-lookup"><span data-stu-id="44a0b-112">actionName</span></span>|<span data-ttu-id="44a0b-113">String</span><span class="sxs-lookup"><span data-stu-id="44a0b-113">String</span></span>|<span data-ttu-id="44a0b-114">操作名称 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="44a0b-114">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="44a0b-115">actionState</span><span class="sxs-lookup"><span data-stu-id="44a0b-115">actionState</span></span>|[<span data-ttu-id="44a0b-116">actionState</span><span class="sxs-lookup"><span data-stu-id="44a0b-116">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="44a0b-117">继承自[deviceActionResult](../resources/intune-devices-deviceactionresult.md)的操作的状态。</span><span class="sxs-lookup"><span data-stu-id="44a0b-117">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="44a0b-118">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed` 或 `notSupported`。</span><span class="sxs-lookup"><span data-stu-id="44a0b-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="44a0b-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="44a0b-119">startDateTime</span></span>|<span data-ttu-id="44a0b-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="44a0b-120">DateTimeOffset</span></span>|<span data-ttu-id="44a0b-121">操作启动的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="44a0b-121">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="44a0b-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="44a0b-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="44a0b-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="44a0b-123">DateTimeOffset</span></span>|<span data-ttu-id="44a0b-124">操作状态上次更新的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="44a0b-124">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="44a0b-125">deviceLocation</span><span class="sxs-lookup"><span data-stu-id="44a0b-125">deviceLocation</span></span>|[<span data-ttu-id="44a0b-126">deviceGeoLocation</span><span class="sxs-lookup"><span data-stu-id="44a0b-126">deviceGeoLocation</span></span>](../resources/intune-devices-devicegeolocation.md)|<span data-ttu-id="44a0b-127">设备位置</span><span class="sxs-lookup"><span data-stu-id="44a0b-127">device location</span></span>|

## <a name="relationships"></a><span data-ttu-id="44a0b-128">关系</span><span class="sxs-lookup"><span data-stu-id="44a0b-128">Relationships</span></span>
<span data-ttu-id="44a0b-129">无</span><span class="sxs-lookup"><span data-stu-id="44a0b-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="44a0b-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="44a0b-130">JSON Representation</span></span>
<span data-ttu-id="44a0b-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="44a0b-131">Here is a JSON representation of the resource.</span></span>
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






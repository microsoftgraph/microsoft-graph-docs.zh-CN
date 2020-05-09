---
title: locateDeviceActionResult 资源类型
description: 查找设备操作结果
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 39ccb7a22109cf77f36505ed2c61f59af19c2994
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/09/2020
ms.locfileid: "44178820"
---
# <a name="locatedeviceactionresult-resource-type"></a><span data-ttu-id="1cb83-103">locateDeviceActionResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="1cb83-103">locateDeviceActionResult resource type</span></span>

<span data-ttu-id="1cb83-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1cb83-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1cb83-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1cb83-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1cb83-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1cb83-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1cb83-107">查找设备操作结果</span><span class="sxs-lookup"><span data-stu-id="1cb83-107">Locate device action result</span></span>


<span data-ttu-id="1cb83-108">继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="1cb83-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="1cb83-109">属性</span><span class="sxs-lookup"><span data-stu-id="1cb83-109">Properties</span></span>
|<span data-ttu-id="1cb83-110">属性</span><span class="sxs-lookup"><span data-stu-id="1cb83-110">Property</span></span>|<span data-ttu-id="1cb83-111">类型</span><span class="sxs-lookup"><span data-stu-id="1cb83-111">Type</span></span>|<span data-ttu-id="1cb83-112">说明</span><span class="sxs-lookup"><span data-stu-id="1cb83-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1cb83-113">actionName</span><span class="sxs-lookup"><span data-stu-id="1cb83-113">actionName</span></span>|<span data-ttu-id="1cb83-114">String</span><span class="sxs-lookup"><span data-stu-id="1cb83-114">String</span></span>|<span data-ttu-id="1cb83-115">操作名称 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="1cb83-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="1cb83-116">actionState</span><span class="sxs-lookup"><span data-stu-id="1cb83-116">actionState</span></span>|[<span data-ttu-id="1cb83-117">actionState</span><span class="sxs-lookup"><span data-stu-id="1cb83-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="1cb83-118">继承自[deviceActionResult](../resources/intune-devices-deviceactionresult.md)的操作的状态。</span><span class="sxs-lookup"><span data-stu-id="1cb83-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="1cb83-119">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed` 或 `notSupported`。</span><span class="sxs-lookup"><span data-stu-id="1cb83-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="1cb83-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="1cb83-120">startDateTime</span></span>|<span data-ttu-id="1cb83-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1cb83-121">DateTimeOffset</span></span>|<span data-ttu-id="1cb83-122">操作启动的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="1cb83-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="1cb83-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="1cb83-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="1cb83-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1cb83-124">DateTimeOffset</span></span>|<span data-ttu-id="1cb83-125">操作状态上次更新的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="1cb83-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="1cb83-126">deviceLocation</span><span class="sxs-lookup"><span data-stu-id="1cb83-126">deviceLocation</span></span>|[<span data-ttu-id="1cb83-127">deviceGeoLocation</span><span class="sxs-lookup"><span data-stu-id="1cb83-127">deviceGeoLocation</span></span>](../resources/intune-devices-devicegeolocation.md)|<span data-ttu-id="1cb83-128">设备位置</span><span class="sxs-lookup"><span data-stu-id="1cb83-128">device location</span></span>|

## <a name="relationships"></a><span data-ttu-id="1cb83-129">关系</span><span class="sxs-lookup"><span data-stu-id="1cb83-129">Relationships</span></span>
<span data-ttu-id="1cb83-130">无</span><span class="sxs-lookup"><span data-stu-id="1cb83-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1cb83-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1cb83-131">JSON Representation</span></span>
<span data-ttu-id="1cb83-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1cb83-132">Here is a JSON representation of the resource.</span></span>
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




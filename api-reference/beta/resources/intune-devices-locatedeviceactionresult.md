---
title: locateDeviceActionResult 资源类型
description: 查找设备操作结果
ms.openlocfilehash: de7a59826478f8e11cf44635dcc4e437b60d7e83
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27049255"
---
# <a name="locatedeviceactionresult-resource-type"></a><span data-ttu-id="25dbd-103">locateDeviceActionResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="25dbd-103">locateDeviceActionResult resource type</span></span>

> <span data-ttu-id="25dbd-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="25dbd-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="25dbd-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="25dbd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="25dbd-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="25dbd-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="25dbd-107">查找设备操作结果</span><span class="sxs-lookup"><span data-stu-id="25dbd-107">Locate device action result</span></span>

<span data-ttu-id="25dbd-108">继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="25dbd-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="25dbd-109">属性</span><span class="sxs-lookup"><span data-stu-id="25dbd-109">Properties</span></span>
|<span data-ttu-id="25dbd-110">属性</span><span class="sxs-lookup"><span data-stu-id="25dbd-110">Property</span></span>|<span data-ttu-id="25dbd-111">类型</span><span class="sxs-lookup"><span data-stu-id="25dbd-111">Type</span></span>|<span data-ttu-id="25dbd-112">说明</span><span class="sxs-lookup"><span data-stu-id="25dbd-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="25dbd-113">actionName</span><span class="sxs-lookup"><span data-stu-id="25dbd-113">actionName</span></span>|<span data-ttu-id="25dbd-114">String</span><span class="sxs-lookup"><span data-stu-id="25dbd-114">String</span></span>|<span data-ttu-id="25dbd-115">操作名称 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="25dbd-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="25dbd-116">actionState</span><span class="sxs-lookup"><span data-stu-id="25dbd-116">actionState</span></span>|[<span data-ttu-id="25dbd-117">actionState</span><span class="sxs-lookup"><span data-stu-id="25dbd-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="25dbd-118">从[deviceActionResult](../resources/intune-devices-deviceactionresult.md)继承操作的状态。</span><span class="sxs-lookup"><span data-stu-id="25dbd-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="25dbd-119">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported`。</span><span class="sxs-lookup"><span data-stu-id="25dbd-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="25dbd-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="25dbd-120">startDateTime</span></span>|<span data-ttu-id="25dbd-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="25dbd-121">DateTimeOffset</span></span>|<span data-ttu-id="25dbd-122">启动操作的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="25dbd-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="25dbd-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="25dbd-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="25dbd-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="25dbd-124">DateTimeOffset</span></span>|<span data-ttu-id="25dbd-125">操作状态上次更新的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="25dbd-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="25dbd-126">deviceLocation</span><span class="sxs-lookup"><span data-stu-id="25dbd-126">deviceLocation</span></span>|[<span data-ttu-id="25dbd-127">deviceGeoLocation</span><span class="sxs-lookup"><span data-stu-id="25dbd-127">deviceGeoLocation</span></span>](../resources/intune-devices-devicegeolocation.md)|<span data-ttu-id="25dbd-128">设备位置</span><span class="sxs-lookup"><span data-stu-id="25dbd-128">device location</span></span>|

## <a name="relationships"></a><span data-ttu-id="25dbd-129">关系</span><span class="sxs-lookup"><span data-stu-id="25dbd-129">Relationships</span></span>
<span data-ttu-id="25dbd-130">无</span><span class="sxs-lookup"><span data-stu-id="25dbd-130">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="25dbd-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="25dbd-131">JSON Representation</span></span>
<span data-ttu-id="25dbd-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="25dbd-132">Here is a JSON representation of the resource.</span></span>
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






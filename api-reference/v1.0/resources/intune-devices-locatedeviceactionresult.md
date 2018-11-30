---
title: locateDeviceActionResult 资源类型
description: 查找设备操作结果
ms.openlocfilehash: 3cabeca1ac07dd1911cf4c60300d07bdc1266134
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27009340"
---
# <a name="locatedeviceactionresult-resource-type"></a><span data-ttu-id="982ca-103">locateDeviceActionResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="982ca-103">locateDeviceActionResult resource type</span></span>

> <span data-ttu-id="982ca-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="982ca-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="982ca-105">查找设备操作结果</span><span class="sxs-lookup"><span data-stu-id="982ca-105">Locate device action result</span></span>

<span data-ttu-id="982ca-106">继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="982ca-106">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="982ca-107">属性</span><span class="sxs-lookup"><span data-stu-id="982ca-107">Properties</span></span>
|<span data-ttu-id="982ca-108">属性</span><span class="sxs-lookup"><span data-stu-id="982ca-108">Property</span></span>|<span data-ttu-id="982ca-109">类型</span><span class="sxs-lookup"><span data-stu-id="982ca-109">Type</span></span>|<span data-ttu-id="982ca-110">说明</span><span class="sxs-lookup"><span data-stu-id="982ca-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="982ca-111">actionName</span><span class="sxs-lookup"><span data-stu-id="982ca-111">actionName</span></span>|<span data-ttu-id="982ca-112">String</span><span class="sxs-lookup"><span data-stu-id="982ca-112">String</span></span>|<span data-ttu-id="982ca-113">操作名称 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="982ca-113">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="982ca-114">actionState</span><span class="sxs-lookup"><span data-stu-id="982ca-114">actionState</span></span>|[<span data-ttu-id="982ca-115">actionState</span><span class="sxs-lookup"><span data-stu-id="982ca-115">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="982ca-116">从[deviceActionResult](../resources/intune-devices-deviceactionresult.md)继承操作的状态。</span><span class="sxs-lookup"><span data-stu-id="982ca-116">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="982ca-117">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported`。</span><span class="sxs-lookup"><span data-stu-id="982ca-117">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="982ca-118">startDateTime</span><span class="sxs-lookup"><span data-stu-id="982ca-118">startDateTime</span></span>|<span data-ttu-id="982ca-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="982ca-119">DateTimeOffset</span></span>|<span data-ttu-id="982ca-120">启动操作的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="982ca-120">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="982ca-121">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="982ca-121">lastUpdatedDateTime</span></span>|<span data-ttu-id="982ca-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="982ca-122">DateTimeOffset</span></span>|<span data-ttu-id="982ca-123">操作状态上次更新的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="982ca-123">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="982ca-124">deviceLocation</span><span class="sxs-lookup"><span data-stu-id="982ca-124">deviceLocation</span></span>|[<span data-ttu-id="982ca-125">deviceGeoLocation</span><span class="sxs-lookup"><span data-stu-id="982ca-125">deviceGeoLocation</span></span>](../resources/intune-devices-devicegeolocation.md)|<span data-ttu-id="982ca-126">设备位置</span><span class="sxs-lookup"><span data-stu-id="982ca-126">device location</span></span>|

## <a name="relationships"></a><span data-ttu-id="982ca-127">关系</span><span class="sxs-lookup"><span data-stu-id="982ca-127">Relationships</span></span>
<span data-ttu-id="982ca-128">无</span><span class="sxs-lookup"><span data-stu-id="982ca-128">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="982ca-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="982ca-129">JSON Representation</span></span>
<span data-ttu-id="982ca-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="982ca-130">Here is a JSON representation of the resource.</span></span>
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




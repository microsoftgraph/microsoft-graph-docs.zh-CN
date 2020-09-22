---
title: rotateBitLockerKeysDeviceActionResult 资源类型
description: RotateBitLockerKeys 设备操作结果
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7189a1c2a1d7de349aa6b92811428849d8f3ab62
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48081011"
---
# <a name="rotatebitlockerkeysdeviceactionresult-resource-type"></a><span data-ttu-id="634ab-103">rotateBitLockerKeysDeviceActionResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="634ab-103">rotateBitLockerKeysDeviceActionResult resource type</span></span>

<span data-ttu-id="634ab-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="634ab-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="634ab-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="634ab-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="634ab-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="634ab-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="634ab-107">RotateBitLockerKeys 设备操作结果</span><span class="sxs-lookup"><span data-stu-id="634ab-107">RotateBitLockerKeys device action result</span></span>


<span data-ttu-id="634ab-108">继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="634ab-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="634ab-109">属性</span><span class="sxs-lookup"><span data-stu-id="634ab-109">Properties</span></span>
|<span data-ttu-id="634ab-110">属性</span><span class="sxs-lookup"><span data-stu-id="634ab-110">Property</span></span>|<span data-ttu-id="634ab-111">类型</span><span class="sxs-lookup"><span data-stu-id="634ab-111">Type</span></span>|<span data-ttu-id="634ab-112">说明</span><span class="sxs-lookup"><span data-stu-id="634ab-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="634ab-113">actionName</span><span class="sxs-lookup"><span data-stu-id="634ab-113">actionName</span></span>|<span data-ttu-id="634ab-114">String</span><span class="sxs-lookup"><span data-stu-id="634ab-114">String</span></span>|<span data-ttu-id="634ab-115">操作名称 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="634ab-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="634ab-116">actionState</span><span class="sxs-lookup"><span data-stu-id="634ab-116">actionState</span></span>|[<span data-ttu-id="634ab-117">actionState</span><span class="sxs-lookup"><span data-stu-id="634ab-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="634ab-118">继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)的操作的状态。</span><span class="sxs-lookup"><span data-stu-id="634ab-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="634ab-119">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed` 或 `notSupported`。</span><span class="sxs-lookup"><span data-stu-id="634ab-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="634ab-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="634ab-120">startDateTime</span></span>|<span data-ttu-id="634ab-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="634ab-121">DateTimeOffset</span></span>|<span data-ttu-id="634ab-122">操作启动的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="634ab-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="634ab-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="634ab-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="634ab-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="634ab-124">DateTimeOffset</span></span>|<span data-ttu-id="634ab-125">操作状态上次更新的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="634ab-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="634ab-126">errorCode</span><span class="sxs-lookup"><span data-stu-id="634ab-126">errorCode</span></span>|<span data-ttu-id="634ab-127">Int32</span><span class="sxs-lookup"><span data-stu-id="634ab-127">Int32</span></span>|<span data-ttu-id="634ab-128">RotateBitLockerKeys 操作错误代码</span><span class="sxs-lookup"><span data-stu-id="634ab-128">RotateBitLockerKeys action error code</span></span>|

## <a name="relationships"></a><span data-ttu-id="634ab-129">关系</span><span class="sxs-lookup"><span data-stu-id="634ab-129">Relationships</span></span>
<span data-ttu-id="634ab-130">无</span><span class="sxs-lookup"><span data-stu-id="634ab-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="634ab-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="634ab-131">JSON Representation</span></span>
<span data-ttu-id="634ab-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="634ab-132">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.rotateBitLockerKeysDeviceActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.rotateBitLockerKeysDeviceActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "errorCode": 1024
}
```







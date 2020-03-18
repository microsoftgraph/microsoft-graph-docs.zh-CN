---
title: rotateBitLockerKeysDeviceActionResult 资源类型
description: RotateBitLockerKeys 设备操作结果
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 28e78b43a29f3fce7ba02da058f7e96d6358c39f
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42783870"
---
# <a name="rotatebitlockerkeysdeviceactionresult-resource-type"></a><span data-ttu-id="0d47d-103">rotateBitLockerKeysDeviceActionResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="0d47d-103">rotateBitLockerKeysDeviceActionResult resource type</span></span>

> <span data-ttu-id="0d47d-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="0d47d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0d47d-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0d47d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0d47d-106">RotateBitLockerKeys 设备操作结果</span><span class="sxs-lookup"><span data-stu-id="0d47d-106">RotateBitLockerKeys device action result</span></span>


<span data-ttu-id="0d47d-107">继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="0d47d-107">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="0d47d-108">属性</span><span class="sxs-lookup"><span data-stu-id="0d47d-108">Properties</span></span>
|<span data-ttu-id="0d47d-109">属性</span><span class="sxs-lookup"><span data-stu-id="0d47d-109">Property</span></span>|<span data-ttu-id="0d47d-110">类型</span><span class="sxs-lookup"><span data-stu-id="0d47d-110">Type</span></span>|<span data-ttu-id="0d47d-111">说明</span><span class="sxs-lookup"><span data-stu-id="0d47d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0d47d-112">actionName</span><span class="sxs-lookup"><span data-stu-id="0d47d-112">actionName</span></span>|<span data-ttu-id="0d47d-113">String</span><span class="sxs-lookup"><span data-stu-id="0d47d-113">String</span></span>|<span data-ttu-id="0d47d-114">操作名称 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="0d47d-114">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="0d47d-115">actionState</span><span class="sxs-lookup"><span data-stu-id="0d47d-115">actionState</span></span>|[<span data-ttu-id="0d47d-116">actionState</span><span class="sxs-lookup"><span data-stu-id="0d47d-116">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="0d47d-117">继承自[deviceActionResult](../resources/intune-devices-deviceactionresult.md)的操作的状态。</span><span class="sxs-lookup"><span data-stu-id="0d47d-117">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="0d47d-118">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed` 或 `notSupported`。</span><span class="sxs-lookup"><span data-stu-id="0d47d-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="0d47d-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="0d47d-119">startDateTime</span></span>|<span data-ttu-id="0d47d-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0d47d-120">DateTimeOffset</span></span>|<span data-ttu-id="0d47d-121">操作启动的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="0d47d-121">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="0d47d-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="0d47d-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="0d47d-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0d47d-123">DateTimeOffset</span></span>|<span data-ttu-id="0d47d-124">操作状态上次更新的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="0d47d-124">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="0d47d-125">errorCode</span><span class="sxs-lookup"><span data-stu-id="0d47d-125">errorCode</span></span>|<span data-ttu-id="0d47d-126">Int32</span><span class="sxs-lookup"><span data-stu-id="0d47d-126">Int32</span></span>|<span data-ttu-id="0d47d-127">RotateBitLockerKeys 操作错误代码</span><span class="sxs-lookup"><span data-stu-id="0d47d-127">RotateBitLockerKeys action error code</span></span>|

## <a name="relationships"></a><span data-ttu-id="0d47d-128">关系</span><span class="sxs-lookup"><span data-stu-id="0d47d-128">Relationships</span></span>
<span data-ttu-id="0d47d-129">无</span><span class="sxs-lookup"><span data-stu-id="0d47d-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0d47d-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0d47d-130">JSON Representation</span></span>
<span data-ttu-id="0d47d-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0d47d-131">Here is a JSON representation of the resource.</span></span>
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




---
title: remoteLockActionResult 资源类型
description: 锁定操作结果，包含用于解锁的 PIN
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 326cfa1305645167146b7e5e8cb56a0774829929
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36030672"
---
# <a name="remotelockactionresult-resource-type"></a><span data-ttu-id="b08e0-103">remoteLockActionResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="b08e0-103">remoteLockActionResult resource type</span></span>

> <span data-ttu-id="b08e0-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b08e0-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b08e0-105">锁定操作结果，包含用于解锁的 PIN</span><span class="sxs-lookup"><span data-stu-id="b08e0-105">Lock action result with a pin to unlock</span></span>


<span data-ttu-id="b08e0-106">继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="b08e0-106">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b08e0-107">属性</span><span class="sxs-lookup"><span data-stu-id="b08e0-107">Properties</span></span>
|<span data-ttu-id="b08e0-108">属性</span><span class="sxs-lookup"><span data-stu-id="b08e0-108">Property</span></span>|<span data-ttu-id="b08e0-109">类型</span><span class="sxs-lookup"><span data-stu-id="b08e0-109">Type</span></span>|<span data-ttu-id="b08e0-110">说明</span><span class="sxs-lookup"><span data-stu-id="b08e0-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b08e0-111">actionName</span><span class="sxs-lookup"><span data-stu-id="b08e0-111">actionName</span></span>|<span data-ttu-id="b08e0-112">String</span><span class="sxs-lookup"><span data-stu-id="b08e0-112">String</span></span>|<span data-ttu-id="b08e0-113">操作名称 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="b08e0-113">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="b08e0-114">actionState</span><span class="sxs-lookup"><span data-stu-id="b08e0-114">actionState</span></span>|[<span data-ttu-id="b08e0-115">actionState</span><span class="sxs-lookup"><span data-stu-id="b08e0-115">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="b08e0-116">继承自[deviceActionResult](../resources/intune-devices-deviceactionresult.md)的操作的状态。</span><span class="sxs-lookup"><span data-stu-id="b08e0-116">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="b08e0-117">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed` 或 `notSupported`。</span><span class="sxs-lookup"><span data-stu-id="b08e0-117">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="b08e0-118">startDateTime</span><span class="sxs-lookup"><span data-stu-id="b08e0-118">startDateTime</span></span>|<span data-ttu-id="b08e0-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b08e0-119">DateTimeOffset</span></span>|<span data-ttu-id="b08e0-120">操作启动的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="b08e0-120">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="b08e0-121">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="b08e0-121">lastUpdatedDateTime</span></span>|<span data-ttu-id="b08e0-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b08e0-122">DateTimeOffset</span></span>|<span data-ttu-id="b08e0-123">上次更新操作状态的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="b08e0-123">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="b08e0-124">unlockPin</span><span class="sxs-lookup"><span data-stu-id="b08e0-124">unlockPin</span></span>|<span data-ttu-id="b08e0-125">String</span><span class="sxs-lookup"><span data-stu-id="b08e0-125">String</span></span>|<span data-ttu-id="b08e0-126">用于解锁客户端的 PIN</span><span class="sxs-lookup"><span data-stu-id="b08e0-126">Pin to unlock the client</span></span>|

## <a name="relationships"></a><span data-ttu-id="b08e0-127">关系</span><span class="sxs-lookup"><span data-stu-id="b08e0-127">Relationships</span></span>
<span data-ttu-id="b08e0-128">无</span><span class="sxs-lookup"><span data-stu-id="b08e0-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b08e0-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b08e0-129">JSON Representation</span></span>
<span data-ttu-id="b08e0-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b08e0-130">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.remoteLockActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.remoteLockActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "unlockPin": "String"
}
```




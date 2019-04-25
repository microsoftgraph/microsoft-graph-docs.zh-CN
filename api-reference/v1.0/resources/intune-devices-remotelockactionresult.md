---
title: remoteLockActionResult 资源类型
description: 锁定操作结果，包含用于解锁的 PIN
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c533d9590acba1518ac3d0dc791af804b9d84452
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32550635"
---
# <a name="remotelockactionresult-resource-type"></a><span data-ttu-id="a1da8-103">remoteLockActionResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="a1da8-103">remoteLockActionResult resource type</span></span>

> <span data-ttu-id="a1da8-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a1da8-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a1da8-105">锁定操作结果，包含用于解锁的 PIN</span><span class="sxs-lookup"><span data-stu-id="a1da8-105">Lock action result with a pin to unlock</span></span>


<span data-ttu-id="a1da8-106">继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="a1da8-106">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a1da8-107">属性</span><span class="sxs-lookup"><span data-stu-id="a1da8-107">Properties</span></span>
|<span data-ttu-id="a1da8-108">属性</span><span class="sxs-lookup"><span data-stu-id="a1da8-108">Property</span></span>|<span data-ttu-id="a1da8-109">类型</span><span class="sxs-lookup"><span data-stu-id="a1da8-109">Type</span></span>|<span data-ttu-id="a1da8-110">说明</span><span class="sxs-lookup"><span data-stu-id="a1da8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a1da8-111">actionName</span><span class="sxs-lookup"><span data-stu-id="a1da8-111">actionName</span></span>|<span data-ttu-id="a1da8-112">String</span><span class="sxs-lookup"><span data-stu-id="a1da8-112">String</span></span>|<span data-ttu-id="a1da8-113">操作名称 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="a1da8-113">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="a1da8-114">actionState</span><span class="sxs-lookup"><span data-stu-id="a1da8-114">actionState</span></span>|[<span data-ttu-id="a1da8-115">actionState</span><span class="sxs-lookup"><span data-stu-id="a1da8-115">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="a1da8-116">继承自[deviceActionResult](../resources/intune-devices-deviceactionresult.md)的操作的状态。</span><span class="sxs-lookup"><span data-stu-id="a1da8-116">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="a1da8-117">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed` 或 `notSupported`。</span><span class="sxs-lookup"><span data-stu-id="a1da8-117">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="a1da8-118">startDateTime</span><span class="sxs-lookup"><span data-stu-id="a1da8-118">startDateTime</span></span>|<span data-ttu-id="a1da8-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a1da8-119">DateTimeOffset</span></span>|<span data-ttu-id="a1da8-120">操作启动的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="a1da8-120">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="a1da8-121">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="a1da8-121">lastUpdatedDateTime</span></span>|<span data-ttu-id="a1da8-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a1da8-122">DateTimeOffset</span></span>|<span data-ttu-id="a1da8-123">上次更新操作状态的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="a1da8-123">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="a1da8-124">unlockPin</span><span class="sxs-lookup"><span data-stu-id="a1da8-124">unlockPin</span></span>|<span data-ttu-id="a1da8-125">String</span><span class="sxs-lookup"><span data-stu-id="a1da8-125">String</span></span>|<span data-ttu-id="a1da8-126">用于解锁客户端的 PIN</span><span class="sxs-lookup"><span data-stu-id="a1da8-126">Pin to unlock the client</span></span>|

## <a name="relationships"></a><span data-ttu-id="a1da8-127">关系</span><span class="sxs-lookup"><span data-stu-id="a1da8-127">Relationships</span></span>
<span data-ttu-id="a1da8-128">无</span><span class="sxs-lookup"><span data-stu-id="a1da8-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a1da8-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a1da8-129">JSON Representation</span></span>
<span data-ttu-id="a1da8-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a1da8-130">Here is a JSON representation of the resource.</span></span>
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




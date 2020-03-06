---
title: remoteLockActionResult 资源类型
description: 锁定操作结果，包含用于解锁的 PIN
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a9205ba5ede57f87cfc56cdbebaea1d5d2ccaa08
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532179"
---
# <a name="remotelockactionresult-resource-type"></a><span data-ttu-id="65322-103">remoteLockActionResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="65322-103">remoteLockActionResult resource type</span></span>

<span data-ttu-id="65322-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="65322-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="65322-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="65322-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="65322-106">锁定操作结果，包含用于解锁的 PIN</span><span class="sxs-lookup"><span data-stu-id="65322-106">Lock action result with a pin to unlock</span></span>


<span data-ttu-id="65322-107">继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="65322-107">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="65322-108">属性</span><span class="sxs-lookup"><span data-stu-id="65322-108">Properties</span></span>
|<span data-ttu-id="65322-109">属性</span><span class="sxs-lookup"><span data-stu-id="65322-109">Property</span></span>|<span data-ttu-id="65322-110">类型</span><span class="sxs-lookup"><span data-stu-id="65322-110">Type</span></span>|<span data-ttu-id="65322-111">说明</span><span class="sxs-lookup"><span data-stu-id="65322-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="65322-112">actionName</span><span class="sxs-lookup"><span data-stu-id="65322-112">actionName</span></span>|<span data-ttu-id="65322-113">字符串</span><span class="sxs-lookup"><span data-stu-id="65322-113">String</span></span>|<span data-ttu-id="65322-114">操作名称 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="65322-114">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="65322-115">actionState</span><span class="sxs-lookup"><span data-stu-id="65322-115">actionState</span></span>|[<span data-ttu-id="65322-116">actionState</span><span class="sxs-lookup"><span data-stu-id="65322-116">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="65322-117">继承自[deviceActionResult](../resources/intune-devices-deviceactionresult.md)的操作的状态。</span><span class="sxs-lookup"><span data-stu-id="65322-117">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="65322-118">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed` 或 `notSupported`。</span><span class="sxs-lookup"><span data-stu-id="65322-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="65322-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="65322-119">startDateTime</span></span>|<span data-ttu-id="65322-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="65322-120">DateTimeOffset</span></span>|<span data-ttu-id="65322-121">操作启动的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="65322-121">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="65322-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="65322-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="65322-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="65322-123">DateTimeOffset</span></span>|<span data-ttu-id="65322-124">上次更新操作状态的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="65322-124">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="65322-125">unlockPin</span><span class="sxs-lookup"><span data-stu-id="65322-125">unlockPin</span></span>|<span data-ttu-id="65322-126">String</span><span class="sxs-lookup"><span data-stu-id="65322-126">String</span></span>|<span data-ttu-id="65322-127">用于解锁客户端的 PIN</span><span class="sxs-lookup"><span data-stu-id="65322-127">Pin to unlock the client</span></span>|

## <a name="relationships"></a><span data-ttu-id="65322-128">关系</span><span class="sxs-lookup"><span data-stu-id="65322-128">Relationships</span></span>
<span data-ttu-id="65322-129">无</span><span class="sxs-lookup"><span data-stu-id="65322-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="65322-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="65322-130">JSON Representation</span></span>
<span data-ttu-id="65322-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="65322-131">Here is a JSON representation of the resource.</span></span>
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





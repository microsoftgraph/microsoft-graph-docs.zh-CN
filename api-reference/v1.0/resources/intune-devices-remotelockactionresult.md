---
title: remoteLockActionResult 资源类型
description: 锁定操作结果，包含用于解锁的 PIN
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c6eae05e799394d37fa5c842b278f60251fbd47a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48091038"
---
# <a name="remotelockactionresult-resource-type"></a><span data-ttu-id="e9b3a-103">remoteLockActionResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="e9b3a-103">remoteLockActionResult resource type</span></span>

<span data-ttu-id="e9b3a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e9b3a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e9b3a-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e9b3a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e9b3a-106">锁定操作结果，包含用于解锁的 PIN</span><span class="sxs-lookup"><span data-stu-id="e9b3a-106">Lock action result with a pin to unlock</span></span>


<span data-ttu-id="e9b3a-107">继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="e9b3a-107">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e9b3a-108">属性</span><span class="sxs-lookup"><span data-stu-id="e9b3a-108">Properties</span></span>
|<span data-ttu-id="e9b3a-109">属性</span><span class="sxs-lookup"><span data-stu-id="e9b3a-109">Property</span></span>|<span data-ttu-id="e9b3a-110">类型</span><span class="sxs-lookup"><span data-stu-id="e9b3a-110">Type</span></span>|<span data-ttu-id="e9b3a-111">说明</span><span class="sxs-lookup"><span data-stu-id="e9b3a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e9b3a-112">actionName</span><span class="sxs-lookup"><span data-stu-id="e9b3a-112">actionName</span></span>|<span data-ttu-id="e9b3a-113">String</span><span class="sxs-lookup"><span data-stu-id="e9b3a-113">String</span></span>|<span data-ttu-id="e9b3a-114">操作名称 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="e9b3a-114">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="e9b3a-115">actionState</span><span class="sxs-lookup"><span data-stu-id="e9b3a-115">actionState</span></span>|[<span data-ttu-id="e9b3a-116">actionState</span><span class="sxs-lookup"><span data-stu-id="e9b3a-116">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="e9b3a-117">继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)的操作的状态。</span><span class="sxs-lookup"><span data-stu-id="e9b3a-117">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="e9b3a-118">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed` 或 `notSupported`。</span><span class="sxs-lookup"><span data-stu-id="e9b3a-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="e9b3a-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="e9b3a-119">startDateTime</span></span>|<span data-ttu-id="e9b3a-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e9b3a-120">DateTimeOffset</span></span>|<span data-ttu-id="e9b3a-121">操作启动的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="e9b3a-121">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="e9b3a-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="e9b3a-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="e9b3a-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e9b3a-123">DateTimeOffset</span></span>|<span data-ttu-id="e9b3a-124">上次更新操作状态的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="e9b3a-124">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="e9b3a-125">unlockPin</span><span class="sxs-lookup"><span data-stu-id="e9b3a-125">unlockPin</span></span>|<span data-ttu-id="e9b3a-126">String</span><span class="sxs-lookup"><span data-stu-id="e9b3a-126">String</span></span>|<span data-ttu-id="e9b3a-127">用于解锁客户端的 PIN</span><span class="sxs-lookup"><span data-stu-id="e9b3a-127">Pin to unlock the client</span></span>|

## <a name="relationships"></a><span data-ttu-id="e9b3a-128">关系</span><span class="sxs-lookup"><span data-stu-id="e9b3a-128">Relationships</span></span>
<span data-ttu-id="e9b3a-129">无</span><span class="sxs-lookup"><span data-stu-id="e9b3a-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e9b3a-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e9b3a-130">JSON Representation</span></span>
<span data-ttu-id="e9b3a-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e9b3a-131">Here is a JSON representation of the resource.</span></span>
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










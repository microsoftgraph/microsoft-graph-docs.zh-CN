---
title: remoteLockActionResult 资源类型
description: 锁定操作结果，包含用于解锁的 PIN
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8a8da7d99425e35c937250eee8a36ba005a133af
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33941742"
---
# <a name="remotelockactionresult-resource-type"></a><span data-ttu-id="859ee-103">remoteLockActionResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="859ee-103">remoteLockActionResult resource type</span></span>

> <span data-ttu-id="859ee-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="859ee-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="859ee-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="859ee-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="859ee-106">锁定操作结果，包含用于解锁的 PIN</span><span class="sxs-lookup"><span data-stu-id="859ee-106">Lock action result with a pin to unlock</span></span>


<span data-ttu-id="859ee-107">继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="859ee-107">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="859ee-108">属性</span><span class="sxs-lookup"><span data-stu-id="859ee-108">Properties</span></span>
|<span data-ttu-id="859ee-109">属性</span><span class="sxs-lookup"><span data-stu-id="859ee-109">Property</span></span>|<span data-ttu-id="859ee-110">类型</span><span class="sxs-lookup"><span data-stu-id="859ee-110">Type</span></span>|<span data-ttu-id="859ee-111">说明</span><span class="sxs-lookup"><span data-stu-id="859ee-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="859ee-112">actionName</span><span class="sxs-lookup"><span data-stu-id="859ee-112">actionName</span></span>|<span data-ttu-id="859ee-113">String</span><span class="sxs-lookup"><span data-stu-id="859ee-113">String</span></span>|<span data-ttu-id="859ee-114">操作名称 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="859ee-114">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="859ee-115">actionState</span><span class="sxs-lookup"><span data-stu-id="859ee-115">actionState</span></span>|[<span data-ttu-id="859ee-116">actionState</span><span class="sxs-lookup"><span data-stu-id="859ee-116">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="859ee-117">继承自[deviceActionResult](../resources/intune-devices-deviceactionresult.md)的操作的状态。</span><span class="sxs-lookup"><span data-stu-id="859ee-117">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="859ee-118">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed` 或 `notSupported`。</span><span class="sxs-lookup"><span data-stu-id="859ee-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="859ee-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="859ee-119">startDateTime</span></span>|<span data-ttu-id="859ee-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="859ee-120">DateTimeOffset</span></span>|<span data-ttu-id="859ee-121">操作启动的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="859ee-121">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="859ee-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="859ee-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="859ee-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="859ee-123">DateTimeOffset</span></span>|<span data-ttu-id="859ee-124">上次更新操作状态的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="859ee-124">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="859ee-125">unlockPin</span><span class="sxs-lookup"><span data-stu-id="859ee-125">unlockPin</span></span>|<span data-ttu-id="859ee-126">String</span><span class="sxs-lookup"><span data-stu-id="859ee-126">String</span></span>|<span data-ttu-id="859ee-127">用于解锁客户端的 PIN</span><span class="sxs-lookup"><span data-stu-id="859ee-127">Pin to unlock the client</span></span>|

## <a name="relationships"></a><span data-ttu-id="859ee-128">关系</span><span class="sxs-lookup"><span data-stu-id="859ee-128">Relationships</span></span>
<span data-ttu-id="859ee-129">无</span><span class="sxs-lookup"><span data-stu-id="859ee-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="859ee-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="859ee-130">JSON Representation</span></span>
<span data-ttu-id="859ee-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="859ee-131">Here is a JSON representation of the resource.</span></span>
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





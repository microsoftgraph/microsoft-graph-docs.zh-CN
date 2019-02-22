---
title: remoteLockActionResult 资源类型
description: 锁定操作结果，包含用于解锁的 PIN
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f90cbc46ca4bc9476ad5d9386581385ae7354261
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30159022"
---
# <a name="remotelockactionresult-resource-type"></a><span data-ttu-id="fa956-103">remoteLockActionResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="fa956-103">remoteLockActionResult resource type</span></span>

> <span data-ttu-id="fa956-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="fa956-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fa956-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fa956-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fa956-106">锁定操作结果，包含用于解锁的 PIN</span><span class="sxs-lookup"><span data-stu-id="fa956-106">Lock action result with a pin to unlock</span></span>


<span data-ttu-id="fa956-107">继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="fa956-107">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="fa956-108">属性</span><span class="sxs-lookup"><span data-stu-id="fa956-108">Properties</span></span>
|<span data-ttu-id="fa956-109">属性</span><span class="sxs-lookup"><span data-stu-id="fa956-109">Property</span></span>|<span data-ttu-id="fa956-110">类型</span><span class="sxs-lookup"><span data-stu-id="fa956-110">Type</span></span>|<span data-ttu-id="fa956-111">说明</span><span class="sxs-lookup"><span data-stu-id="fa956-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fa956-112">actionName</span><span class="sxs-lookup"><span data-stu-id="fa956-112">actionName</span></span>|<span data-ttu-id="fa956-113">String</span><span class="sxs-lookup"><span data-stu-id="fa956-113">String</span></span>|<span data-ttu-id="fa956-114">操作名称 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="fa956-114">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="fa956-115">actionState</span><span class="sxs-lookup"><span data-stu-id="fa956-115">actionState</span></span>|[<span data-ttu-id="fa956-116">actionState</span><span class="sxs-lookup"><span data-stu-id="fa956-116">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="fa956-117">继承自[deviceActionResult](../resources/intune-devices-deviceactionresult.md)的操作的状态。</span><span class="sxs-lookup"><span data-stu-id="fa956-117">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="fa956-118">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported`。</span><span class="sxs-lookup"><span data-stu-id="fa956-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="fa956-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="fa956-119">startDateTime</span></span>|<span data-ttu-id="fa956-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fa956-120">DateTimeOffset</span></span>|<span data-ttu-id="fa956-121">启动操作的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="fa956-121">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="fa956-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="fa956-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="fa956-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fa956-123">DateTimeOffset</span></span>|<span data-ttu-id="fa956-124">上次更新操作状态的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="fa956-124">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="fa956-125">unlockPin</span><span class="sxs-lookup"><span data-stu-id="fa956-125">unlockPin</span></span>|<span data-ttu-id="fa956-126">String</span><span class="sxs-lookup"><span data-stu-id="fa956-126">String</span></span>|<span data-ttu-id="fa956-127">用于解锁客户端的 PIN</span><span class="sxs-lookup"><span data-stu-id="fa956-127">Pin to unlock the client</span></span>|

## <a name="relationships"></a><span data-ttu-id="fa956-128">关系</span><span class="sxs-lookup"><span data-stu-id="fa956-128">Relationships</span></span>
<span data-ttu-id="fa956-129">无</span><span class="sxs-lookup"><span data-stu-id="fa956-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fa956-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fa956-130">JSON Representation</span></span>
<span data-ttu-id="fa956-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fa956-131">Here is a JSON representation of the resource.</span></span>
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





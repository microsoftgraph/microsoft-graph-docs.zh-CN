---
title: remoteLockActionResult 资源类型
description: 锁定操作结果，包含用于解锁的 PIN
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b16a99c793d60de04201fc057a58da122c83fd6c
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31788518"
---
# <a name="remotelockactionresult-resource-type"></a><span data-ttu-id="4f9e1-103">remoteLockActionResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="4f9e1-103">remoteLockActionResult resource type</span></span>

> <span data-ttu-id="4f9e1-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4f9e1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4f9e1-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4f9e1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4f9e1-106">锁定操作结果，包含用于解锁的 PIN</span><span class="sxs-lookup"><span data-stu-id="4f9e1-106">Lock action result with a pin to unlock</span></span>


<span data-ttu-id="4f9e1-107">继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="4f9e1-107">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4f9e1-108">属性</span><span class="sxs-lookup"><span data-stu-id="4f9e1-108">Properties</span></span>
|<span data-ttu-id="4f9e1-109">属性</span><span class="sxs-lookup"><span data-stu-id="4f9e1-109">Property</span></span>|<span data-ttu-id="4f9e1-110">类型</span><span class="sxs-lookup"><span data-stu-id="4f9e1-110">Type</span></span>|<span data-ttu-id="4f9e1-111">说明</span><span class="sxs-lookup"><span data-stu-id="4f9e1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4f9e1-112">actionName</span><span class="sxs-lookup"><span data-stu-id="4f9e1-112">actionName</span></span>|<span data-ttu-id="4f9e1-113">String</span><span class="sxs-lookup"><span data-stu-id="4f9e1-113">String</span></span>|<span data-ttu-id="4f9e1-114">操作名称 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="4f9e1-114">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="4f9e1-115">actionState</span><span class="sxs-lookup"><span data-stu-id="4f9e1-115">actionState</span></span>|[<span data-ttu-id="4f9e1-116">actionState</span><span class="sxs-lookup"><span data-stu-id="4f9e1-116">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="4f9e1-117">继承自[deviceActionResult](../resources/intune-devices-deviceactionresult.md)的操作的状态。</span><span class="sxs-lookup"><span data-stu-id="4f9e1-117">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="4f9e1-118">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed` 或 `notSupported`。</span><span class="sxs-lookup"><span data-stu-id="4f9e1-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="4f9e1-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="4f9e1-119">startDateTime</span></span>|<span data-ttu-id="4f9e1-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4f9e1-120">DateTimeOffset</span></span>|<span data-ttu-id="4f9e1-121">操作启动的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="4f9e1-121">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="4f9e1-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="4f9e1-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="4f9e1-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4f9e1-123">DateTimeOffset</span></span>|<span data-ttu-id="4f9e1-124">上次更新操作状态的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="4f9e1-124">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="4f9e1-125">unlockPin</span><span class="sxs-lookup"><span data-stu-id="4f9e1-125">unlockPin</span></span>|<span data-ttu-id="4f9e1-126">String</span><span class="sxs-lookup"><span data-stu-id="4f9e1-126">String</span></span>|<span data-ttu-id="4f9e1-127">用于解锁客户端的 PIN</span><span class="sxs-lookup"><span data-stu-id="4f9e1-127">Pin to unlock the client</span></span>|

## <a name="relationships"></a><span data-ttu-id="4f9e1-128">关系</span><span class="sxs-lookup"><span data-stu-id="4f9e1-128">Relationships</span></span>
<span data-ttu-id="4f9e1-129">无</span><span class="sxs-lookup"><span data-stu-id="4f9e1-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4f9e1-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4f9e1-130">JSON Representation</span></span>
<span data-ttu-id="4f9e1-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4f9e1-131">Here is a JSON representation of the resource.</span></span>
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






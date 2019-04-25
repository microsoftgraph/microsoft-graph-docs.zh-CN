---
title: remoteLockActionResult 资源类型
description: 锁定操作结果，包含用于解锁的 PIN
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b16a99c793d60de04201fc057a58da122c83fd6c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32526158"
---
# <a name="remotelockactionresult-resource-type"></a><span data-ttu-id="0d3c3-103">remoteLockActionResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="0d3c3-103">remoteLockActionResult resource type</span></span>

> <span data-ttu-id="0d3c3-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="0d3c3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0d3c3-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0d3c3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0d3c3-106">锁定操作结果，包含用于解锁的 PIN</span><span class="sxs-lookup"><span data-stu-id="0d3c3-106">Lock action result with a pin to unlock</span></span>


<span data-ttu-id="0d3c3-107">继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="0d3c3-107">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="0d3c3-108">属性</span><span class="sxs-lookup"><span data-stu-id="0d3c3-108">Properties</span></span>
|<span data-ttu-id="0d3c3-109">属性</span><span class="sxs-lookup"><span data-stu-id="0d3c3-109">Property</span></span>|<span data-ttu-id="0d3c3-110">类型</span><span class="sxs-lookup"><span data-stu-id="0d3c3-110">Type</span></span>|<span data-ttu-id="0d3c3-111">说明</span><span class="sxs-lookup"><span data-stu-id="0d3c3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0d3c3-112">actionName</span><span class="sxs-lookup"><span data-stu-id="0d3c3-112">actionName</span></span>|<span data-ttu-id="0d3c3-113">String</span><span class="sxs-lookup"><span data-stu-id="0d3c3-113">String</span></span>|<span data-ttu-id="0d3c3-114">操作名称 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="0d3c3-114">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="0d3c3-115">actionState</span><span class="sxs-lookup"><span data-stu-id="0d3c3-115">actionState</span></span>|[<span data-ttu-id="0d3c3-116">actionState</span><span class="sxs-lookup"><span data-stu-id="0d3c3-116">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="0d3c3-117">继承自[deviceActionResult](../resources/intune-devices-deviceactionresult.md)的操作的状态。</span><span class="sxs-lookup"><span data-stu-id="0d3c3-117">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="0d3c3-118">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed` 或 `notSupported`。</span><span class="sxs-lookup"><span data-stu-id="0d3c3-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="0d3c3-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="0d3c3-119">startDateTime</span></span>|<span data-ttu-id="0d3c3-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0d3c3-120">DateTimeOffset</span></span>|<span data-ttu-id="0d3c3-121">操作启动的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="0d3c3-121">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="0d3c3-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="0d3c3-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="0d3c3-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0d3c3-123">DateTimeOffset</span></span>|<span data-ttu-id="0d3c3-124">上次更新操作状态的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="0d3c3-124">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="0d3c3-125">unlockPin</span><span class="sxs-lookup"><span data-stu-id="0d3c3-125">unlockPin</span></span>|<span data-ttu-id="0d3c3-126">String</span><span class="sxs-lookup"><span data-stu-id="0d3c3-126">String</span></span>|<span data-ttu-id="0d3c3-127">用于解锁客户端的 PIN</span><span class="sxs-lookup"><span data-stu-id="0d3c3-127">Pin to unlock the client</span></span>|

## <a name="relationships"></a><span data-ttu-id="0d3c3-128">关系</span><span class="sxs-lookup"><span data-stu-id="0d3c3-128">Relationships</span></span>
<span data-ttu-id="0d3c3-129">无</span><span class="sxs-lookup"><span data-stu-id="0d3c3-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0d3c3-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0d3c3-130">JSON Representation</span></span>
<span data-ttu-id="0d3c3-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0d3c3-131">Here is a JSON representation of the resource.</span></span>
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






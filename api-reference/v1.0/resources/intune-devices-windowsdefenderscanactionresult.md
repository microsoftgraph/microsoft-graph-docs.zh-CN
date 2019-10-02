---
title: windowsDefenderScanActionResult 资源类型
description: Windows Defender 最后扫描结果
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 1ce77c0e034cacf301dfdfa5df96070bd1944160
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37356882"
---
# <a name="windowsdefenderscanactionresult-resource-type"></a><span data-ttu-id="7a3c0-103">windowsDefenderScanActionResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="7a3c0-103">windowsDefenderScanActionResult resource type</span></span>

> <span data-ttu-id="7a3c0-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7a3c0-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7a3c0-105">Windows Defender 最后扫描结果</span><span class="sxs-lookup"><span data-stu-id="7a3c0-105">Windows Defender last scan result</span></span>


<span data-ttu-id="7a3c0-106">继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="7a3c0-106">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="7a3c0-107">属性</span><span class="sxs-lookup"><span data-stu-id="7a3c0-107">Properties</span></span>
|<span data-ttu-id="7a3c0-108">属性</span><span class="sxs-lookup"><span data-stu-id="7a3c0-108">Property</span></span>|<span data-ttu-id="7a3c0-109">类型</span><span class="sxs-lookup"><span data-stu-id="7a3c0-109">Type</span></span>|<span data-ttu-id="7a3c0-110">说明</span><span class="sxs-lookup"><span data-stu-id="7a3c0-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7a3c0-111">actionName</span><span class="sxs-lookup"><span data-stu-id="7a3c0-111">actionName</span></span>|<span data-ttu-id="7a3c0-112">String</span><span class="sxs-lookup"><span data-stu-id="7a3c0-112">String</span></span>|<span data-ttu-id="7a3c0-113">操作名称 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="7a3c0-113">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="7a3c0-114">actionState</span><span class="sxs-lookup"><span data-stu-id="7a3c0-114">actionState</span></span>|[<span data-ttu-id="7a3c0-115">actionState</span><span class="sxs-lookup"><span data-stu-id="7a3c0-115">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="7a3c0-116">继承自[deviceActionResult](../resources/intune-devices-deviceactionresult.md)的操作的状态。</span><span class="sxs-lookup"><span data-stu-id="7a3c0-116">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="7a3c0-117">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed` 或 `notSupported`。</span><span class="sxs-lookup"><span data-stu-id="7a3c0-117">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="7a3c0-118">startDateTime</span><span class="sxs-lookup"><span data-stu-id="7a3c0-118">startDateTime</span></span>|<span data-ttu-id="7a3c0-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7a3c0-119">DateTimeOffset</span></span>|<span data-ttu-id="7a3c0-120">操作启动的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="7a3c0-120">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="7a3c0-121">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="7a3c0-121">lastUpdatedDateTime</span></span>|<span data-ttu-id="7a3c0-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7a3c0-122">DateTimeOffset</span></span>|<span data-ttu-id="7a3c0-123">操作状态上次更新的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="7a3c0-123">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="7a3c0-124">scanType</span><span class="sxs-lookup"><span data-stu-id="7a3c0-124">scanType</span></span>|<span data-ttu-id="7a3c0-125">String</span><span class="sxs-lookup"><span data-stu-id="7a3c0-125">String</span></span>|<span data-ttu-id="7a3c0-126">扫描类型（完全扫描或快速扫描）</span><span class="sxs-lookup"><span data-stu-id="7a3c0-126">Scan type either full scan or quick scan</span></span>|

## <a name="relationships"></a><span data-ttu-id="7a3c0-127">关系</span><span class="sxs-lookup"><span data-stu-id="7a3c0-127">Relationships</span></span>
<span data-ttu-id="7a3c0-128">无</span><span class="sxs-lookup"><span data-stu-id="7a3c0-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7a3c0-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7a3c0-129">JSON Representation</span></span>
<span data-ttu-id="7a3c0-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7a3c0-130">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsDefenderScanActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsDefenderScanActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "scanType": "String"
}
```





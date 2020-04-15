---
title: windowsDefenderScanActionResult 资源类型
description: Windows Defender 最后扫描结果
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8f0d0296442ebb9c67dea8dc87b1a42bd980c92c
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43406817"
---
# <a name="windowsdefenderscanactionresult-resource-type"></a><span data-ttu-id="a26e9-103">windowsDefenderScanActionResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="a26e9-103">windowsDefenderScanActionResult resource type</span></span>

<span data-ttu-id="a26e9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a26e9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a26e9-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a26e9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a26e9-106">Windows Defender 最后扫描结果</span><span class="sxs-lookup"><span data-stu-id="a26e9-106">Windows Defender last scan result</span></span>


<span data-ttu-id="a26e9-107">继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="a26e9-107">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a26e9-108">属性</span><span class="sxs-lookup"><span data-stu-id="a26e9-108">Properties</span></span>
|<span data-ttu-id="a26e9-109">属性</span><span class="sxs-lookup"><span data-stu-id="a26e9-109">Property</span></span>|<span data-ttu-id="a26e9-110">类型</span><span class="sxs-lookup"><span data-stu-id="a26e9-110">Type</span></span>|<span data-ttu-id="a26e9-111">说明</span><span class="sxs-lookup"><span data-stu-id="a26e9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a26e9-112">actionName</span><span class="sxs-lookup"><span data-stu-id="a26e9-112">actionName</span></span>|<span data-ttu-id="a26e9-113">String</span><span class="sxs-lookup"><span data-stu-id="a26e9-113">String</span></span>|<span data-ttu-id="a26e9-114">操作名称 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="a26e9-114">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="a26e9-115">actionState</span><span class="sxs-lookup"><span data-stu-id="a26e9-115">actionState</span></span>|[<span data-ttu-id="a26e9-116">actionState</span><span class="sxs-lookup"><span data-stu-id="a26e9-116">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="a26e9-117">继承自[deviceActionResult](../resources/intune-devices-deviceactionresult.md)的操作的状态。</span><span class="sxs-lookup"><span data-stu-id="a26e9-117">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="a26e9-118">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed` 或 `notSupported`。</span><span class="sxs-lookup"><span data-stu-id="a26e9-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="a26e9-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="a26e9-119">startDateTime</span></span>|<span data-ttu-id="a26e9-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a26e9-120">DateTimeOffset</span></span>|<span data-ttu-id="a26e9-121">操作启动的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="a26e9-121">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="a26e9-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="a26e9-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="a26e9-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a26e9-123">DateTimeOffset</span></span>|<span data-ttu-id="a26e9-124">操作状态上次更新的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="a26e9-124">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="a26e9-125">scanType</span><span class="sxs-lookup"><span data-stu-id="a26e9-125">scanType</span></span>|<span data-ttu-id="a26e9-126">String</span><span class="sxs-lookup"><span data-stu-id="a26e9-126">String</span></span>|<span data-ttu-id="a26e9-127">扫描类型（完全扫描或快速扫描）</span><span class="sxs-lookup"><span data-stu-id="a26e9-127">Scan type either full scan or quick scan</span></span>|

## <a name="relationships"></a><span data-ttu-id="a26e9-128">关系</span><span class="sxs-lookup"><span data-stu-id="a26e9-128">Relationships</span></span>
<span data-ttu-id="a26e9-129">无</span><span class="sxs-lookup"><span data-stu-id="a26e9-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a26e9-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a26e9-130">JSON Representation</span></span>
<span data-ttu-id="a26e9-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a26e9-131">Here is a JSON representation of the resource.</span></span>
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








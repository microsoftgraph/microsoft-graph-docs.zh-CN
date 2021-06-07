---
title: windowsDefenderScanActionResult 资源类型
description: Windows Defender 最后扫描结果
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 857494e6c4e08fe2f659bf26ae63a0be19c17c3e
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755005"
---
# <a name="windowsdefenderscanactionresult-resource-type"></a><span data-ttu-id="7910e-103">windowsDefenderScanActionResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="7910e-103">windowsDefenderScanActionResult resource type</span></span>

<span data-ttu-id="7910e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7910e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7910e-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7910e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7910e-106">Windows Defender 最后扫描结果</span><span class="sxs-lookup"><span data-stu-id="7910e-106">Windows Defender last scan result</span></span>


<span data-ttu-id="7910e-107">继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="7910e-107">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="7910e-108">属性</span><span class="sxs-lookup"><span data-stu-id="7910e-108">Properties</span></span>
|<span data-ttu-id="7910e-109">属性</span><span class="sxs-lookup"><span data-stu-id="7910e-109">Property</span></span>|<span data-ttu-id="7910e-110">类型</span><span class="sxs-lookup"><span data-stu-id="7910e-110">Type</span></span>|<span data-ttu-id="7910e-111">Description</span><span class="sxs-lookup"><span data-stu-id="7910e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7910e-112">actionName</span><span class="sxs-lookup"><span data-stu-id="7910e-112">actionName</span></span>|<span data-ttu-id="7910e-113">String</span><span class="sxs-lookup"><span data-stu-id="7910e-113">String</span></span>|<span data-ttu-id="7910e-114">操作名称 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="7910e-114">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="7910e-115">actionState</span><span class="sxs-lookup"><span data-stu-id="7910e-115">actionState</span></span>|[<span data-ttu-id="7910e-116">actionState</span><span class="sxs-lookup"><span data-stu-id="7910e-116">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="7910e-117">操作的状态 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)。</span><span class="sxs-lookup"><span data-stu-id="7910e-117">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="7910e-118">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed` 或 `notSupported`。</span><span class="sxs-lookup"><span data-stu-id="7910e-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="7910e-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="7910e-119">startDateTime</span></span>|<span data-ttu-id="7910e-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7910e-120">DateTimeOffset</span></span>|<span data-ttu-id="7910e-121">操作启动的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="7910e-121">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="7910e-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="7910e-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="7910e-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7910e-123">DateTimeOffset</span></span>|<span data-ttu-id="7910e-124">操作状态上次更新的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="7910e-124">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="7910e-125">scanType</span><span class="sxs-lookup"><span data-stu-id="7910e-125">scanType</span></span>|<span data-ttu-id="7910e-126">String</span><span class="sxs-lookup"><span data-stu-id="7910e-126">String</span></span>|<span data-ttu-id="7910e-127">扫描类型（完全扫描或快速扫描）</span><span class="sxs-lookup"><span data-stu-id="7910e-127">Scan type either full scan or quick scan</span></span>|

## <a name="relationships"></a><span data-ttu-id="7910e-128">关系</span><span class="sxs-lookup"><span data-stu-id="7910e-128">Relationships</span></span>
<span data-ttu-id="7910e-129">无</span><span class="sxs-lookup"><span data-stu-id="7910e-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7910e-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7910e-130">JSON Representation</span></span>
<span data-ttu-id="7910e-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7910e-131">Here is a JSON representation of the resource.</span></span>
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





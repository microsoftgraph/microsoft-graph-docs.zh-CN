---
title: windowsDefenderScanActionResult 资源类型
description: Windows Defender 最后扫描结果
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 094880247ee2612d0066bb44aa6f6bb581f7efe5
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30148641"
---
# <a name="windowsdefenderscanactionresult-resource-type"></a><span data-ttu-id="3a077-103">windowsDefenderScanActionResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="3a077-103">windowsDefenderScanActionResult resource type</span></span>

> <span data-ttu-id="3a077-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3a077-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3a077-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3a077-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3a077-106">Windows Defender 最后扫描结果</span><span class="sxs-lookup"><span data-stu-id="3a077-106">Windows Defender last scan result</span></span>


<span data-ttu-id="3a077-107">继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="3a077-107">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="3a077-108">属性</span><span class="sxs-lookup"><span data-stu-id="3a077-108">Properties</span></span>
|<span data-ttu-id="3a077-109">属性</span><span class="sxs-lookup"><span data-stu-id="3a077-109">Property</span></span>|<span data-ttu-id="3a077-110">类型</span><span class="sxs-lookup"><span data-stu-id="3a077-110">Type</span></span>|<span data-ttu-id="3a077-111">说明</span><span class="sxs-lookup"><span data-stu-id="3a077-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3a077-112">actionName</span><span class="sxs-lookup"><span data-stu-id="3a077-112">actionName</span></span>|<span data-ttu-id="3a077-113">String</span><span class="sxs-lookup"><span data-stu-id="3a077-113">String</span></span>|<span data-ttu-id="3a077-114">操作名称 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="3a077-114">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="3a077-115">actionState</span><span class="sxs-lookup"><span data-stu-id="3a077-115">actionState</span></span>|[<span data-ttu-id="3a077-116">actionState</span><span class="sxs-lookup"><span data-stu-id="3a077-116">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="3a077-117">继承自[deviceActionResult](../resources/intune-devices-deviceactionresult.md)的操作的状态。</span><span class="sxs-lookup"><span data-stu-id="3a077-117">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="3a077-118">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported`。</span><span class="sxs-lookup"><span data-stu-id="3a077-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="3a077-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="3a077-119">startDateTime</span></span>|<span data-ttu-id="3a077-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3a077-120">DateTimeOffset</span></span>|<span data-ttu-id="3a077-121">启动操作的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="3a077-121">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="3a077-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="3a077-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="3a077-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3a077-123">DateTimeOffset</span></span>|<span data-ttu-id="3a077-124">操作状态上次更新的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="3a077-124">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="3a077-125">scanType</span><span class="sxs-lookup"><span data-stu-id="3a077-125">scanType</span></span>|<span data-ttu-id="3a077-126">String</span><span class="sxs-lookup"><span data-stu-id="3a077-126">String</span></span>|<span data-ttu-id="3a077-127">扫描类型（完全扫描或快速扫描）</span><span class="sxs-lookup"><span data-stu-id="3a077-127">Scan type either full scan or quick scan</span></span>|

## <a name="relationships"></a><span data-ttu-id="3a077-128">关系</span><span class="sxs-lookup"><span data-stu-id="3a077-128">Relationships</span></span>
<span data-ttu-id="3a077-129">无</span><span class="sxs-lookup"><span data-stu-id="3a077-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3a077-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3a077-130">JSON Representation</span></span>
<span data-ttu-id="3a077-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3a077-131">Here is a JSON representation of the resource.</span></span>
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





---
title: windowsDefenderScanActionResult 资源类型
description: Windows Defender 最后扫描结果
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 58e2490e0b473c1a59cb3ac35525fbc57b5790a8
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42783737"
---
# <a name="windowsdefenderscanactionresult-resource-type"></a><span data-ttu-id="4a9a1-103">windowsDefenderScanActionResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="4a9a1-103">windowsDefenderScanActionResult resource type</span></span>

> <span data-ttu-id="4a9a1-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4a9a1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4a9a1-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4a9a1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4a9a1-106">Windows Defender 最后扫描结果</span><span class="sxs-lookup"><span data-stu-id="4a9a1-106">Windows Defender last scan result</span></span>


<span data-ttu-id="4a9a1-107">继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="4a9a1-107">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4a9a1-108">属性</span><span class="sxs-lookup"><span data-stu-id="4a9a1-108">Properties</span></span>
|<span data-ttu-id="4a9a1-109">属性</span><span class="sxs-lookup"><span data-stu-id="4a9a1-109">Property</span></span>|<span data-ttu-id="4a9a1-110">类型</span><span class="sxs-lookup"><span data-stu-id="4a9a1-110">Type</span></span>|<span data-ttu-id="4a9a1-111">说明</span><span class="sxs-lookup"><span data-stu-id="4a9a1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4a9a1-112">actionName</span><span class="sxs-lookup"><span data-stu-id="4a9a1-112">actionName</span></span>|<span data-ttu-id="4a9a1-113">String</span><span class="sxs-lookup"><span data-stu-id="4a9a1-113">String</span></span>|<span data-ttu-id="4a9a1-114">操作名称 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="4a9a1-114">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="4a9a1-115">actionState</span><span class="sxs-lookup"><span data-stu-id="4a9a1-115">actionState</span></span>|[<span data-ttu-id="4a9a1-116">actionState</span><span class="sxs-lookup"><span data-stu-id="4a9a1-116">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="4a9a1-117">继承自[deviceActionResult](../resources/intune-devices-deviceactionresult.md)的操作的状态。</span><span class="sxs-lookup"><span data-stu-id="4a9a1-117">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="4a9a1-118">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed` 或 `notSupported`。</span><span class="sxs-lookup"><span data-stu-id="4a9a1-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="4a9a1-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="4a9a1-119">startDateTime</span></span>|<span data-ttu-id="4a9a1-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4a9a1-120">DateTimeOffset</span></span>|<span data-ttu-id="4a9a1-121">操作启动的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="4a9a1-121">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="4a9a1-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="4a9a1-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="4a9a1-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4a9a1-123">DateTimeOffset</span></span>|<span data-ttu-id="4a9a1-124">操作状态上次更新的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="4a9a1-124">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="4a9a1-125">scanType</span><span class="sxs-lookup"><span data-stu-id="4a9a1-125">scanType</span></span>|<span data-ttu-id="4a9a1-126">String</span><span class="sxs-lookup"><span data-stu-id="4a9a1-126">String</span></span>|<span data-ttu-id="4a9a1-127">扫描类型（完全扫描或快速扫描）</span><span class="sxs-lookup"><span data-stu-id="4a9a1-127">Scan type either full scan or quick scan</span></span>|

## <a name="relationships"></a><span data-ttu-id="4a9a1-128">关系</span><span class="sxs-lookup"><span data-stu-id="4a9a1-128">Relationships</span></span>
<span data-ttu-id="4a9a1-129">无</span><span class="sxs-lookup"><span data-stu-id="4a9a1-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4a9a1-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4a9a1-130">JSON Representation</span></span>
<span data-ttu-id="4a9a1-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4a9a1-131">Here is a JSON representation of the resource.</span></span>
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




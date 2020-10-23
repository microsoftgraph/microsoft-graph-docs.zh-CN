---
title: windowsDefenderScanActionResult 资源类型
description: Windows Defender 最后扫描结果
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 221fee2c96170534a6c20c151b813497598f774f
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48727370"
---
# <a name="windowsdefenderscanactionresult-resource-type"></a><span data-ttu-id="90ba0-103">windowsDefenderScanActionResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="90ba0-103">windowsDefenderScanActionResult resource type</span></span>

<span data-ttu-id="90ba0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="90ba0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="90ba0-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="90ba0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="90ba0-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="90ba0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="90ba0-107">Windows Defender 最后扫描结果</span><span class="sxs-lookup"><span data-stu-id="90ba0-107">Windows Defender last scan result</span></span>


<span data-ttu-id="90ba0-108">继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="90ba0-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="90ba0-109">属性</span><span class="sxs-lookup"><span data-stu-id="90ba0-109">Properties</span></span>
|<span data-ttu-id="90ba0-110">属性</span><span class="sxs-lookup"><span data-stu-id="90ba0-110">Property</span></span>|<span data-ttu-id="90ba0-111">类型</span><span class="sxs-lookup"><span data-stu-id="90ba0-111">Type</span></span>|<span data-ttu-id="90ba0-112">说明</span><span class="sxs-lookup"><span data-stu-id="90ba0-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="90ba0-113">actionName</span><span class="sxs-lookup"><span data-stu-id="90ba0-113">actionName</span></span>|<span data-ttu-id="90ba0-114">String</span><span class="sxs-lookup"><span data-stu-id="90ba0-114">String</span></span>|<span data-ttu-id="90ba0-115">操作名称 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="90ba0-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="90ba0-116">actionState</span><span class="sxs-lookup"><span data-stu-id="90ba0-116">actionState</span></span>|[<span data-ttu-id="90ba0-117">actionState</span><span class="sxs-lookup"><span data-stu-id="90ba0-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="90ba0-118">继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)的操作的状态。</span><span class="sxs-lookup"><span data-stu-id="90ba0-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="90ba0-119">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed` 或 `notSupported`。</span><span class="sxs-lookup"><span data-stu-id="90ba0-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="90ba0-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="90ba0-120">startDateTime</span></span>|<span data-ttu-id="90ba0-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="90ba0-121">DateTimeOffset</span></span>|<span data-ttu-id="90ba0-122">操作启动的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="90ba0-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="90ba0-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="90ba0-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="90ba0-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="90ba0-124">DateTimeOffset</span></span>|<span data-ttu-id="90ba0-125">操作状态上次更新的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="90ba0-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="90ba0-126">scanType</span><span class="sxs-lookup"><span data-stu-id="90ba0-126">scanType</span></span>|<span data-ttu-id="90ba0-127">String</span><span class="sxs-lookup"><span data-stu-id="90ba0-127">String</span></span>|<span data-ttu-id="90ba0-128">扫描类型（完全扫描或快速扫描）</span><span class="sxs-lookup"><span data-stu-id="90ba0-128">Scan type either full scan or quick scan</span></span>|

## <a name="relationships"></a><span data-ttu-id="90ba0-129">关系</span><span class="sxs-lookup"><span data-stu-id="90ba0-129">Relationships</span></span>
<span data-ttu-id="90ba0-130">无</span><span class="sxs-lookup"><span data-stu-id="90ba0-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="90ba0-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="90ba0-131">JSON Representation</span></span>
<span data-ttu-id="90ba0-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="90ba0-132">Here is a JSON representation of the resource.</span></span>
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






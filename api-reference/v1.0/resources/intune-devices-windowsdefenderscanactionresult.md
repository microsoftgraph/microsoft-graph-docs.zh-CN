---
title: windowsDefenderScanActionResult 资源类型
description: Windows Defender 最后扫描结果
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0e9bcf4d45a184ea54a15bedc85efc6fc9bb4073
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36027403"
---
# <a name="windowsdefenderscanactionresult-resource-type"></a><span data-ttu-id="40a5b-103">windowsDefenderScanActionResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="40a5b-103">windowsDefenderScanActionResult resource type</span></span>

> <span data-ttu-id="40a5b-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="40a5b-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="40a5b-105">Windows Defender 最后扫描结果</span><span class="sxs-lookup"><span data-stu-id="40a5b-105">Windows Defender last scan result</span></span>


<span data-ttu-id="40a5b-106">继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="40a5b-106">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="40a5b-107">属性</span><span class="sxs-lookup"><span data-stu-id="40a5b-107">Properties</span></span>
|<span data-ttu-id="40a5b-108">属性</span><span class="sxs-lookup"><span data-stu-id="40a5b-108">Property</span></span>|<span data-ttu-id="40a5b-109">类型</span><span class="sxs-lookup"><span data-stu-id="40a5b-109">Type</span></span>|<span data-ttu-id="40a5b-110">说明</span><span class="sxs-lookup"><span data-stu-id="40a5b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="40a5b-111">actionName</span><span class="sxs-lookup"><span data-stu-id="40a5b-111">actionName</span></span>|<span data-ttu-id="40a5b-112">String</span><span class="sxs-lookup"><span data-stu-id="40a5b-112">String</span></span>|<span data-ttu-id="40a5b-113">操作名称 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="40a5b-113">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="40a5b-114">actionState</span><span class="sxs-lookup"><span data-stu-id="40a5b-114">actionState</span></span>|[<span data-ttu-id="40a5b-115">actionState</span><span class="sxs-lookup"><span data-stu-id="40a5b-115">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="40a5b-116">继承自[deviceActionResult](../resources/intune-devices-deviceactionresult.md)的操作的状态。</span><span class="sxs-lookup"><span data-stu-id="40a5b-116">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="40a5b-117">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed` 或 `notSupported`。</span><span class="sxs-lookup"><span data-stu-id="40a5b-117">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="40a5b-118">startDateTime</span><span class="sxs-lookup"><span data-stu-id="40a5b-118">startDateTime</span></span>|<span data-ttu-id="40a5b-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="40a5b-119">DateTimeOffset</span></span>|<span data-ttu-id="40a5b-120">操作启动的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="40a5b-120">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="40a5b-121">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="40a5b-121">lastUpdatedDateTime</span></span>|<span data-ttu-id="40a5b-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="40a5b-122">DateTimeOffset</span></span>|<span data-ttu-id="40a5b-123">操作状态上次更新的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="40a5b-123">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="40a5b-124">scanType</span><span class="sxs-lookup"><span data-stu-id="40a5b-124">scanType</span></span>|<span data-ttu-id="40a5b-125">String</span><span class="sxs-lookup"><span data-stu-id="40a5b-125">String</span></span>|<span data-ttu-id="40a5b-126">扫描类型（完全扫描或快速扫描）</span><span class="sxs-lookup"><span data-stu-id="40a5b-126">Scan type either full scan or quick scan</span></span>|

## <a name="relationships"></a><span data-ttu-id="40a5b-127">关系</span><span class="sxs-lookup"><span data-stu-id="40a5b-127">Relationships</span></span>
<span data-ttu-id="40a5b-128">无</span><span class="sxs-lookup"><span data-stu-id="40a5b-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="40a5b-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="40a5b-129">JSON Representation</span></span>
<span data-ttu-id="40a5b-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="40a5b-130">Here is a JSON representation of the resource.</span></span>
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




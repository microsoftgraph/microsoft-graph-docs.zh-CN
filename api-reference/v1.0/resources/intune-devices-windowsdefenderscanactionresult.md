---
title: windowsDefenderScanActionResult 资源类型
description: Windows Defender 最后扫描结果
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 407db79fa0caf333dfb092620320aeb339e1b195
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27812150"
---
# <a name="windowsdefenderscanactionresult-resource-type"></a><span data-ttu-id="d059b-103">windowsDefenderScanActionResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="d059b-103">windowsDefenderScanActionResult resource type</span></span>

> <span data-ttu-id="d059b-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="d059b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d059b-105">Windows Defender 最后扫描结果</span><span class="sxs-lookup"><span data-stu-id="d059b-105">Windows Defender last scan result</span></span>

<span data-ttu-id="d059b-106">继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="d059b-106">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d059b-107">属性</span><span class="sxs-lookup"><span data-stu-id="d059b-107">Properties</span></span>
|<span data-ttu-id="d059b-108">属性</span><span class="sxs-lookup"><span data-stu-id="d059b-108">Property</span></span>|<span data-ttu-id="d059b-109">类型</span><span class="sxs-lookup"><span data-stu-id="d059b-109">Type</span></span>|<span data-ttu-id="d059b-110">说明</span><span class="sxs-lookup"><span data-stu-id="d059b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d059b-111">actionName</span><span class="sxs-lookup"><span data-stu-id="d059b-111">actionName</span></span>|<span data-ttu-id="d059b-112">String</span><span class="sxs-lookup"><span data-stu-id="d059b-112">String</span></span>|<span data-ttu-id="d059b-113">操作名称 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="d059b-113">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="d059b-114">actionState</span><span class="sxs-lookup"><span data-stu-id="d059b-114">actionState</span></span>|[<span data-ttu-id="d059b-115">actionState</span><span class="sxs-lookup"><span data-stu-id="d059b-115">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="d059b-116">从[deviceActionResult](../resources/intune-devices-deviceactionresult.md)继承操作的状态。</span><span class="sxs-lookup"><span data-stu-id="d059b-116">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="d059b-117">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported`。</span><span class="sxs-lookup"><span data-stu-id="d059b-117">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="d059b-118">startDateTime</span><span class="sxs-lookup"><span data-stu-id="d059b-118">startDateTime</span></span>|<span data-ttu-id="d059b-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d059b-119">DateTimeOffset</span></span>|<span data-ttu-id="d059b-120">启动操作的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="d059b-120">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="d059b-121">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="d059b-121">lastUpdatedDateTime</span></span>|<span data-ttu-id="d059b-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d059b-122">DateTimeOffset</span></span>|<span data-ttu-id="d059b-123">操作状态上次更新的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="d059b-123">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="d059b-124">scanType</span><span class="sxs-lookup"><span data-stu-id="d059b-124">scanType</span></span>|<span data-ttu-id="d059b-125">String</span><span class="sxs-lookup"><span data-stu-id="d059b-125">String</span></span>|<span data-ttu-id="d059b-126">扫描类型（完全扫描或快速扫描）</span><span class="sxs-lookup"><span data-stu-id="d059b-126">Scan type either full scan or quick scan</span></span>|

## <a name="relationships"></a><span data-ttu-id="d059b-127">关系</span><span class="sxs-lookup"><span data-stu-id="d059b-127">Relationships</span></span>
<span data-ttu-id="d059b-128">无</span><span class="sxs-lookup"><span data-stu-id="d059b-128">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d059b-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d059b-129">JSON Representation</span></span>
<span data-ttu-id="d059b-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d059b-130">Here is a JSON representation of the resource.</span></span>
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




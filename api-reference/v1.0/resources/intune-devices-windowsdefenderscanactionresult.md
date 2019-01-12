---
title: windowsDefenderScanActionResult 资源类型
description: Windows Defender 最后扫描结果
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8a323b0438c7edf50d745b3b21498ad5c50f6424
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27911684"
---
# <a name="windowsdefenderscanactionresult-resource-type"></a><span data-ttu-id="4d8bf-103">windowsDefenderScanActionResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="4d8bf-103">windowsDefenderScanActionResult resource type</span></span>

> <span data-ttu-id="4d8bf-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="4d8bf-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4d8bf-105">Windows Defender 最后扫描结果</span><span class="sxs-lookup"><span data-stu-id="4d8bf-105">Windows Defender last scan result</span></span>

<span data-ttu-id="4d8bf-106">继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="4d8bf-106">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4d8bf-107">属性</span><span class="sxs-lookup"><span data-stu-id="4d8bf-107">Properties</span></span>
|<span data-ttu-id="4d8bf-108">属性</span><span class="sxs-lookup"><span data-stu-id="4d8bf-108">Property</span></span>|<span data-ttu-id="4d8bf-109">类型</span><span class="sxs-lookup"><span data-stu-id="4d8bf-109">Type</span></span>|<span data-ttu-id="4d8bf-110">说明</span><span class="sxs-lookup"><span data-stu-id="4d8bf-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4d8bf-111">actionName</span><span class="sxs-lookup"><span data-stu-id="4d8bf-111">actionName</span></span>|<span data-ttu-id="4d8bf-112">String</span><span class="sxs-lookup"><span data-stu-id="4d8bf-112">String</span></span>|<span data-ttu-id="4d8bf-113">操作名称 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="4d8bf-113">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="4d8bf-114">actionState</span><span class="sxs-lookup"><span data-stu-id="4d8bf-114">actionState</span></span>|[<span data-ttu-id="4d8bf-115">actionState</span><span class="sxs-lookup"><span data-stu-id="4d8bf-115">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="4d8bf-116">从[deviceActionResult](../resources/intune-devices-deviceactionresult.md)继承操作的状态。</span><span class="sxs-lookup"><span data-stu-id="4d8bf-116">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="4d8bf-117">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported`。</span><span class="sxs-lookup"><span data-stu-id="4d8bf-117">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="4d8bf-118">startDateTime</span><span class="sxs-lookup"><span data-stu-id="4d8bf-118">startDateTime</span></span>|<span data-ttu-id="4d8bf-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4d8bf-119">DateTimeOffset</span></span>|<span data-ttu-id="4d8bf-120">启动操作的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="4d8bf-120">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="4d8bf-121">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="4d8bf-121">lastUpdatedDateTime</span></span>|<span data-ttu-id="4d8bf-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4d8bf-122">DateTimeOffset</span></span>|<span data-ttu-id="4d8bf-123">操作状态上次更新的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="4d8bf-123">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="4d8bf-124">scanType</span><span class="sxs-lookup"><span data-stu-id="4d8bf-124">scanType</span></span>|<span data-ttu-id="4d8bf-125">String</span><span class="sxs-lookup"><span data-stu-id="4d8bf-125">String</span></span>|<span data-ttu-id="4d8bf-126">扫描类型（完全扫描或快速扫描）</span><span class="sxs-lookup"><span data-stu-id="4d8bf-126">Scan type either full scan or quick scan</span></span>|

## <a name="relationships"></a><span data-ttu-id="4d8bf-127">关系</span><span class="sxs-lookup"><span data-stu-id="4d8bf-127">Relationships</span></span>
<span data-ttu-id="4d8bf-128">无</span><span class="sxs-lookup"><span data-stu-id="4d8bf-128">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="4d8bf-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4d8bf-129">JSON Representation</span></span>
<span data-ttu-id="4d8bf-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4d8bf-130">Here is a JSON representation of the resource.</span></span>
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




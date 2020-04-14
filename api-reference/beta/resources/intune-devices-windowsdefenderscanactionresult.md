---
title: windowsDefenderScanActionResult 资源类型
description: Windows Defender 最后扫描结果
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 14ed1b41445625b6c460a1438df2b48e17c5e48a
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43401824"
---
# <a name="windowsdefenderscanactionresult-resource-type"></a><span data-ttu-id="105bd-103">windowsDefenderScanActionResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="105bd-103">windowsDefenderScanActionResult resource type</span></span>

<span data-ttu-id="105bd-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="105bd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="105bd-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="105bd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="105bd-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="105bd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="105bd-107">Windows Defender 最后扫描结果</span><span class="sxs-lookup"><span data-stu-id="105bd-107">Windows Defender last scan result</span></span>


<span data-ttu-id="105bd-108">继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="105bd-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="105bd-109">属性</span><span class="sxs-lookup"><span data-stu-id="105bd-109">Properties</span></span>
|<span data-ttu-id="105bd-110">属性</span><span class="sxs-lookup"><span data-stu-id="105bd-110">Property</span></span>|<span data-ttu-id="105bd-111">类型</span><span class="sxs-lookup"><span data-stu-id="105bd-111">Type</span></span>|<span data-ttu-id="105bd-112">说明</span><span class="sxs-lookup"><span data-stu-id="105bd-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="105bd-113">actionName</span><span class="sxs-lookup"><span data-stu-id="105bd-113">actionName</span></span>|<span data-ttu-id="105bd-114">字符串</span><span class="sxs-lookup"><span data-stu-id="105bd-114">String</span></span>|<span data-ttu-id="105bd-115">操作名称 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="105bd-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="105bd-116">actionState</span><span class="sxs-lookup"><span data-stu-id="105bd-116">actionState</span></span>|[<span data-ttu-id="105bd-117">actionState</span><span class="sxs-lookup"><span data-stu-id="105bd-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="105bd-118">继承自[deviceActionResult](../resources/intune-devices-deviceactionresult.md)的操作的状态。</span><span class="sxs-lookup"><span data-stu-id="105bd-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="105bd-119">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed` 或 `notSupported`。</span><span class="sxs-lookup"><span data-stu-id="105bd-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="105bd-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="105bd-120">startDateTime</span></span>|<span data-ttu-id="105bd-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="105bd-121">DateTimeOffset</span></span>|<span data-ttu-id="105bd-122">操作启动的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="105bd-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="105bd-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="105bd-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="105bd-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="105bd-124">DateTimeOffset</span></span>|<span data-ttu-id="105bd-125">操作状态上次更新的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="105bd-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="105bd-126">scanType</span><span class="sxs-lookup"><span data-stu-id="105bd-126">scanType</span></span>|<span data-ttu-id="105bd-127">String</span><span class="sxs-lookup"><span data-stu-id="105bd-127">String</span></span>|<span data-ttu-id="105bd-128">扫描类型（完全扫描或快速扫描）</span><span class="sxs-lookup"><span data-stu-id="105bd-128">Scan type either full scan or quick scan</span></span>|

## <a name="relationships"></a><span data-ttu-id="105bd-129">关系</span><span class="sxs-lookup"><span data-stu-id="105bd-129">Relationships</span></span>
<span data-ttu-id="105bd-130">无</span><span class="sxs-lookup"><span data-stu-id="105bd-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="105bd-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="105bd-131">JSON Representation</span></span>
<span data-ttu-id="105bd-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="105bd-132">Here is a JSON representation of the resource.</span></span>
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




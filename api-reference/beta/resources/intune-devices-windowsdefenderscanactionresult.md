---
title: windowsDefenderScanActionResult 资源类型
description: Windows Defender 最后扫描结果
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 1e26904504d882af0ed253b547709a29e075954c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42528434"
---
# <a name="windowsdefenderscanactionresult-resource-type"></a><span data-ttu-id="786cd-103">windowsDefenderScanActionResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="786cd-103">windowsDefenderScanActionResult resource type</span></span>

<span data-ttu-id="786cd-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="786cd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="786cd-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="786cd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="786cd-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="786cd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="786cd-107">Windows Defender 最后扫描结果</span><span class="sxs-lookup"><span data-stu-id="786cd-107">Windows Defender last scan result</span></span>


<span data-ttu-id="786cd-108">继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="786cd-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="786cd-109">属性</span><span class="sxs-lookup"><span data-stu-id="786cd-109">Properties</span></span>
|<span data-ttu-id="786cd-110">属性</span><span class="sxs-lookup"><span data-stu-id="786cd-110">Property</span></span>|<span data-ttu-id="786cd-111">类型</span><span class="sxs-lookup"><span data-stu-id="786cd-111">Type</span></span>|<span data-ttu-id="786cd-112">说明</span><span class="sxs-lookup"><span data-stu-id="786cd-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="786cd-113">actionName</span><span class="sxs-lookup"><span data-stu-id="786cd-113">actionName</span></span>|<span data-ttu-id="786cd-114">String</span><span class="sxs-lookup"><span data-stu-id="786cd-114">String</span></span>|<span data-ttu-id="786cd-115">操作名称 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="786cd-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="786cd-116">actionState</span><span class="sxs-lookup"><span data-stu-id="786cd-116">actionState</span></span>|[<span data-ttu-id="786cd-117">actionState</span><span class="sxs-lookup"><span data-stu-id="786cd-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="786cd-118">继承自[deviceActionResult](../resources/intune-devices-deviceactionresult.md)的操作的状态。</span><span class="sxs-lookup"><span data-stu-id="786cd-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="786cd-119">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed` 或 `notSupported`。</span><span class="sxs-lookup"><span data-stu-id="786cd-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="786cd-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="786cd-120">startDateTime</span></span>|<span data-ttu-id="786cd-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="786cd-121">DateTimeOffset</span></span>|<span data-ttu-id="786cd-122">操作启动的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="786cd-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="786cd-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="786cd-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="786cd-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="786cd-124">DateTimeOffset</span></span>|<span data-ttu-id="786cd-125">操作状态上次更新的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="786cd-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="786cd-126">scanType</span><span class="sxs-lookup"><span data-stu-id="786cd-126">scanType</span></span>|<span data-ttu-id="786cd-127">String</span><span class="sxs-lookup"><span data-stu-id="786cd-127">String</span></span>|<span data-ttu-id="786cd-128">扫描类型（完全扫描或快速扫描）</span><span class="sxs-lookup"><span data-stu-id="786cd-128">Scan type either full scan or quick scan</span></span>|

## <a name="relationships"></a><span data-ttu-id="786cd-129">关系</span><span class="sxs-lookup"><span data-stu-id="786cd-129">Relationships</span></span>
<span data-ttu-id="786cd-130">无</span><span class="sxs-lookup"><span data-stu-id="786cd-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="786cd-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="786cd-131">JSON Representation</span></span>
<span data-ttu-id="786cd-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="786cd-132">Here is a JSON representation of the resource.</span></span>
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




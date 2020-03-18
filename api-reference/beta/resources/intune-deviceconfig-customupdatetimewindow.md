---
title: customUpdateTimeWindow 资源类型
description: 自定义更新时间窗口
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f56cf571b24c2bcee52e82100f5c087772c336e5
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42795643"
---
# <a name="customupdatetimewindow-resource-type"></a><span data-ttu-id="2a20e-103">customUpdateTimeWindow 资源类型</span><span class="sxs-lookup"><span data-stu-id="2a20e-103">customUpdateTimeWindow resource type</span></span>

> <span data-ttu-id="2a20e-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2a20e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2a20e-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2a20e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2a20e-106">自定义更新时间窗口</span><span class="sxs-lookup"><span data-stu-id="2a20e-106">Custom update time window</span></span>

## <a name="properties"></a><span data-ttu-id="2a20e-107">属性</span><span class="sxs-lookup"><span data-stu-id="2a20e-107">Properties</span></span>
|<span data-ttu-id="2a20e-108">属性</span><span class="sxs-lookup"><span data-stu-id="2a20e-108">Property</span></span>|<span data-ttu-id="2a20e-109">类型</span><span class="sxs-lookup"><span data-stu-id="2a20e-109">Type</span></span>|<span data-ttu-id="2a20e-110">说明</span><span class="sxs-lookup"><span data-stu-id="2a20e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2a20e-111">startDay</span><span class="sxs-lookup"><span data-stu-id="2a20e-111">startDay</span></span>|[<span data-ttu-id="2a20e-112">dayOfWeek</span><span class="sxs-lookup"><span data-stu-id="2a20e-112">dayOfWeek</span></span>](../resources/intune-deviceconfig-dayofweek.md)|<span data-ttu-id="2a20e-113">时间范围的开始日期。</span><span class="sxs-lookup"><span data-stu-id="2a20e-113">Start day of the time window.</span></span> <span data-ttu-id="2a20e-114">可取值为：`sunday`、`monday`、`tuesday`、`wednesday`、`thursday`、`friday` 或 `saturday`。</span><span class="sxs-lookup"><span data-stu-id="2a20e-114">Possible values are: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="2a20e-115">endDay</span><span class="sxs-lookup"><span data-stu-id="2a20e-115">endDay</span></span>|[<span data-ttu-id="2a20e-116">dayOfWeek</span><span class="sxs-lookup"><span data-stu-id="2a20e-116">dayOfWeek</span></span>](../resources/intune-deviceconfig-dayofweek.md)|<span data-ttu-id="2a20e-117">时间范围的结束日期。</span><span class="sxs-lookup"><span data-stu-id="2a20e-117">End day of the time window.</span></span> <span data-ttu-id="2a20e-118">可取值为：`sunday`、`monday`、`tuesday`、`wednesday`、`thursday`、`friday` 或 `saturday`。</span><span class="sxs-lookup"><span data-stu-id="2a20e-118">Possible values are: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="2a20e-119">startTime</span><span class="sxs-lookup"><span data-stu-id="2a20e-119">startTime</span></span>|<span data-ttu-id="2a20e-120">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="2a20e-120">TimeOfDay</span></span>|<span data-ttu-id="2a20e-121">时间范围的开始时间</span><span class="sxs-lookup"><span data-stu-id="2a20e-121">Start time of the time window</span></span>|
|<span data-ttu-id="2a20e-122">endTime</span><span class="sxs-lookup"><span data-stu-id="2a20e-122">endTime</span></span>|<span data-ttu-id="2a20e-123">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="2a20e-123">TimeOfDay</span></span>|<span data-ttu-id="2a20e-124">时间范围的结束时间</span><span class="sxs-lookup"><span data-stu-id="2a20e-124">End time of the time window</span></span>|

## <a name="relationships"></a><span data-ttu-id="2a20e-125">关系</span><span class="sxs-lookup"><span data-stu-id="2a20e-125">Relationships</span></span>
<span data-ttu-id="2a20e-126">无</span><span class="sxs-lookup"><span data-stu-id="2a20e-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2a20e-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2a20e-127">JSON Representation</span></span>
<span data-ttu-id="2a20e-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2a20e-128">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.customUpdateTimeWindow"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.customUpdateTimeWindow",
  "startDay": "String",
  "endDay": "String",
  "startTime": "String (time of day)",
  "endTime": "String (time of day)"
}
```




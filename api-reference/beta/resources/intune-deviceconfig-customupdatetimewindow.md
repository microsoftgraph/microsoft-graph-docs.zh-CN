---
title: customUpdateTimeWindow 资源类型
description: 自定义更新时间窗口
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d412f568a48c4da7b41d56b44180ac5200961238
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/20/2020
ms.locfileid: "42160935"
---
# <a name="customupdatetimewindow-resource-type"></a><span data-ttu-id="fe309-103">customUpdateTimeWindow 资源类型</span><span class="sxs-lookup"><span data-stu-id="fe309-103">customUpdateTimeWindow resource type</span></span>

> <span data-ttu-id="fe309-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="fe309-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fe309-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fe309-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fe309-106">自定义更新时间窗口</span><span class="sxs-lookup"><span data-stu-id="fe309-106">Custom update time window</span></span>

## <a name="properties"></a><span data-ttu-id="fe309-107">属性</span><span class="sxs-lookup"><span data-stu-id="fe309-107">Properties</span></span>
|<span data-ttu-id="fe309-108">属性</span><span class="sxs-lookup"><span data-stu-id="fe309-108">Property</span></span>|<span data-ttu-id="fe309-109">类型</span><span class="sxs-lookup"><span data-stu-id="fe309-109">Type</span></span>|<span data-ttu-id="fe309-110">说明</span><span class="sxs-lookup"><span data-stu-id="fe309-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fe309-111">startDay</span><span class="sxs-lookup"><span data-stu-id="fe309-111">startDay</span></span>|[<span data-ttu-id="fe309-112">dayOfWeek</span><span class="sxs-lookup"><span data-stu-id="fe309-112">dayOfWeek</span></span>](../resources/intune-deviceconfig-dayofweek.md)|<span data-ttu-id="fe309-113">时间范围的开始日期。</span><span class="sxs-lookup"><span data-stu-id="fe309-113">Start day of the time window.</span></span> <span data-ttu-id="fe309-114">可取值为：`sunday`、`monday`、`tuesday`、`wednesday`、`thursday`、`friday` 或 `saturday`。</span><span class="sxs-lookup"><span data-stu-id="fe309-114">Possible values are: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="fe309-115">endDay</span><span class="sxs-lookup"><span data-stu-id="fe309-115">endDay</span></span>|[<span data-ttu-id="fe309-116">dayOfWeek</span><span class="sxs-lookup"><span data-stu-id="fe309-116">dayOfWeek</span></span>](../resources/intune-deviceconfig-dayofweek.md)|<span data-ttu-id="fe309-117">时间范围的结束日期。</span><span class="sxs-lookup"><span data-stu-id="fe309-117">End day of the time window.</span></span> <span data-ttu-id="fe309-118">可取值为：`sunday`、`monday`、`tuesday`、`wednesday`、`thursday`、`friday` 或 `saturday`。</span><span class="sxs-lookup"><span data-stu-id="fe309-118">Possible values are: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="fe309-119">startTime</span><span class="sxs-lookup"><span data-stu-id="fe309-119">startTime</span></span>|<span data-ttu-id="fe309-120">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="fe309-120">TimeOfDay</span></span>|<span data-ttu-id="fe309-121">时间范围的开始时间</span><span class="sxs-lookup"><span data-stu-id="fe309-121">Start time of the time window</span></span>|
|<span data-ttu-id="fe309-122">endTime</span><span class="sxs-lookup"><span data-stu-id="fe309-122">endTime</span></span>|<span data-ttu-id="fe309-123">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="fe309-123">TimeOfDay</span></span>|<span data-ttu-id="fe309-124">时间范围的结束时间</span><span class="sxs-lookup"><span data-stu-id="fe309-124">End time of the time window</span></span>|

## <a name="relationships"></a><span data-ttu-id="fe309-125">关系</span><span class="sxs-lookup"><span data-stu-id="fe309-125">Relationships</span></span>
<span data-ttu-id="fe309-126">无</span><span class="sxs-lookup"><span data-stu-id="fe309-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fe309-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fe309-127">JSON Representation</span></span>
<span data-ttu-id="fe309-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fe309-128">Here is a JSON representation of the resource.</span></span>
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




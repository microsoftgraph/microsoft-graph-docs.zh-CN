---
title: customUpdateTimeWindow 资源类型
description: 自定义更新时间窗口
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6aa5ac1dfe78f2eb05ddee236689a1707f87389f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42526931"
---
# <a name="customupdatetimewindow-resource-type"></a><span data-ttu-id="9fffb-103">customUpdateTimeWindow 资源类型</span><span class="sxs-lookup"><span data-stu-id="9fffb-103">customUpdateTimeWindow resource type</span></span>

<span data-ttu-id="9fffb-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="9fffb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9fffb-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9fffb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9fffb-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9fffb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9fffb-107">自定义更新时间窗口</span><span class="sxs-lookup"><span data-stu-id="9fffb-107">Custom update time window</span></span>

## <a name="properties"></a><span data-ttu-id="9fffb-108">属性</span><span class="sxs-lookup"><span data-stu-id="9fffb-108">Properties</span></span>
|<span data-ttu-id="9fffb-109">属性</span><span class="sxs-lookup"><span data-stu-id="9fffb-109">Property</span></span>|<span data-ttu-id="9fffb-110">类型</span><span class="sxs-lookup"><span data-stu-id="9fffb-110">Type</span></span>|<span data-ttu-id="9fffb-111">说明</span><span class="sxs-lookup"><span data-stu-id="9fffb-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9fffb-112">startDay</span><span class="sxs-lookup"><span data-stu-id="9fffb-112">startDay</span></span>|[<span data-ttu-id="9fffb-113">dayOfWeek</span><span class="sxs-lookup"><span data-stu-id="9fffb-113">dayOfWeek</span></span>](../resources/intune-deviceconfig-dayofweek.md)|<span data-ttu-id="9fffb-114">时间范围的开始日期。</span><span class="sxs-lookup"><span data-stu-id="9fffb-114">Start day of the time window.</span></span> <span data-ttu-id="9fffb-115">可取值为：`sunday`、`monday`、`tuesday`、`wednesday`、`thursday`、`friday` 或 `saturday`。</span><span class="sxs-lookup"><span data-stu-id="9fffb-115">Possible values are: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="9fffb-116">endDay</span><span class="sxs-lookup"><span data-stu-id="9fffb-116">endDay</span></span>|[<span data-ttu-id="9fffb-117">dayOfWeek</span><span class="sxs-lookup"><span data-stu-id="9fffb-117">dayOfWeek</span></span>](../resources/intune-deviceconfig-dayofweek.md)|<span data-ttu-id="9fffb-118">时间范围的结束日期。</span><span class="sxs-lookup"><span data-stu-id="9fffb-118">End day of the time window.</span></span> <span data-ttu-id="9fffb-119">可取值为：`sunday`、`monday`、`tuesday`、`wednesday`、`thursday`、`friday` 或 `saturday`。</span><span class="sxs-lookup"><span data-stu-id="9fffb-119">Possible values are: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="9fffb-120">startTime</span><span class="sxs-lookup"><span data-stu-id="9fffb-120">startTime</span></span>|<span data-ttu-id="9fffb-121">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="9fffb-121">TimeOfDay</span></span>|<span data-ttu-id="9fffb-122">时间范围的开始时间</span><span class="sxs-lookup"><span data-stu-id="9fffb-122">Start time of the time window</span></span>|
|<span data-ttu-id="9fffb-123">endTime</span><span class="sxs-lookup"><span data-stu-id="9fffb-123">endTime</span></span>|<span data-ttu-id="9fffb-124">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="9fffb-124">TimeOfDay</span></span>|<span data-ttu-id="9fffb-125">时间范围的结束时间</span><span class="sxs-lookup"><span data-stu-id="9fffb-125">End time of the time window</span></span>|

## <a name="relationships"></a><span data-ttu-id="9fffb-126">关系</span><span class="sxs-lookup"><span data-stu-id="9fffb-126">Relationships</span></span>
<span data-ttu-id="9fffb-127">无</span><span class="sxs-lookup"><span data-stu-id="9fffb-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9fffb-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9fffb-128">JSON Representation</span></span>
<span data-ttu-id="9fffb-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9fffb-129">Here is a JSON representation of the resource.</span></span>
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




---
title: customUpdateTimeWindow 资源类型
description: 自定义更新时间窗口
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6f46490aff53eea8e8e6436b85d2f11fd0ac086f
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49256711"
---
# <a name="customupdatetimewindow-resource-type"></a><span data-ttu-id="dc7b8-103">customUpdateTimeWindow 资源类型</span><span class="sxs-lookup"><span data-stu-id="dc7b8-103">customUpdateTimeWindow resource type</span></span>

<span data-ttu-id="dc7b8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dc7b8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dc7b8-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="dc7b8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dc7b8-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="dc7b8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dc7b8-107">自定义更新时间窗口</span><span class="sxs-lookup"><span data-stu-id="dc7b8-107">Custom update time window</span></span>

## <a name="properties"></a><span data-ttu-id="dc7b8-108">属性</span><span class="sxs-lookup"><span data-stu-id="dc7b8-108">Properties</span></span>
|<span data-ttu-id="dc7b8-109">属性</span><span class="sxs-lookup"><span data-stu-id="dc7b8-109">Property</span></span>|<span data-ttu-id="dc7b8-110">类型</span><span class="sxs-lookup"><span data-stu-id="dc7b8-110">Type</span></span>|<span data-ttu-id="dc7b8-111">描述</span><span class="sxs-lookup"><span data-stu-id="dc7b8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dc7b8-112">startDay</span><span class="sxs-lookup"><span data-stu-id="dc7b8-112">startDay</span></span>|[<span data-ttu-id="dc7b8-113">dayOfWeek</span><span class="sxs-lookup"><span data-stu-id="dc7b8-113">dayOfWeek</span></span>](../resources/intune-deviceconfig-dayofweek.md)|<span data-ttu-id="dc7b8-114">时间范围的开始日期。</span><span class="sxs-lookup"><span data-stu-id="dc7b8-114">Start day of the time window.</span></span> <span data-ttu-id="dc7b8-115">可取值为：`sunday`、`monday`、`tuesday`、`wednesday`、`thursday`、`friday` 或 `saturday`。</span><span class="sxs-lookup"><span data-stu-id="dc7b8-115">Possible values are: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="dc7b8-116">endDay</span><span class="sxs-lookup"><span data-stu-id="dc7b8-116">endDay</span></span>|[<span data-ttu-id="dc7b8-117">dayOfWeek</span><span class="sxs-lookup"><span data-stu-id="dc7b8-117">dayOfWeek</span></span>](../resources/intune-deviceconfig-dayofweek.md)|<span data-ttu-id="dc7b8-118">时间范围的结束日期。</span><span class="sxs-lookup"><span data-stu-id="dc7b8-118">End day of the time window.</span></span> <span data-ttu-id="dc7b8-119">可取值为：`sunday`、`monday`、`tuesday`、`wednesday`、`thursday`、`friday` 或 `saturday`。</span><span class="sxs-lookup"><span data-stu-id="dc7b8-119">Possible values are: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="dc7b8-120">startTime</span><span class="sxs-lookup"><span data-stu-id="dc7b8-120">startTime</span></span>|<span data-ttu-id="dc7b8-121">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="dc7b8-121">TimeOfDay</span></span>|<span data-ttu-id="dc7b8-122">时间范围的开始时间</span><span class="sxs-lookup"><span data-stu-id="dc7b8-122">Start time of the time window</span></span>|
|<span data-ttu-id="dc7b8-123">endTime</span><span class="sxs-lookup"><span data-stu-id="dc7b8-123">endTime</span></span>|<span data-ttu-id="dc7b8-124">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="dc7b8-124">TimeOfDay</span></span>|<span data-ttu-id="dc7b8-125">时间范围的结束时间</span><span class="sxs-lookup"><span data-stu-id="dc7b8-125">End time of the time window</span></span>|

## <a name="relationships"></a><span data-ttu-id="dc7b8-126">关系</span><span class="sxs-lookup"><span data-stu-id="dc7b8-126">Relationships</span></span>
<span data-ttu-id="dc7b8-127">无</span><span class="sxs-lookup"><span data-stu-id="dc7b8-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="dc7b8-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="dc7b8-128">JSON Representation</span></span>
<span data-ttu-id="dc7b8-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dc7b8-129">Here is a JSON representation of the resource.</span></span>
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





---
title: customUpdateTimeWindow 资源类型
description: 自定义更新时间窗口
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7392ba0eeb3af516682ff63f9f65fce94d08f0e9
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48729789"
---
# <a name="customupdatetimewindow-resource-type"></a><span data-ttu-id="a6bec-103">customUpdateTimeWindow 资源类型</span><span class="sxs-lookup"><span data-stu-id="a6bec-103">customUpdateTimeWindow resource type</span></span>

<span data-ttu-id="a6bec-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a6bec-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a6bec-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a6bec-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a6bec-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a6bec-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a6bec-107">自定义更新时间窗口</span><span class="sxs-lookup"><span data-stu-id="a6bec-107">Custom update time window</span></span>

## <a name="properties"></a><span data-ttu-id="a6bec-108">属性</span><span class="sxs-lookup"><span data-stu-id="a6bec-108">Properties</span></span>
|<span data-ttu-id="a6bec-109">属性</span><span class="sxs-lookup"><span data-stu-id="a6bec-109">Property</span></span>|<span data-ttu-id="a6bec-110">类型</span><span class="sxs-lookup"><span data-stu-id="a6bec-110">Type</span></span>|<span data-ttu-id="a6bec-111">说明</span><span class="sxs-lookup"><span data-stu-id="a6bec-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a6bec-112">startDay</span><span class="sxs-lookup"><span data-stu-id="a6bec-112">startDay</span></span>|[<span data-ttu-id="a6bec-113">dayOfWeek</span><span class="sxs-lookup"><span data-stu-id="a6bec-113">dayOfWeek</span></span>](../resources/intune-deviceconfig-dayofweek.md)|<span data-ttu-id="a6bec-114">时间范围的开始日期。</span><span class="sxs-lookup"><span data-stu-id="a6bec-114">Start day of the time window.</span></span> <span data-ttu-id="a6bec-115">可取值为：`sunday`、`monday`、`tuesday`、`wednesday`、`thursday`、`friday` 或 `saturday`。</span><span class="sxs-lookup"><span data-stu-id="a6bec-115">Possible values are: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="a6bec-116">endDay</span><span class="sxs-lookup"><span data-stu-id="a6bec-116">endDay</span></span>|[<span data-ttu-id="a6bec-117">dayOfWeek</span><span class="sxs-lookup"><span data-stu-id="a6bec-117">dayOfWeek</span></span>](../resources/intune-deviceconfig-dayofweek.md)|<span data-ttu-id="a6bec-118">时间范围的结束日期。</span><span class="sxs-lookup"><span data-stu-id="a6bec-118">End day of the time window.</span></span> <span data-ttu-id="a6bec-119">可取值为：`sunday`、`monday`、`tuesday`、`wednesday`、`thursday`、`friday` 或 `saturday`。</span><span class="sxs-lookup"><span data-stu-id="a6bec-119">Possible values are: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="a6bec-120">startTime</span><span class="sxs-lookup"><span data-stu-id="a6bec-120">startTime</span></span>|<span data-ttu-id="a6bec-121">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="a6bec-121">TimeOfDay</span></span>|<span data-ttu-id="a6bec-122">时间范围的开始时间</span><span class="sxs-lookup"><span data-stu-id="a6bec-122">Start time of the time window</span></span>|
|<span data-ttu-id="a6bec-123">endTime</span><span class="sxs-lookup"><span data-stu-id="a6bec-123">endTime</span></span>|<span data-ttu-id="a6bec-124">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="a6bec-124">TimeOfDay</span></span>|<span data-ttu-id="a6bec-125">时间范围的结束时间</span><span class="sxs-lookup"><span data-stu-id="a6bec-125">End time of the time window</span></span>|

## <a name="relationships"></a><span data-ttu-id="a6bec-126">关系</span><span class="sxs-lookup"><span data-stu-id="a6bec-126">Relationships</span></span>
<span data-ttu-id="a6bec-127">无</span><span class="sxs-lookup"><span data-stu-id="a6bec-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a6bec-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a6bec-128">JSON Representation</span></span>
<span data-ttu-id="a6bec-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a6bec-129">Here is a JSON representation of the resource.</span></span>
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






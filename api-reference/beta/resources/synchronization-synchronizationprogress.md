---
title: synchronizationProgress 资源类型
description: 表示 synchronizationJob 的进度向完成。
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: c9a9ea8b5bd9d2a0fbfbcb1a64381b46e2f96283
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/10/2020
ms.locfileid: "43217400"
---
# <a name="synchronizationprogress-resource-type"></a><span data-ttu-id="2ffbe-103">synchronizationProgress 资源类型</span><span class="sxs-lookup"><span data-stu-id="2ffbe-103">synchronizationProgress resource type</span></span>

<span data-ttu-id="2ffbe-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2ffbe-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2ffbe-105">表示[synchronizationJob](synchronization-synchronizationjob.md)的进度向完成。</span><span class="sxs-lookup"><span data-stu-id="2ffbe-105">Represents the progress of a [synchronizationJob](synchronization-synchronizationjob.md) toward completion.</span></span>

## <a name="properties"></a><span data-ttu-id="2ffbe-106">属性</span><span class="sxs-lookup"><span data-stu-id="2ffbe-106">Properties</span></span>

| <span data-ttu-id="2ffbe-107">属性</span><span class="sxs-lookup"><span data-stu-id="2ffbe-107">Property</span></span>                              | <span data-ttu-id="2ffbe-108">类型</span><span class="sxs-lookup"><span data-stu-id="2ffbe-108">Type</span></span>      | <span data-ttu-id="2ffbe-109">Description</span><span class="sxs-lookup"><span data-stu-id="2ffbe-109">Description</span></span>    |
|:--------------------------------------|:----------|:---------------|
|<span data-ttu-id="2ffbe-110">completedUnits</span><span class="sxs-lookup"><span data-stu-id="2ffbe-110">completedUnits</span></span>|<span data-ttu-id="2ffbe-111">Int32</span><span class="sxs-lookup"><span data-stu-id="2ffbe-111">Int32</span></span>|<span data-ttu-id="2ffbe-112">进度比率的分子;已处理的更改的单位数。</span><span class="sxs-lookup"><span data-stu-id="2ffbe-112">The numerator of a progress ratio; the number of units of changes already processed.</span></span>|
|<span data-ttu-id="2ffbe-113">progressObservationDateTime</span><span class="sxs-lookup"><span data-stu-id="2ffbe-113">progressObservationDateTime</span></span>|<span data-ttu-id="2ffbe-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2ffbe-114">DateTimeOffset</span></span>|<span data-ttu-id="2ffbe-115">进度观察的时间，作为从 UTC 的偏移量（以分钟为单位）。</span><span class="sxs-lookup"><span data-stu-id="2ffbe-115">The time of a progress observation as an offset in minutes from UTC.</span></span>|
|<span data-ttu-id="2ffbe-116">totalUnits</span><span class="sxs-lookup"><span data-stu-id="2ffbe-116">totalUnits</span></span>|<span data-ttu-id="2ffbe-117">Int32</span><span class="sxs-lookup"><span data-stu-id="2ffbe-117">Int32</span></span>|<span data-ttu-id="2ffbe-118">进度比率的分母;要处理的用于完成同步的更改的多个单元。</span><span class="sxs-lookup"><span data-stu-id="2ffbe-118">The denominator of a progress ratio; a number of units of changes to be processed to accomplish synchronization.</span></span>|
|<span data-ttu-id="2ffbe-119">units</span><span class="sxs-lookup"><span data-stu-id="2ffbe-119">units</span></span>|<span data-ttu-id="2ffbe-120">字符串</span><span class="sxs-lookup"><span data-stu-id="2ffbe-120">String</span></span>|<span data-ttu-id="2ffbe-121">单位的可选说明。</span><span class="sxs-lookup"><span data-stu-id="2ffbe-121">An optional description of the units.</span></span>|

<!-- The troubleshootingUrl property is missing a description -->

## <a name="json-representation"></a><span data-ttu-id="2ffbe-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2ffbe-122">JSON representation</span></span>

<span data-ttu-id="2ffbe-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2ffbe-123">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationProgress"
}-->

```json
{
  "completedUnits": 1025,
  "progressObservationDateTime": "2017-10-10T17:00:00Z",
  "totalUnits": 3024,
  "units": "pages"
}

```

<!-- uuid: 15571993-7e2f-4842-84d5-01ceb67cdc05
20185-08-14 22:30:00 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationProcess resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

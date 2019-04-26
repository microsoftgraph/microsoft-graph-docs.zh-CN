---
title: synchronizationProgress 资源类型
description: 表示 synchronizationJob 的进度向完成。
localization_priority: Normal
ms.openlocfilehash: d05193c7c242dc3f890aba6f4fcec5a8badc087f
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340006"
---
# <a name="synchronizationprogress-resource-type"></a><span data-ttu-id="17e4d-103">synchronizationProgress 资源类型</span><span class="sxs-lookup"><span data-stu-id="17e4d-103">synchronizationProgress resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="17e4d-104">表示[synchronizationJob](synchronization-synchronizationjob.md)的进度向完成。</span><span class="sxs-lookup"><span data-stu-id="17e4d-104">Represents the progress of a [synchronizationJob](synchronization-synchronizationjob.md) toward completion.</span></span>

## <a name="properties"></a><span data-ttu-id="17e4d-105">属性</span><span class="sxs-lookup"><span data-stu-id="17e4d-105">Properties</span></span>

| <span data-ttu-id="17e4d-106">属性</span><span class="sxs-lookup"><span data-stu-id="17e4d-106">Property</span></span>                              | <span data-ttu-id="17e4d-107">类型</span><span class="sxs-lookup"><span data-stu-id="17e4d-107">Type</span></span>      | <span data-ttu-id="17e4d-108">说明</span><span class="sxs-lookup"><span data-stu-id="17e4d-108">Description</span></span>    |
|:--------------------------------------|:----------|:---------------|
|<span data-ttu-id="17e4d-109">completedUnits</span><span class="sxs-lookup"><span data-stu-id="17e4d-109">completedUnits</span></span>|<span data-ttu-id="17e4d-110">Int32</span><span class="sxs-lookup"><span data-stu-id="17e4d-110">Int32</span></span>|<span data-ttu-id="17e4d-111">进度比率的分子;已处理的更改的单位数。</span><span class="sxs-lookup"><span data-stu-id="17e4d-111">The numerator of a progress ratio; the number of units of changes already processed.</span></span>|
|<span data-ttu-id="17e4d-112">progressObservationDateTime</span><span class="sxs-lookup"><span data-stu-id="17e4d-112">progressObservationDateTime</span></span>|<span data-ttu-id="17e4d-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="17e4d-113">DateTimeOffset</span></span>|<span data-ttu-id="17e4d-114">进度观察的时间, 作为从 UTC 的偏移量 (以分钟为单位)。</span><span class="sxs-lookup"><span data-stu-id="17e4d-114">The time of a progress observation as an offset in minutes from UTC.</span></span>|
|<span data-ttu-id="17e4d-115">totalUnits</span><span class="sxs-lookup"><span data-stu-id="17e4d-115">totalUnits</span></span>|<span data-ttu-id="17e4d-116">Int32</span><span class="sxs-lookup"><span data-stu-id="17e4d-116">Int32</span></span>|<span data-ttu-id="17e4d-117">进度比率的分母;要处理的用于完成同步的更改的多个单元。</span><span class="sxs-lookup"><span data-stu-id="17e4d-117">The denominator of a progress ratio; a number of units of changes to be processed to accomplish synchronization.</span></span>|
|<span data-ttu-id="17e4d-118">units</span><span class="sxs-lookup"><span data-stu-id="17e4d-118">units</span></span>|<span data-ttu-id="17e4d-119">String</span><span class="sxs-lookup"><span data-stu-id="17e4d-119">String</span></span>|<span data-ttu-id="17e4d-120">单位的可选说明。</span><span class="sxs-lookup"><span data-stu-id="17e4d-120">An optional description of the units.</span></span>|

<!-- The troubleshootingUrl property is missing a description -->

## <a name="json-representation"></a><span data-ttu-id="17e4d-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="17e4d-121">JSON representation</span></span>

<span data-ttu-id="17e4d-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="17e4d-122">The following is a JSON representation of the resource.</span></span>

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

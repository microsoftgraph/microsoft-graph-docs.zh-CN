---
title: synchronizationProgress 资源类型
description: 表示 synchronizationJob 的进度向完成。
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: dd1292d34abdc745075e030609d3f28a17b2431a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964639"
---
# <a name="synchronizationprogress-resource-type"></a><span data-ttu-id="40c14-103">synchronizationProgress 资源类型</span><span class="sxs-lookup"><span data-stu-id="40c14-103">synchronizationProgress resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="40c14-104">表示[synchronizationJob](synchronization-synchronizationjob.md)的进度向完成。</span><span class="sxs-lookup"><span data-stu-id="40c14-104">Represents the progress of a [synchronizationJob](synchronization-synchronizationjob.md) toward completion.</span></span>

## <a name="properties"></a><span data-ttu-id="40c14-105">属性</span><span class="sxs-lookup"><span data-stu-id="40c14-105">Properties</span></span>

| <span data-ttu-id="40c14-106">属性</span><span class="sxs-lookup"><span data-stu-id="40c14-106">Property</span></span>                              | <span data-ttu-id="40c14-107">类型</span><span class="sxs-lookup"><span data-stu-id="40c14-107">Type</span></span>      | <span data-ttu-id="40c14-108">说明</span><span class="sxs-lookup"><span data-stu-id="40c14-108">Description</span></span>    |
|:--------------------------------------|:----------|:---------------|
|<span data-ttu-id="40c14-109">completedUnits</span><span class="sxs-lookup"><span data-stu-id="40c14-109">completedUnits</span></span>|<span data-ttu-id="40c14-110">Int32</span><span class="sxs-lookup"><span data-stu-id="40c14-110">Int32</span></span>|<span data-ttu-id="40c14-111">进度比率的分子;已处理的更改的单位数。</span><span class="sxs-lookup"><span data-stu-id="40c14-111">The numerator of a progress ratio; the number of units of changes already processed.</span></span>|
|<span data-ttu-id="40c14-112">progressObservationDateTime</span><span class="sxs-lookup"><span data-stu-id="40c14-112">progressObservationDateTime</span></span>|<span data-ttu-id="40c14-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="40c14-113">DateTimeOffset</span></span>|<span data-ttu-id="40c14-114">进度观察的时间, 作为从 UTC 的偏移量 (以分钟为单位)。</span><span class="sxs-lookup"><span data-stu-id="40c14-114">The time of a progress observation as an offset in minutes from UTC.</span></span>|
|<span data-ttu-id="40c14-115">totalUnits</span><span class="sxs-lookup"><span data-stu-id="40c14-115">totalUnits</span></span>|<span data-ttu-id="40c14-116">Int32</span><span class="sxs-lookup"><span data-stu-id="40c14-116">Int32</span></span>|<span data-ttu-id="40c14-117">进度比率的分母;要处理的用于完成同步的更改的多个单元。</span><span class="sxs-lookup"><span data-stu-id="40c14-117">The denominator of a progress ratio; a number of units of changes to be processed to accomplish synchronization.</span></span>|
|<span data-ttu-id="40c14-118">units</span><span class="sxs-lookup"><span data-stu-id="40c14-118">units</span></span>|<span data-ttu-id="40c14-119">String</span><span class="sxs-lookup"><span data-stu-id="40c14-119">String</span></span>|<span data-ttu-id="40c14-120">单位的可选说明。</span><span class="sxs-lookup"><span data-stu-id="40c14-120">An optional description of the units.</span></span>|

<!-- The troubleshootingUrl property is missing a description -->

## <a name="json-representation"></a><span data-ttu-id="40c14-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="40c14-121">JSON representation</span></span>

<span data-ttu-id="40c14-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="40c14-122">The following is a JSON representation of the resource.</span></span>

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

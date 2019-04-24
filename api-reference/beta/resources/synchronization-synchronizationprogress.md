---
title: synchronizationProgress 资源类型
description: 表示 synchronizationJob 的进度向完成。
localization_priority: Normal
ms.openlocfilehash: b22bd95f54a9f268524dc98a8d3df94fcc14f773
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32453955"
---
# <a name="synchronizationprogress-resource-type"></a><span data-ttu-id="bfeae-103">synchronizationProgress 资源类型</span><span class="sxs-lookup"><span data-stu-id="bfeae-103">synchronizationProgress resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bfeae-104">表示[synchronizationJob](synchronization-synchronizationjob.md)的进度向完成。</span><span class="sxs-lookup"><span data-stu-id="bfeae-104">Represents the progress of a [synchronizationJob](synchronization-synchronizationjob.md) toward completion.</span></span>

## <a name="properties"></a><span data-ttu-id="bfeae-105">属性</span><span class="sxs-lookup"><span data-stu-id="bfeae-105">Properties</span></span>

| <span data-ttu-id="bfeae-106">属性</span><span class="sxs-lookup"><span data-stu-id="bfeae-106">Property</span></span>                              | <span data-ttu-id="bfeae-107">类型</span><span class="sxs-lookup"><span data-stu-id="bfeae-107">Type</span></span>      | <span data-ttu-id="bfeae-108">描述</span><span class="sxs-lookup"><span data-stu-id="bfeae-108">Description</span></span>    |
|:--------------------------------------|:----------|:---------------|
|<span data-ttu-id="bfeae-109">completedUnits</span><span class="sxs-lookup"><span data-stu-id="bfeae-109">completedUnits</span></span>|<span data-ttu-id="bfeae-110">Int32</span><span class="sxs-lookup"><span data-stu-id="bfeae-110">Int32</span></span>|<span data-ttu-id="bfeae-111">进度比率的分子;已处理的更改的单位数。</span><span class="sxs-lookup"><span data-stu-id="bfeae-111">The numerator of a progress ratio; the number of units of changes already processed.</span></span>|
|<span data-ttu-id="bfeae-112">progressObservationDateTime</span><span class="sxs-lookup"><span data-stu-id="bfeae-112">progressObservationDateTime</span></span>|<span data-ttu-id="bfeae-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bfeae-113">DateTimeOffset</span></span>|<span data-ttu-id="bfeae-114">进度观察的时间, 作为从 UTC 的偏移量 (以分钟为单位)。</span><span class="sxs-lookup"><span data-stu-id="bfeae-114">The time of a progress observation as an offset in minutes from UTC.</span></span>|
|<span data-ttu-id="bfeae-115">totalUnits</span><span class="sxs-lookup"><span data-stu-id="bfeae-115">totalUnits</span></span>|<span data-ttu-id="bfeae-116">Int32</span><span class="sxs-lookup"><span data-stu-id="bfeae-116">Int32</span></span>|<span data-ttu-id="bfeae-117">进度比率的分母;要处理的用于完成同步的更改的多个单元。</span><span class="sxs-lookup"><span data-stu-id="bfeae-117">The denominator of a progress ratio; a number of units of changes to be processed to accomplish synchronization.</span></span>|
|<span data-ttu-id="bfeae-118">units</span><span class="sxs-lookup"><span data-stu-id="bfeae-118">units</span></span>|<span data-ttu-id="bfeae-119">字符串</span><span class="sxs-lookup"><span data-stu-id="bfeae-119">String</span></span>|<span data-ttu-id="bfeae-120">单位的可选说明。</span><span class="sxs-lookup"><span data-stu-id="bfeae-120">An optional description of the units.</span></span>|

<!-- The troubleshootingUrl property is missing a description -->

## <a name="json-representation"></a><span data-ttu-id="bfeae-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bfeae-121">JSON representation</span></span>

<span data-ttu-id="bfeae-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bfeae-122">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationStatus"
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
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-synchronizationprogress.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

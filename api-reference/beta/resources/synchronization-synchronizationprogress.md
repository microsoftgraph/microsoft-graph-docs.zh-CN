---
title: synchronizationProgress 资源类型
description: 代表完成 synchronizationJob 的进度。
localization_priority: Normal
ms.openlocfilehash: b22bd95f54a9f268524dc98a8d3df94fcc14f773
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510972"
---
# <a name="synchronizationprogress-resource-type"></a><span data-ttu-id="fee1c-103">synchronizationProgress 资源类型</span><span class="sxs-lookup"><span data-stu-id="fee1c-103">synchronizationProgress resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fee1c-104">代表完成[synchronizationJob](synchronization-synchronizationjob.md)的进度。</span><span class="sxs-lookup"><span data-stu-id="fee1c-104">Represents the progress of a [synchronizationJob](synchronization-synchronizationjob.md) toward completion.</span></span>

## <a name="properties"></a><span data-ttu-id="fee1c-105">属性</span><span class="sxs-lookup"><span data-stu-id="fee1c-105">Properties</span></span>

| <span data-ttu-id="fee1c-106">属性</span><span class="sxs-lookup"><span data-stu-id="fee1c-106">Property</span></span>                              | <span data-ttu-id="fee1c-107">类型</span><span class="sxs-lookup"><span data-stu-id="fee1c-107">Type</span></span>      | <span data-ttu-id="fee1c-108">说明</span><span class="sxs-lookup"><span data-stu-id="fee1c-108">Description</span></span>    |
|:--------------------------------------|:----------|:---------------|
|<span data-ttu-id="fee1c-109">completedUnits</span><span class="sxs-lookup"><span data-stu-id="fee1c-109">completedUnits</span></span>|<span data-ttu-id="fee1c-110">Int32</span><span class="sxs-lookup"><span data-stu-id="fee1c-110">Int32</span></span>|<span data-ttu-id="fee1c-111">进度比例; 分子已处理的更改的单位数。</span><span class="sxs-lookup"><span data-stu-id="fee1c-111">The numerator of a progress ratio; the number of units of changes already processed.</span></span>|
|<span data-ttu-id="fee1c-112">progressObservationDateTime</span><span class="sxs-lookup"><span data-stu-id="fee1c-112">progressObservationDateTime</span></span>|<span data-ttu-id="fee1c-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fee1c-113">DateTimeOffset</span></span>|<span data-ttu-id="fee1c-114">进度观察值作为偏移量，以分钟为单位从 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="fee1c-114">The time of a progress observation as an offset in minutes from UTC.</span></span>|
|<span data-ttu-id="fee1c-115">totalUnits</span><span class="sxs-lookup"><span data-stu-id="fee1c-115">totalUnits</span></span>|<span data-ttu-id="fee1c-116">Int32</span><span class="sxs-lookup"><span data-stu-id="fee1c-116">Int32</span></span>|<span data-ttu-id="fee1c-117">进度比例; 分母处理以完成同步更改的单位数。</span><span class="sxs-lookup"><span data-stu-id="fee1c-117">The denominator of a progress ratio; a number of units of changes to be processed to accomplish synchronization.</span></span>|
|<span data-ttu-id="fee1c-118">Units</span><span class="sxs-lookup"><span data-stu-id="fee1c-118">units</span></span>|<span data-ttu-id="fee1c-119">String</span><span class="sxs-lookup"><span data-stu-id="fee1c-119">String</span></span>|<span data-ttu-id="fee1c-120">单位的可选说明。</span><span class="sxs-lookup"><span data-stu-id="fee1c-120">An optional description of the units.</span></span>|

<!-- The troubleshootingUrl property is missing a description -->

## <a name="json-representation"></a><span data-ttu-id="fee1c-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fee1c-121">JSON representation</span></span>

<span data-ttu-id="fee1c-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fee1c-122">The following is a JSON representation of the resource.</span></span>

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

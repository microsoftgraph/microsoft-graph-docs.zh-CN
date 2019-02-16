---
title: attendeeAvailabilityDataModel 资源类型
description: 与会者的类型和忙/闲状态。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 6d7436a640b4aaba0a9b71ef62ee91b3fe0d7cee
ms.sourcegitcommit: 539ed08adf3b7ad3253c98636d4ab303ce00176e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/15/2019
ms.locfileid: "30057346"
---
# <a name="attendeeavailabilitydatamodel-resource-type"></a><span data-ttu-id="69d39-103">attendeeAvailabilityDataModel 资源类型</span><span class="sxs-lookup"><span data-stu-id="69d39-103">attendeeAvailabilityDataModel resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="69d39-104">表示人员或资源及其在会议中的可用性。</span><span class="sxs-lookup"><span data-stu-id="69d39-104">Represents a person or resource and their availability for a meeting.</span></span>

## <a name="json-representation"></a><span data-ttu-id="69d39-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="69d39-105">JSON representation</span></span>

<span data-ttu-id="69d39-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="69d39-106">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attendeeAvailabilityDataModel"
}-->

```json
{
  "attendee": {"@odata.type": "microsoft.graph.attendeeDataModel"},
  "availability": "String"
}

```
## <a name="properties"></a><span data-ttu-id="69d39-107">属性</span><span class="sxs-lookup"><span data-stu-id="69d39-107">Properties</span></span>
| <span data-ttu-id="69d39-108">属性</span><span class="sxs-lookup"><span data-stu-id="69d39-108">Property</span></span>     | <span data-ttu-id="69d39-109">类型</span><span class="sxs-lookup"><span data-stu-id="69d39-109">Type</span></span>   |<span data-ttu-id="69d39-110">说明</span><span class="sxs-lookup"><span data-stu-id="69d39-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="69d39-111">attendee</span><span class="sxs-lookup"><span data-stu-id="69d39-111">attendee</span></span>|[<span data-ttu-id="69d39-112">attendeeDataModel</span><span class="sxs-lookup"><span data-stu-id="69d39-112">attendeeDataModel</span></span>](attendeedatamodel.md)|<span data-ttu-id="69d39-113">代表人员或资源参与者以及与会者是会议所必需的还是可选的。</span><span class="sxs-lookup"><span data-stu-id="69d39-113">Represents a person or resource attendee and whether the attendee is required or optional for the meeting.</span></span>|
|<span data-ttu-id="69d39-114">availability</span><span class="sxs-lookup"><span data-stu-id="69d39-114">availability</span></span>|<span data-ttu-id="69d39-115">availabilityStatus</span><span class="sxs-lookup"><span data-stu-id="69d39-115">availabilityStatus</span></span>| <span data-ttu-id="69d39-116">与会者的可用性状态。</span><span class="sxs-lookup"><span data-stu-id="69d39-116">The availability status of the attendee.</span></span> <span data-ttu-id="69d39-117">可能的值为: `free`、 `tentative`、 `busy` `oof`、、 `workingElsewhere`、 `unknown`。</span><span class="sxs-lookup"><span data-stu-id="69d39-117">The possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "attendeeAvailabilityDataModel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/attendeeavailabilitydatamodel.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
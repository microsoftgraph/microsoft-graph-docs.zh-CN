---
title: attendeeAvailability 资源类型
description: 与会者的类型和忙/闲状态。
localization_priority: Normal
ms.openlocfilehash: f831a88a14fc6ec970332208389e15a5adc49377
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/30/2019
ms.locfileid: "29640488"
---
# <a name="attendeeavailability-resource-type"></a><span data-ttu-id="62d15-103">attendeeAvailability 资源类型</span><span class="sxs-lookup"><span data-stu-id="62d15-103">attendeeAvailability resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="62d15-104">与会者的类型和忙/闲状态。</span><span class="sxs-lookup"><span data-stu-id="62d15-104">The type and availability of an attendee.</span></span>

## <a name="json-representation"></a><span data-ttu-id="62d15-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="62d15-105">JSON representation</span></span>

<span data-ttu-id="62d15-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="62d15-106">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attendeeAvailability"
}-->

```json
{
  "attendee": {"@odata.type": "microsoft.graph.attendeeBase"},
  "availability": "String"
}

```
## <a name="properties"></a><span data-ttu-id="62d15-107">属性</span><span class="sxs-lookup"><span data-stu-id="62d15-107">Properties</span></span>
| <span data-ttu-id="62d15-108">属性</span><span class="sxs-lookup"><span data-stu-id="62d15-108">Property</span></span>     | <span data-ttu-id="62d15-109">类型</span><span class="sxs-lookup"><span data-stu-id="62d15-109">Type</span></span>   |<span data-ttu-id="62d15-110">说明</span><span class="sxs-lookup"><span data-stu-id="62d15-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="62d15-111">attendee</span><span class="sxs-lookup"><span data-stu-id="62d15-111">attendee</span></span>|[<span data-ttu-id="62d15-112">AttendeeBase</span><span class="sxs-lookup"><span data-stu-id="62d15-112">AttendeeBase</span></span>](attendeebase.md)|<span data-ttu-id="62d15-113">与会者类型，即是人员还是资源；如果是人员，是必需还是可选。</span><span class="sxs-lookup"><span data-stu-id="62d15-113">The type of attendee - whether it's a person or a resource, and whether required or optional if it's a person.</span></span>|
|<span data-ttu-id="62d15-114">availability</span><span class="sxs-lookup"><span data-stu-id="62d15-114">availability</span></span>|<span data-ttu-id="62d15-115">String</span><span class="sxs-lookup"><span data-stu-id="62d15-115">String</span></span>| <span data-ttu-id="62d15-p101">与会者的忙/闲状态。可取值为：`free`、`tentative`、`busy`、`oof`、`workingElsewhere`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="62d15-p101">The availability status of the attendee. Possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "attendeeAvailability resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/attendeeavailability.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

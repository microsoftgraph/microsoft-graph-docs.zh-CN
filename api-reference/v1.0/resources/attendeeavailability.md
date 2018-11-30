---
title: attendeeAvailability 资源类型
description: 与会者的类型和忙/闲状态。
ms.openlocfilehash: 446dfb77d8f85021f41795038c3c1d597c6f1a6d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27008451"
---
# <a name="attendeeavailability-resource-type"></a><span data-ttu-id="608c7-103">attendeeAvailability 资源类型</span><span class="sxs-lookup"><span data-stu-id="608c7-103">attendeeAvailability resource type</span></span>

<span data-ttu-id="608c7-104">与会者的类型和忙/闲状态。</span><span class="sxs-lookup"><span data-stu-id="608c7-104">The type and availability of an attendee.</span></span>

## <a name="json-representation"></a><span data-ttu-id="608c7-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="608c7-105">JSON representation</span></span>

<span data-ttu-id="608c7-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="608c7-106">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="608c7-107">属性</span><span class="sxs-lookup"><span data-stu-id="608c7-107">Properties</span></span>
| <span data-ttu-id="608c7-108">属性</span><span class="sxs-lookup"><span data-stu-id="608c7-108">Property</span></span>     | <span data-ttu-id="608c7-109">类型</span><span class="sxs-lookup"><span data-stu-id="608c7-109">Type</span></span>   |<span data-ttu-id="608c7-110">说明</span><span class="sxs-lookup"><span data-stu-id="608c7-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="608c7-111">attendee</span><span class="sxs-lookup"><span data-stu-id="608c7-111">attendee</span></span>|[<span data-ttu-id="608c7-112">AttendeeBase</span><span class="sxs-lookup"><span data-stu-id="608c7-112">AttendeeBase</span></span>](attendeebase.md)|<span data-ttu-id="608c7-113">与会者类型，即是人员还是资源；如果是人员，是必需还是可选。</span><span class="sxs-lookup"><span data-stu-id="608c7-113">The type of attendee - whether it's a person or a resource, and whether required or optional if it's a person.</span></span>|
|<span data-ttu-id="608c7-114">availability</span><span class="sxs-lookup"><span data-stu-id="608c7-114">availability</span></span>|<span data-ttu-id="608c7-115">freeBusyStatus</span><span class="sxs-lookup"><span data-stu-id="608c7-115">freeBusyStatus</span></span>| <span data-ttu-id="608c7-116">可用性的与会者的状态。</span><span class="sxs-lookup"><span data-stu-id="608c7-116">The availability status of the attendee.</span></span> <span data-ttu-id="608c7-117">可能的值为： `free`， `tentative`， `busy`， `oof`， `workingElsewhere`， `unknown`。</span><span class="sxs-lookup"><span data-stu-id="608c7-117">The possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "attendeeAvailability resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

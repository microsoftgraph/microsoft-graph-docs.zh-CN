---
title: attendeeAvailability 资源类型
description: 与会者的可用性。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 396c53b8d03f573c214dcf43a3637cf06f412a33
ms.sourcegitcommit: a90abf5b89dbbdfefb1b7794d1f12c6e2bfb0cda
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/28/2019
ms.locfileid: "30937766"
---
# <a name="attendeeavailability-resource-type"></a><span data-ttu-id="94d98-103">attendeeAvailability 资源类型</span><span class="sxs-lookup"><span data-stu-id="94d98-103">attendeeAvailability resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="94d98-104">与会者的可用性。</span><span class="sxs-lookup"><span data-stu-id="94d98-104">The availability of an attendee.</span></span>

## <a name="json-representation"></a><span data-ttu-id="94d98-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="94d98-105">JSON representation</span></span>

<span data-ttu-id="94d98-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="94d98-106">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="94d98-107">属性</span><span class="sxs-lookup"><span data-stu-id="94d98-107">Properties</span></span>
| <span data-ttu-id="94d98-108">属性</span><span class="sxs-lookup"><span data-stu-id="94d98-108">Property</span></span>     | <span data-ttu-id="94d98-109">类型</span><span class="sxs-lookup"><span data-stu-id="94d98-109">Type</span></span>   |<span data-ttu-id="94d98-110">说明</span><span class="sxs-lookup"><span data-stu-id="94d98-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="94d98-111">attendee</span><span class="sxs-lookup"><span data-stu-id="94d98-111">attendee</span></span>|[<span data-ttu-id="94d98-112">attendeeBase</span><span class="sxs-lookup"><span data-stu-id="94d98-112">attendeeBase</span></span>](attendeebase.md)|<span data-ttu-id="94d98-113">电子邮件地址和与会者类型-无论是个人还是资源, 如果是个人或资源, 是必需的还是可选的。</span><span class="sxs-lookup"><span data-stu-id="94d98-113">The email address and type of attendee - whether it's a person or a resource, and whether required or optional if it's a person.</span></span>|
|<span data-ttu-id="94d98-114">availability</span><span class="sxs-lookup"><span data-stu-id="94d98-114">availability</span></span>|<span data-ttu-id="94d98-115">freeBusyStatus</span><span class="sxs-lookup"><span data-stu-id="94d98-115">freeBusyStatus</span></span>| <span data-ttu-id="94d98-p101">与会者的忙/闲状态。可取值为：`free`、`tentative`、`busy`、`oof`、`workingElsewhere`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="94d98-p101">The availability status of the attendee. Possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span>|

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
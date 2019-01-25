---
title: meetingParticipants 资源类型
description: 在会议中的参与者。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 57a07e29beae6915c7e40f7fb8a6e941351fd38f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508781"
---
# <a name="meetingparticipants-resource-type"></a><span data-ttu-id="16a01-103">meetingParticipants 资源类型</span><span class="sxs-lookup"><span data-stu-id="16a01-103">meetingParticipants resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="16a01-104">在会议中的参与者。</span><span class="sxs-lookup"><span data-stu-id="16a01-104">Participants in a meeting.</span></span>

## <a name="properties"></a><span data-ttu-id="16a01-105">属性</span><span class="sxs-lookup"><span data-stu-id="16a01-105">Properties</span></span>

| <span data-ttu-id="16a01-106">属性</span><span class="sxs-lookup"><span data-stu-id="16a01-106">Property</span></span>       | <span data-ttu-id="16a01-107">类型</span><span class="sxs-lookup"><span data-stu-id="16a01-107">Type</span></span>    | <span data-ttu-id="16a01-108">说明</span><span class="sxs-lookup"><span data-stu-id="16a01-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="16a01-109">attendees</span><span class="sxs-lookup"><span data-stu-id="16a01-109">attendees</span></span> | <span data-ttu-id="16a01-110">[meetingParticipantInfo](meetingparticipantinfo.md)集合</span><span class="sxs-lookup"><span data-stu-id="16a01-110">[meetingParticipantInfo](meetingparticipantinfo.md) collection</span></span> |  |
| <span data-ttu-id="16a01-111">organizer</span><span class="sxs-lookup"><span data-stu-id="16a01-111">organizer</span></span> | [<span data-ttu-id="16a01-112">meetingParticipantInfo</span><span class="sxs-lookup"><span data-stu-id="16a01-112">meetingParticipantInfo</span></span>](meetingparticipantinfo.md) |  |

## <a name="json-representation"></a><span data-ttu-id="16a01-113">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="16a01-113">JSON representation</span></span>

<span data-ttu-id="16a01-114">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="16a01-114">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingParticipants"
}-->
```json
{
  "attendees": [{"@odata.type": "#microsoft.graph.meetingParticipantInfo"}],
  "organizer": {"@odata.type": "#microsoft.graph.meetingParticipantInfo"}
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "meetingParticipants resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/meetingparticipants.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

---
title: meetingParticipants 资源类型
description: 会议中的参与者。
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: ce312f3dab1151c18389e6b88a848bb2b700472c
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40871070"
---
# <a name="meetingparticipants-resource-type"></a><span data-ttu-id="a0d02-103">meetingParticipants 资源类型</span><span class="sxs-lookup"><span data-stu-id="a0d02-103">meetingParticipants resource type</span></span>

<span data-ttu-id="a0d02-104">会议中的参与者。</span><span class="sxs-lookup"><span data-stu-id="a0d02-104">Participants in a meeting.</span></span>

## <a name="properties"></a><span data-ttu-id="a0d02-105">属性</span><span class="sxs-lookup"><span data-stu-id="a0d02-105">Properties</span></span>

| <span data-ttu-id="a0d02-106">属性</span><span class="sxs-lookup"><span data-stu-id="a0d02-106">Property</span></span>       | <span data-ttu-id="a0d02-107">类型</span><span class="sxs-lookup"><span data-stu-id="a0d02-107">Type</span></span>    | <span data-ttu-id="a0d02-108">说明</span><span class="sxs-lookup"><span data-stu-id="a0d02-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a0d02-109">attendees</span><span class="sxs-lookup"><span data-stu-id="a0d02-109">attendees</span></span> | <span data-ttu-id="a0d02-110">[meetingParticipantInfo](meetingparticipantinfo.md)集合</span><span class="sxs-lookup"><span data-stu-id="a0d02-110">[meetingParticipantInfo](meetingparticipantinfo.md) collection</span></span> |  |
| <span data-ttu-id="a0d02-111">组织者</span><span class="sxs-lookup"><span data-stu-id="a0d02-111">organizer</span></span> | [<span data-ttu-id="a0d02-112">meetingParticipantInfo</span><span class="sxs-lookup"><span data-stu-id="a0d02-112">meetingParticipantInfo</span></span>](meetingparticipantinfo.md) |  |

## <a name="json-representation"></a><span data-ttu-id="a0d02-113">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a0d02-113">JSON representation</span></span>

<span data-ttu-id="a0d02-114">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a0d02-114">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->

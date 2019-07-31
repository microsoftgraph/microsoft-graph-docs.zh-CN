---
title: meetingParticipants 资源类型
description: 会议中的参与者。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: b88a59b3d9def58217ca3badd833b275760b49c1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966828"
---
# <a name="meetingparticipants-resource-type"></a><span data-ttu-id="aa7b0-103">meetingParticipants 资源类型</span><span class="sxs-lookup"><span data-stu-id="aa7b0-103">meetingParticipants resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aa7b0-104">会议中的参与者。</span><span class="sxs-lookup"><span data-stu-id="aa7b0-104">Participants in a meeting.</span></span>

## <a name="properties"></a><span data-ttu-id="aa7b0-105">属性</span><span class="sxs-lookup"><span data-stu-id="aa7b0-105">Properties</span></span>

| <span data-ttu-id="aa7b0-106">属性</span><span class="sxs-lookup"><span data-stu-id="aa7b0-106">Property</span></span>       | <span data-ttu-id="aa7b0-107">类型</span><span class="sxs-lookup"><span data-stu-id="aa7b0-107">Type</span></span>    | <span data-ttu-id="aa7b0-108">说明</span><span class="sxs-lookup"><span data-stu-id="aa7b0-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="aa7b0-109">attendees</span><span class="sxs-lookup"><span data-stu-id="aa7b0-109">attendees</span></span> | <span data-ttu-id="aa7b0-110">[meetingParticipantInfo](meetingparticipantinfo.md)集合</span><span class="sxs-lookup"><span data-stu-id="aa7b0-110">[meetingParticipantInfo](meetingparticipantinfo.md) collection</span></span> |  |
| <span data-ttu-id="aa7b0-111">organizer － 组织者</span><span class="sxs-lookup"><span data-stu-id="aa7b0-111">organizer</span></span> | [<span data-ttu-id="aa7b0-112">meetingParticipantInfo</span><span class="sxs-lookup"><span data-stu-id="aa7b0-112">meetingParticipantInfo</span></span>](meetingparticipantinfo.md) |  |

## <a name="json-representation"></a><span data-ttu-id="aa7b0-113">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="aa7b0-113">JSON representation</span></span>

<span data-ttu-id="aa7b0-114">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="aa7b0-114">The following is a JSON representation of the resource.</span></span>

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

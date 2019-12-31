---
title: meetingParticipants 资源类型
description: 会议中的参与者。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 66bb521ae9a2222b5ea60709ac3687da930161d6
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913553"
---
# <a name="meetingparticipants-resource-type"></a><span data-ttu-id="3dbf5-103">meetingParticipants 资源类型</span><span class="sxs-lookup"><span data-stu-id="3dbf5-103">meetingParticipants resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3dbf5-104">会议中的参与者。</span><span class="sxs-lookup"><span data-stu-id="3dbf5-104">Participants in a meeting.</span></span>

## <a name="properties"></a><span data-ttu-id="3dbf5-105">属性</span><span class="sxs-lookup"><span data-stu-id="3dbf5-105">Properties</span></span>

| <span data-ttu-id="3dbf5-106">属性</span><span class="sxs-lookup"><span data-stu-id="3dbf5-106">Property</span></span>       | <span data-ttu-id="3dbf5-107">类型</span><span class="sxs-lookup"><span data-stu-id="3dbf5-107">Type</span></span>    | <span data-ttu-id="3dbf5-108">说明</span><span class="sxs-lookup"><span data-stu-id="3dbf5-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="3dbf5-109">attendees</span><span class="sxs-lookup"><span data-stu-id="3dbf5-109">attendees</span></span> | <span data-ttu-id="3dbf5-110">[meetingParticipantInfo](meetingparticipantinfo.md)集合</span><span class="sxs-lookup"><span data-stu-id="3dbf5-110">[meetingParticipantInfo](meetingparticipantinfo.md) collection</span></span> |  |
| <span data-ttu-id="3dbf5-111">organizer － 组织者</span><span class="sxs-lookup"><span data-stu-id="3dbf5-111">organizer</span></span> | [<span data-ttu-id="3dbf5-112">meetingParticipantInfo</span><span class="sxs-lookup"><span data-stu-id="3dbf5-112">meetingParticipantInfo</span></span>](meetingparticipantinfo.md) |  |
| <span data-ttu-id="3dbf5-113">创建器</span><span class="sxs-lookup"><span data-stu-id="3dbf5-113">producers</span></span> | <span data-ttu-id="3dbf5-114">[meetingParticipantInfo](meetingparticipantinfo.md)集合</span><span class="sxs-lookup"><span data-stu-id="3dbf5-114">[meetingParticipantInfo](meetingparticipantinfo.md) collection</span></span> | <span data-ttu-id="3dbf5-115">仅适用于广播会议。</span><span class="sxs-lookup"><span data-stu-id="3dbf5-115">For broadcast meeting only.</span></span> |
| <span data-ttu-id="3dbf5-116">参与者</span><span class="sxs-lookup"><span data-stu-id="3dbf5-116">contributors</span></span> | <span data-ttu-id="3dbf5-117">[meetingParticipantInfo](meetingparticipantinfo.md)集合</span><span class="sxs-lookup"><span data-stu-id="3dbf5-117">[meetingParticipantInfo](meetingparticipantinfo.md) collection</span></span> | <span data-ttu-id="3dbf5-118">仅适用于广播会议。</span><span class="sxs-lookup"><span data-stu-id="3dbf5-118">For broadcast meeting only.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="3dbf5-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3dbf5-119">JSON representation</span></span>

<span data-ttu-id="3dbf5-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3dbf5-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingParticipants"
}-->
```json
{
  "attendees": [{"@odata.type": "#microsoft.graph.meetingParticipantInfo"}],
  "organizer": {"@odata.type": "#microsoft.graph.meetingParticipantInfo"},
  "producers": [{"@odata.type": "#microsoft.graph.meetingParticipantInfo"}],
  "contributors": [{"@odata.type": "#microsoft.graph.meetingParticipantInfo"}],
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

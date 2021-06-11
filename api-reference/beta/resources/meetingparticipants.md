---
title: meetingParticipants 资源类型
description: 会议参与者。
author: mkhribech
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 8ee5cf115a80c642f5442230d7111dfaeffca930
ms.sourcegitcommit: 7abb0672a38a6d9b11a2e0d2cc221222cb8358bb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/11/2021
ms.locfileid: "52896618"
---
# <a name="meetingparticipants-resource-type"></a><span data-ttu-id="1df92-103">meetingParticipants 资源类型</span><span class="sxs-lookup"><span data-stu-id="1df92-103">meetingParticipants resource type</span></span>

<span data-ttu-id="1df92-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1df92-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1df92-105">会议参与者。</span><span class="sxs-lookup"><span data-stu-id="1df92-105">Participants in a meeting.</span></span>

## <a name="properties"></a><span data-ttu-id="1df92-106">属性</span><span class="sxs-lookup"><span data-stu-id="1df92-106">Properties</span></span>

| <span data-ttu-id="1df92-107">属性</span><span class="sxs-lookup"><span data-stu-id="1df92-107">Property</span></span>                  | <span data-ttu-id="1df92-108">类型</span><span class="sxs-lookup"><span data-stu-id="1df92-108">Type</span></span>                                                           | <span data-ttu-id="1df92-109">说明</span><span class="sxs-lookup"><span data-stu-id="1df92-109">Description</span></span>                           |
| :------------------------ | :------------------------------------------------------------- | :------------------------------------ |
| <span data-ttu-id="1df92-110">attendees</span><span class="sxs-lookup"><span data-stu-id="1df92-110">attendees</span></span>                 | <span data-ttu-id="1df92-111">[meetingParticipantInfo](meetingparticipantinfo.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1df92-111">[meetingParticipantInfo](meetingparticipantinfo.md) collection</span></span> | <span data-ttu-id="1df92-112">与会者的信息。</span><span class="sxs-lookup"><span data-stu-id="1df92-112">Information of the meeting attendees.</span></span> |
| <span data-ttu-id="1df92-113">organizer － 组织者</span><span class="sxs-lookup"><span data-stu-id="1df92-113">organizer</span></span>                 | [<span data-ttu-id="1df92-114">meetingParticipantInfo</span><span class="sxs-lookup"><span data-stu-id="1df92-114">meetingParticipantInfo</span></span>](meetingparticipantinfo.md)            | <span data-ttu-id="1df92-115">会议组织者的信息。</span><span class="sxs-lookup"><span data-stu-id="1df92-115">Information of the meeting organizer.</span></span> |
| <span data-ttu-id="1df92-116">创建 (已弃) </span><span class="sxs-lookup"><span data-stu-id="1df92-116">producers (deprecated)</span></span>    | <span data-ttu-id="1df92-117">[meetingParticipantInfo](meetingparticipantinfo.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1df92-117">[meetingParticipantInfo](meetingparticipantinfo.md) collection</span></span> | <span data-ttu-id="1df92-118">仅适用于直播会议。</span><span class="sxs-lookup"><span data-stu-id="1df92-118">For broadcast meeting only.</span></span>           |
| <span data-ttu-id="1df92-119">参与者 (弃用) </span><span class="sxs-lookup"><span data-stu-id="1df92-119">contributors (deprecated)</span></span> | <span data-ttu-id="1df92-120">[meetingParticipantInfo](meetingparticipantinfo.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1df92-120">[meetingParticipantInfo](meetingparticipantinfo.md) collection</span></span> | <span data-ttu-id="1df92-121">仅适用于直播会议。</span><span class="sxs-lookup"><span data-stu-id="1df92-121">For broadcast meeting only.</span></span>           |

> [!CAUTION]
> <span data-ttu-id="1df92-122">创建 **者和\*\*\*\*参与者** 属性已弃用。</span><span class="sxs-lookup"><span data-stu-id="1df92-122">The **producers** and **contributors** properties are deprecated.</span></span> <span data-ttu-id="1df92-123">所有会议参与者都返回到 **与会者集合** 中。</span><span class="sxs-lookup"><span data-stu-id="1df92-123">All meeting participants are returned in the **attendees** collection.</span></span> <span data-ttu-id="1df92-124">使用[meetingParticipantInfo](meetingparticipantinfo.md)的 role 属性标识与会者的会议角色。</span><span class="sxs-lookup"><span data-stu-id="1df92-124">Use the **role** property of [meetingParticipantInfo](meetingparticipantinfo.md) to identify the meeting role of the attendee.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1df92-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1df92-125">JSON representation</span></span>

<span data-ttu-id="1df92-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1df92-126">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.meetingParticipants"
}-->
```json
{
  "attendees": [{"@odata.type": "#microsoft.graph.meetingParticipantInfo"}],
  "organizer": {"@odata.type": "#microsoft.graph.meetingParticipantInfo"},
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



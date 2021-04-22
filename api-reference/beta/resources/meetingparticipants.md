---
title: meetingParticipants 资源类型
description: 会议参与者。
author: jsandoval-msft
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 93ca3d73518f9739cc3115c80efd2aec551629b5
ms.sourcegitcommit: 6e7d9987a255f1bee04f196a4a7e37f56621bfb8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2021
ms.locfileid: "51944161"
---
# <a name="meetingparticipants-resource-type"></a><span data-ttu-id="72248-103">meetingParticipants 资源类型</span><span class="sxs-lookup"><span data-stu-id="72248-103">meetingParticipants resource type</span></span>

<span data-ttu-id="72248-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="72248-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="72248-105">会议参与者。</span><span class="sxs-lookup"><span data-stu-id="72248-105">Participants in a meeting.</span></span>

## <a name="properties"></a><span data-ttu-id="72248-106">属性</span><span class="sxs-lookup"><span data-stu-id="72248-106">Properties</span></span>

| <span data-ttu-id="72248-107">属性</span><span class="sxs-lookup"><span data-stu-id="72248-107">Property</span></span>                  | <span data-ttu-id="72248-108">类型</span><span class="sxs-lookup"><span data-stu-id="72248-108">Type</span></span>                                                           | <span data-ttu-id="72248-109">说明</span><span class="sxs-lookup"><span data-stu-id="72248-109">Description</span></span>                           |
| :------------------------ | :------------------------------------------------------------- | :------------------------------------ |
| <span data-ttu-id="72248-110">attendees</span><span class="sxs-lookup"><span data-stu-id="72248-110">attendees</span></span>                 | <span data-ttu-id="72248-111">[meetingParticipantInfo](meetingparticipantinfo.md) 集合</span><span class="sxs-lookup"><span data-stu-id="72248-111">[meetingParticipantInfo](meetingparticipantinfo.md) collection</span></span> | <span data-ttu-id="72248-112">与会者的信息。</span><span class="sxs-lookup"><span data-stu-id="72248-112">Information of the meeting attendees.</span></span> |
| <span data-ttu-id="72248-113">organizer － 组织者</span><span class="sxs-lookup"><span data-stu-id="72248-113">organizer</span></span>                 | [<span data-ttu-id="72248-114">meetingParticipantInfo</span><span class="sxs-lookup"><span data-stu-id="72248-114">meetingParticipantInfo</span></span>](meetingparticipantinfo.md)            | <span data-ttu-id="72248-115">会议组织者的信息。</span><span class="sxs-lookup"><span data-stu-id="72248-115">Information of the meeting organizer.</span></span> |
| <span data-ttu-id="72248-116">创建 (已弃) </span><span class="sxs-lookup"><span data-stu-id="72248-116">producers (deprecated)</span></span>    | <span data-ttu-id="72248-117">[meetingParticipantInfo](meetingparticipantinfo.md) 集合</span><span class="sxs-lookup"><span data-stu-id="72248-117">[meetingParticipantInfo](meetingparticipantinfo.md) collection</span></span> | <span data-ttu-id="72248-118">仅适用于直播会议。</span><span class="sxs-lookup"><span data-stu-id="72248-118">For broadcast meeting only.</span></span>           |
| <span data-ttu-id="72248-119">参与者 (弃用) </span><span class="sxs-lookup"><span data-stu-id="72248-119">contributors (deprecated)</span></span> | <span data-ttu-id="72248-120">[meetingParticipantInfo](meetingparticipantinfo.md) 集合</span><span class="sxs-lookup"><span data-stu-id="72248-120">[meetingParticipantInfo](meetingparticipantinfo.md) collection</span></span> | <span data-ttu-id="72248-121">仅适用于直播会议。</span><span class="sxs-lookup"><span data-stu-id="72248-121">For broadcast meeting only.</span></span>           |

> [!CAUTION]
> <span data-ttu-id="72248-122">创建 **者和\*\*\*\*参与者** 属性已弃用。</span><span class="sxs-lookup"><span data-stu-id="72248-122">The **producers** and **contributors** properties are deprecated.</span></span> <span data-ttu-id="72248-123">所有会议参与者都返回到 **与会者集合** 中。</span><span class="sxs-lookup"><span data-stu-id="72248-123">All meeting participants are returned in the **attendees** collection.</span></span> <span data-ttu-id="72248-124">使用[meetingParticipantInfo](meetingparticipantinfo.md)的 role 属性标识与会者的会议角色。</span><span class="sxs-lookup"><span data-stu-id="72248-124">Use the **role** property of [meetingParticipantInfo](meetingparticipantinfo.md) to identify the meeting role of the attendee.</span></span>

## <a name="json-representation"></a><span data-ttu-id="72248-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="72248-125">JSON representation</span></span>

<span data-ttu-id="72248-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="72248-126">The following is a JSON representation of the resource.</span></span>

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



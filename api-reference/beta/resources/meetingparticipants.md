---
title: meetingParticipants 资源类型
description: 会议中的参与者。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 2d40479390703f50ac87b7c3196aa4d5bc55bc8a
ms.sourcegitcommit: c68a83d28fa4bfca6e0618467934813a9ae17b12
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/07/2019
ms.locfileid: "36792763"
---
# <a name="meetingparticipants-resource-type"></a><span data-ttu-id="dba37-103">meetingParticipants 资源类型</span><span class="sxs-lookup"><span data-stu-id="dba37-103">meetingParticipants resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dba37-104">会议中的参与者。</span><span class="sxs-lookup"><span data-stu-id="dba37-104">Participants in a meeting.</span></span>

## <a name="properties"></a><span data-ttu-id="dba37-105">属性</span><span class="sxs-lookup"><span data-stu-id="dba37-105">Properties</span></span>

| <span data-ttu-id="dba37-106">属性</span><span class="sxs-lookup"><span data-stu-id="dba37-106">Property</span></span>       | <span data-ttu-id="dba37-107">类型</span><span class="sxs-lookup"><span data-stu-id="dba37-107">Type</span></span>    | <span data-ttu-id="dba37-108">说明</span><span class="sxs-lookup"><span data-stu-id="dba37-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="dba37-109">attendees</span><span class="sxs-lookup"><span data-stu-id="dba37-109">attendees</span></span> | <span data-ttu-id="dba37-110">[meetingParticipantInfo](meetingparticipantinfo.md)集合</span><span class="sxs-lookup"><span data-stu-id="dba37-110">[meetingParticipantInfo](meetingparticipantinfo.md) collection</span></span> |  |
| <span data-ttu-id="dba37-111">organizer － 组织者</span><span class="sxs-lookup"><span data-stu-id="dba37-111">organizer</span></span> | [<span data-ttu-id="dba37-112">meetingParticipantInfo</span><span class="sxs-lookup"><span data-stu-id="dba37-112">meetingParticipantInfo</span></span>](meetingparticipantinfo.md) |  |
| <span data-ttu-id="dba37-113">创建器</span><span class="sxs-lookup"><span data-stu-id="dba37-113">producers</span></span> | <span data-ttu-id="dba37-114">[meetingParticipantInfo](meetingparticipantinfo.md)集合</span><span class="sxs-lookup"><span data-stu-id="dba37-114">[meetingParticipantInfo](meetingparticipantinfo.md) collection</span></span> | <span data-ttu-id="dba37-115">仅适用于广播会议。</span><span class="sxs-lookup"><span data-stu-id="dba37-115">For broadcast meeting only.</span></span> |
| <span data-ttu-id="dba37-116">参与者</span><span class="sxs-lookup"><span data-stu-id="dba37-116">contributors</span></span> | <span data-ttu-id="dba37-117">[meetingParticipantInfo](meetingparticipantinfo.md)集合</span><span class="sxs-lookup"><span data-stu-id="dba37-117">[meetingParticipantInfo](meetingparticipantinfo.md) collection</span></span> | <span data-ttu-id="dba37-118">仅适用于广播会议。</span><span class="sxs-lookup"><span data-stu-id="dba37-118">For broadcast meeting only.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="dba37-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="dba37-119">JSON representation</span></span>

<span data-ttu-id="dba37-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dba37-120">The following is a JSON representation of the resource.</span></span>

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

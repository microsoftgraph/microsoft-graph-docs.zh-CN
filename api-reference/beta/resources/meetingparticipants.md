---
title: meetingParticipants 资源类型
description: 会议中的参与者。
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 171d24629c8a219f788ad17cdf97874bbf299a62
ms.sourcegitcommit: 9bddc0b7746383e8d05ce50d163af3f4196f12a6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/06/2019
ms.locfileid: "38006625"
---
# <a name="meetingparticipants-resource-type"></a><span data-ttu-id="7ad76-103">meetingParticipants 资源类型</span><span class="sxs-lookup"><span data-stu-id="7ad76-103">meetingParticipants resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7ad76-104">会议中的参与者。</span><span class="sxs-lookup"><span data-stu-id="7ad76-104">Participants in a meeting.</span></span>

## <a name="properties"></a><span data-ttu-id="7ad76-105">属性</span><span class="sxs-lookup"><span data-stu-id="7ad76-105">Properties</span></span>

| <span data-ttu-id="7ad76-106">属性</span><span class="sxs-lookup"><span data-stu-id="7ad76-106">Property</span></span>       | <span data-ttu-id="7ad76-107">类型</span><span class="sxs-lookup"><span data-stu-id="7ad76-107">Type</span></span>    | <span data-ttu-id="7ad76-108">说明</span><span class="sxs-lookup"><span data-stu-id="7ad76-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="7ad76-109">attendees</span><span class="sxs-lookup"><span data-stu-id="7ad76-109">attendees</span></span> | <span data-ttu-id="7ad76-110">[meetingParticipantInfo](meetingparticipantinfo.md)集合</span><span class="sxs-lookup"><span data-stu-id="7ad76-110">[meetingParticipantInfo](meetingparticipantinfo.md) collection</span></span> |  |
| <span data-ttu-id="7ad76-111">组织者</span><span class="sxs-lookup"><span data-stu-id="7ad76-111">organizer</span></span> | [<span data-ttu-id="7ad76-112">meetingParticipantInfo</span><span class="sxs-lookup"><span data-stu-id="7ad76-112">meetingParticipantInfo</span></span>](meetingparticipantinfo.md) |  |
| <span data-ttu-id="7ad76-113">创建器</span><span class="sxs-lookup"><span data-stu-id="7ad76-113">producers</span></span> | <span data-ttu-id="7ad76-114">[meetingParticipantInfo](meetingparticipantinfo.md)集合</span><span class="sxs-lookup"><span data-stu-id="7ad76-114">[meetingParticipantInfo](meetingparticipantinfo.md) collection</span></span> | <span data-ttu-id="7ad76-115">仅适用于广播会议。</span><span class="sxs-lookup"><span data-stu-id="7ad76-115">For broadcast meeting only.</span></span> |
| <span data-ttu-id="7ad76-116">参与者</span><span class="sxs-lookup"><span data-stu-id="7ad76-116">contributors</span></span> | <span data-ttu-id="7ad76-117">[meetingParticipantInfo](meetingparticipantinfo.md)集合</span><span class="sxs-lookup"><span data-stu-id="7ad76-117">[meetingParticipantInfo](meetingparticipantinfo.md) collection</span></span> | <span data-ttu-id="7ad76-118">仅适用于广播会议。</span><span class="sxs-lookup"><span data-stu-id="7ad76-118">For broadcast meeting only.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="7ad76-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7ad76-119">JSON representation</span></span>

<span data-ttu-id="7ad76-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7ad76-120">The following is a JSON representation of the resource.</span></span>

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

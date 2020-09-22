---
title: meetingParticipants 资源类型
description: 会议中的参与者。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: e6d53d0359b9dc71e538c5bbe025e093a4912ffb
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47971655"
---
# <a name="meetingparticipants-resource-type"></a><span data-ttu-id="16e3c-103">meetingParticipants 资源类型</span><span class="sxs-lookup"><span data-stu-id="16e3c-103">meetingParticipants resource type</span></span>

<span data-ttu-id="16e3c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="16e3c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="16e3c-105">会议中的参与者。</span><span class="sxs-lookup"><span data-stu-id="16e3c-105">Participants in a meeting.</span></span>

## <a name="properties"></a><span data-ttu-id="16e3c-106">属性</span><span class="sxs-lookup"><span data-stu-id="16e3c-106">Properties</span></span>

| <span data-ttu-id="16e3c-107">属性</span><span class="sxs-lookup"><span data-stu-id="16e3c-107">Property</span></span>       | <span data-ttu-id="16e3c-108">类型</span><span class="sxs-lookup"><span data-stu-id="16e3c-108">Type</span></span>    | <span data-ttu-id="16e3c-109">说明</span><span class="sxs-lookup"><span data-stu-id="16e3c-109">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="16e3c-110">attendees</span><span class="sxs-lookup"><span data-stu-id="16e3c-110">attendees</span></span> | <span data-ttu-id="16e3c-111">[meetingParticipantInfo](meetingparticipantinfo.md) 集合</span><span class="sxs-lookup"><span data-stu-id="16e3c-111">[meetingParticipantInfo](meetingparticipantinfo.md) collection</span></span> |  |
| <span data-ttu-id="16e3c-112">组织者</span><span class="sxs-lookup"><span data-stu-id="16e3c-112">organizer</span></span> | [<span data-ttu-id="16e3c-113">meetingParticipantInfo</span><span class="sxs-lookup"><span data-stu-id="16e3c-113">meetingParticipantInfo</span></span>](meetingparticipantinfo.md) |  |
| <span data-ttu-id="16e3c-114">创建器</span><span class="sxs-lookup"><span data-stu-id="16e3c-114">producers</span></span> | <span data-ttu-id="16e3c-115">[meetingParticipantInfo](meetingparticipantinfo.md) 集合</span><span class="sxs-lookup"><span data-stu-id="16e3c-115">[meetingParticipantInfo](meetingparticipantinfo.md) collection</span></span> | <span data-ttu-id="16e3c-116">仅适用于广播会议。</span><span class="sxs-lookup"><span data-stu-id="16e3c-116">For broadcast meeting only.</span></span> |
| <span data-ttu-id="16e3c-117">参与者</span><span class="sxs-lookup"><span data-stu-id="16e3c-117">contributors</span></span> | <span data-ttu-id="16e3c-118">[meetingParticipantInfo](meetingparticipantinfo.md) 集合</span><span class="sxs-lookup"><span data-stu-id="16e3c-118">[meetingParticipantInfo](meetingparticipantinfo.md) collection</span></span> | <span data-ttu-id="16e3c-119">仅适用于广播会议。</span><span class="sxs-lookup"><span data-stu-id="16e3c-119">For broadcast meeting only.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="16e3c-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="16e3c-120">JSON representation</span></span>

<span data-ttu-id="16e3c-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="16e3c-121">The following is a JSON representation of the resource.</span></span>

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



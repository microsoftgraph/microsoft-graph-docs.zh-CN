---
title: meetingParticipants 资源类型
description: 会议中的参与者。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: dd00cbf5ce8395a819136ad9e655fa7670e5f3fa
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447414"
---
# <a name="meetingparticipants-resource-type"></a><span data-ttu-id="6c162-103">meetingParticipants 资源类型</span><span class="sxs-lookup"><span data-stu-id="6c162-103">meetingParticipants resource type</span></span>

<span data-ttu-id="6c162-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="6c162-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6c162-105">会议中的参与者。</span><span class="sxs-lookup"><span data-stu-id="6c162-105">Participants in a meeting.</span></span>

## <a name="properties"></a><span data-ttu-id="6c162-106">属性</span><span class="sxs-lookup"><span data-stu-id="6c162-106">Properties</span></span>

| <span data-ttu-id="6c162-107">属性</span><span class="sxs-lookup"><span data-stu-id="6c162-107">Property</span></span>       | <span data-ttu-id="6c162-108">类型</span><span class="sxs-lookup"><span data-stu-id="6c162-108">Type</span></span>    | <span data-ttu-id="6c162-109">说明</span><span class="sxs-lookup"><span data-stu-id="6c162-109">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="6c162-110">attendees</span><span class="sxs-lookup"><span data-stu-id="6c162-110">attendees</span></span> | <span data-ttu-id="6c162-111">[meetingParticipantInfo](meetingparticipantinfo.md)集合</span><span class="sxs-lookup"><span data-stu-id="6c162-111">[meetingParticipantInfo](meetingparticipantinfo.md) collection</span></span> |  |
| <span data-ttu-id="6c162-112">组织者</span><span class="sxs-lookup"><span data-stu-id="6c162-112">organizer</span></span> | [<span data-ttu-id="6c162-113">meetingParticipantInfo</span><span class="sxs-lookup"><span data-stu-id="6c162-113">meetingParticipantInfo</span></span>](meetingparticipantinfo.md) |  |

## <a name="json-representation"></a><span data-ttu-id="6c162-114">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6c162-114">JSON representation</span></span>

<span data-ttu-id="6c162-115">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6c162-115">The following is a JSON representation of the resource.</span></span>

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

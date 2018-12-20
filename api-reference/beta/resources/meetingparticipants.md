---
title: meetingParticipants 资源类型
description: 在会议中的参与者。
author: VinodRavichandran
ms.openlocfilehash: 7e44863004dab5405251e2effaf2af8c2ae31f67
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380280"
---
# <a name="meetingparticipants-resource-type"></a><span data-ttu-id="77a75-103">meetingParticipants 资源类型</span><span class="sxs-lookup"><span data-stu-id="77a75-103">meetingParticipants resource type</span></span>

> <span data-ttu-id="77a75-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="77a75-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="77a75-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="77a75-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="77a75-106">在会议中的参与者。</span><span class="sxs-lookup"><span data-stu-id="77a75-106">Participants in a meeting.</span></span>

## <a name="properties"></a><span data-ttu-id="77a75-107">属性</span><span class="sxs-lookup"><span data-stu-id="77a75-107">Properties</span></span>

| <span data-ttu-id="77a75-108">属性</span><span class="sxs-lookup"><span data-stu-id="77a75-108">Property</span></span>       | <span data-ttu-id="77a75-109">类型</span><span class="sxs-lookup"><span data-stu-id="77a75-109">Type</span></span>    | <span data-ttu-id="77a75-110">说明</span><span class="sxs-lookup"><span data-stu-id="77a75-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="77a75-111">attendees</span><span class="sxs-lookup"><span data-stu-id="77a75-111">attendees</span></span> | <span data-ttu-id="77a75-112">[meetingParticipantInfo](meetingparticipantinfo.md)集合</span><span class="sxs-lookup"><span data-stu-id="77a75-112">[meetingParticipantInfo](meetingparticipantinfo.md) collection</span></span> |  |
| <span data-ttu-id="77a75-113">organizer</span><span class="sxs-lookup"><span data-stu-id="77a75-113">organizer</span></span> | [<span data-ttu-id="77a75-114">meetingParticipantInfo</span><span class="sxs-lookup"><span data-stu-id="77a75-114">meetingParticipantInfo</span></span>](meetingparticipantinfo.md) |  |

## <a name="json-representation"></a><span data-ttu-id="77a75-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="77a75-115">JSON representation</span></span>

<span data-ttu-id="77a75-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="77a75-116">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "meetingParticipants resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

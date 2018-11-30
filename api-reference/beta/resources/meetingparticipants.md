---
title: meetingParticipants 资源类型
description: 下面是资源的 JSON 表示形式。
ms.openlocfilehash: 4f91c9198018e903eccff7e8fe07d6668d9fd2c9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27049046"
---
# <a name="meetingparticipants-resource-type"></a><span data-ttu-id="b201d-103">meetingParticipants 资源类型</span><span class="sxs-lookup"><span data-stu-id="b201d-103">meetingParticipants resource type</span></span>

> <span data-ttu-id="b201d-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="b201d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b201d-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b201d-105">Use of these APIs in production applications is not supported.</span></span>

## <a name="properties"></a><span data-ttu-id="b201d-106">属性</span><span class="sxs-lookup"><span data-stu-id="b201d-106">Properties</span></span>

| <span data-ttu-id="b201d-107">属性</span><span class="sxs-lookup"><span data-stu-id="b201d-107">Property</span></span>       | <span data-ttu-id="b201d-108">类型</span><span class="sxs-lookup"><span data-stu-id="b201d-108">Type</span></span>    | <span data-ttu-id="b201d-109">说明</span><span class="sxs-lookup"><span data-stu-id="b201d-109">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b201d-110">attendees</span><span class="sxs-lookup"><span data-stu-id="b201d-110">attendees</span></span> | <span data-ttu-id="b201d-111">[meetingParticipantInfo](meetingparticipantinfo.md)集合</span><span class="sxs-lookup"><span data-stu-id="b201d-111">[meetingParticipantInfo](meetingparticipantinfo.md) collection</span></span> |  |
| <span data-ttu-id="b201d-112">organizer</span><span class="sxs-lookup"><span data-stu-id="b201d-112">organizer</span></span> | [<span data-ttu-id="b201d-113">meetingParticipantInfo</span><span class="sxs-lookup"><span data-stu-id="b201d-113">meetingParticipantInfo</span></span>](meetingparticipantinfo.md) |  |

## <a name="json-representation"></a><span data-ttu-id="b201d-114">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b201d-114">JSON representation</span></span>

<span data-ttu-id="b201d-115">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b201d-115">The following is a JSON representation of the resource.</span></span>

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

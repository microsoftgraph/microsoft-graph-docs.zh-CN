---
title: meetingParticipantInfo 资源类型
description: 会议参与者的相关信息。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 1ba727344b1f653125a482b592e7d28c11d1d3d5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32457114"
---
# <a name="meetingparticipantinfo-resource-type"></a><span data-ttu-id="843c8-103">meetingParticipantInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="843c8-103">meetingParticipantInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="843c8-104">会议参与者的相关信息。</span><span class="sxs-lookup"><span data-stu-id="843c8-104">Information about a participant in a meeting.</span></span>

## <a name="properties"></a><span data-ttu-id="843c8-105">属性</span><span class="sxs-lookup"><span data-stu-id="843c8-105">Properties</span></span>

| <span data-ttu-id="843c8-106">属性</span><span class="sxs-lookup"><span data-stu-id="843c8-106">Property</span></span>       | <span data-ttu-id="843c8-107">类型</span><span class="sxs-lookup"><span data-stu-id="843c8-107">Type</span></span>                          | <span data-ttu-id="843c8-108">描述</span><span class="sxs-lookup"><span data-stu-id="843c8-108">Description</span></span>                              |
|:---------------|:------------------------------|:-----------------------------------------|
| <span data-ttu-id="843c8-109">窃取</span><span class="sxs-lookup"><span data-stu-id="843c8-109">identity</span></span>       | [<span data-ttu-id="843c8-110">identitySet</span><span class="sxs-lookup"><span data-stu-id="843c8-110">identitySet</span></span>](identityset.md) | <span data-ttu-id="843c8-111">参与者的标识信息。</span><span class="sxs-lookup"><span data-stu-id="843c8-111">Identity information of the participant.</span></span> |
| <span data-ttu-id="843c8-112">upn</span><span class="sxs-lookup"><span data-stu-id="843c8-112">upn</span></span>            | <span data-ttu-id="843c8-113">字符串</span><span class="sxs-lookup"><span data-stu-id="843c8-113">String</span></span>                        | <span data-ttu-id="843c8-114">参与者的用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="843c8-114">User principal name of the participant.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="843c8-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="843c8-115">JSON representation</span></span>

<span data-ttu-id="843c8-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="843c8-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingParticipantInfo"
}-->
```json
{
  "identity": {"@odata.type": "#microsoft.graph.identitySet"},
  "upn": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "meetingParticipantInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/meetingparticipantinfo.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

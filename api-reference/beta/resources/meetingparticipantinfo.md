---
title: meetingParticipantInfo 资源类型
description: 有关会议中的参与者的信息。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 1ba727344b1f653125a482b592e7d28c11d1d3d5
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515025"
---
# <a name="meetingparticipantinfo-resource-type"></a><span data-ttu-id="457c0-103">meetingParticipantInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="457c0-103">meetingParticipantInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="457c0-104">有关会议中的参与者的信息。</span><span class="sxs-lookup"><span data-stu-id="457c0-104">Information about a participant in a meeting.</span></span>

## <a name="properties"></a><span data-ttu-id="457c0-105">属性</span><span class="sxs-lookup"><span data-stu-id="457c0-105">Properties</span></span>

| <span data-ttu-id="457c0-106">属性</span><span class="sxs-lookup"><span data-stu-id="457c0-106">Property</span></span>       | <span data-ttu-id="457c0-107">类型</span><span class="sxs-lookup"><span data-stu-id="457c0-107">Type</span></span>                          | <span data-ttu-id="457c0-108">说明</span><span class="sxs-lookup"><span data-stu-id="457c0-108">Description</span></span>                              |
|:---------------|:------------------------------|:-----------------------------------------|
| <span data-ttu-id="457c0-109">Identity</span><span class="sxs-lookup"><span data-stu-id="457c0-109">identity</span></span>       | [<span data-ttu-id="457c0-110">identitySet</span><span class="sxs-lookup"><span data-stu-id="457c0-110">identitySet</span></span>](identityset.md) | <span data-ttu-id="457c0-111">参与者的标识信息。</span><span class="sxs-lookup"><span data-stu-id="457c0-111">Identity information of the participant.</span></span> |
| <span data-ttu-id="457c0-112">UPN</span><span class="sxs-lookup"><span data-stu-id="457c0-112">upn</span></span>            | <span data-ttu-id="457c0-113">String</span><span class="sxs-lookup"><span data-stu-id="457c0-113">String</span></span>                        | <span data-ttu-id="457c0-114">参与者的用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="457c0-114">User principal name of the participant.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="457c0-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="457c0-115">JSON representation</span></span>

<span data-ttu-id="457c0-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="457c0-116">The following is a JSON representation of the resource.</span></span>

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

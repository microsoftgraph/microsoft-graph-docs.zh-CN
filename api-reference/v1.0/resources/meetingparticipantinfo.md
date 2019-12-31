---
title: meetingParticipantInfo 资源类型
description: 会议参与者的相关信息。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 2e61b4032e3d8c0976659cb34de2b043fac2ef8e
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913070"
---
# <a name="meetingparticipantinfo-resource-type"></a><span data-ttu-id="d20fb-103">meetingParticipantInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="d20fb-103">meetingParticipantInfo resource type</span></span>

<span data-ttu-id="d20fb-104">会议参与者的相关信息。</span><span class="sxs-lookup"><span data-stu-id="d20fb-104">Information about a participant in a meeting.</span></span>

## <a name="properties"></a><span data-ttu-id="d20fb-105">属性</span><span class="sxs-lookup"><span data-stu-id="d20fb-105">Properties</span></span>

| <span data-ttu-id="d20fb-106">属性</span><span class="sxs-lookup"><span data-stu-id="d20fb-106">Property</span></span>       | <span data-ttu-id="d20fb-107">类型</span><span class="sxs-lookup"><span data-stu-id="d20fb-107">Type</span></span>                          | <span data-ttu-id="d20fb-108">说明</span><span class="sxs-lookup"><span data-stu-id="d20fb-108">Description</span></span>                              |
|:---------------|:------------------------------|:-----------------------------------------|
| <span data-ttu-id="d20fb-109">窃取</span><span class="sxs-lookup"><span data-stu-id="d20fb-109">identity</span></span>       | [<span data-ttu-id="d20fb-110">identitySet</span><span class="sxs-lookup"><span data-stu-id="d20fb-110">identitySet</span></span>](identityset.md) | <span data-ttu-id="d20fb-111">参与者的标识信息。</span><span class="sxs-lookup"><span data-stu-id="d20fb-111">Identity information of the participant.</span></span> |
| <span data-ttu-id="d20fb-112">upn</span><span class="sxs-lookup"><span data-stu-id="d20fb-112">upn</span></span>            | <span data-ttu-id="d20fb-113">String</span><span class="sxs-lookup"><span data-stu-id="d20fb-113">String</span></span>                        | <span data-ttu-id="d20fb-114">参与者的用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="d20fb-114">User principal name of the participant.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="d20fb-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d20fb-115">JSON representation</span></span>

<span data-ttu-id="d20fb-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d20fb-116">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->

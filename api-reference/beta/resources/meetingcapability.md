---
title: meetingCapability 资源类型
description: 包含会议的功能
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: e71d7c8c6489d5856e5f2441cd93c7fdea033bd4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32457142"
---
# <a name="meetingcapability-resource-type"></a><span data-ttu-id="48e38-103">meetingCapability 资源类型</span><span class="sxs-lookup"><span data-stu-id="48e38-103">meetingCapability resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="48e38-104">包含会议的功能</span><span class="sxs-lookup"><span data-stu-id="48e38-104">Contains the capabilities of a meeting</span></span>

## <a name="properties"></a><span data-ttu-id="48e38-105">属性</span><span class="sxs-lookup"><span data-stu-id="48e38-105">Properties</span></span>

| <span data-ttu-id="48e38-106">属性</span><span class="sxs-lookup"><span data-stu-id="48e38-106">Property</span></span>                          | <span data-ttu-id="48e38-107">类型</span><span class="sxs-lookup"><span data-stu-id="48e38-107">Type</span></span>    | <span data-ttu-id="48e38-108">描述</span><span class="sxs-lookup"><span data-stu-id="48e38-108">Description</span></span>                                                        |
|:----------------------------------|:--------|:-------------------------------------------------------------------|
| <span data-ttu-id="48e38-109">allowAnonymousUsersToDialOut</span><span class="sxs-lookup"><span data-stu-id="48e38-109">allowAnonymousUsersToDialOut</span></span>      | <span data-ttu-id="48e38-110">Boolean</span><span class="sxs-lookup"><span data-stu-id="48e38-110">Boolean</span></span> | <span data-ttu-id="48e38-111">指示是否允许在会议中拨出匿名用户。</span><span class="sxs-lookup"><span data-stu-id="48e38-111">Indicates whether anonymous users dialout is allowed in a meeting.</span></span> |
| <span data-ttu-id="48e38-112">allowAnonymousUsersToStartMeeting</span><span class="sxs-lookup"><span data-stu-id="48e38-112">allowAnonymousUsersToStartMeeting</span></span> | <span data-ttu-id="48e38-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="48e38-113">Boolean</span></span> | <span data-ttu-id="48e38-114">指示是否允许匿名用户启动会议。</span><span class="sxs-lookup"><span data-stu-id="48e38-114">Indicates whether anonymous users are allowed to start a meeting.</span></span>  |
| <span data-ttu-id="48e38-115">autoAdmittedUsers</span><span class="sxs-lookup"><span data-stu-id="48e38-115">autoAdmittedUsers</span></span>                 | <span data-ttu-id="48e38-116">String</span><span class="sxs-lookup"><span data-stu-id="48e38-116">String</span></span>  | <span data-ttu-id="48e38-117">可取值为：`everyoneInCompany`、`everyone`。</span><span class="sxs-lookup"><span data-stu-id="48e38-117">Possible values are: `everyoneInCompany`, `everyone`.</span></span>              |

## <a name="json-representation"></a><span data-ttu-id="48e38-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="48e38-118">JSON representation</span></span>

<span data-ttu-id="48e38-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="48e38-119">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingCapability"
}-->
```json
{
  "allowAnonymousUsersToDialOut": true,
  "allowAnonymousUsersToStartMeeting": true,
  "autoAdmittedUsers": "everyoneInCompany | everyone"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "meetingCapability resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/meetingcapability.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

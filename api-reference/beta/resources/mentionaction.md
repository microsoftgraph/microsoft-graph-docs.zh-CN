---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: MentionAction
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 9101ffed094fd78189b73eab511be88c8bf449de
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513009"
---
# <a name="mentionaction-resource-type"></a><span data-ttu-id="729a6-102">MentionAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="729a6-102">MentionAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="729a6-103">**MentionAction** 资源提供了有关提到人员的[活动][]的信息。</span><span class="sxs-lookup"><span data-stu-id="729a6-103">The **MentionAction** resource provides information about an [activity][] that mentioned people.</span></span>

[活动]: itemactivity.md
[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="729a6-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="729a6-105">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.mentionAction"
}-->

```json
{
  "mentionees": [{"@odata.type": "microsoft.graph.identitySet"}]
}
```

## <a name="properties"></a><span data-ttu-id="729a6-106">属性</span><span class="sxs-lookup"><span data-stu-id="729a6-106">Properties</span></span>

| <span data-ttu-id="729a6-107">属性名称</span><span class="sxs-lookup"><span data-stu-id="729a6-107">Property name</span></span> | <span data-ttu-id="729a6-108">类型</span><span class="sxs-lookup"><span data-stu-id="729a6-108">Type</span></span>                       | <span data-ttu-id="729a6-109">说明</span><span class="sxs-lookup"><span data-stu-id="729a6-109">Description</span></span>
|:--------------|:---------------------------|:-----------------------------
| <span data-ttu-id="729a6-110">mentionees</span><span class="sxs-lookup"><span data-stu-id="729a6-110">mentionees</span></span>    | <span data-ttu-id="729a6-111">[identitySet][] 集合</span><span class="sxs-lookup"><span data-stu-id="729a6-111">[identitySet][] collection</span></span> | <span data-ttu-id="729a6-112">此操作提及的用户的标识。</span><span class="sxs-lookup"><span data-stu-id="729a6-112">The identities of the users mentioned in this action.</span></span>

[identitySet]: identityset.md

## <a name="remarks"></a><span data-ttu-id="729a6-114">注解</span><span class="sxs-lookup"><span data-stu-id="729a6-114">Remarks</span></span>

<span data-ttu-id="729a6-115">项活动记录当前仅在 SharePoint 和 OneDrive for Business 上可用。</span><span class="sxs-lookup"><span data-stu-id="729a6-115">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The MentionAction object provides information about who was mentioned during an activity.",
  "keywords": "activities,activity,action,mention",
  "section": "documentation",
  "tocPath": "Resources/MentionAction",
  "suppressions": [
    "Error: /api-reference/beta/resources/mentionaction.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: MentionAction
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: ad75f3a796f29f7f9c4497a3a15fd31dec0f1c6f
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342266"
---
# <a name="mentionaction-resource-type"></a><span data-ttu-id="fca6f-102">MentionAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="fca6f-102">MentionAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fca6f-103">**MentionAction** 资源提供了有关提到人员的[活动][]的信息。</span><span class="sxs-lookup"><span data-stu-id="fca6f-103">The **MentionAction** resource provides information about an [activity][] that mentioned people.</span></span>

[活动]: itemactivity.md
[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="fca6f-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fca6f-105">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="fca6f-106">属性</span><span class="sxs-lookup"><span data-stu-id="fca6f-106">Properties</span></span>

| <span data-ttu-id="fca6f-107">属性名称</span><span class="sxs-lookup"><span data-stu-id="fca6f-107">Property name</span></span> | <span data-ttu-id="fca6f-108">类型</span><span class="sxs-lookup"><span data-stu-id="fca6f-108">Type</span></span>                       | <span data-ttu-id="fca6f-109">说明</span><span class="sxs-lookup"><span data-stu-id="fca6f-109">Description</span></span>
|:--------------|:---------------------------|:-----------------------------
| <span data-ttu-id="fca6f-110">mentionees</span><span class="sxs-lookup"><span data-stu-id="fca6f-110">mentionees</span></span>    | <span data-ttu-id="fca6f-111">[identitySet][] 集合</span><span class="sxs-lookup"><span data-stu-id="fca6f-111">[identitySet][] collection</span></span> | <span data-ttu-id="fca6f-112">此操作提及的用户的标识。</span><span class="sxs-lookup"><span data-stu-id="fca6f-112">The identities of the users mentioned in this action.</span></span>

[identitySet]: identityset.md

## <a name="remarks"></a><span data-ttu-id="fca6f-114">注解</span><span class="sxs-lookup"><span data-stu-id="fca6f-114">Remarks</span></span>

<span data-ttu-id="fca6f-115">项活动记录当前仅在 SharePoint 和 OneDrive for Business 上可用。</span><span class="sxs-lookup"><span data-stu-id="fca6f-115">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The MentionAction object provides information about who was mentioned during an activity.",
  "keywords": "activities,activity,action,mention",
  "section": "documentation",
  "tocPath": "Resources/MentionAction",
  "suppressions": []
}
-->

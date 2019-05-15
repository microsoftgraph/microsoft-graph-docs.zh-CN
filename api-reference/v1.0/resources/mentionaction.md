---
author: daspek
ms.author: dspektor
title: mentionAction 资源类型
description: MentionAction 对象提供有关在活动过程中提及的内容的信息。
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: d8c09de2a36be2cd83d5e33cf2ed948c25819fe4
ms.sourcegitcommit: 52baf24d1d08096214b12f60e7c755291fe03ab5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2019
ms.locfileid: "33970658"
---
# <a name="mentionaction-resource-type"></a><span data-ttu-id="a5cd3-103">mentionAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="a5cd3-103">mentionAction resource type</span></span>

<span data-ttu-id="a5cd3-104">**MentionAction** 资源提供了有关提到人员的[活动][]的信息。</span><span class="sxs-lookup"><span data-stu-id="a5cd3-104">The **MentionAction** resource provides information about an [activity][] that mentioned people.</span></span>

><span data-ttu-id="a5cd3-105">**注意:** 项目活动记录当前仅在 SharePoint 和 OneDrive for Business 上可用。</span><span class="sxs-lookup"><span data-stu-id="a5cd3-105">**Note:** Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

[活动]: itemactivity.md
[activity]: itemactivity.md

## <a name="properties"></a><span data-ttu-id="a5cd3-107">属性</span><span class="sxs-lookup"><span data-stu-id="a5cd3-107">Properties</span></span>

| <span data-ttu-id="a5cd3-108">属性名称</span><span class="sxs-lookup"><span data-stu-id="a5cd3-108">Property name</span></span> | <span data-ttu-id="a5cd3-109">类型</span><span class="sxs-lookup"><span data-stu-id="a5cd3-109">Type</span></span>                       | <span data-ttu-id="a5cd3-110">说明</span><span class="sxs-lookup"><span data-stu-id="a5cd3-110">Description</span></span>
|:--------------|:---------------------------|:-----------------------------
| <span data-ttu-id="a5cd3-111">mentionees</span><span class="sxs-lookup"><span data-stu-id="a5cd3-111">mentionees</span></span>    | <span data-ttu-id="a5cd3-112">[identitySet][] 集合</span><span class="sxs-lookup"><span data-stu-id="a5cd3-112">[identitySet][] collection</span></span> | <span data-ttu-id="a5cd3-113">此操作提及的用户的标识。</span><span class="sxs-lookup"><span data-stu-id="a5cd3-113">The identities of the users mentioned in this action.</span></span>

[identitySet]: identityset.md

## <a name="json-representation"></a><span data-ttu-id="a5cd3-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a5cd3-115">JSON representation</span></span>

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

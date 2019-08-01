---
author: daspek
ms.author: dspektor
title: mentionAction 资源类型
description: MentionAction 对象提供有关在活动过程中提及的内容的信息。
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 511519439f4079b2d7d618767855582f201c00f7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36036181"
---
# <a name="mentionaction-resource-type"></a><span data-ttu-id="b73a8-103">mentionAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="b73a8-103">mentionAction resource type</span></span>

<span data-ttu-id="b73a8-104">**MentionAction** 资源提供了有关提到人员的[活动][]的信息。</span><span class="sxs-lookup"><span data-stu-id="b73a8-104">The **MentionAction** resource provides information about an [activity][] that mentioned people.</span></span>

><span data-ttu-id="b73a8-105">**注意:** 项目活动记录当前仅在 SharePoint 和 OneDrive for Business 上可用。</span><span class="sxs-lookup"><span data-stu-id="b73a8-105">**Note:** Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

[活动]: itemactivity.md
[activity]: itemactivity.md

## <a name="properties"></a><span data-ttu-id="b73a8-107">属性</span><span class="sxs-lookup"><span data-stu-id="b73a8-107">Properties</span></span>

| <span data-ttu-id="b73a8-108">属性名称</span><span class="sxs-lookup"><span data-stu-id="b73a8-108">Property name</span></span> | <span data-ttu-id="b73a8-109">类型</span><span class="sxs-lookup"><span data-stu-id="b73a8-109">Type</span></span>                       | <span data-ttu-id="b73a8-110">说明</span><span class="sxs-lookup"><span data-stu-id="b73a8-110">Description</span></span>
|:--------------|:---------------------------|:-----------------------------
| <span data-ttu-id="b73a8-111">mentionees</span><span class="sxs-lookup"><span data-stu-id="b73a8-111">mentionees</span></span>    | <span data-ttu-id="b73a8-112">[identitySet][] 集合</span><span class="sxs-lookup"><span data-stu-id="b73a8-112">[identitySet][] collection</span></span> | <span data-ttu-id="b73a8-113">此操作提及的用户的标识。</span><span class="sxs-lookup"><span data-stu-id="b73a8-113">The identities of the users mentioned in this action.</span></span>

[identitySet]: identityset.md

## <a name="json-representation"></a><span data-ttu-id="b73a8-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b73a8-115">JSON representation</span></span>

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

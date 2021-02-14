---
author: daspek
title: mentionAction 资源类型
description: MentionAction 对象提供有关在活动期间被提及者的信息。
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: bc876f05949beb09b3e495a8b9b0536070b352cb
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/14/2021
ms.locfileid: "50238384"
---
# <a name="mentionaction-resource-type"></a><span data-ttu-id="b9fab-103">mentionAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="b9fab-103">mentionAction resource type</span></span>

<span data-ttu-id="b9fab-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b9fab-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b9fab-105">**MentionAction** 资源提供了有关提到人员的 [活动][]的信息。</span><span class="sxs-lookup"><span data-stu-id="b9fab-105">The **MentionAction** resource provides information about an [activity][] that mentioned people.</span></span>

><span data-ttu-id="b9fab-106">**注意：** 项目活动记录当前仅在 SharePoint 和 OneDrive for Business 上可用。</span><span class="sxs-lookup"><span data-stu-id="b9fab-106">**Note:** Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

[活动]: itemactivity.md
[activity]: itemactivity.md

## <a name="properties"></a><span data-ttu-id="b9fab-108">属性</span><span class="sxs-lookup"><span data-stu-id="b9fab-108">Properties</span></span>

| <span data-ttu-id="b9fab-109">属性名称</span><span class="sxs-lookup"><span data-stu-id="b9fab-109">Property name</span></span> | <span data-ttu-id="b9fab-110">类型</span><span class="sxs-lookup"><span data-stu-id="b9fab-110">Type</span></span>                       | <span data-ttu-id="b9fab-111">说明</span><span class="sxs-lookup"><span data-stu-id="b9fab-111">Description</span></span>
|:--------------|:---------------------------|:-----------------------------
| <span data-ttu-id="b9fab-112">mentionees</span><span class="sxs-lookup"><span data-stu-id="b9fab-112">mentionees</span></span>    | <span data-ttu-id="b9fab-113">[identitySet][] 集合</span><span class="sxs-lookup"><span data-stu-id="b9fab-113">[identitySet][] collection</span></span> | <span data-ttu-id="b9fab-114">此操作提及的用户的标识。</span><span class="sxs-lookup"><span data-stu-id="b9fab-114">The identities of the users mentioned in this action.</span></span>

[identitySet]: identityset.md

## <a name="json-representation"></a><span data-ttu-id="b9fab-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b9fab-116">JSON representation</span></span>

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


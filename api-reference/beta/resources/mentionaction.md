---
author: daspek
description: MentionAction 资源提供了有关提到人员的活动的信息。
ms.date: 09/14/2017
title: MentionAction
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: b0f8376c3fcc86cdd16c1eeb32507e5b26469285
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47971600"
---
# <a name="mentionaction-resource-type"></a><span data-ttu-id="cd5e0-103">MentionAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="cd5e0-103">MentionAction resource type</span></span>

<span data-ttu-id="cd5e0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cd5e0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cd5e0-105">**MentionAction** 资源提供了有关提到人员的[活动][]的信息。</span><span class="sxs-lookup"><span data-stu-id="cd5e0-105">The **MentionAction** resource provides information about an [activity][] that mentioned people.</span></span>

[活动]: itemactivity.md
[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="cd5e0-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cd5e0-107">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="cd5e0-108">属性</span><span class="sxs-lookup"><span data-stu-id="cd5e0-108">Properties</span></span>

| <span data-ttu-id="cd5e0-109">属性名称</span><span class="sxs-lookup"><span data-stu-id="cd5e0-109">Property name</span></span> | <span data-ttu-id="cd5e0-110">类型</span><span class="sxs-lookup"><span data-stu-id="cd5e0-110">Type</span></span>                       | <span data-ttu-id="cd5e0-111">说明</span><span class="sxs-lookup"><span data-stu-id="cd5e0-111">Description</span></span>
|:--------------|:---------------------------|:-----------------------------
| <span data-ttu-id="cd5e0-112">mentionees</span><span class="sxs-lookup"><span data-stu-id="cd5e0-112">mentionees</span></span>    | <span data-ttu-id="cd5e0-113">[identitySet][] 集合</span><span class="sxs-lookup"><span data-stu-id="cd5e0-113">[identitySet][] collection</span></span> | <span data-ttu-id="cd5e0-114">此操作提及的用户的标识。</span><span class="sxs-lookup"><span data-stu-id="cd5e0-114">The identities of the users mentioned in this action.</span></span>

[identitySet]: identityset.md

## <a name="remarks"></a><span data-ttu-id="cd5e0-116">注解</span><span class="sxs-lookup"><span data-stu-id="cd5e0-116">Remarks</span></span>

<span data-ttu-id="cd5e0-117">项活动记录当前仅在 SharePoint 和 OneDrive for Business 上可用。</span><span class="sxs-lookup"><span data-stu-id="cd5e0-117">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

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



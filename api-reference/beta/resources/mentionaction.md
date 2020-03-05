---
author: daspek
description: MentionAction 资源提供了有关提到人员的活动的信息。
ms.date: 09/14/2017
title: MentionAction
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 2e2a430ed25dd6a64049fc6dc49c282bf6a47e00
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522692"
---
# <a name="mentionaction-resource-type"></a><span data-ttu-id="c0755-103">MentionAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="c0755-103">MentionAction resource type</span></span>

<span data-ttu-id="c0755-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="c0755-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c0755-105">**MentionAction** 资源提供了有关提到人员的[活动][]的信息。</span><span class="sxs-lookup"><span data-stu-id="c0755-105">The **MentionAction** resource provides information about an [activity][] that mentioned people.</span></span>

[活动]: itemactivity.md
[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="c0755-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c0755-107">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="c0755-108">属性</span><span class="sxs-lookup"><span data-stu-id="c0755-108">Properties</span></span>

| <span data-ttu-id="c0755-109">属性名称</span><span class="sxs-lookup"><span data-stu-id="c0755-109">Property name</span></span> | <span data-ttu-id="c0755-110">类型</span><span class="sxs-lookup"><span data-stu-id="c0755-110">Type</span></span>                       | <span data-ttu-id="c0755-111">说明</span><span class="sxs-lookup"><span data-stu-id="c0755-111">Description</span></span>
|:--------------|:---------------------------|:-----------------------------
| <span data-ttu-id="c0755-112">mentionees</span><span class="sxs-lookup"><span data-stu-id="c0755-112">mentionees</span></span>    | <span data-ttu-id="c0755-113">[identitySet][] 集合</span><span class="sxs-lookup"><span data-stu-id="c0755-113">[identitySet][] collection</span></span> | <span data-ttu-id="c0755-114">此操作提及的用户的标识。</span><span class="sxs-lookup"><span data-stu-id="c0755-114">The identities of the users mentioned in this action.</span></span>

[identitySet]: identityset.md

## <a name="remarks"></a><span data-ttu-id="c0755-116">注解</span><span class="sxs-lookup"><span data-stu-id="c0755-116">Remarks</span></span>

<span data-ttu-id="c0755-117">项活动记录当前仅在 SharePoint 和 OneDrive for Business 上可用。</span><span class="sxs-lookup"><span data-stu-id="c0755-117">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

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

---
author: daspek
description: MentionAction 资源提供了有关提到人员的活动的信息。
ms.date: 09/14/2017
title: MentionAction
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 1b08233569fe655b5a8f0e878c4e14d178be279f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966816"
---
# <a name="mentionaction-resource-type"></a><span data-ttu-id="eb708-103">MentionAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="eb708-103">MentionAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eb708-104">**MentionAction** 资源提供了有关提到人员的[活动][]的信息。</span><span class="sxs-lookup"><span data-stu-id="eb708-104">The **MentionAction** resource provides information about an [activity][] that mentioned people.</span></span>

[活动]: itemactivity.md
[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="eb708-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="eb708-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="eb708-107">属性</span><span class="sxs-lookup"><span data-stu-id="eb708-107">Properties</span></span>

| <span data-ttu-id="eb708-108">属性名称</span><span class="sxs-lookup"><span data-stu-id="eb708-108">Property name</span></span> | <span data-ttu-id="eb708-109">类型</span><span class="sxs-lookup"><span data-stu-id="eb708-109">Type</span></span>                       | <span data-ttu-id="eb708-110">说明</span><span class="sxs-lookup"><span data-stu-id="eb708-110">Description</span></span>
|:--------------|:---------------------------|:-----------------------------
| <span data-ttu-id="eb708-111">mentionees</span><span class="sxs-lookup"><span data-stu-id="eb708-111">mentionees</span></span>    | <span data-ttu-id="eb708-112">[identitySet][] 集合</span><span class="sxs-lookup"><span data-stu-id="eb708-112">[identitySet][] collection</span></span> | <span data-ttu-id="eb708-113">此操作提及的用户的标识。</span><span class="sxs-lookup"><span data-stu-id="eb708-113">The identities of the users mentioned in this action.</span></span>

[identitySet]: identityset.md

## <a name="remarks"></a><span data-ttu-id="eb708-115">注解</span><span class="sxs-lookup"><span data-stu-id="eb708-115">Remarks</span></span>

<span data-ttu-id="eb708-116">项活动记录当前仅在 SharePoint 和 OneDrive for Business 上可用。</span><span class="sxs-lookup"><span data-stu-id="eb708-116">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

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

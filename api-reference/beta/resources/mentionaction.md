---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: MentionAction
localization_priority: Normal
ms.openlocfilehash: 7843feebd8ebca2022b276007d21a89b754217a0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27804968"
---
# <a name="mentionaction-resource-type"></a><span data-ttu-id="c5e53-102">MentionAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="c5e53-102">MentionAction resource type</span></span>

> <span data-ttu-id="c5e53-103">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="c5e53-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c5e53-104">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c5e53-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c5e53-105">**MentionAction** 资源提供了有关提到人员的[活动][]的信息。</span><span class="sxs-lookup"><span data-stu-id="c5e53-105">The **MentionAction** resource provides information about an [activity][] that mentioned people.</span></span>

[活动]: itemactivity.md
[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="c5e53-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c5e53-107">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="c5e53-108">属性</span><span class="sxs-lookup"><span data-stu-id="c5e53-108">Properties</span></span>

| <span data-ttu-id="c5e53-109">属性名称</span><span class="sxs-lookup"><span data-stu-id="c5e53-109">Property name</span></span> | <span data-ttu-id="c5e53-110">类型</span><span class="sxs-lookup"><span data-stu-id="c5e53-110">Type</span></span>                       | <span data-ttu-id="c5e53-111">说明</span><span class="sxs-lookup"><span data-stu-id="c5e53-111">Description</span></span>
|:--------------|:---------------------------|:-----------------------------
| <span data-ttu-id="c5e53-112">mentionees</span><span class="sxs-lookup"><span data-stu-id="c5e53-112">mentionees</span></span>    | <span data-ttu-id="c5e53-113">[identitySet][] 集合</span><span class="sxs-lookup"><span data-stu-id="c5e53-113">[identitySet][] collection</span></span> | <span data-ttu-id="c5e53-114">此操作提及的用户的标识。</span><span class="sxs-lookup"><span data-stu-id="c5e53-114">The identities of the users mentioned in this action.</span></span>

[identitySet]: identityset.md

## <a name="remarks"></a><span data-ttu-id="c5e53-116">注解</span><span class="sxs-lookup"><span data-stu-id="c5e53-116">Remarks</span></span>

<span data-ttu-id="c5e53-117">项活动记录当前仅在 SharePoint 和 OneDrive for Business 上可用。</span><span class="sxs-lookup"><span data-stu-id="c5e53-117">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The MentionAction object provides information about who was mentioned during an activity.",
  "keywords": "activities,activity,action,mention",
  "section": "documentation",
  "tocPath": "Resources/MentionAction"
} -->

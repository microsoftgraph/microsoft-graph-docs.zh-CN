---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: MentionAction
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 48ac49c80a39fd6bc51b048a8eb7dab6e62da810
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27974138"
---
# <a name="mentionaction-resource-type"></a><span data-ttu-id="f0027-102">MentionAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="f0027-102">MentionAction resource type</span></span>

> <span data-ttu-id="f0027-103">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="f0027-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f0027-104">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="f0027-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f0027-105">**MentionAction** 资源提供了有关提到人员的[活动][]的信息。</span><span class="sxs-lookup"><span data-stu-id="f0027-105">The **MentionAction** resource provides information about an [activity][] that mentioned people.</span></span>

[活动]: itemactivity.md
[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="f0027-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f0027-107">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="f0027-108">属性</span><span class="sxs-lookup"><span data-stu-id="f0027-108">Properties</span></span>

| <span data-ttu-id="f0027-109">属性名称</span><span class="sxs-lookup"><span data-stu-id="f0027-109">Property name</span></span> | <span data-ttu-id="f0027-110">类型</span><span class="sxs-lookup"><span data-stu-id="f0027-110">Type</span></span>                       | <span data-ttu-id="f0027-111">说明</span><span class="sxs-lookup"><span data-stu-id="f0027-111">Description</span></span>
|:--------------|:---------------------------|:-----------------------------
| <span data-ttu-id="f0027-112">mentionees</span><span class="sxs-lookup"><span data-stu-id="f0027-112">mentionees</span></span>    | <span data-ttu-id="f0027-113">[identitySet][] 集合</span><span class="sxs-lookup"><span data-stu-id="f0027-113">[identitySet][] collection</span></span> | <span data-ttu-id="f0027-114">此操作提及的用户的标识。</span><span class="sxs-lookup"><span data-stu-id="f0027-114">The identities of the users mentioned in this action.</span></span>

[identitySet]: identityset.md

## <a name="remarks"></a><span data-ttu-id="f0027-116">注解</span><span class="sxs-lookup"><span data-stu-id="f0027-116">Remarks</span></span>

<span data-ttu-id="f0027-117">项活动记录当前仅在 SharePoint 和 OneDrive for Business 上可用。</span><span class="sxs-lookup"><span data-stu-id="f0027-117">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The MentionAction object provides information about who was mentioned during an activity.",
  "keywords": "activities,activity,action,mention",
  "section": "documentation",
  "tocPath": "Resources/MentionAction"
} -->

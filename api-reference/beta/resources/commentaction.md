---
author: daspek
description: CommentAction 资源提供有关对某个项所做的注释活动的信息。
ms.date: 09/14/2017
title: CommentAction
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: b7782c6e4dd30b503a9be88737ef6bd2dbad109b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973256"
---
# <a name="commentaction-resource-type"></a><span data-ttu-id="71cc0-103">CommentAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="71cc0-103">CommentAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="71cc0-104">**CommentAction** 资源提供有关对某个项所做的注释[活动][]的信息。</span><span class="sxs-lookup"><span data-stu-id="71cc0-104">The **CommentAction** resource provides information about a comment [activity][] made on an item.</span></span>

[活动]: itemactivity.md
[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="71cc0-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="71cc0-106">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.commentAction"
}-->

```json
{
  "isReply": false,
  "parentAuthor": {"@odata.type": "microsoft.graph.identitySet"},
  "participants": [{"@odata.type": "microsoft.graph.identitySet"}]
}
```

## <a name="properties"></a><span data-ttu-id="71cc0-107">属性</span><span class="sxs-lookup"><span data-stu-id="71cc0-107">Properties</span></span>

| <span data-ttu-id="71cc0-108">属性名称</span><span class="sxs-lookup"><span data-stu-id="71cc0-108">Property name</span></span>    | <span data-ttu-id="71cc0-109">类型</span><span class="sxs-lookup"><span data-stu-id="71cc0-109">Type</span></span>                       | <span data-ttu-id="71cc0-110">说明</span><span class="sxs-lookup"><span data-stu-id="71cc0-110">Description</span></span>
|:-----------------|:---------------------------|:-----------------------------
| <span data-ttu-id="71cc0-111">isReply</span><span class="sxs-lookup"><span data-stu-id="71cc0-111">isReply</span></span>          | <span data-ttu-id="71cc0-112">boolean</span><span class="sxs-lookup"><span data-stu-id="71cc0-112">boolean</span></span>                    | <span data-ttu-id="71cc0-113">如果为 true，此活动是对现有注释线程的回复。</span><span class="sxs-lookup"><span data-stu-id="71cc0-113">If true, this activity was a reply to an existing comment thread.</span></span>
| <span data-ttu-id="71cc0-114">parentAuthor</span><span class="sxs-lookup"><span data-stu-id="71cc0-114">parentAuthor</span></span>     | <span data-ttu-id="71cc0-115">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="71cc0-115">[identitySet][]</span></span>            | <span data-ttu-id="71cc0-116">启动注释线程的用户的标识。</span><span class="sxs-lookup"><span data-stu-id="71cc0-116">The identity of the user who started the comment thread.</span></span>
| <span data-ttu-id="71cc0-117">participants</span><span class="sxs-lookup"><span data-stu-id="71cc0-117">participants</span></span>     | <span data-ttu-id="71cc0-118">[identitySet][] 集合</span><span class="sxs-lookup"><span data-stu-id="71cc0-118">[identitySet][] collection</span></span> | <span data-ttu-id="71cc0-119">参与此注释线程的用户的标识。</span><span class="sxs-lookup"><span data-stu-id="71cc0-119">The identities of the users participating in this comment thread.</span></span>

[identitySet]: identityset.md

## <a name="remarks"></a><span data-ttu-id="71cc0-121">注解</span><span class="sxs-lookup"><span data-stu-id="71cc0-121">Remarks</span></span>

<span data-ttu-id="71cc0-122">项活动记录当前仅在 SharePoint 和 OneDrive for Business 上可用。</span><span class="sxs-lookup"><span data-stu-id="71cc0-122">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The CommentAction object provides information about a comment that was made on an item.",
  "keywords": "activities,activity,action,comment",
  "section": "documentation",
  "tocPath": "Resources/CommentAction",
  "suppressions": []
}
-->

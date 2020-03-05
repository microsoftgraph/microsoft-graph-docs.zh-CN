---
author: daspek
description: CommentAction 资源提供有关对某个项所做的注释活动的信息。
ms.date: 09/14/2017
title: CommentAction
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 26b521bbc6ccb94abd2e5a494fae9de10cfacedf
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507609"
---
# <a name="commentaction-resource-type"></a><span data-ttu-id="4730e-103">CommentAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="4730e-103">CommentAction resource type</span></span>

<span data-ttu-id="4730e-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="4730e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4730e-105">**CommentAction** 资源提供有关对某个项所做的注释[活动][]的信息。</span><span class="sxs-lookup"><span data-stu-id="4730e-105">The **CommentAction** resource provides information about a comment [activity][] made on an item.</span></span>

[活动]: itemactivity.md
[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="4730e-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4730e-107">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="4730e-108">属性</span><span class="sxs-lookup"><span data-stu-id="4730e-108">Properties</span></span>

| <span data-ttu-id="4730e-109">属性名称</span><span class="sxs-lookup"><span data-stu-id="4730e-109">Property name</span></span>    | <span data-ttu-id="4730e-110">类型</span><span class="sxs-lookup"><span data-stu-id="4730e-110">Type</span></span>                       | <span data-ttu-id="4730e-111">说明</span><span class="sxs-lookup"><span data-stu-id="4730e-111">Description</span></span>
|:-----------------|:---------------------------|:-----------------------------
| <span data-ttu-id="4730e-112">isReply</span><span class="sxs-lookup"><span data-stu-id="4730e-112">isReply</span></span>          | <span data-ttu-id="4730e-113">boolean</span><span class="sxs-lookup"><span data-stu-id="4730e-113">boolean</span></span>                    | <span data-ttu-id="4730e-114">如果为 true，此活动是对现有注释线程的回复。</span><span class="sxs-lookup"><span data-stu-id="4730e-114">If true, this activity was a reply to an existing comment thread.</span></span>
| <span data-ttu-id="4730e-115">parentAuthor</span><span class="sxs-lookup"><span data-stu-id="4730e-115">parentAuthor</span></span>     | <span data-ttu-id="4730e-116">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="4730e-116">[identitySet][]</span></span>            | <span data-ttu-id="4730e-117">启动注释线程的用户的标识。</span><span class="sxs-lookup"><span data-stu-id="4730e-117">The identity of the user who started the comment thread.</span></span>
| <span data-ttu-id="4730e-118">participants</span><span class="sxs-lookup"><span data-stu-id="4730e-118">participants</span></span>     | <span data-ttu-id="4730e-119">[identitySet][] 集合</span><span class="sxs-lookup"><span data-stu-id="4730e-119">[identitySet][] collection</span></span> | <span data-ttu-id="4730e-120">参与此注释线程的用户的标识。</span><span class="sxs-lookup"><span data-stu-id="4730e-120">The identities of the users participating in this comment thread.</span></span>

[identitySet]: identityset.md

## <a name="remarks"></a><span data-ttu-id="4730e-122">注解</span><span class="sxs-lookup"><span data-stu-id="4730e-122">Remarks</span></span>

<span data-ttu-id="4730e-123">项活动记录当前仅在 SharePoint 和 OneDrive for Business 上可用。</span><span class="sxs-lookup"><span data-stu-id="4730e-123">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

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

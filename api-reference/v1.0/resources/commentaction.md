---
author: daspek
ms.author: dspektor
title: commentAction 资源类型
description: CommentAction 对象提供有关对项目所做的注释的信息。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 12e6cd68d5809b8e4c1765234eeb77b40b30a78e
ms.sourcegitcommit: 52baf24d1d08096214b12f60e7c755291fe03ab5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2019
ms.locfileid: "33970629"
---
# <a name="commentaction-resource-type"></a><span data-ttu-id="a4e60-103">commentAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="a4e60-103">commentAction resource type</span></span>

<span data-ttu-id="a4e60-104">**CommentAction**资源提供有关对项目进行的注释[活动][]的信息。</span><span class="sxs-lookup"><span data-stu-id="a4e60-104">The **commentAction** resource provides information about a comment [activity][] made on an item.</span></span>

><span data-ttu-id="a4e60-105">**注意:** 项目活动记录当前仅在 SharePoint 和 OneDrive for Business 上可用。</span><span class="sxs-lookup"><span data-stu-id="a4e60-105">**Note:** Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

[活动]: itemactivity.md
[activity]: itemactivity.md

## <a name="properties"></a><span data-ttu-id="a4e60-107">属性</span><span class="sxs-lookup"><span data-stu-id="a4e60-107">Properties</span></span>

| <span data-ttu-id="a4e60-108">属性名称</span><span class="sxs-lookup"><span data-stu-id="a4e60-108">Property name</span></span>    | <span data-ttu-id="a4e60-109">类型</span><span class="sxs-lookup"><span data-stu-id="a4e60-109">Type</span></span>                       | <span data-ttu-id="a4e60-110">说明</span><span class="sxs-lookup"><span data-stu-id="a4e60-110">Description</span></span>
|:-----------------|:---------------------------|:-----------------------------
| <span data-ttu-id="a4e60-111">isReply</span><span class="sxs-lookup"><span data-stu-id="a4e60-111">isReply</span></span>          | <span data-ttu-id="a4e60-112">boolean</span><span class="sxs-lookup"><span data-stu-id="a4e60-112">boolean</span></span>                    | <span data-ttu-id="a4e60-113">如果为 true，此活动是对现有注释线程的回复。</span><span class="sxs-lookup"><span data-stu-id="a4e60-113">If true, this activity was a reply to an existing comment thread.</span></span>
| <span data-ttu-id="a4e60-114">parentAuthor</span><span class="sxs-lookup"><span data-stu-id="a4e60-114">parentAuthor</span></span>     | <span data-ttu-id="a4e60-115">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="a4e60-115">[identitySet][]</span></span>            | <span data-ttu-id="a4e60-116">启动注释线程的用户的标识。</span><span class="sxs-lookup"><span data-stu-id="a4e60-116">The identity of the user who started the comment thread.</span></span>
| <span data-ttu-id="a4e60-117">participants</span><span class="sxs-lookup"><span data-stu-id="a4e60-117">participants</span></span>     | <span data-ttu-id="a4e60-118">[identitySet][] 集合</span><span class="sxs-lookup"><span data-stu-id="a4e60-118">[identitySet][] collection</span></span> | <span data-ttu-id="a4e60-119">参与此注释线程的用户的标识。</span><span class="sxs-lookup"><span data-stu-id="a4e60-119">The identities of the users participating in this comment thread.</span></span>

[identitySet]: identityset.md

## <a name="json-representation"></a><span data-ttu-id="a4e60-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a4e60-121">JSON representation</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "The commentAction object provides information about a comment that was made on an item.",
  "keywords": "activities,activity,action,comment",
  "section": "documentation",
  "tocPath": "Resources/commentAction",
  "suppressions": []
}
-->

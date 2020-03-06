---
author: daspek
ms.author: dspektor
title: commentAction 资源类型
description: CommentAction 对象提供有关对项目所做的注释的信息。
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: f3720d84624fa728a168515beb28422ab355b335
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531807"
---
# <a name="commentaction-resource-type"></a><span data-ttu-id="548a6-103">commentAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="548a6-103">commentAction resource type</span></span>

<span data-ttu-id="548a6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="548a6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="548a6-105">**CommentAction**资源提供有关对项目进行的注释[活动][]的信息。</span><span class="sxs-lookup"><span data-stu-id="548a6-105">The **commentAction** resource provides information about a comment [activity][] made on an item.</span></span>

><span data-ttu-id="548a6-106">**注意：** 项目活动记录当前仅在 SharePoint 和 OneDrive for Business 上可用。</span><span class="sxs-lookup"><span data-stu-id="548a6-106">**Note:** Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

[活动]: itemactivity.md
[activity]: itemactivity.md

## <a name="properties"></a><span data-ttu-id="548a6-108">属性</span><span class="sxs-lookup"><span data-stu-id="548a6-108">Properties</span></span>

| <span data-ttu-id="548a6-109">属性名称</span><span class="sxs-lookup"><span data-stu-id="548a6-109">Property name</span></span>    | <span data-ttu-id="548a6-110">类型</span><span class="sxs-lookup"><span data-stu-id="548a6-110">Type</span></span>                       | <span data-ttu-id="548a6-111">说明</span><span class="sxs-lookup"><span data-stu-id="548a6-111">Description</span></span>
|:-----------------|:---------------------------|:-----------------------------
| <span data-ttu-id="548a6-112">isReply</span><span class="sxs-lookup"><span data-stu-id="548a6-112">isReply</span></span>          | <span data-ttu-id="548a6-113">boolean</span><span class="sxs-lookup"><span data-stu-id="548a6-113">boolean</span></span>                    | <span data-ttu-id="548a6-114">如果为 true，此活动是对现有注释线程的回复。</span><span class="sxs-lookup"><span data-stu-id="548a6-114">If true, this activity was a reply to an existing comment thread.</span></span>
| <span data-ttu-id="548a6-115">parentAuthor</span><span class="sxs-lookup"><span data-stu-id="548a6-115">parentAuthor</span></span>     | <span data-ttu-id="548a6-116">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="548a6-116">[identitySet][]</span></span>            | <span data-ttu-id="548a6-117">启动注释线程的用户的标识。</span><span class="sxs-lookup"><span data-stu-id="548a6-117">The identity of the user who started the comment thread.</span></span>
| <span data-ttu-id="548a6-118">participants</span><span class="sxs-lookup"><span data-stu-id="548a6-118">participants</span></span>     | <span data-ttu-id="548a6-119">[identitySet][] 集合</span><span class="sxs-lookup"><span data-stu-id="548a6-119">[identitySet][] collection</span></span> | <span data-ttu-id="548a6-120">参与此注释线程的用户的标识。</span><span class="sxs-lookup"><span data-stu-id="548a6-120">The identities of the users participating in this comment thread.</span></span>

[identitySet]: identityset.md

## <a name="json-representation"></a><span data-ttu-id="548a6-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="548a6-122">JSON representation</span></span>

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

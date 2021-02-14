---
author: daspek
title: commentAction 资源类型
description: commentAction 对象提供有关对项目进行注释的信息。
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: f2f3ab7f0798ee1020b107c38262a912fdae53ef
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/14/2021
ms.locfileid: "50238412"
---
# <a name="commentaction-resource-type"></a><span data-ttu-id="7ef02-103">commentAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="7ef02-103">commentAction resource type</span></span>

<span data-ttu-id="7ef02-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7ef02-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7ef02-105">**commentAction** 资源提供有关对项目进行注释 [][]活动的信息。</span><span class="sxs-lookup"><span data-stu-id="7ef02-105">The **commentAction** resource provides information about a comment [activity][] made on an item.</span></span>

><span data-ttu-id="7ef02-106">**注意：** 项目活动记录当前仅在 SharePoint 和 OneDrive for Business 上可用。</span><span class="sxs-lookup"><span data-stu-id="7ef02-106">**Note:** Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

[活动]: itemactivity.md
[activity]: itemactivity.md

## <a name="properties"></a><span data-ttu-id="7ef02-108">属性</span><span class="sxs-lookup"><span data-stu-id="7ef02-108">Properties</span></span>

| <span data-ttu-id="7ef02-109">属性名称</span><span class="sxs-lookup"><span data-stu-id="7ef02-109">Property name</span></span>    | <span data-ttu-id="7ef02-110">类型</span><span class="sxs-lookup"><span data-stu-id="7ef02-110">Type</span></span>                       | <span data-ttu-id="7ef02-111">说明</span><span class="sxs-lookup"><span data-stu-id="7ef02-111">Description</span></span>
|:-----------------|:---------------------------|:-----------------------------
| <span data-ttu-id="7ef02-112">isReply</span><span class="sxs-lookup"><span data-stu-id="7ef02-112">isReply</span></span>          | <span data-ttu-id="7ef02-113">boolean</span><span class="sxs-lookup"><span data-stu-id="7ef02-113">boolean</span></span>                    | <span data-ttu-id="7ef02-114">如果为 true，此活动是对现有注释线程的回复。</span><span class="sxs-lookup"><span data-stu-id="7ef02-114">If true, this activity was a reply to an existing comment thread.</span></span>
| <span data-ttu-id="7ef02-115">parentAuthor</span><span class="sxs-lookup"><span data-stu-id="7ef02-115">parentAuthor</span></span>     | <span data-ttu-id="7ef02-116">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="7ef02-116">[identitySet][]</span></span>            | <span data-ttu-id="7ef02-117">启动注释线程的用户的标识。</span><span class="sxs-lookup"><span data-stu-id="7ef02-117">The identity of the user who started the comment thread.</span></span>
| <span data-ttu-id="7ef02-118">participants</span><span class="sxs-lookup"><span data-stu-id="7ef02-118">participants</span></span>     | <span data-ttu-id="7ef02-119">[identitySet][] 集合</span><span class="sxs-lookup"><span data-stu-id="7ef02-119">[identitySet][] collection</span></span> | <span data-ttu-id="7ef02-120">参与此注释线程的用户的标识。</span><span class="sxs-lookup"><span data-stu-id="7ef02-120">The identities of the users participating in this comment thread.</span></span>

[identitySet]: identityset.md

## <a name="json-representation"></a><span data-ttu-id="7ef02-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7ef02-122">JSON representation</span></span>

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


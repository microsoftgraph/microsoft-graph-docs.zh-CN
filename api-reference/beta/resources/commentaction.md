---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: CommentAction
ms.openlocfilehash: 92dc26945cd591de2ba107907a593159f1e128c9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27049161"
---
# <a name="commentaction-resource-type"></a><span data-ttu-id="a9bd8-102">CommentAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="a9bd8-102">CommentAction resource type</span></span>

> <span data-ttu-id="a9bd8-103">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="a9bd8-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a9bd8-104">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a9bd8-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a9bd8-105">**CommentAction** 资源提供有关对某个项所做的注释[活动][]的信息。</span><span class="sxs-lookup"><span data-stu-id="a9bd8-105">The **CommentAction** resource provides information about a comment [activity][] made on an item.</span></span>

[活动]: itemactivity.md
[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="a9bd8-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a9bd8-107">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="a9bd8-108">属性</span><span class="sxs-lookup"><span data-stu-id="a9bd8-108">Properties</span></span>

| <span data-ttu-id="a9bd8-109">属性名称</span><span class="sxs-lookup"><span data-stu-id="a9bd8-109">Property name</span></span>    | <span data-ttu-id="a9bd8-110">类型</span><span class="sxs-lookup"><span data-stu-id="a9bd8-110">Type</span></span>                       | <span data-ttu-id="a9bd8-111">说明</span><span class="sxs-lookup"><span data-stu-id="a9bd8-111">Description</span></span>
|:-----------------|:---------------------------|:-----------------------------
| <span data-ttu-id="a9bd8-112">isReply</span><span class="sxs-lookup"><span data-stu-id="a9bd8-112">isReply</span></span>          | <span data-ttu-id="a9bd8-113">boolean</span><span class="sxs-lookup"><span data-stu-id="a9bd8-113">boolean</span></span>                    | <span data-ttu-id="a9bd8-114">如果为 true，此活动是对现有注释线程的回复。</span><span class="sxs-lookup"><span data-stu-id="a9bd8-114">If true, this activity was a reply to an existing comment thread.</span></span>
| <span data-ttu-id="a9bd8-115">parentAuthor</span><span class="sxs-lookup"><span data-stu-id="a9bd8-115">parentAuthor</span></span>     | <span data-ttu-id="a9bd8-116">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="a9bd8-116">[identitySet][]</span></span>            | <span data-ttu-id="a9bd8-117">启动注释线程的用户的标识。</span><span class="sxs-lookup"><span data-stu-id="a9bd8-117">The identity of the user who started the comment thread.</span></span>
| <span data-ttu-id="a9bd8-118">participants</span><span class="sxs-lookup"><span data-stu-id="a9bd8-118">participants</span></span>     | <span data-ttu-id="a9bd8-119">[identitySet][] 集合</span><span class="sxs-lookup"><span data-stu-id="a9bd8-119">[identitySet][] collection</span></span> | <span data-ttu-id="a9bd8-120">参与此注释线程的用户的标识。</span><span class="sxs-lookup"><span data-stu-id="a9bd8-120">The identities of the users participating in this comment thread.</span></span>

[identitySet]: identityset.md

## <a name="remarks"></a><span data-ttu-id="a9bd8-122">注解</span><span class="sxs-lookup"><span data-stu-id="a9bd8-122">Remarks</span></span>

<span data-ttu-id="a9bd8-123">项活动记录当前仅在 SharePoint 和 OneDrive for Business 上可用。</span><span class="sxs-lookup"><span data-stu-id="a9bd8-123">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The CommentAction object provides information about a comment that was made on an item.",
  "keywords": "activities,activity,action,comment",
  "section": "documentation",
  "tocPath": "Resources/CommentAction"
} -->

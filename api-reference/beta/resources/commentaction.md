---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: CommentAction
localization_priority: Normal
ms.openlocfilehash: e674c996002b3a54c92886dd1c5dca7a76c56b51
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543460"
---
# <a name="commentaction-resource-type"></a><span data-ttu-id="3e650-102">CommentAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="3e650-102">CommentAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3e650-103">**CommentAction** 资源提供有关对某个项所做的注释[活动][]的信息。</span><span class="sxs-lookup"><span data-stu-id="3e650-103">The **CommentAction** resource provides information about a comment [activity][] made on an item.</span></span>

[活动]: itemactivity.md
[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="3e650-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3e650-105">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="3e650-106">属性</span><span class="sxs-lookup"><span data-stu-id="3e650-106">Properties</span></span>

| <span data-ttu-id="3e650-107">属性名称</span><span class="sxs-lookup"><span data-stu-id="3e650-107">Property name</span></span>    | <span data-ttu-id="3e650-108">类型</span><span class="sxs-lookup"><span data-stu-id="3e650-108">Type</span></span>                       | <span data-ttu-id="3e650-109">说明</span><span class="sxs-lookup"><span data-stu-id="3e650-109">Description</span></span>
|:-----------------|:---------------------------|:-----------------------------
| <span data-ttu-id="3e650-110">isReply</span><span class="sxs-lookup"><span data-stu-id="3e650-110">isReply</span></span>          | <span data-ttu-id="3e650-111">boolean</span><span class="sxs-lookup"><span data-stu-id="3e650-111">boolean</span></span>                    | <span data-ttu-id="3e650-112">如果为 true，此活动是对现有注释线程的回复。</span><span class="sxs-lookup"><span data-stu-id="3e650-112">If true, this activity was a reply to an existing comment thread.</span></span>
| <span data-ttu-id="3e650-113">parentAuthor</span><span class="sxs-lookup"><span data-stu-id="3e650-113">parentAuthor</span></span>     | <span data-ttu-id="3e650-114">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="3e650-114">[identitySet][]</span></span>            | <span data-ttu-id="3e650-115">启动注释线程的用户的标识。</span><span class="sxs-lookup"><span data-stu-id="3e650-115">The identity of the user who started the comment thread.</span></span>
| <span data-ttu-id="3e650-116">participants</span><span class="sxs-lookup"><span data-stu-id="3e650-116">participants</span></span>     | <span data-ttu-id="3e650-117">[identitySet][] 集合</span><span class="sxs-lookup"><span data-stu-id="3e650-117">[identitySet][] collection</span></span> | <span data-ttu-id="3e650-118">参与此注释线程的用户的标识。</span><span class="sxs-lookup"><span data-stu-id="3e650-118">The identities of the users participating in this comment thread.</span></span>

[identitySet]: identityset.md

## <a name="remarks"></a><span data-ttu-id="3e650-120">注解</span><span class="sxs-lookup"><span data-stu-id="3e650-120">Remarks</span></span>

<span data-ttu-id="3e650-121">项活动记录当前仅在 SharePoint 和 OneDrive for Business 上可用。</span><span class="sxs-lookup"><span data-stu-id="3e650-121">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The CommentAction object provides information about a comment that was made on an item.",
  "keywords": "activities,activity,action,comment",
  "section": "documentation",
  "tocPath": "Resources/CommentAction",
  "suppressions": [
    "Error: /api-reference/beta/resources/commentaction.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

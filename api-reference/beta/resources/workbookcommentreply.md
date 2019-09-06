---
title: workbookCommentReply 资源类型
description: WorkbookCommentReply 资源类型的定义
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 0a4dfc215eec435c67f1259a85e899db4dfb2b63
ms.sourcegitcommit: c74195b8725c3f28bb3bded43c855261590a0cec
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/06/2019
ms.locfileid: "36775900"
---
# <a name="workbookcommentreply-resource-type"></a><span data-ttu-id="10d31-103">workbookCommentReply 资源类型</span><span class="sxs-lookup"><span data-stu-id="10d31-103">workbookCommentReply resource type</span></span>

<span data-ttu-id="10d31-104">表示对 excel 注释的答复。</span><span class="sxs-lookup"><span data-stu-id="10d31-104">Represents a reply to an excel comment.</span></span>

## <a name="methods"></a><span data-ttu-id="10d31-105">方法</span><span class="sxs-lookup"><span data-stu-id="10d31-105">Methods</span></span>

| <span data-ttu-id="10d31-106">方法</span><span class="sxs-lookup"><span data-stu-id="10d31-106">Method</span></span>       | <span data-ttu-id="10d31-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="10d31-107">Return Type</span></span> | <span data-ttu-id="10d31-108">说明</span><span class="sxs-lookup"><span data-stu-id="10d31-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="10d31-109">列出 workbookCommentReplies</span><span class="sxs-lookup"><span data-stu-id="10d31-109">List workbookCommentReplies</span></span>](../api/workbookcomment-list-replies.md) | <span data-ttu-id="10d31-110">[workbookCommentReply](workbookcommentreply.md)集合</span><span class="sxs-lookup"><span data-stu-id="10d31-110">[workbookCommentReply](workbookcommentreply.md) collection</span></span> | <span data-ttu-id="10d31-111">检索 workbookcommentreply 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="10d31-111">Retrieve a list of workbookcommentreply objects.</span></span> |
| [<span data-ttu-id="10d31-112">获取 workbookCommentReply</span><span class="sxs-lookup"><span data-stu-id="10d31-112">Get workbookCommentReply</span></span>](../api/workbookcommentreply-get.md) | [<span data-ttu-id="10d31-113">workbookCommentReply</span><span class="sxs-lookup"><span data-stu-id="10d31-113">workbookCommentReply</span></span>](workbookcommentreply.md) | <span data-ttu-id="10d31-114">读取 workbookCommentReply 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="10d31-114">Read properties and relationships of workbookCommentReply object.</span></span> |
| [<span data-ttu-id="10d31-115">创建 workbookCommentReply</span><span class="sxs-lookup"><span data-stu-id="10d31-115">Create workbookCommentReply</span></span>](../api/workbookcomment-post-replies.md) | [<span data-ttu-id="10d31-116">workbookCommentReply</span><span class="sxs-lookup"><span data-stu-id="10d31-116">workbookCommentReply</span></span>](workbookcommentreply.md) | <span data-ttu-id="10d31-117">创建新的 workbookCommentReply。</span><span class="sxs-lookup"><span data-stu-id="10d31-117">Create a new workbookCommentReply.</span></span> |

## <a name="properties"></a><span data-ttu-id="10d31-118">属性</span><span class="sxs-lookup"><span data-stu-id="10d31-118">Properties</span></span>

| <span data-ttu-id="10d31-119">属性</span><span class="sxs-lookup"><span data-stu-id="10d31-119">Property</span></span>     | <span data-ttu-id="10d31-120">类型</span><span class="sxs-lookup"><span data-stu-id="10d31-120">Type</span></span>        | <span data-ttu-id="10d31-121">说明</span><span class="sxs-lookup"><span data-stu-id="10d31-121">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="10d31-122">内容</span><span class="sxs-lookup"><span data-stu-id="10d31-122">content</span></span>|<span data-ttu-id="10d31-123">String</span><span class="sxs-lookup"><span data-stu-id="10d31-123">String</span></span>|<span data-ttu-id="10d31-124">已回复的注释的内容。</span><span class="sxs-lookup"><span data-stu-id="10d31-124">The content of replied comment.</span></span>|
|<span data-ttu-id="10d31-125">contentType</span><span class="sxs-lookup"><span data-stu-id="10d31-125">contentType</span></span>|<span data-ttu-id="10d31-126">String</span><span class="sxs-lookup"><span data-stu-id="10d31-126">String</span></span>|<span data-ttu-id="10d31-127">指示答复的批注的类型。</span><span class="sxs-lookup"><span data-stu-id="10d31-127">Indicates the type for the replied comment.</span></span>|
|<span data-ttu-id="10d31-128">id</span><span class="sxs-lookup"><span data-stu-id="10d31-128">id</span></span>|<span data-ttu-id="10d31-129">字符串</span><span class="sxs-lookup"><span data-stu-id="10d31-129">String</span></span>|<span data-ttu-id="10d31-130">表示批注标识符。</span><span class="sxs-lookup"><span data-stu-id="10d31-130">Represents the comment identifier.</span></span> <span data-ttu-id="10d31-131">只读。</span><span class="sxs-lookup"><span data-stu-id="10d31-131">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="10d31-132">关系</span><span class="sxs-lookup"><span data-stu-id="10d31-132">Relationships</span></span>

<span data-ttu-id="10d31-133">无</span><span class="sxs-lookup"><span data-stu-id="10d31-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="10d31-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="10d31-134">JSON representation</span></span>

<span data-ttu-id="10d31-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="10d31-135">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookCommentReply",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "content": "String",
  "contentType": "String",
  "id": "String (identifier)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "workbookCommentReply resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

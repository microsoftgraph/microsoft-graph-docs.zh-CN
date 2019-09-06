---
title: workbookCommentReply 资源类型
description: WorkbookCommentReply 资源类型的定义
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 8c93dcb4a4ccd1289de8d19b8970cbf0b87e80cc
ms.sourcegitcommit: c74195b8725c3f28bb3bded43c855261590a0cec
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/06/2019
ms.locfileid: "36775732"
---
# <a name="workbookcommentreply-resource-type"></a><span data-ttu-id="62b6b-103">workbookCommentReply 资源类型</span><span class="sxs-lookup"><span data-stu-id="62b6b-103">workbookCommentReply resource type</span></span>

<span data-ttu-id="62b6b-104">表示对 Excel 注释的答复。</span><span class="sxs-lookup"><span data-stu-id="62b6b-104">Represents a reply to an Excel comment.</span></span>

## <a name="methods"></a><span data-ttu-id="62b6b-105">方法</span><span class="sxs-lookup"><span data-stu-id="62b6b-105">Methods</span></span>

| <span data-ttu-id="62b6b-106">方法</span><span class="sxs-lookup"><span data-stu-id="62b6b-106">Method</span></span>       | <span data-ttu-id="62b6b-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="62b6b-107">Return Type</span></span> | <span data-ttu-id="62b6b-108">说明</span><span class="sxs-lookup"><span data-stu-id="62b6b-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="62b6b-109">列出 workbookCommentReplies</span><span class="sxs-lookup"><span data-stu-id="62b6b-109">List workbookCommentReplies</span></span>](../api/workbookcomment-list-replies.md) | <span data-ttu-id="62b6b-110">[workbookCommentReply](workbookcommentreply.md)集合</span><span class="sxs-lookup"><span data-stu-id="62b6b-110">[workbookCommentReply](workbookcommentreply.md) collection</span></span> | <span data-ttu-id="62b6b-111">检索 workbookcommentreply 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="62b6b-111">Retrieve a list of workbookcommentreply objects.</span></span> |
| [<span data-ttu-id="62b6b-112">获取 workbookCommentReply</span><span class="sxs-lookup"><span data-stu-id="62b6b-112">Get workbookCommentReply</span></span>](../api/workbookcommentreply-get.md) | [<span data-ttu-id="62b6b-113">workbookCommentReply</span><span class="sxs-lookup"><span data-stu-id="62b6b-113">workbookCommentReply</span></span>](workbookcommentreply.md) | <span data-ttu-id="62b6b-114">读取 workbookCommentReply 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="62b6b-114">Read properties and relationships of workbookCommentReply object.</span></span> |
| [<span data-ttu-id="62b6b-115">创建 workbookCommentReply</span><span class="sxs-lookup"><span data-stu-id="62b6b-115">Create workbookCommentReply</span></span>](../api/workbookcomment-post-replies.md) | [<span data-ttu-id="62b6b-116">workbookCommentReply</span><span class="sxs-lookup"><span data-stu-id="62b6b-116">workbookCommentReply</span></span>](workbookcommentreply.md) | <span data-ttu-id="62b6b-117">创建新的 workbookCommentReply。</span><span class="sxs-lookup"><span data-stu-id="62b6b-117">Create a new workbookCommentReply.</span></span> |
## <a name="properties"></a><span data-ttu-id="62b6b-118">属性</span><span class="sxs-lookup"><span data-stu-id="62b6b-118">Properties</span></span>

| <span data-ttu-id="62b6b-119">属性</span><span class="sxs-lookup"><span data-stu-id="62b6b-119">Property</span></span>     | <span data-ttu-id="62b6b-120">类型</span><span class="sxs-lookup"><span data-stu-id="62b6b-120">Type</span></span>        | <span data-ttu-id="62b6b-121">说明</span><span class="sxs-lookup"><span data-stu-id="62b6b-121">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="62b6b-122">内容</span><span class="sxs-lookup"><span data-stu-id="62b6b-122">content</span></span>|<span data-ttu-id="62b6b-123">String</span><span class="sxs-lookup"><span data-stu-id="62b6b-123">String</span></span>|<span data-ttu-id="62b6b-124">批注答复的内容。</span><span class="sxs-lookup"><span data-stu-id="62b6b-124">The content of a comment reply.</span></span>|
|<span data-ttu-id="62b6b-125">contentType</span><span class="sxs-lookup"><span data-stu-id="62b6b-125">contentType</span></span>|<span data-ttu-id="62b6b-126">String</span><span class="sxs-lookup"><span data-stu-id="62b6b-126">String</span></span>|<span data-ttu-id="62b6b-127">指示批注答复的类型。</span><span class="sxs-lookup"><span data-stu-id="62b6b-127">Indicates the type for the comment reply.</span></span>|
|<span data-ttu-id="62b6b-128">id</span><span class="sxs-lookup"><span data-stu-id="62b6b-128">id</span></span>|<span data-ttu-id="62b6b-129">字符串</span><span class="sxs-lookup"><span data-stu-id="62b6b-129">String</span></span>|<span data-ttu-id="62b6b-130">表示批注标识符。</span><span class="sxs-lookup"><span data-stu-id="62b6b-130">Represents the comment identifier.</span></span> <span data-ttu-id="62b6b-131">只读。</span><span class="sxs-lookup"><span data-stu-id="62b6b-131">Read-only.</span></span>|


## <a name="relationships"></a><span data-ttu-id="62b6b-132">关系</span><span class="sxs-lookup"><span data-stu-id="62b6b-132">Relationships</span></span>

<span data-ttu-id="62b6b-133">无。</span><span class="sxs-lookup"><span data-stu-id="62b6b-133">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="62b6b-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="62b6b-134">JSON representation</span></span>

<span data-ttu-id="62b6b-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="62b6b-135">The following is a JSON representation of the resource.</span></span>

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

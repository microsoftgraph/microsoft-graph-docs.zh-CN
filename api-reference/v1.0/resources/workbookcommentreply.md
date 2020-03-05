---
title: workbookCommentReply 资源类型
description: WorkbookCommentReply 资源类型的定义
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 77402ad1566bcfa6822a326270306f1ea604896f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42446728"
---
# <a name="workbookcommentreply-resource-type"></a><span data-ttu-id="d9a54-103">workbookCommentReply 资源类型</span><span class="sxs-lookup"><span data-stu-id="d9a54-103">workbookCommentReply resource type</span></span>

<span data-ttu-id="d9a54-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="d9a54-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d9a54-105">表示对 Excel 注释的答复。</span><span class="sxs-lookup"><span data-stu-id="d9a54-105">Represents a reply to an Excel comment.</span></span>

## <a name="methods"></a><span data-ttu-id="d9a54-106">方法</span><span class="sxs-lookup"><span data-stu-id="d9a54-106">Methods</span></span>

| <span data-ttu-id="d9a54-107">方法</span><span class="sxs-lookup"><span data-stu-id="d9a54-107">Method</span></span>       | <span data-ttu-id="d9a54-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="d9a54-108">Return Type</span></span> | <span data-ttu-id="d9a54-109">说明</span><span class="sxs-lookup"><span data-stu-id="d9a54-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="d9a54-110">列出 workbookCommentReplies</span><span class="sxs-lookup"><span data-stu-id="d9a54-110">List workbookCommentReplies</span></span>](../api/workbookcomment-list-replies.md) | <span data-ttu-id="d9a54-111">[workbookCommentReply](workbookcommentreply.md)集合</span><span class="sxs-lookup"><span data-stu-id="d9a54-111">[workbookCommentReply](workbookcommentreply.md) collection</span></span> | <span data-ttu-id="d9a54-112">检索 workbookcommentreply 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="d9a54-112">Retrieve a list of workbookcommentreply objects.</span></span> |
| [<span data-ttu-id="d9a54-113">获取 workbookCommentReply</span><span class="sxs-lookup"><span data-stu-id="d9a54-113">Get workbookCommentReply</span></span>](../api/workbookcommentreply-get.md) | [<span data-ttu-id="d9a54-114">workbookCommentReply</span><span class="sxs-lookup"><span data-stu-id="d9a54-114">workbookCommentReply</span></span>](workbookcommentreply.md) | <span data-ttu-id="d9a54-115">读取 workbookCommentReply 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d9a54-115">Read properties and relationships of workbookCommentReply object.</span></span> |
| [<span data-ttu-id="d9a54-116">创建 workbookCommentReply</span><span class="sxs-lookup"><span data-stu-id="d9a54-116">Create workbookCommentReply</span></span>](../api/workbookcomment-post-replies.md) | [<span data-ttu-id="d9a54-117">workbookCommentReply</span><span class="sxs-lookup"><span data-stu-id="d9a54-117">workbookCommentReply</span></span>](workbookcommentreply.md) | <span data-ttu-id="d9a54-118">创建新的 workbookCommentReply。</span><span class="sxs-lookup"><span data-stu-id="d9a54-118">Create a new workbookCommentReply.</span></span> |
## <a name="properties"></a><span data-ttu-id="d9a54-119">属性</span><span class="sxs-lookup"><span data-stu-id="d9a54-119">Properties</span></span>

| <span data-ttu-id="d9a54-120">属性</span><span class="sxs-lookup"><span data-stu-id="d9a54-120">Property</span></span>     | <span data-ttu-id="d9a54-121">类型</span><span class="sxs-lookup"><span data-stu-id="d9a54-121">Type</span></span>        | <span data-ttu-id="d9a54-122">说明</span><span class="sxs-lookup"><span data-stu-id="d9a54-122">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d9a54-123">内容</span><span class="sxs-lookup"><span data-stu-id="d9a54-123">content</span></span>|<span data-ttu-id="d9a54-124">String</span><span class="sxs-lookup"><span data-stu-id="d9a54-124">String</span></span>|<span data-ttu-id="d9a54-125">批注答复的内容。</span><span class="sxs-lookup"><span data-stu-id="d9a54-125">The content of a comment reply.</span></span>|
|<span data-ttu-id="d9a54-126">contentType</span><span class="sxs-lookup"><span data-stu-id="d9a54-126">contentType</span></span>|<span data-ttu-id="d9a54-127">String</span><span class="sxs-lookup"><span data-stu-id="d9a54-127">String</span></span>|<span data-ttu-id="d9a54-128">指示批注答复的类型。</span><span class="sxs-lookup"><span data-stu-id="d9a54-128">Indicates the type for the comment reply.</span></span>|
|<span data-ttu-id="d9a54-129">id</span><span class="sxs-lookup"><span data-stu-id="d9a54-129">id</span></span>|<span data-ttu-id="d9a54-130">字符串</span><span class="sxs-lookup"><span data-stu-id="d9a54-130">String</span></span>|<span data-ttu-id="d9a54-131">表示批注标识符。</span><span class="sxs-lookup"><span data-stu-id="d9a54-131">Represents the comment identifier.</span></span> <span data-ttu-id="d9a54-132">只读。</span><span class="sxs-lookup"><span data-stu-id="d9a54-132">Read-only.</span></span>|


## <a name="relationships"></a><span data-ttu-id="d9a54-133">关系</span><span class="sxs-lookup"><span data-stu-id="d9a54-133">Relationships</span></span>

<span data-ttu-id="d9a54-134">无。</span><span class="sxs-lookup"><span data-stu-id="d9a54-134">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d9a54-135">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d9a54-135">JSON representation</span></span>

<span data-ttu-id="d9a54-136">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d9a54-136">The following is a JSON representation of the resource.</span></span>

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

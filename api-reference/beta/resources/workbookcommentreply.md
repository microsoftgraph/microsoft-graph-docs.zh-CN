---
title: workbookCommentReply 资源类型
description: WorkbookCommentReply 资源类型的定义
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 8206f2cef7996bd0abc64a1f99493b701c4730e2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48079643"
---
# <a name="workbookcommentreply-resource-type"></a><span data-ttu-id="1d948-103">workbookCommentReply 资源类型</span><span class="sxs-lookup"><span data-stu-id="1d948-103">workbookCommentReply resource type</span></span>

<span data-ttu-id="1d948-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1d948-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1d948-105">表示对 excel 注释的答复。</span><span class="sxs-lookup"><span data-stu-id="1d948-105">Represents a reply to an excel comment.</span></span>

## <a name="methods"></a><span data-ttu-id="1d948-106">方法</span><span class="sxs-lookup"><span data-stu-id="1d948-106">Methods</span></span>

| <span data-ttu-id="1d948-107">方法</span><span class="sxs-lookup"><span data-stu-id="1d948-107">Method</span></span>       | <span data-ttu-id="1d948-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="1d948-108">Return Type</span></span> | <span data-ttu-id="1d948-109">说明</span><span class="sxs-lookup"><span data-stu-id="1d948-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="1d948-110">列出 workbookCommentReplies</span><span class="sxs-lookup"><span data-stu-id="1d948-110">List workbookCommentReplies</span></span>](../api/workbookcomment-list-replies.md) | <span data-ttu-id="1d948-111">[workbookCommentReply](workbookcommentreply.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1d948-111">[workbookCommentReply](workbookcommentreply.md) collection</span></span> | <span data-ttu-id="1d948-112">检索 workbookcommentreply 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="1d948-112">Retrieve a list of workbookcommentreply objects.</span></span> |
| [<span data-ttu-id="1d948-113">获取 workbookCommentReply</span><span class="sxs-lookup"><span data-stu-id="1d948-113">Get workbookCommentReply</span></span>](../api/workbookcommentreply-get.md) | [<span data-ttu-id="1d948-114">workbookCommentReply</span><span class="sxs-lookup"><span data-stu-id="1d948-114">workbookCommentReply</span></span>](workbookcommentreply.md) | <span data-ttu-id="1d948-115">读取 workbookCommentReply 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="1d948-115">Read properties and relationships of workbookCommentReply object.</span></span> |
| [<span data-ttu-id="1d948-116">创建 workbookCommentReply</span><span class="sxs-lookup"><span data-stu-id="1d948-116">Create workbookCommentReply</span></span>](../api/workbookcomment-post-replies.md) | [<span data-ttu-id="1d948-117">workbookCommentReply</span><span class="sxs-lookup"><span data-stu-id="1d948-117">workbookCommentReply</span></span>](workbookcommentreply.md) | <span data-ttu-id="1d948-118">创建新的 workbookCommentReply。</span><span class="sxs-lookup"><span data-stu-id="1d948-118">Create a new workbookCommentReply.</span></span> |

## <a name="properties"></a><span data-ttu-id="1d948-119">属性</span><span class="sxs-lookup"><span data-stu-id="1d948-119">Properties</span></span>

| <span data-ttu-id="1d948-120">属性</span><span class="sxs-lookup"><span data-stu-id="1d948-120">Property</span></span>     | <span data-ttu-id="1d948-121">类型</span><span class="sxs-lookup"><span data-stu-id="1d948-121">Type</span></span>        | <span data-ttu-id="1d948-122">说明</span><span class="sxs-lookup"><span data-stu-id="1d948-122">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="1d948-123">内容</span><span class="sxs-lookup"><span data-stu-id="1d948-123">content</span></span>|<span data-ttu-id="1d948-124">String</span><span class="sxs-lookup"><span data-stu-id="1d948-124">String</span></span>|<span data-ttu-id="1d948-125">已回复的注释的内容。</span><span class="sxs-lookup"><span data-stu-id="1d948-125">The content of replied comment.</span></span>|
|<span data-ttu-id="1d948-126">contentType</span><span class="sxs-lookup"><span data-stu-id="1d948-126">contentType</span></span>|<span data-ttu-id="1d948-127">String</span><span class="sxs-lookup"><span data-stu-id="1d948-127">String</span></span>|<span data-ttu-id="1d948-128">指示答复的批注的类型。</span><span class="sxs-lookup"><span data-stu-id="1d948-128">Indicates the type for the replied comment.</span></span>|
|<span data-ttu-id="1d948-129">id</span><span class="sxs-lookup"><span data-stu-id="1d948-129">id</span></span>|<span data-ttu-id="1d948-130">String</span><span class="sxs-lookup"><span data-stu-id="1d948-130">String</span></span>|<span data-ttu-id="1d948-131">表示批注标识符。</span><span class="sxs-lookup"><span data-stu-id="1d948-131">Represents the comment identifier.</span></span> <span data-ttu-id="1d948-132">只读。</span><span class="sxs-lookup"><span data-stu-id="1d948-132">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1d948-133">关系</span><span class="sxs-lookup"><span data-stu-id="1d948-133">Relationships</span></span>

<span data-ttu-id="1d948-134">无</span><span class="sxs-lookup"><span data-stu-id="1d948-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1d948-135">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1d948-135">JSON representation</span></span>

<span data-ttu-id="1d948-136">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1d948-136">The following is a JSON representation of the resource.</span></span>

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



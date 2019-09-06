---
title: workbookComment 资源类型
description: WorkbookComment 资源类型的定义
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: f2f081dd5bf3732b104ab20a28df0f61956b8490
ms.sourcegitcommit: c74195b8725c3f28bb3bded43c855261590a0cec
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/06/2019
ms.locfileid: "36775753"
---
# <a name="workbookcomment-resource-type"></a><span data-ttu-id="2d9d6-103">workbookComment 资源类型</span><span class="sxs-lookup"><span data-stu-id="2d9d6-103">workbookComment resource type</span></span>

<span data-ttu-id="2d9d6-104">代表工作簿中的注释。</span><span class="sxs-lookup"><span data-stu-id="2d9d6-104">Represents a comment in workbook.</span></span>

## <a name="methods"></a><span data-ttu-id="2d9d6-105">方法</span><span class="sxs-lookup"><span data-stu-id="2d9d6-105">Methods</span></span>

| <span data-ttu-id="2d9d6-106">方法</span><span class="sxs-lookup"><span data-stu-id="2d9d6-106">Method</span></span>       | <span data-ttu-id="2d9d6-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="2d9d6-107">Return Type</span></span> | <span data-ttu-id="2d9d6-108">说明</span><span class="sxs-lookup"><span data-stu-id="2d9d6-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="2d9d6-109">列出 workbookComments</span><span class="sxs-lookup"><span data-stu-id="2d9d6-109">List workbookComments</span></span>](../api/workbook-list-comments.md) | <span data-ttu-id="2d9d6-110">[workbookComment](workbookComment.md)集合</span><span class="sxs-lookup"><span data-stu-id="2d9d6-110">[workbookComment](workbookComment.md) collection</span></span> | <span data-ttu-id="2d9d6-111">获取**workbookComment**对象集合。</span><span class="sxs-lookup"><span data-stu-id="2d9d6-111">Get a **workbookComment** object collection.</span></span> |
| [<span data-ttu-id="2d9d6-112">获取 workbookComment</span><span class="sxs-lookup"><span data-stu-id="2d9d6-112">Get workbookComment</span></span>](../api/workbookcomment-get.md) | [<span data-ttu-id="2d9d6-113">workbookComment</span><span class="sxs-lookup"><span data-stu-id="2d9d6-113">workbookComment</span></span>](workbookcomment.md) | <span data-ttu-id="2d9d6-114">读取**workbookComment**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="2d9d6-114">Read the properties and relationships of a **workbookComment** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="2d9d6-115">属性</span><span class="sxs-lookup"><span data-stu-id="2d9d6-115">Properties</span></span>

| <span data-ttu-id="2d9d6-116">属性</span><span class="sxs-lookup"><span data-stu-id="2d9d6-116">Property</span></span>     | <span data-ttu-id="2d9d6-117">类型</span><span class="sxs-lookup"><span data-stu-id="2d9d6-117">Type</span></span>        | <span data-ttu-id="2d9d6-118">说明</span><span class="sxs-lookup"><span data-stu-id="2d9d6-118">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2d9d6-119">内容</span><span class="sxs-lookup"><span data-stu-id="2d9d6-119">content</span></span>|<span data-ttu-id="2d9d6-120">String</span><span class="sxs-lookup"><span data-stu-id="2d9d6-120">String</span></span>|<span data-ttu-id="2d9d6-121">注释的内容。</span><span class="sxs-lookup"><span data-stu-id="2d9d6-121">The content of comment.</span></span>|
|<span data-ttu-id="2d9d6-122">contentType</span><span class="sxs-lookup"><span data-stu-id="2d9d6-122">contentType</span></span>|<span data-ttu-id="2d9d6-123">String</span><span class="sxs-lookup"><span data-stu-id="2d9d6-123">String</span></span>|<span data-ttu-id="2d9d6-124">指示注释的类型。</span><span class="sxs-lookup"><span data-stu-id="2d9d6-124">Indicates the type for the comment.</span></span>|
|<span data-ttu-id="2d9d6-125">id</span><span class="sxs-lookup"><span data-stu-id="2d9d6-125">id</span></span>|<span data-ttu-id="2d9d6-126">字符串</span><span class="sxs-lookup"><span data-stu-id="2d9d6-126">String</span></span>| <span data-ttu-id="2d9d6-127">表示批注标识符。</span><span class="sxs-lookup"><span data-stu-id="2d9d6-127">Represents the comment identifier.</span></span> <span data-ttu-id="2d9d6-128">只读。</span><span class="sxs-lookup"><span data-stu-id="2d9d6-128">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2d9d6-129">关系</span><span class="sxs-lookup"><span data-stu-id="2d9d6-129">Relationships</span></span>

| <span data-ttu-id="2d9d6-130">关系</span><span class="sxs-lookup"><span data-stu-id="2d9d6-130">Relationship</span></span> | <span data-ttu-id="2d9d6-131">类型</span><span class="sxs-lookup"><span data-stu-id="2d9d6-131">Type</span></span>        | <span data-ttu-id="2d9d6-132">说明</span><span class="sxs-lookup"><span data-stu-id="2d9d6-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2d9d6-133">应答</span><span class="sxs-lookup"><span data-stu-id="2d9d6-133">replies</span></span>|<span data-ttu-id="2d9d6-134">[workbookCommentReply](workbookcommentreply.md)集合</span><span class="sxs-lookup"><span data-stu-id="2d9d6-134">[workbookCommentReply](workbookcommentreply.md) collection</span></span>| <span data-ttu-id="2d9d6-p102">只读。可为空。</span><span class="sxs-lookup"><span data-stu-id="2d9d6-p102">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2d9d6-137">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2d9d6-137">JSON representation</span></span>

<span data-ttu-id="2d9d6-138">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2d9d6-138">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookComment",
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
  "description": "workbookComment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

---
title: workbookComment 资源类型
description: 表示工作簿中的注释。
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 920eff7126d3628e798e10a3e1cc9985d64d6602
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50154234"
---
# <a name="workbookcomment-resource-type"></a><span data-ttu-id="3a770-103">workbookComment 资源类型</span><span class="sxs-lookup"><span data-stu-id="3a770-103">workbookComment resource type</span></span>

<span data-ttu-id="3a770-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3a770-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3a770-105">表示工作簿中的注释。</span><span class="sxs-lookup"><span data-stu-id="3a770-105">Represents a comment in workbook.</span></span>

## <a name="methods"></a><span data-ttu-id="3a770-106">方法</span><span class="sxs-lookup"><span data-stu-id="3a770-106">Methods</span></span>

| <span data-ttu-id="3a770-107">方法</span><span class="sxs-lookup"><span data-stu-id="3a770-107">Method</span></span>       | <span data-ttu-id="3a770-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="3a770-108">Return Type</span></span> | <span data-ttu-id="3a770-109">说明</span><span class="sxs-lookup"><span data-stu-id="3a770-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="3a770-110">列出 workbookComments</span><span class="sxs-lookup"><span data-stu-id="3a770-110">List workbookComments</span></span>](../api/workbook-list-comments.md) | <span data-ttu-id="3a770-111">[workbookComment](workbookComment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3a770-111">[workbookComment](workbookComment.md) collection</span></span> | <span data-ttu-id="3a770-112">获取 **workbookComment** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="3a770-112">Get a **workbookComment** object collection.</span></span> |
| [<span data-ttu-id="3a770-113">获取 workbookComment</span><span class="sxs-lookup"><span data-stu-id="3a770-113">Get workbookComment</span></span>](../api/workbookcomment-get.md) | [<span data-ttu-id="3a770-114">workbookComment</span><span class="sxs-lookup"><span data-stu-id="3a770-114">workbookComment</span></span>](workbookcomment.md) | <span data-ttu-id="3a770-115">读取 **workbookComment** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="3a770-115">Read the properties and relationships of a **workbookComment** object.</span></span> |


## <a name="properties"></a><span data-ttu-id="3a770-116">属性</span><span class="sxs-lookup"><span data-stu-id="3a770-116">Properties</span></span>

| <span data-ttu-id="3a770-117">属性</span><span class="sxs-lookup"><span data-stu-id="3a770-117">Property</span></span>     | <span data-ttu-id="3a770-118">类型</span><span class="sxs-lookup"><span data-stu-id="3a770-118">Type</span></span>        | <span data-ttu-id="3a770-119">说明</span><span class="sxs-lookup"><span data-stu-id="3a770-119">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="3a770-120">内容</span><span class="sxs-lookup"><span data-stu-id="3a770-120">content</span></span>|<span data-ttu-id="3a770-121">String</span><span class="sxs-lookup"><span data-stu-id="3a770-121">String</span></span>|<span data-ttu-id="3a770-122">注释的内容。</span><span class="sxs-lookup"><span data-stu-id="3a770-122">The content of the comment.</span></span>|
|<span data-ttu-id="3a770-123">contentType</span><span class="sxs-lookup"><span data-stu-id="3a770-123">contentType</span></span>|<span data-ttu-id="3a770-124">String</span><span class="sxs-lookup"><span data-stu-id="3a770-124">String</span></span>|<span data-ttu-id="3a770-125">指示注释的类型。</span><span class="sxs-lookup"><span data-stu-id="3a770-125">Indicates the type for the comment.</span></span>|
|<span data-ttu-id="3a770-126">id</span><span class="sxs-lookup"><span data-stu-id="3a770-126">id</span></span>|<span data-ttu-id="3a770-127">String</span><span class="sxs-lookup"><span data-stu-id="3a770-127">String</span></span>| <span data-ttu-id="3a770-128">表示批注标识符。</span><span class="sxs-lookup"><span data-stu-id="3a770-128">Represents the comment identifier.</span></span> <span data-ttu-id="3a770-129">只读。</span><span class="sxs-lookup"><span data-stu-id="3a770-129">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3a770-130">关系</span><span class="sxs-lookup"><span data-stu-id="3a770-130">Relationships</span></span>

| <span data-ttu-id="3a770-131">关系</span><span class="sxs-lookup"><span data-stu-id="3a770-131">Relationship</span></span> | <span data-ttu-id="3a770-132">类型</span><span class="sxs-lookup"><span data-stu-id="3a770-132">Type</span></span>        | <span data-ttu-id="3a770-133">说明</span><span class="sxs-lookup"><span data-stu-id="3a770-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="3a770-134">replies</span><span class="sxs-lookup"><span data-stu-id="3a770-134">replies</span></span>|<span data-ttu-id="3a770-135">[workbookCommentReply](workbookcommentreply.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3a770-135">[workbookCommentReply](workbookcommentreply.md) collection</span></span>| <span data-ttu-id="3a770-p102">只读。可为空。</span><span class="sxs-lookup"><span data-stu-id="3a770-p102">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3a770-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3a770-138">JSON representation</span></span>

<span data-ttu-id="3a770-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3a770-139">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookComment",
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



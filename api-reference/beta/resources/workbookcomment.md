---
title: workbookComment 资源类型
description: 代表工作簿中的注释。
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 11e0b1538f6d2b41a8b211e1a7cc4ac45d2703a7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48079638"
---
# <a name="workbookcomment-resource-type"></a><span data-ttu-id="b8a9f-103">workbookComment 资源类型</span><span class="sxs-lookup"><span data-stu-id="b8a9f-103">workbookComment resource type</span></span>

<span data-ttu-id="b8a9f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b8a9f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b8a9f-105">代表工作簿中的注释。</span><span class="sxs-lookup"><span data-stu-id="b8a9f-105">Represents a comment in workbook.</span></span>

## <a name="methods"></a><span data-ttu-id="b8a9f-106">方法</span><span class="sxs-lookup"><span data-stu-id="b8a9f-106">Methods</span></span>

| <span data-ttu-id="b8a9f-107">方法</span><span class="sxs-lookup"><span data-stu-id="b8a9f-107">Method</span></span>       | <span data-ttu-id="b8a9f-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="b8a9f-108">Return Type</span></span> | <span data-ttu-id="b8a9f-109">说明</span><span class="sxs-lookup"><span data-stu-id="b8a9f-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="b8a9f-110">列出 workbookComments</span><span class="sxs-lookup"><span data-stu-id="b8a9f-110">List workbookComments</span></span>](../api/workbook-list-comments.md) | <span data-ttu-id="b8a9f-111">[workbookComment](workbookComment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b8a9f-111">[workbookComment](workbookComment.md) collection</span></span> | <span data-ttu-id="b8a9f-112">获取 **workbookComment** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="b8a9f-112">Get a **workbookComment** object collection.</span></span> |
| [<span data-ttu-id="b8a9f-113">获取 workbookComment</span><span class="sxs-lookup"><span data-stu-id="b8a9f-113">Get workbookComment</span></span>](../api/workbookcomment-get.md) | [<span data-ttu-id="b8a9f-114">workbookComment</span><span class="sxs-lookup"><span data-stu-id="b8a9f-114">workbookComment</span></span>](workbookcomment.md) | <span data-ttu-id="b8a9f-115">读取 **workbookComment** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b8a9f-115">Read the properties and relationships of a **workbookComment** object.</span></span> |


## <a name="properties"></a><span data-ttu-id="b8a9f-116">属性</span><span class="sxs-lookup"><span data-stu-id="b8a9f-116">Properties</span></span>

| <span data-ttu-id="b8a9f-117">属性</span><span class="sxs-lookup"><span data-stu-id="b8a9f-117">Property</span></span>     | <span data-ttu-id="b8a9f-118">类型</span><span class="sxs-lookup"><span data-stu-id="b8a9f-118">Type</span></span>        | <span data-ttu-id="b8a9f-119">说明</span><span class="sxs-lookup"><span data-stu-id="b8a9f-119">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b8a9f-120">内容</span><span class="sxs-lookup"><span data-stu-id="b8a9f-120">content</span></span>|<span data-ttu-id="b8a9f-121">String</span><span class="sxs-lookup"><span data-stu-id="b8a9f-121">String</span></span>|<span data-ttu-id="b8a9f-122">注释的内容。</span><span class="sxs-lookup"><span data-stu-id="b8a9f-122">The content of the comment.</span></span>|
|<span data-ttu-id="b8a9f-123">contentType</span><span class="sxs-lookup"><span data-stu-id="b8a9f-123">contentType</span></span>|<span data-ttu-id="b8a9f-124">String</span><span class="sxs-lookup"><span data-stu-id="b8a9f-124">String</span></span>|<span data-ttu-id="b8a9f-125">指示注释的类型。</span><span class="sxs-lookup"><span data-stu-id="b8a9f-125">Indicates the type for the comment.</span></span>|
|<span data-ttu-id="b8a9f-126">id</span><span class="sxs-lookup"><span data-stu-id="b8a9f-126">id</span></span>|<span data-ttu-id="b8a9f-127">String</span><span class="sxs-lookup"><span data-stu-id="b8a9f-127">String</span></span>| <span data-ttu-id="b8a9f-128">表示批注标识符。</span><span class="sxs-lookup"><span data-stu-id="b8a9f-128">Represents the comment identifier.</span></span> <span data-ttu-id="b8a9f-129">只读。</span><span class="sxs-lookup"><span data-stu-id="b8a9f-129">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b8a9f-130">关系</span><span class="sxs-lookup"><span data-stu-id="b8a9f-130">Relationships</span></span>

| <span data-ttu-id="b8a9f-131">关系</span><span class="sxs-lookup"><span data-stu-id="b8a9f-131">Relationship</span></span> | <span data-ttu-id="b8a9f-132">类型</span><span class="sxs-lookup"><span data-stu-id="b8a9f-132">Type</span></span>        | <span data-ttu-id="b8a9f-133">说明</span><span class="sxs-lookup"><span data-stu-id="b8a9f-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b8a9f-134">应答</span><span class="sxs-lookup"><span data-stu-id="b8a9f-134">replies</span></span>|<span data-ttu-id="b8a9f-135">[workbookCommentReply](workbookcommentreply.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b8a9f-135">[workbookCommentReply](workbookcommentreply.md) collection</span></span>| <span data-ttu-id="b8a9f-p102">只读。可为空。</span><span class="sxs-lookup"><span data-stu-id="b8a9f-p102">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b8a9f-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b8a9f-138">JSON representation</span></span>

<span data-ttu-id="b8a9f-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b8a9f-139">The following is a JSON representation of the resource.</span></span>

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



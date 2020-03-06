---
title: workbookComment 资源类型
description: WorkbookComment 资源类型的定义
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 3a238ab9b033cd1906842f61d9f2d72b6d642335
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533389"
---
# <a name="workbookcomment-resource-type"></a><span data-ttu-id="4698b-103">workbookComment 资源类型</span><span class="sxs-lookup"><span data-stu-id="4698b-103">workbookComment resource type</span></span>

<span data-ttu-id="4698b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4698b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4698b-105">代表工作簿中的注释。</span><span class="sxs-lookup"><span data-stu-id="4698b-105">Represents a comment in workbook.</span></span>

## <a name="methods"></a><span data-ttu-id="4698b-106">Methods</span><span class="sxs-lookup"><span data-stu-id="4698b-106">Methods</span></span>

| <span data-ttu-id="4698b-107">方法</span><span class="sxs-lookup"><span data-stu-id="4698b-107">Method</span></span>       | <span data-ttu-id="4698b-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="4698b-108">Return Type</span></span> | <span data-ttu-id="4698b-109">说明</span><span class="sxs-lookup"><span data-stu-id="4698b-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="4698b-110">列出 workbookComments</span><span class="sxs-lookup"><span data-stu-id="4698b-110">List workbookComments</span></span>](../api/workbook-list-comments.md) | <span data-ttu-id="4698b-111">[workbookComment](workbookComment.md)集合</span><span class="sxs-lookup"><span data-stu-id="4698b-111">[workbookComment](workbookComment.md) collection</span></span> | <span data-ttu-id="4698b-112">获取**workbookComment**对象集合。</span><span class="sxs-lookup"><span data-stu-id="4698b-112">Get a **workbookComment** object collection.</span></span> |
| [<span data-ttu-id="4698b-113">获取 workbookComment</span><span class="sxs-lookup"><span data-stu-id="4698b-113">Get workbookComment</span></span>](../api/workbookcomment-get.md) | [<span data-ttu-id="4698b-114">workbookComment</span><span class="sxs-lookup"><span data-stu-id="4698b-114">workbookComment</span></span>](workbookcomment.md) | <span data-ttu-id="4698b-115">读取**workbookComment**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4698b-115">Read the properties and relationships of a **workbookComment** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="4698b-116">属性</span><span class="sxs-lookup"><span data-stu-id="4698b-116">Properties</span></span>

| <span data-ttu-id="4698b-117">属性</span><span class="sxs-lookup"><span data-stu-id="4698b-117">Property</span></span>     | <span data-ttu-id="4698b-118">类型</span><span class="sxs-lookup"><span data-stu-id="4698b-118">Type</span></span>        | <span data-ttu-id="4698b-119">说明</span><span class="sxs-lookup"><span data-stu-id="4698b-119">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="4698b-120">内容</span><span class="sxs-lookup"><span data-stu-id="4698b-120">content</span></span>|<span data-ttu-id="4698b-121">String</span><span class="sxs-lookup"><span data-stu-id="4698b-121">String</span></span>|<span data-ttu-id="4698b-122">注释的内容。</span><span class="sxs-lookup"><span data-stu-id="4698b-122">The content of comment.</span></span>|
|<span data-ttu-id="4698b-123">contentType</span><span class="sxs-lookup"><span data-stu-id="4698b-123">contentType</span></span>|<span data-ttu-id="4698b-124">String</span><span class="sxs-lookup"><span data-stu-id="4698b-124">String</span></span>|<span data-ttu-id="4698b-125">指示注释的类型。</span><span class="sxs-lookup"><span data-stu-id="4698b-125">Indicates the type for the comment.</span></span>|
|<span data-ttu-id="4698b-126">id</span><span class="sxs-lookup"><span data-stu-id="4698b-126">id</span></span>|<span data-ttu-id="4698b-127">字符串</span><span class="sxs-lookup"><span data-stu-id="4698b-127">String</span></span>| <span data-ttu-id="4698b-128">表示批注标识符。</span><span class="sxs-lookup"><span data-stu-id="4698b-128">Represents the comment identifier.</span></span> <span data-ttu-id="4698b-129">只读。</span><span class="sxs-lookup"><span data-stu-id="4698b-129">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4698b-130">关系</span><span class="sxs-lookup"><span data-stu-id="4698b-130">Relationships</span></span>

| <span data-ttu-id="4698b-131">关系</span><span class="sxs-lookup"><span data-stu-id="4698b-131">Relationship</span></span> | <span data-ttu-id="4698b-132">类型</span><span class="sxs-lookup"><span data-stu-id="4698b-132">Type</span></span>        | <span data-ttu-id="4698b-133">说明</span><span class="sxs-lookup"><span data-stu-id="4698b-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="4698b-134">应答</span><span class="sxs-lookup"><span data-stu-id="4698b-134">replies</span></span>|<span data-ttu-id="4698b-135">[workbookCommentReply](workbookcommentreply.md)集合</span><span class="sxs-lookup"><span data-stu-id="4698b-135">[workbookCommentReply](workbookcommentreply.md) collection</span></span>| <span data-ttu-id="4698b-p102">只读。可为空。</span><span class="sxs-lookup"><span data-stu-id="4698b-p102">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4698b-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4698b-138">JSON representation</span></span>

<span data-ttu-id="4698b-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4698b-139">The following is a JSON representation of the resource.</span></span>

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

---
title: TableRow 资源类型
description: 表示表中的行。
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: fe95b62236322451893e3859f9d6599cc637848c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27807173"
---
# <a name="tablerow-resource-type"></a><span data-ttu-id="5f66b-103">TableRow 资源类型</span><span class="sxs-lookup"><span data-stu-id="5f66b-103">TableRow resource type</span></span>

> <span data-ttu-id="5f66b-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="5f66b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5f66b-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="5f66b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5f66b-106">表示表中的行。</span><span class="sxs-lookup"><span data-stu-id="5f66b-106">Represents a row in a table.</span></span>


## <a name="methods"></a><span data-ttu-id="5f66b-107">方法</span><span class="sxs-lookup"><span data-stu-id="5f66b-107">Methods</span></span>

| <span data-ttu-id="5f66b-108">方法</span><span class="sxs-lookup"><span data-stu-id="5f66b-108">Method</span></span>           | <span data-ttu-id="5f66b-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="5f66b-109">Return Type</span></span>    |<span data-ttu-id="5f66b-110">说明</span><span class="sxs-lookup"><span data-stu-id="5f66b-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5f66b-111">获取 TableRow</span><span class="sxs-lookup"><span data-stu-id="5f66b-111">Get TableRow</span></span>](../api/tablerow-get.md) | [<span data-ttu-id="5f66b-112">TableRow</span><span class="sxs-lookup"><span data-stu-id="5f66b-112">TableRow</span></span>](tablerow.md) |<span data-ttu-id="5f66b-113">读取 tableRow 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5f66b-113">Read properties and relationships of tableRow object.</span></span>|
|[<span data-ttu-id="5f66b-114">Update</span><span class="sxs-lookup"><span data-stu-id="5f66b-114">Update</span></span>](../api/tablerow-update.md) | [<span data-ttu-id="5f66b-115">TableRow</span><span class="sxs-lookup"><span data-stu-id="5f66b-115">TableRow</span></span>](tablerow.md)  |<span data-ttu-id="5f66b-116">更新 TableRow 对象。</span><span class="sxs-lookup"><span data-stu-id="5f66b-116">Update TableRow object.</span></span> |
|[<span data-ttu-id="5f66b-117">区域</span><span class="sxs-lookup"><span data-stu-id="5f66b-117">Range</span></span>](../api/tablerow-range.md)|[<span data-ttu-id="5f66b-118">Range</span><span class="sxs-lookup"><span data-stu-id="5f66b-118">Range</span></span>](range.md)|<span data-ttu-id="5f66b-119">返回与整个行相关联的范围对象。</span><span class="sxs-lookup"><span data-stu-id="5f66b-119">Returns the range object associated with the entire row.</span></span>|
|[<span data-ttu-id="5f66b-120">删除</span><span class="sxs-lookup"><span data-stu-id="5f66b-120">Delete</span></span>](../api/tablerow-delete.md)|<span data-ttu-id="5f66b-121">无</span><span class="sxs-lookup"><span data-stu-id="5f66b-121">None</span></span>|<span data-ttu-id="5f66b-122">从表中删除行。</span><span class="sxs-lookup"><span data-stu-id="5f66b-122">Deletes the row from the table.</span></span>|
|[<span data-ttu-id="5f66b-123">List</span><span class="sxs-lookup"><span data-stu-id="5f66b-123">List</span></span>](../api/tablerow-list.md) | <span data-ttu-id="5f66b-124">[TableRow](tablerow.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5f66b-124">[TableRow](tablerow.md) collection</span></span> |<span data-ttu-id="5f66b-125">获取 tableRow 对象的集合。</span><span class="sxs-lookup"><span data-stu-id="5f66b-125">Get tableRow object collection.</span></span> |
|[<span data-ttu-id="5f66b-126">Itemat</span><span class="sxs-lookup"><span data-stu-id="5f66b-126">Itemat</span></span>](../api/tablerowcollection-itemat.md)|[<span data-ttu-id="5f66b-127">TableRow</span><span class="sxs-lookup"><span data-stu-id="5f66b-127">TableRow</span></span>](tablerow.md)|<span data-ttu-id="5f66b-128">按行在集合中的位置获取此对象。</span><span class="sxs-lookup"><span data-stu-id="5f66b-128">Gets a row based on its position in the collection.</span></span>|
|[<span data-ttu-id="5f66b-129">Add</span><span class="sxs-lookup"><span data-stu-id="5f66b-129">Add</span></span>](../api/tablerowcollection-add.md)|[<span data-ttu-id="5f66b-130">TableRow</span><span class="sxs-lookup"><span data-stu-id="5f66b-130">TableRow</span></span>](tablerow.md)|<span data-ttu-id="5f66b-131">向表中添加新行。</span><span class="sxs-lookup"><span data-stu-id="5f66b-131">Adds a new row to the table.</span></span>|

## <a name="properties"></a><span data-ttu-id="5f66b-132">属性</span><span class="sxs-lookup"><span data-stu-id="5f66b-132">Properties</span></span>
| <span data-ttu-id="5f66b-133">属性</span><span class="sxs-lookup"><span data-stu-id="5f66b-133">Property</span></span>     | <span data-ttu-id="5f66b-134">类型</span><span class="sxs-lookup"><span data-stu-id="5f66b-134">Type</span></span>   |<span data-ttu-id="5f66b-135">说明</span><span class="sxs-lookup"><span data-stu-id="5f66b-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5f66b-136">index</span><span class="sxs-lookup"><span data-stu-id="5f66b-136">index</span></span>|<span data-ttu-id="5f66b-137">int</span><span class="sxs-lookup"><span data-stu-id="5f66b-137">int</span></span>|<span data-ttu-id="5f66b-p102">返回表的行集合内行的索引编号。从零开始编制索引。只读。</span><span class="sxs-lookup"><span data-stu-id="5f66b-p102">Returns the index number of the row within the rows collection of the table. Zero-indexed. Read-only.</span></span>|
|<span data-ttu-id="5f66b-141">values</span><span class="sxs-lookup"><span data-stu-id="5f66b-141">values</span></span>|<span data-ttu-id="5f66b-142">json</span><span class="sxs-lookup"><span data-stu-id="5f66b-142">json</span></span>|<span data-ttu-id="5f66b-p103">表示指定区域的原始值。返回的数据类型可能是字符串、数字或布尔值。包含一个将返回错误字符串的错误的单元格。</span><span class="sxs-lookup"><span data-stu-id="5f66b-p103">Represents the raw values of the specified range. The data returned could be of type string, number, or a boolean. Cell that contain an error will return the error string.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5f66b-146">Relationships</span><span class="sxs-lookup"><span data-stu-id="5f66b-146">Relationships</span></span>
<span data-ttu-id="5f66b-147">无</span><span class="sxs-lookup"><span data-stu-id="5f66b-147">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="5f66b-148">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5f66b-148">JSON representation</span></span>

<span data-ttu-id="5f66b-149">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5f66b-149">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.tableRow"
}-->

```json
{
  "index": 1024,
  "values": "json"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "TableRow resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

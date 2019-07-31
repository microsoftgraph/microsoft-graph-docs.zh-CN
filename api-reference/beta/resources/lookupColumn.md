---
author: JeremyKelley
description: columnDefinition 资源上的 lookupColumn 指示从网站中的另一个源查找列的值。
ms.date: 09/11/2017
title: LookupColumn
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 8c92bce6b6d7ba401f6b9274f2ba0eee4439929e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009907"
---
# <a name="lookupcolumn-resource-type"></a><span data-ttu-id="77516-103">LookupColumn 资源类型</span><span class="sxs-lookup"><span data-stu-id="77516-103">LookupColumn resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="77516-104">[columnDefinition](columndefinition.md) 资源上的 **lookupColumn** 指示从网站中的另一个源查找列的值。</span><span class="sxs-lookup"><span data-stu-id="77516-104">The **lookupColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are looked up from another source in the site.</span></span>

## <a name="json-representation"></a><span data-ttu-id="77516-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="77516-105">JSON representation</span></span>

<span data-ttu-id="77516-106">下面是 **lookupColumn** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="77516-106">Here is a JSON representation of a **lookupColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.lookupColumn" } -->

```json
{
  "allowMultipleValues": true,
  "allowUnlimitedLength": false,
  "columnName": "string",
  "listId": "string",
  "primaryLookupColumnId": "string"
}
```

## <a name="properties"></a><span data-ttu-id="77516-107">属性</span><span class="sxs-lookup"><span data-stu-id="77516-107">Properties</span></span>

| <span data-ttu-id="77516-108">属性名称</span><span class="sxs-lookup"><span data-stu-id="77516-108">Property name</span></span>             | <span data-ttu-id="77516-109">类型</span><span class="sxs-lookup"><span data-stu-id="77516-109">Type</span></span>    | <span data-ttu-id="77516-110">说明</span><span class="sxs-lookup"><span data-stu-id="77516-110">Description</span></span>
|:--------------------------|:--------|:---------------------------------------
| <span data-ttu-id="77516-111">**allowMultipleValues**</span><span class="sxs-lookup"><span data-stu-id="77516-111">**allowMultipleValues**</span></span>   | <span data-ttu-id="77516-112">boolean</span><span class="sxs-lookup"><span data-stu-id="77516-112">boolean</span></span> | <span data-ttu-id="77516-113">指示是否可以从源中选择多个值。</span><span class="sxs-lookup"><span data-stu-id="77516-113">Indicates whether multiple values can be selected from the source.</span></span>
| <span data-ttu-id="77516-114">**allowUnlimitedLength**</span><span class="sxs-lookup"><span data-stu-id="77516-114">**allowUnlimitedLength**</span></span>  | <span data-ttu-id="77516-115">boolean</span><span class="sxs-lookup"><span data-stu-id="77516-115">boolean</span></span> | <span data-ttu-id="77516-116">指示列中的值是否可以超过 255 个字符的标准限制。</span><span class="sxs-lookup"><span data-stu-id="77516-116">Indicates whether values in the column should be able to exceed the standard limit of 255 characters.</span></span>
| <span data-ttu-id="77516-117">**columnName**</span><span class="sxs-lookup"><span data-stu-id="77516-117">**columnName**</span></span>            | <span data-ttu-id="77516-118">string</span><span class="sxs-lookup"><span data-stu-id="77516-118">string</span></span>  | <span data-ttu-id="77516-119">查找源列的名称。</span><span class="sxs-lookup"><span data-stu-id="77516-119">The name of the lookup source column.</span></span>
| <span data-ttu-id="77516-120">**listId**</span><span class="sxs-lookup"><span data-stu-id="77516-120">**listId**</span></span>                | <span data-ttu-id="77516-121">string</span><span class="sxs-lookup"><span data-stu-id="77516-121">string</span></span>  | <span data-ttu-id="77516-122">查找源列表的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="77516-122">The unique identifier of the lookup source list.</span></span>
| <span data-ttu-id="77516-123">**primaryLookupColumnId**</span><span class="sxs-lookup"><span data-stu-id="77516-123">**primaryLookupColumnId**</span></span> | <span data-ttu-id="77516-124">string</span><span class="sxs-lookup"><span data-stu-id="77516-124">string</span></span>  | <span data-ttu-id="77516-125">如果已指定，则此列为*辅助查找*，同时从*主查找*查找的列表项中拉取一个附加字段。</span><span class="sxs-lookup"><span data-stu-id="77516-125">If specified, this column is a *secondary lookup*, pulling an additional field from the list item looked up by the *primary lookup*.</span></span> <span data-ttu-id="77516-126">使用*主查找*查找的列表项作为此处列出的列的源。</span><span class="sxs-lookup"><span data-stu-id="77516-126">Use the list item looked up by the *primary* as the source for the column named here.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/LookupColumn",
  "suppressions": []
}
-->

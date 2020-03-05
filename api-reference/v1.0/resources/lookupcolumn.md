---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: LookupColumn
localization_priority: Normal
description: columnDefinition 资源上的 lookupColumn 指示从网站中的另一个源查找列的值。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 752d60bbb1ac93b5a58eb326e7a6769921c47a66
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447519"
---
# <a name="lookupcolumn-resource-type"></a><span data-ttu-id="a1d9f-103">LookupColumn 资源类型</span><span class="sxs-lookup"><span data-stu-id="a1d9f-103">LookupColumn resource type</span></span>

<span data-ttu-id="a1d9f-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="a1d9f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a1d9f-105">[columnDefinition](columndefinition.md) 资源上的 **lookupColumn** 指示从网站中的另一个源查找列的值。</span><span class="sxs-lookup"><span data-stu-id="a1d9f-105">The **lookupColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are looked up from another source in the site.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a1d9f-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a1d9f-106">JSON representation</span></span>

<span data-ttu-id="a1d9f-107">下面是 **lookupColumn** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a1d9f-107">Here is a JSON representation of a **lookupColumn** resource.</span></span>
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

## <a name="properties"></a><span data-ttu-id="a1d9f-108">属性</span><span class="sxs-lookup"><span data-stu-id="a1d9f-108">Properties</span></span>

| <span data-ttu-id="a1d9f-109">属性名称</span><span class="sxs-lookup"><span data-stu-id="a1d9f-109">Property name</span></span>             | <span data-ttu-id="a1d9f-110">类型</span><span class="sxs-lookup"><span data-stu-id="a1d9f-110">Type</span></span>    | <span data-ttu-id="a1d9f-111">说明</span><span class="sxs-lookup"><span data-stu-id="a1d9f-111">Description</span></span>
|:--------------------------|:--------|:---------------------------------------
| <span data-ttu-id="a1d9f-112">**allowMultipleValues**</span><span class="sxs-lookup"><span data-stu-id="a1d9f-112">**allowMultipleValues**</span></span>   | <span data-ttu-id="a1d9f-113">boolean</span><span class="sxs-lookup"><span data-stu-id="a1d9f-113">boolean</span></span> | <span data-ttu-id="a1d9f-114">指示是否可以从源中选择多个值。</span><span class="sxs-lookup"><span data-stu-id="a1d9f-114">Indicates whether multiple values can be selected from the source.</span></span>
| <span data-ttu-id="a1d9f-115">**allowUnlimitedLength**</span><span class="sxs-lookup"><span data-stu-id="a1d9f-115">**allowUnlimitedLength**</span></span>  | <span data-ttu-id="a1d9f-116">boolean</span><span class="sxs-lookup"><span data-stu-id="a1d9f-116">boolean</span></span> | <span data-ttu-id="a1d9f-117">指示列中的值是否可以超过 255 个字符的标准限制。</span><span class="sxs-lookup"><span data-stu-id="a1d9f-117">Indicates whether values in the column should be able to exceed the standard limit of 255 characters.</span></span>
| <span data-ttu-id="a1d9f-118">**columnName**</span><span class="sxs-lookup"><span data-stu-id="a1d9f-118">**columnName**</span></span>            | <span data-ttu-id="a1d9f-119">string</span><span class="sxs-lookup"><span data-stu-id="a1d9f-119">string</span></span>  | <span data-ttu-id="a1d9f-120">查找源列的名称。</span><span class="sxs-lookup"><span data-stu-id="a1d9f-120">The name of the lookup source column.</span></span>
| <span data-ttu-id="a1d9f-121">**listId**</span><span class="sxs-lookup"><span data-stu-id="a1d9f-121">**listId**</span></span>                | <span data-ttu-id="a1d9f-122">string</span><span class="sxs-lookup"><span data-stu-id="a1d9f-122">string</span></span>  | <span data-ttu-id="a1d9f-123">查找源列表的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="a1d9f-123">The unique identifier of the lookup source list.</span></span>
| <span data-ttu-id="a1d9f-124">**primaryLookupColumnId**</span><span class="sxs-lookup"><span data-stu-id="a1d9f-124">**primaryLookupColumnId**</span></span> | <span data-ttu-id="a1d9f-125">string</span><span class="sxs-lookup"><span data-stu-id="a1d9f-125">string</span></span>  | <span data-ttu-id="a1d9f-126">如果已指定，则此列为*辅助查找*，同时从*主查找*查找的列表项中拉取一个附加字段。</span><span class="sxs-lookup"><span data-stu-id="a1d9f-126">If specified, this column is a *secondary lookup*, pulling an additional field from the list item looked up by the *primary lookup*.</span></span> <span data-ttu-id="a1d9f-127">使用*主查找*查找的列表项作为此处列出的列的源。</span><span class="sxs-lookup"><span data-stu-id="a1d9f-127">Use the list item looked up by the *primary* as the source for the column named here.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/LookupColumn"
} -->

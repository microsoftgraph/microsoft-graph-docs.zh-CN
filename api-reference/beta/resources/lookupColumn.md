---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: LookupColumn
localization_priority: Normal
ms.openlocfilehash: 1c7ab364777e1e3f82bb78d8e0940cf4f85576a0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27885706"
---
# <a name="lookupcolumn-resource-type"></a><span data-ttu-id="c81e6-102">LookupColumn 资源类型</span><span class="sxs-lookup"><span data-stu-id="c81e6-102">LookupColumn resource type</span></span>

> <span data-ttu-id="c81e6-103">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="c81e6-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c81e6-104">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c81e6-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c81e6-105">[columnDefinition](columndefinition.md) 资源上的 **lookupColumn** 指示从网站中的另一个源查找列的值。</span><span class="sxs-lookup"><span data-stu-id="c81e6-105">The **lookupColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are looked up from another source in the site.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c81e6-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c81e6-106">JSON representation</span></span>

<span data-ttu-id="c81e6-107">下面是 **lookupColumn** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c81e6-107">Here is a JSON representation of a **lookupColumn** resource.</span></span>
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

## <a name="properties"></a><span data-ttu-id="c81e6-108">属性</span><span class="sxs-lookup"><span data-stu-id="c81e6-108">Properties</span></span>

| <span data-ttu-id="c81e6-109">属性名称</span><span class="sxs-lookup"><span data-stu-id="c81e6-109">Property name</span></span>             | <span data-ttu-id="c81e6-110">类型</span><span class="sxs-lookup"><span data-stu-id="c81e6-110">Type</span></span>    | <span data-ttu-id="c81e6-111">说明</span><span class="sxs-lookup"><span data-stu-id="c81e6-111">Description</span></span>
|:--------------------------|:--------|:---------------------------------------
| <span data-ttu-id="c81e6-112">**allowMultipleValues**</span><span class="sxs-lookup"><span data-stu-id="c81e6-112">**allowMultipleValues**</span></span>   | <span data-ttu-id="c81e6-113">boolean</span><span class="sxs-lookup"><span data-stu-id="c81e6-113">boolean</span></span> | <span data-ttu-id="c81e6-114">指示是否可以从源中选择多个值。</span><span class="sxs-lookup"><span data-stu-id="c81e6-114">Indicates whether multiple values can be selected from the source.</span></span>
| <span data-ttu-id="c81e6-115">**allowUnlimitedLength**</span><span class="sxs-lookup"><span data-stu-id="c81e6-115">**allowUnlimitedLength**</span></span>  | <span data-ttu-id="c81e6-116">boolean</span><span class="sxs-lookup"><span data-stu-id="c81e6-116">boolean</span></span> | <span data-ttu-id="c81e6-117">指示列中的值是否可以超过 255 个字符的标准限制。</span><span class="sxs-lookup"><span data-stu-id="c81e6-117">Indicates whether values in the column should be able to exceed the standard limit of 255 characters.</span></span>
| <span data-ttu-id="c81e6-118">**columnName**</span><span class="sxs-lookup"><span data-stu-id="c81e6-118">**columnName**</span></span>            | <span data-ttu-id="c81e6-119">string</span><span class="sxs-lookup"><span data-stu-id="c81e6-119">string</span></span>  | <span data-ttu-id="c81e6-120">查找源列的名称。</span><span class="sxs-lookup"><span data-stu-id="c81e6-120">The name of the lookup source column.</span></span>
| <span data-ttu-id="c81e6-121">**listId**</span><span class="sxs-lookup"><span data-stu-id="c81e6-121">**listId**</span></span>                | <span data-ttu-id="c81e6-122">string</span><span class="sxs-lookup"><span data-stu-id="c81e6-122">string</span></span>  | <span data-ttu-id="c81e6-123">查找源列表的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="c81e6-123">The unique identifier of the lookup source list.</span></span>
| <span data-ttu-id="c81e6-124">**primaryLookupColumnId**</span><span class="sxs-lookup"><span data-stu-id="c81e6-124">**primaryLookupColumnId**</span></span> | <span data-ttu-id="c81e6-125">string</span><span class="sxs-lookup"><span data-stu-id="c81e6-125">string</span></span>  | <span data-ttu-id="c81e6-126">如果已指定，则此列为*辅助查找*，同时从*主查找*查找的列表项中拉取一个附加字段。</span><span class="sxs-lookup"><span data-stu-id="c81e6-126">If specified, this column is a *secondary lookup*, pulling an additional field from the list item looked up by the *primary lookup*.</span></span> <span data-ttu-id="c81e6-127">使用*主查找*查找的列表项作为此处列出的列的源。</span><span class="sxs-lookup"><span data-stu-id="c81e6-127">Use the list item looked up by the *primary* as the source for the column named here.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/LookupColumn"
} -->

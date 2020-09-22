---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: TextColumn
localization_priority: Normal
description: columnDefinition 资源上的 textColumn 指示该列的值为文本。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: e425c3345360702fa9a2b45c84e83ffcd8708160
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48090912"
---
# <a name="textcolumn-resource-type"></a><span data-ttu-id="8d2d5-103">TextColumn 资源类型</span><span class="sxs-lookup"><span data-stu-id="8d2d5-103">TextColumn resource type</span></span>

<span data-ttu-id="8d2d5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8d2d5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8d2d5-105">[columnDefinition](columndefinition.md) 资源上的 **textColumn** 指示该列的值为文本。</span><span class="sxs-lookup"><span data-stu-id="8d2d5-105">The **textColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are text.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8d2d5-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8d2d5-106">JSON representation</span></span>

<span data-ttu-id="8d2d5-107">下面是 **textColumn** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8d2d5-107">Here is a JSON representation of a **textColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.textColumn" } -->

```json
{
  "allowMultipleLines": true,
  "appendChangesToExistingText": false,
  "linesForEditing": 6,
  "maxLength": 300,
  "textType": "plain | richText"
}
```

## <a name="properties"></a><span data-ttu-id="8d2d5-108">属性</span><span class="sxs-lookup"><span data-stu-id="8d2d5-108">Properties</span></span>

| <span data-ttu-id="8d2d5-109">属性名称</span><span class="sxs-lookup"><span data-stu-id="8d2d5-109">Property name</span></span>                   | <span data-ttu-id="8d2d5-110">类型</span><span class="sxs-lookup"><span data-stu-id="8d2d5-110">Type</span></span>    | <span data-ttu-id="8d2d5-111">说明</span><span class="sxs-lookup"><span data-stu-id="8d2d5-111">Description</span></span>
|:--------------------------------|:--------|:---------------------------------
| <span data-ttu-id="8d2d5-112">**allowMultipleLines**</span><span class="sxs-lookup"><span data-stu-id="8d2d5-112">**allowMultipleLines**</span></span>          | <span data-ttu-id="8d2d5-113">boolean</span><span class="sxs-lookup"><span data-stu-id="8d2d5-113">boolean</span></span> | <span data-ttu-id="8d2d5-114">是否支持多行文本。</span><span class="sxs-lookup"><span data-stu-id="8d2d5-114">Whether to allow multiple lines of text.</span></span>
| <span data-ttu-id="8d2d5-115">**appendChangesToExistingText**</span><span class="sxs-lookup"><span data-stu-id="8d2d5-115">**appendChangesToExistingText**</span></span> | <span data-ttu-id="8d2d5-116">boolean</span><span class="sxs-lookup"><span data-stu-id="8d2d5-116">boolean</span></span> | <span data-ttu-id="8d2d5-117">对此列的更新应替换现有文本，还是附加到现有文本。</span><span class="sxs-lookup"><span data-stu-id="8d2d5-117">Whether updates to this column should replace existing text, or append to it.</span></span>
| <span data-ttu-id="8d2d5-118">**linesForEditing**</span><span class="sxs-lookup"><span data-stu-id="8d2d5-118">**linesForEditing**</span></span>             | <span data-ttu-id="8d2d5-119">int32</span><span class="sxs-lookup"><span data-stu-id="8d2d5-119">int32</span></span>   | <span data-ttu-id="8d2d5-120">文本框的大小。</span><span class="sxs-lookup"><span data-stu-id="8d2d5-120">The size of the text box.</span></span>
| <span data-ttu-id="8d2d5-121">**maxLength**</span><span class="sxs-lookup"><span data-stu-id="8d2d5-121">**maxLength**</span></span>                   | <span data-ttu-id="8d2d5-122">int32</span><span class="sxs-lookup"><span data-stu-id="8d2d5-122">int32</span></span>   | <span data-ttu-id="8d2d5-123">值的最大字符数。</span><span class="sxs-lookup"><span data-stu-id="8d2d5-123">The maximum number of characters for the value.</span></span>
| <span data-ttu-id="8d2d5-124">**textType**</span><span class="sxs-lookup"><span data-stu-id="8d2d5-124">**textType**</span></span>                    | <span data-ttu-id="8d2d5-125">string</span><span class="sxs-lookup"><span data-stu-id="8d2d5-125">string</span></span>  | <span data-ttu-id="8d2d5-126">要存储的文本类型。</span><span class="sxs-lookup"><span data-stu-id="8d2d5-126">The type of text being stored.</span></span> <span data-ttu-id="8d2d5-127">必须为 `plain` 或 `richText`.的其中一个</span><span class="sxs-lookup"><span data-stu-id="8d2d5-127">Must be one of `plain` or `richText`</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/textcolumn.md:
      Found potential enums in resource example that weren't defined in a table:(plain,richText) are in resource, but () are in table"
  ],
  "tocPath": "Resources/TextColumn"
} -->


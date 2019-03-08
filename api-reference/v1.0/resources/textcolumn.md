---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: TextColumn
localization_priority: Normal
ms.openlocfilehash: 1e10997bd70f97fa91177aee48a6ffcecff40ab5
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2019
ms.locfileid: "30480836"
---
# <a name="textcolumn-resource-type"></a><span data-ttu-id="e7b0f-102">TextColumn 资源类型</span><span class="sxs-lookup"><span data-stu-id="e7b0f-102">TextColumn resource type</span></span>

<span data-ttu-id="e7b0f-103">[columnDefinition](columndefinition.md) 资源上的 **textColumn** 指示该列的值为文本。</span><span class="sxs-lookup"><span data-stu-id="e7b0f-103">The **textColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are text.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e7b0f-104">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e7b0f-104">JSON representation</span></span>

<span data-ttu-id="e7b0f-105">下面是 **textColumn** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e7b0f-105">Here is a JSON representation of a **textColumn** resource.</span></span>
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

## <a name="properties"></a><span data-ttu-id="e7b0f-106">属性</span><span class="sxs-lookup"><span data-stu-id="e7b0f-106">Properties</span></span>

| <span data-ttu-id="e7b0f-107">属性名称</span><span class="sxs-lookup"><span data-stu-id="e7b0f-107">Property name</span></span>                   | <span data-ttu-id="e7b0f-108">类型</span><span class="sxs-lookup"><span data-stu-id="e7b0f-108">Type</span></span>    | <span data-ttu-id="e7b0f-109">说明</span><span class="sxs-lookup"><span data-stu-id="e7b0f-109">Description</span></span>
|:--------------------------------|:--------|:---------------------------------
| <span data-ttu-id="e7b0f-110">**allowMultipleLines**</span><span class="sxs-lookup"><span data-stu-id="e7b0f-110">**allowMultipleLines**</span></span>          | <span data-ttu-id="e7b0f-111">布尔</span><span class="sxs-lookup"><span data-stu-id="e7b0f-111">boolean</span></span> | <span data-ttu-id="e7b0f-112">是否支持多行文本。</span><span class="sxs-lookup"><span data-stu-id="e7b0f-112">Whether to allow multiple lines of text.</span></span>
| <span data-ttu-id="e7b0f-113">**appendChangesToExistingText**</span><span class="sxs-lookup"><span data-stu-id="e7b0f-113">**appendChangesToExistingText**</span></span> | <span data-ttu-id="e7b0f-114">布尔</span><span class="sxs-lookup"><span data-stu-id="e7b0f-114">boolean</span></span> | <span data-ttu-id="e7b0f-115">对此列的更新应替换现有文本，还是附加到现有文本。</span><span class="sxs-lookup"><span data-stu-id="e7b0f-115">Whether updates to this column should replace existing text, or append to it.</span></span>
| <span data-ttu-id="e7b0f-116">**linesForEditing**</span><span class="sxs-lookup"><span data-stu-id="e7b0f-116">**linesForEditing**</span></span>             | <span data-ttu-id="e7b0f-117">时会</span><span class="sxs-lookup"><span data-stu-id="e7b0f-117">int32</span></span>   | <span data-ttu-id="e7b0f-118">文本框的大小。</span><span class="sxs-lookup"><span data-stu-id="e7b0f-118">The size of the text box.</span></span>
| <span data-ttu-id="e7b0f-119">**maxLength**</span><span class="sxs-lookup"><span data-stu-id="e7b0f-119">**maxLength**</span></span>                   | <span data-ttu-id="e7b0f-120">时会</span><span class="sxs-lookup"><span data-stu-id="e7b0f-120">int32</span></span>   | <span data-ttu-id="e7b0f-121">值的最大字符数。</span><span class="sxs-lookup"><span data-stu-id="e7b0f-121">The maximum number of characters for the value.</span></span>
| <span data-ttu-id="e7b0f-122">**textType**</span><span class="sxs-lookup"><span data-stu-id="e7b0f-122">**textType**</span></span>                    | <span data-ttu-id="e7b0f-123">string</span><span class="sxs-lookup"><span data-stu-id="e7b0f-123">string</span></span>  | <span data-ttu-id="e7b0f-124">要存储的文本类型。</span><span class="sxs-lookup"><span data-stu-id="e7b0f-124">The type of text being stored.</span></span> <span data-ttu-id="e7b0f-125">必须为 `plain` 或 `richText`.的其中一个</span><span class="sxs-lookup"><span data-stu-id="e7b0f-125">Must be one of `plain` or `richText`</span></span>

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

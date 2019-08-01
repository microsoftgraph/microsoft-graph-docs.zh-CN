---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: TextColumn
localization_priority: Normal
description: columnDefinition 资源上的 textColumn 指示该列的值为文本。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 37a5bbd985d163cf627f4bc0a16a756eaf00af66
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033654"
---
# <a name="textcolumn-resource-type"></a><span data-ttu-id="47821-103">TextColumn 资源类型</span><span class="sxs-lookup"><span data-stu-id="47821-103">TextColumn resource type</span></span>

<span data-ttu-id="47821-104">[columnDefinition](columndefinition.md) 资源上的 **textColumn** 指示该列的值为文本。</span><span class="sxs-lookup"><span data-stu-id="47821-104">The **textColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are text.</span></span>

## <a name="json-representation"></a><span data-ttu-id="47821-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="47821-105">JSON representation</span></span>

<span data-ttu-id="47821-106">下面是 **textColumn** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="47821-106">Here is a JSON representation of a **textColumn** resource.</span></span>
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

## <a name="properties"></a><span data-ttu-id="47821-107">属性</span><span class="sxs-lookup"><span data-stu-id="47821-107">Properties</span></span>

| <span data-ttu-id="47821-108">属性名称</span><span class="sxs-lookup"><span data-stu-id="47821-108">Property name</span></span>                   | <span data-ttu-id="47821-109">类型</span><span class="sxs-lookup"><span data-stu-id="47821-109">Type</span></span>    | <span data-ttu-id="47821-110">说明</span><span class="sxs-lookup"><span data-stu-id="47821-110">Description</span></span>
|:--------------------------------|:--------|:---------------------------------
| <span data-ttu-id="47821-111">**allowMultipleLines**</span><span class="sxs-lookup"><span data-stu-id="47821-111">**allowMultipleLines**</span></span>          | <span data-ttu-id="47821-112">boolean</span><span class="sxs-lookup"><span data-stu-id="47821-112">boolean</span></span> | <span data-ttu-id="47821-113">是否支持多行文本。</span><span class="sxs-lookup"><span data-stu-id="47821-113">Whether to allow multiple lines of text.</span></span>
| <span data-ttu-id="47821-114">**appendChangesToExistingText**</span><span class="sxs-lookup"><span data-stu-id="47821-114">**appendChangesToExistingText**</span></span> | <span data-ttu-id="47821-115">boolean</span><span class="sxs-lookup"><span data-stu-id="47821-115">boolean</span></span> | <span data-ttu-id="47821-116">对此列的更新应替换现有文本，还是附加到现有文本。</span><span class="sxs-lookup"><span data-stu-id="47821-116">Whether updates to this column should replace existing text, or append to it.</span></span>
| <span data-ttu-id="47821-117">**linesForEditing**</span><span class="sxs-lookup"><span data-stu-id="47821-117">**linesForEditing**</span></span>             | <span data-ttu-id="47821-118">int32</span><span class="sxs-lookup"><span data-stu-id="47821-118">int32</span></span>   | <span data-ttu-id="47821-119">文本框的大小。</span><span class="sxs-lookup"><span data-stu-id="47821-119">The size of the text box.</span></span>
| <span data-ttu-id="47821-120">**maxLength**</span><span class="sxs-lookup"><span data-stu-id="47821-120">**maxLength**</span></span>                   | <span data-ttu-id="47821-121">int32</span><span class="sxs-lookup"><span data-stu-id="47821-121">int32</span></span>   | <span data-ttu-id="47821-122">值的最大字符数。</span><span class="sxs-lookup"><span data-stu-id="47821-122">The maximum number of characters for the value.</span></span>
| <span data-ttu-id="47821-123">**textType**</span><span class="sxs-lookup"><span data-stu-id="47821-123">**textType**</span></span>                    | <span data-ttu-id="47821-124">string</span><span class="sxs-lookup"><span data-stu-id="47821-124">string</span></span>  | <span data-ttu-id="47821-125">要存储的文本类型。</span><span class="sxs-lookup"><span data-stu-id="47821-125">The type of text being stored.</span></span> <span data-ttu-id="47821-126">必须为 `plain` 或 `richText`.的其中一个</span><span class="sxs-lookup"><span data-stu-id="47821-126">Must be one of `plain` or `richText`</span></span>

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

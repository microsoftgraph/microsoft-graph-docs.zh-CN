---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: TextColumn
localization_priority: Normal
description: columnDefinition 资源上的 textColumn 指示该列的值为文本。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 67e6b1f24155a8cfcecb2fb2443f3b1536ba48bd
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533470"
---
# <a name="textcolumn-resource-type"></a><span data-ttu-id="1d1ba-103">TextColumn 资源类型</span><span class="sxs-lookup"><span data-stu-id="1d1ba-103">TextColumn resource type</span></span>

<span data-ttu-id="1d1ba-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1d1ba-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1d1ba-105">[columnDefinition](columndefinition.md) 资源上的 **textColumn** 指示该列的值为文本。</span><span class="sxs-lookup"><span data-stu-id="1d1ba-105">The **textColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are text.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1d1ba-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1d1ba-106">JSON representation</span></span>

<span data-ttu-id="1d1ba-107">下面是 **textColumn** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1d1ba-107">Here is a JSON representation of a **textColumn** resource.</span></span>
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

## <a name="properties"></a><span data-ttu-id="1d1ba-108">属性</span><span class="sxs-lookup"><span data-stu-id="1d1ba-108">Properties</span></span>

| <span data-ttu-id="1d1ba-109">属性名称</span><span class="sxs-lookup"><span data-stu-id="1d1ba-109">Property name</span></span>                   | <span data-ttu-id="1d1ba-110">类型</span><span class="sxs-lookup"><span data-stu-id="1d1ba-110">Type</span></span>    | <span data-ttu-id="1d1ba-111">说明</span><span class="sxs-lookup"><span data-stu-id="1d1ba-111">Description</span></span>
|:--------------------------------|:--------|:---------------------------------
| <span data-ttu-id="1d1ba-112">**allowMultipleLines**</span><span class="sxs-lookup"><span data-stu-id="1d1ba-112">**allowMultipleLines**</span></span>          | <span data-ttu-id="1d1ba-113">boolean</span><span class="sxs-lookup"><span data-stu-id="1d1ba-113">boolean</span></span> | <span data-ttu-id="1d1ba-114">是否支持多行文本。</span><span class="sxs-lookup"><span data-stu-id="1d1ba-114">Whether to allow multiple lines of text.</span></span>
| <span data-ttu-id="1d1ba-115">**appendChangesToExistingText**</span><span class="sxs-lookup"><span data-stu-id="1d1ba-115">**appendChangesToExistingText**</span></span> | <span data-ttu-id="1d1ba-116">boolean</span><span class="sxs-lookup"><span data-stu-id="1d1ba-116">boolean</span></span> | <span data-ttu-id="1d1ba-117">对此列的更新应替换现有文本，还是附加到现有文本。</span><span class="sxs-lookup"><span data-stu-id="1d1ba-117">Whether updates to this column should replace existing text, or append to it.</span></span>
| <span data-ttu-id="1d1ba-118">**linesForEditing**</span><span class="sxs-lookup"><span data-stu-id="1d1ba-118">**linesForEditing**</span></span>             | <span data-ttu-id="1d1ba-119">int32</span><span class="sxs-lookup"><span data-stu-id="1d1ba-119">int32</span></span>   | <span data-ttu-id="1d1ba-120">文本框的大小。</span><span class="sxs-lookup"><span data-stu-id="1d1ba-120">The size of the text box.</span></span>
| <span data-ttu-id="1d1ba-121">**maxLength**</span><span class="sxs-lookup"><span data-stu-id="1d1ba-121">**maxLength**</span></span>                   | <span data-ttu-id="1d1ba-122">int32</span><span class="sxs-lookup"><span data-stu-id="1d1ba-122">int32</span></span>   | <span data-ttu-id="1d1ba-123">值的最大字符数。</span><span class="sxs-lookup"><span data-stu-id="1d1ba-123">The maximum number of characters for the value.</span></span>
| <span data-ttu-id="1d1ba-124">**textType**</span><span class="sxs-lookup"><span data-stu-id="1d1ba-124">**textType**</span></span>                    | <span data-ttu-id="1d1ba-125">string</span><span class="sxs-lookup"><span data-stu-id="1d1ba-125">string</span></span>  | <span data-ttu-id="1d1ba-126">要存储的文本类型。</span><span class="sxs-lookup"><span data-stu-id="1d1ba-126">The type of text being stored.</span></span> <span data-ttu-id="1d1ba-127">必须为 `plain` 或 `richText`.的其中一个</span><span class="sxs-lookup"><span data-stu-id="1d1ba-127">Must be one of `plain` or `richText`</span></span>

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

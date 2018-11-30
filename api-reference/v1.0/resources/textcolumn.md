---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: TextColumn
ms.openlocfilehash: 810554620e747d3160a6d8c74913518b8590c19d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27010898"
---
# <a name="textcolumn-resource-type"></a><span data-ttu-id="c486c-102">TextColumn 资源类型</span><span class="sxs-lookup"><span data-stu-id="c486c-102">TextColumn resource type</span></span>

<span data-ttu-id="c486c-103">[columnDefinition](columndefinition.md) 资源上的 **textColumn** 指示该列的值为文本。</span><span class="sxs-lookup"><span data-stu-id="c486c-103">The **textColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are text.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c486c-104">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c486c-104">JSON representation</span></span>

<span data-ttu-id="c486c-105">下面是 **textColumn** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c486c-105">Here is a JSON representation of a **textColumn** resource.</span></span>
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

## <a name="properties"></a><span data-ttu-id="c486c-106">属性</span><span class="sxs-lookup"><span data-stu-id="c486c-106">Properties</span></span>

| <span data-ttu-id="c486c-107">属性名称</span><span class="sxs-lookup"><span data-stu-id="c486c-107">Property name</span></span>                   | <span data-ttu-id="c486c-108">类型</span><span class="sxs-lookup"><span data-stu-id="c486c-108">Type</span></span>    | <span data-ttu-id="c486c-109">说明</span><span class="sxs-lookup"><span data-stu-id="c486c-109">Description</span></span>
|:--------------------------------|:--------|:---------------------------------
| <span data-ttu-id="c486c-110">**allowMultipleLines**</span><span class="sxs-lookup"><span data-stu-id="c486c-110">**allowMultipleLines**</span></span>          | <span data-ttu-id="c486c-111">boolean</span><span class="sxs-lookup"><span data-stu-id="c486c-111">boolean</span></span> | <span data-ttu-id="c486c-112">是否支持多行文本。</span><span class="sxs-lookup"><span data-stu-id="c486c-112">Whether to allow multiple lines of text.</span></span>
| <span data-ttu-id="c486c-113">**appendChangesToExistingText**</span><span class="sxs-lookup"><span data-stu-id="c486c-113">**appendChangesToExistingText**</span></span> | <span data-ttu-id="c486c-114">boolean</span><span class="sxs-lookup"><span data-stu-id="c486c-114">boolean</span></span> | <span data-ttu-id="c486c-115">对此列的更新应替换现有文本，还是附加到现有文本。</span><span class="sxs-lookup"><span data-stu-id="c486c-115">Whether updates to this column should replace existing text, or append to it.</span></span>
| <span data-ttu-id="c486c-116">**linesForEditing**</span><span class="sxs-lookup"><span data-stu-id="c486c-116">**linesForEditing**</span></span>             | <span data-ttu-id="c486c-117">int32</span><span class="sxs-lookup"><span data-stu-id="c486c-117">int32</span></span>   | <span data-ttu-id="c486c-118">文本框的大小。</span><span class="sxs-lookup"><span data-stu-id="c486c-118">The size of the text box.</span></span>
| <span data-ttu-id="c486c-119">**maxLength**</span><span class="sxs-lookup"><span data-stu-id="c486c-119">**maxLength**</span></span>                   | <span data-ttu-id="c486c-120">int32</span><span class="sxs-lookup"><span data-stu-id="c486c-120">int32</span></span>   | <span data-ttu-id="c486c-121">值的最大字符数。</span><span class="sxs-lookup"><span data-stu-id="c486c-121">The maximum number of characters for the value.</span></span>
| <span data-ttu-id="c486c-122">**textType**</span><span class="sxs-lookup"><span data-stu-id="c486c-122">**textType**</span></span>                    | <span data-ttu-id="c486c-123">string</span><span class="sxs-lookup"><span data-stu-id="c486c-123">string</span></span>  | <span data-ttu-id="c486c-124">要存储的文本类型。</span><span class="sxs-lookup"><span data-stu-id="c486c-124">The type of text being stored.</span></span> <span data-ttu-id="c486c-125">必须为 `plain` 或 `richText`.的其中一个</span><span class="sxs-lookup"><span data-stu-id="c486c-125">Must be one of `plain` or `richText`</span></span>

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

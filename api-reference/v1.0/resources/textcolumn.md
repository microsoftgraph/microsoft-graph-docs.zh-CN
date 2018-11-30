---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: TextColumn
ms.openlocfilehash: 80e41b379b9b4ce51a3ee6c910447a22f43356c3
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/28/2017
---
# <a name="textcolumn-resource-type"></a><span data-ttu-id="80004-102">TextColumn 资源类型</span><span class="sxs-lookup"><span data-stu-id="80004-102">TextColumn resource type</span></span>

<span data-ttu-id="80004-103">[columnDefinition](columnDefinition.md) 资源上的 **textColumn** 指示该列的值为文本。</span><span class="sxs-lookup"><span data-stu-id="80004-103">The **textColumn** on a [columnDefinition](columnDefinition.md) resource indicates that the column's values are text.</span></span>

## <a name="json-representation"></a><span data-ttu-id="80004-104">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="80004-104">JSON representation</span></span>

<span data-ttu-id="80004-105">下面是 **textColumn** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="80004-105">Here is a JSON representation of a **baseItem** resource.</span></span>
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

## <a name="properties"></a><span data-ttu-id="80004-106">属性</span><span class="sxs-lookup"><span data-stu-id="80004-106">Properties</span></span>

| <span data-ttu-id="80004-107">属性名称</span><span class="sxs-lookup"><span data-stu-id="80004-107">Property name</span></span>                   | <span data-ttu-id="80004-108">类型</span><span class="sxs-lookup"><span data-stu-id="80004-108">Type</span></span>   | <span data-ttu-id="80004-109">说明</span><span class="sxs-lookup"><span data-stu-id="80004-109">Description</span></span>
|:--------------------------------|:-------|:-----------------------------------------------
| <span data-ttu-id="80004-110">**allowMultipleLines**</span><span class="sxs-lookup"><span data-stu-id="80004-110">**allowMultipleLines**</span></span>          | <span data-ttu-id="80004-111">string</span><span class="sxs-lookup"><span data-stu-id="80004-111">string</span></span> | <span data-ttu-id="80004-112">是否允许多行文本。</span><span class="sxs-lookup"><span data-stu-id="80004-112">Whether to allow multiple lines of text.</span></span>
| <span data-ttu-id="80004-113">**appendChangesToExistingText**</span><span class="sxs-lookup"><span data-stu-id="80004-113">**appendChangesToExistingText**</span></span> | <span data-ttu-id="80004-114">string</span><span class="sxs-lookup"><span data-stu-id="80004-114">string</span></span> | <span data-ttu-id="80004-115">对此列的更新是应替换现有文本，还是追加到现有文本。</span><span class="sxs-lookup"><span data-stu-id="80004-115">Whether updates to this column should replace existing text, or append to it.</span></span>
| <span data-ttu-id="80004-116">**linesForEditing**</span><span class="sxs-lookup"><span data-stu-id="80004-116">**linesForEditing**</span></span>             | <span data-ttu-id="80004-117">int</span><span class="sxs-lookup"><span data-stu-id="80004-117">int</span></span>    | <span data-ttu-id="80004-118">文本框的大小。</span><span class="sxs-lookup"><span data-stu-id="80004-118">The size of the text box.</span></span>
| <span data-ttu-id="80004-119">**maxLength**</span><span class="sxs-lookup"><span data-stu-id="80004-119">**maxLength**</span></span>                   | <span data-ttu-id="80004-120">int</span><span class="sxs-lookup"><span data-stu-id="80004-120">int</span></span>    | <span data-ttu-id="80004-121">值的最大字符数。</span><span class="sxs-lookup"><span data-stu-id="80004-121">The maximum number of characters for the value.</span></span>
| <span data-ttu-id="80004-122">**textType**</span><span class="sxs-lookup"><span data-stu-id="80004-122">**textType**</span></span>                    | <span data-ttu-id="80004-123">string</span><span class="sxs-lookup"><span data-stu-id="80004-123">string</span></span> | <span data-ttu-id="80004-124">要存储的文本类型。</span><span class="sxs-lookup"><span data-stu-id="80004-124">The type of text being stored.</span></span> <span data-ttu-id="80004-125">必须是 `plain` 或 `richText` 的其中一个</span><span class="sxs-lookup"><span data-stu-id="80004-125">Must be one of `plain` or `richText`</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/TextColumn"
} -->

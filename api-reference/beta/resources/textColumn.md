---
author: JeremyKelley
description: columnDefinition 资源上的 textColumn 指示该列的值为文本。
ms.date: 09/11/2017
title: TextColumn
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 6681875328695d2e67cc10508f47183fcedb0df4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964338"
---
# <a name="textcolumn-resource-type"></a><span data-ttu-id="0f144-103">TextColumn 资源类型</span><span class="sxs-lookup"><span data-stu-id="0f144-103">TextColumn resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0f144-104">[columnDefinition](columndefinition.md) 资源上的 **textColumn** 指示该列的值为文本。</span><span class="sxs-lookup"><span data-stu-id="0f144-104">The **textColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are text.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0f144-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0f144-105">JSON representation</span></span>

<span data-ttu-id="0f144-106">下面是 **textColumn** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0f144-106">Here is a JSON representation of a **textColumn** resource.</span></span>
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

## <a name="properties"></a><span data-ttu-id="0f144-107">属性</span><span class="sxs-lookup"><span data-stu-id="0f144-107">Properties</span></span>

| <span data-ttu-id="0f144-108">属性名称</span><span class="sxs-lookup"><span data-stu-id="0f144-108">Property name</span></span>                   | <span data-ttu-id="0f144-109">类型</span><span class="sxs-lookup"><span data-stu-id="0f144-109">Type</span></span>   | <span data-ttu-id="0f144-110">说明</span><span class="sxs-lookup"><span data-stu-id="0f144-110">Description</span></span>
|:--------------------------------|:-------|:-----------------------------------------------
| <span data-ttu-id="0f144-111">**allowMultipleLines**</span><span class="sxs-lookup"><span data-stu-id="0f144-111">**allowMultipleLines**</span></span>          | <span data-ttu-id="0f144-112">string</span><span class="sxs-lookup"><span data-stu-id="0f144-112">string</span></span> | <span data-ttu-id="0f144-113">是否支持多行文本。</span><span class="sxs-lookup"><span data-stu-id="0f144-113">Whether to allow multiple lines of text.</span></span>
| <span data-ttu-id="0f144-114">**appendChangesToExistingText**</span><span class="sxs-lookup"><span data-stu-id="0f144-114">**appendChangesToExistingText**</span></span> | <span data-ttu-id="0f144-115">string</span><span class="sxs-lookup"><span data-stu-id="0f144-115">string</span></span> | <span data-ttu-id="0f144-116">对此列的更新应替换现有文本，还是附加到现有文本。</span><span class="sxs-lookup"><span data-stu-id="0f144-116">Whether updates to this column should replace existing text, or append to it.</span></span>
| <span data-ttu-id="0f144-117">**linesForEditing**</span><span class="sxs-lookup"><span data-stu-id="0f144-117">**linesForEditing**</span></span>             | <span data-ttu-id="0f144-118">int</span><span class="sxs-lookup"><span data-stu-id="0f144-118">int</span></span>    | <span data-ttu-id="0f144-119">文本框的大小。</span><span class="sxs-lookup"><span data-stu-id="0f144-119">The size of the text box.</span></span>
| <span data-ttu-id="0f144-120">**maxLength**</span><span class="sxs-lookup"><span data-stu-id="0f144-120">**maxLength**</span></span>                   | <span data-ttu-id="0f144-121">int</span><span class="sxs-lookup"><span data-stu-id="0f144-121">int</span></span>    | <span data-ttu-id="0f144-122">值的最大字符数。</span><span class="sxs-lookup"><span data-stu-id="0f144-122">The maximum number of characters for the value.</span></span>
| <span data-ttu-id="0f144-123">**textType**</span><span class="sxs-lookup"><span data-stu-id="0f144-123">**textType**</span></span>                    | <span data-ttu-id="0f144-124">string</span><span class="sxs-lookup"><span data-stu-id="0f144-124">string</span></span> | <span data-ttu-id="0f144-125">要存储的文本类型。</span><span class="sxs-lookup"><span data-stu-id="0f144-125">The type of text being stored.</span></span> <span data-ttu-id="0f144-126">必须为 `plain` 或 `richText`.的其中一个</span><span class="sxs-lookup"><span data-stu-id="0f144-126">Must be one of `plain` or `richText`</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/TextColumn",
  "suppressions": []
}
-->

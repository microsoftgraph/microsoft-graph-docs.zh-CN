---
author: JeremyKelley
description: columnDefinition 资源上的 textColumn 指示该列的值为文本。
ms.date: 09/11/2017
title: TextColumn
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: ecfd6d72e0946519b570962577b03a9ffcbcdf10
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47973545"
---
# <a name="textcolumn-resource-type"></a><span data-ttu-id="5d37c-103">TextColumn 资源类型</span><span class="sxs-lookup"><span data-stu-id="5d37c-103">TextColumn resource type</span></span>

<span data-ttu-id="5d37c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5d37c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5d37c-105">[columnDefinition](columndefinition.md) 资源上的 **textColumn** 指示该列的值为文本。</span><span class="sxs-lookup"><span data-stu-id="5d37c-105">The **textColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are text.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5d37c-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5d37c-106">JSON representation</span></span>

<span data-ttu-id="5d37c-107">下面是 **textColumn** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5d37c-107">Here is a JSON representation of a **textColumn** resource.</span></span>
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

## <a name="properties"></a><span data-ttu-id="5d37c-108">属性</span><span class="sxs-lookup"><span data-stu-id="5d37c-108">Properties</span></span>

| <span data-ttu-id="5d37c-109">属性名称</span><span class="sxs-lookup"><span data-stu-id="5d37c-109">Property name</span></span>                   | <span data-ttu-id="5d37c-110">类型</span><span class="sxs-lookup"><span data-stu-id="5d37c-110">Type</span></span>   | <span data-ttu-id="5d37c-111">说明</span><span class="sxs-lookup"><span data-stu-id="5d37c-111">Description</span></span>
|:--------------------------------|:-------|:-----------------------------------------------
| <span data-ttu-id="5d37c-112">**allowMultipleLines**</span><span class="sxs-lookup"><span data-stu-id="5d37c-112">**allowMultipleLines**</span></span>          | <span data-ttu-id="5d37c-113">string</span><span class="sxs-lookup"><span data-stu-id="5d37c-113">string</span></span> | <span data-ttu-id="5d37c-114">是否支持多行文本。</span><span class="sxs-lookup"><span data-stu-id="5d37c-114">Whether to allow multiple lines of text.</span></span>
| <span data-ttu-id="5d37c-115">**appendChangesToExistingText**</span><span class="sxs-lookup"><span data-stu-id="5d37c-115">**appendChangesToExistingText**</span></span> | <span data-ttu-id="5d37c-116">string</span><span class="sxs-lookup"><span data-stu-id="5d37c-116">string</span></span> | <span data-ttu-id="5d37c-117">对此列的更新应替换现有文本，还是附加到现有文本。</span><span class="sxs-lookup"><span data-stu-id="5d37c-117">Whether updates to this column should replace existing text, or append to it.</span></span>
| <span data-ttu-id="5d37c-118">**linesForEditing**</span><span class="sxs-lookup"><span data-stu-id="5d37c-118">**linesForEditing**</span></span>             | <span data-ttu-id="5d37c-119">int</span><span class="sxs-lookup"><span data-stu-id="5d37c-119">int</span></span>    | <span data-ttu-id="5d37c-120">文本框的大小。</span><span class="sxs-lookup"><span data-stu-id="5d37c-120">The size of the text box.</span></span>
| <span data-ttu-id="5d37c-121">**maxLength**</span><span class="sxs-lookup"><span data-stu-id="5d37c-121">**maxLength**</span></span>                   | <span data-ttu-id="5d37c-122">int</span><span class="sxs-lookup"><span data-stu-id="5d37c-122">int</span></span>    | <span data-ttu-id="5d37c-123">值的最大字符数。</span><span class="sxs-lookup"><span data-stu-id="5d37c-123">The maximum number of characters for the value.</span></span>
| <span data-ttu-id="5d37c-124">**textType**</span><span class="sxs-lookup"><span data-stu-id="5d37c-124">**textType**</span></span>                    | <span data-ttu-id="5d37c-125">string</span><span class="sxs-lookup"><span data-stu-id="5d37c-125">string</span></span> | <span data-ttu-id="5d37c-126">要存储的文本类型。</span><span class="sxs-lookup"><span data-stu-id="5d37c-126">The type of text being stored.</span></span> <span data-ttu-id="5d37c-127">必须为 `plain` 或 `richText`.的其中一个</span><span class="sxs-lookup"><span data-stu-id="5d37c-127">Must be one of `plain` or `richText`</span></span>

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



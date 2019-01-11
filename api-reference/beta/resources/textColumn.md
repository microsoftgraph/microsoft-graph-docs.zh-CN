---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: TextColumn
localization_priority: Normal
ms.openlocfilehash: 87a5e27544a49613d1d1e44cd6f3e0e3b7fcf8c4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27822566"
---
# <a name="textcolumn-resource-type"></a><span data-ttu-id="d4246-102">TextColumn 资源类型</span><span class="sxs-lookup"><span data-stu-id="d4246-102">TextColumn resource type</span></span>

> <span data-ttu-id="d4246-103">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="d4246-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d4246-104">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d4246-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d4246-105">[columnDefinition](columndefinition.md) 资源上的 **textColumn** 指示该列的值为文本。</span><span class="sxs-lookup"><span data-stu-id="d4246-105">The **textColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are text.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d4246-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d4246-106">JSON representation</span></span>

<span data-ttu-id="d4246-107">下面是 **textColumn** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d4246-107">Here is a JSON representation of a **textColumn** resource.</span></span>
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

## <a name="properties"></a><span data-ttu-id="d4246-108">属性</span><span class="sxs-lookup"><span data-stu-id="d4246-108">Properties</span></span>

| <span data-ttu-id="d4246-109">属性名称</span><span class="sxs-lookup"><span data-stu-id="d4246-109">Property name</span></span>                   | <span data-ttu-id="d4246-110">类型</span><span class="sxs-lookup"><span data-stu-id="d4246-110">Type</span></span>   | <span data-ttu-id="d4246-111">说明</span><span class="sxs-lookup"><span data-stu-id="d4246-111">Description</span></span>
|:--------------------------------|:-------|:-----------------------------------------------
| <span data-ttu-id="d4246-112">**allowMultipleLines**</span><span class="sxs-lookup"><span data-stu-id="d4246-112">**allowMultipleLines**</span></span>          | <span data-ttu-id="d4246-113">string</span><span class="sxs-lookup"><span data-stu-id="d4246-113">string</span></span> | <span data-ttu-id="d4246-114">是否支持多行文本。</span><span class="sxs-lookup"><span data-stu-id="d4246-114">Whether to allow multiple lines of text.</span></span>
| <span data-ttu-id="d4246-115">**appendChangesToExistingText**</span><span class="sxs-lookup"><span data-stu-id="d4246-115">**appendChangesToExistingText**</span></span> | <span data-ttu-id="d4246-116">string</span><span class="sxs-lookup"><span data-stu-id="d4246-116">string</span></span> | <span data-ttu-id="d4246-117">对此列的更新应替换现有文本，还是附加到现有文本。</span><span class="sxs-lookup"><span data-stu-id="d4246-117">Whether updates to this column should replace existing text, or append to it.</span></span>
| <span data-ttu-id="d4246-118">**linesForEditing**</span><span class="sxs-lookup"><span data-stu-id="d4246-118">**linesForEditing**</span></span>             | <span data-ttu-id="d4246-119">int</span><span class="sxs-lookup"><span data-stu-id="d4246-119">int</span></span>    | <span data-ttu-id="d4246-120">文本框的大小。</span><span class="sxs-lookup"><span data-stu-id="d4246-120">The size of the text box.</span></span>
| <span data-ttu-id="d4246-121">**maxLength**</span><span class="sxs-lookup"><span data-stu-id="d4246-121">**maxLength**</span></span>                   | <span data-ttu-id="d4246-122">int</span><span class="sxs-lookup"><span data-stu-id="d4246-122">int</span></span>    | <span data-ttu-id="d4246-123">值的最大字符数。</span><span class="sxs-lookup"><span data-stu-id="d4246-123">The maximum number of characters for the value.</span></span>
| <span data-ttu-id="d4246-124">**textType**</span><span class="sxs-lookup"><span data-stu-id="d4246-124">**textType**</span></span>                    | <span data-ttu-id="d4246-125">string</span><span class="sxs-lookup"><span data-stu-id="d4246-125">string</span></span> | <span data-ttu-id="d4246-126">要存储的文本类型。</span><span class="sxs-lookup"><span data-stu-id="d4246-126">The type of text being stored.</span></span> <span data-ttu-id="d4246-127">必须为 `plain` 或 `richText`.的其中一个</span><span class="sxs-lookup"><span data-stu-id="d4246-127">Must be one of `plain` or `richText`</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/TextColumn"
} -->

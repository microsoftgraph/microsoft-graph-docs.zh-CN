---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: TextColumn
localization_priority: Normal
ms.openlocfilehash: c69dc7c30bff0f43327ec256af6071e34de6b898
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2019
ms.locfileid: "30481494"
---
# <a name="textcolumn-resource-type"></a><span data-ttu-id="d6182-102">TextColumn 资源类型</span><span class="sxs-lookup"><span data-stu-id="d6182-102">TextColumn resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d6182-103">[columnDefinition](columndefinition.md) 资源上的 **textColumn** 指示该列的值为文本。</span><span class="sxs-lookup"><span data-stu-id="d6182-103">The **textColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are text.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d6182-104">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d6182-104">JSON representation</span></span>

<span data-ttu-id="d6182-105">下面是 **textColumn** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d6182-105">Here is a JSON representation of a **textColumn** resource.</span></span>
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

## <a name="properties"></a><span data-ttu-id="d6182-106">属性</span><span class="sxs-lookup"><span data-stu-id="d6182-106">Properties</span></span>

| <span data-ttu-id="d6182-107">属性名称</span><span class="sxs-lookup"><span data-stu-id="d6182-107">Property name</span></span>                   | <span data-ttu-id="d6182-108">类型</span><span class="sxs-lookup"><span data-stu-id="d6182-108">Type</span></span>   | <span data-ttu-id="d6182-109">说明</span><span class="sxs-lookup"><span data-stu-id="d6182-109">Description</span></span>
|:--------------------------------|:-------|:-----------------------------------------------
| <span data-ttu-id="d6182-110">**allowMultipleLines**</span><span class="sxs-lookup"><span data-stu-id="d6182-110">**allowMultipleLines**</span></span>          | <span data-ttu-id="d6182-111">string</span><span class="sxs-lookup"><span data-stu-id="d6182-111">string</span></span> | <span data-ttu-id="d6182-112">是否支持多行文本。</span><span class="sxs-lookup"><span data-stu-id="d6182-112">Whether to allow multiple lines of text.</span></span>
| <span data-ttu-id="d6182-113">**appendChangesToExistingText**</span><span class="sxs-lookup"><span data-stu-id="d6182-113">**appendChangesToExistingText**</span></span> | <span data-ttu-id="d6182-114">string</span><span class="sxs-lookup"><span data-stu-id="d6182-114">string</span></span> | <span data-ttu-id="d6182-115">对此列的更新应替换现有文本，还是附加到现有文本。</span><span class="sxs-lookup"><span data-stu-id="d6182-115">Whether updates to this column should replace existing text, or append to it.</span></span>
| <span data-ttu-id="d6182-116">**linesForEditing**</span><span class="sxs-lookup"><span data-stu-id="d6182-116">**linesForEditing**</span></span>             | <span data-ttu-id="d6182-117">int</span><span class="sxs-lookup"><span data-stu-id="d6182-117">int</span></span>    | <span data-ttu-id="d6182-118">文本框的大小。</span><span class="sxs-lookup"><span data-stu-id="d6182-118">The size of the text box.</span></span>
| <span data-ttu-id="d6182-119">**maxLength**</span><span class="sxs-lookup"><span data-stu-id="d6182-119">**maxLength**</span></span>                   | <span data-ttu-id="d6182-120">int</span><span class="sxs-lookup"><span data-stu-id="d6182-120">int</span></span>    | <span data-ttu-id="d6182-121">值的最大字符数。</span><span class="sxs-lookup"><span data-stu-id="d6182-121">The maximum number of characters for the value.</span></span>
| <span data-ttu-id="d6182-122">**textType**</span><span class="sxs-lookup"><span data-stu-id="d6182-122">**textType**</span></span>                    | <span data-ttu-id="d6182-123">string</span><span class="sxs-lookup"><span data-stu-id="d6182-123">string</span></span> | <span data-ttu-id="d6182-124">要存储的文本类型。</span><span class="sxs-lookup"><span data-stu-id="d6182-124">The type of text being stored.</span></span> <span data-ttu-id="d6182-125">必须为 `plain` 或 `richText`.的其中一个</span><span class="sxs-lookup"><span data-stu-id="d6182-125">Must be one of `plain` or `richText`</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/TextColumn",
  "suppressions": [
    "Error: /api-reference/beta/resources/textColumn.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

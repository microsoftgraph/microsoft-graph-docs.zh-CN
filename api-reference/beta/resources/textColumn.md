---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: TextColumn
localization_priority: Normal
ms.openlocfilehash: 524f25b6b5097197daeb8b130b10ff7513010965
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525001"
---
# <a name="textcolumn-resource-type"></a><span data-ttu-id="c8966-102">TextColumn 资源类型</span><span class="sxs-lookup"><span data-stu-id="c8966-102">TextColumn resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c8966-103">[columnDefinition](columndefinition.md) 资源上的 **textColumn** 指示该列的值为文本。</span><span class="sxs-lookup"><span data-stu-id="c8966-103">The **textColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are text.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c8966-104">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c8966-104">JSON representation</span></span>

<span data-ttu-id="c8966-105">下面是 **textColumn** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c8966-105">Here is a JSON representation of a **textColumn** resource.</span></span>
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

## <a name="properties"></a><span data-ttu-id="c8966-106">属性</span><span class="sxs-lookup"><span data-stu-id="c8966-106">Properties</span></span>

| <span data-ttu-id="c8966-107">属性名称</span><span class="sxs-lookup"><span data-stu-id="c8966-107">Property name</span></span>                   | <span data-ttu-id="c8966-108">类型</span><span class="sxs-lookup"><span data-stu-id="c8966-108">Type</span></span>   | <span data-ttu-id="c8966-109">说明</span><span class="sxs-lookup"><span data-stu-id="c8966-109">Description</span></span>
|:--------------------------------|:-------|:-----------------------------------------------
| <span data-ttu-id="c8966-110">**allowMultipleLines**</span><span class="sxs-lookup"><span data-stu-id="c8966-110">**allowMultipleLines**</span></span>          | <span data-ttu-id="c8966-111">string</span><span class="sxs-lookup"><span data-stu-id="c8966-111">string</span></span> | <span data-ttu-id="c8966-112">是否支持多行文本。</span><span class="sxs-lookup"><span data-stu-id="c8966-112">Whether to allow multiple lines of text.</span></span>
| <span data-ttu-id="c8966-113">**appendChangesToExistingText**</span><span class="sxs-lookup"><span data-stu-id="c8966-113">**appendChangesToExistingText**</span></span> | <span data-ttu-id="c8966-114">string</span><span class="sxs-lookup"><span data-stu-id="c8966-114">string</span></span> | <span data-ttu-id="c8966-115">对此列的更新应替换现有文本，还是附加到现有文本。</span><span class="sxs-lookup"><span data-stu-id="c8966-115">Whether updates to this column should replace existing text, or append to it.</span></span>
| <span data-ttu-id="c8966-116">**linesForEditing**</span><span class="sxs-lookup"><span data-stu-id="c8966-116">**linesForEditing**</span></span>             | <span data-ttu-id="c8966-117">int</span><span class="sxs-lookup"><span data-stu-id="c8966-117">int</span></span>    | <span data-ttu-id="c8966-118">文本框的大小。</span><span class="sxs-lookup"><span data-stu-id="c8966-118">The size of the text box.</span></span>
| <span data-ttu-id="c8966-119">**maxLength**</span><span class="sxs-lookup"><span data-stu-id="c8966-119">**maxLength**</span></span>                   | <span data-ttu-id="c8966-120">int</span><span class="sxs-lookup"><span data-stu-id="c8966-120">int</span></span>    | <span data-ttu-id="c8966-121">值的最大字符数。</span><span class="sxs-lookup"><span data-stu-id="c8966-121">The maximum number of characters for the value.</span></span>
| <span data-ttu-id="c8966-122">**textType**</span><span class="sxs-lookup"><span data-stu-id="c8966-122">**textType**</span></span>                    | <span data-ttu-id="c8966-123">string</span><span class="sxs-lookup"><span data-stu-id="c8966-123">string</span></span> | <span data-ttu-id="c8966-124">要存储的文本类型。</span><span class="sxs-lookup"><span data-stu-id="c8966-124">The type of text being stored.</span></span> <span data-ttu-id="c8966-125">必须为 `plain` 或 `richText`.的其中一个</span><span class="sxs-lookup"><span data-stu-id="c8966-125">Must be one of `plain` or `richText`</span></span>

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

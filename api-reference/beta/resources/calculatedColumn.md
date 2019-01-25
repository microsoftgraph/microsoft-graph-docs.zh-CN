---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: CalculatedColumn
localization_priority: Normal
ms.openlocfilehash: b3a0d76a236cc4bce53bf476a90e8f37757ae003
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512624"
---
# <a name="calculatedcolumn-resource-type"></a><span data-ttu-id="b1542-102">CalculatedColumn 资源类型</span><span class="sxs-lookup"><span data-stu-id="b1542-102">CalculatedColumn resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b1542-103">[columnDefinition](columndefinition.md) 资源上的 **calculatedColumn** 指出列数据基于站点中的其他列计算。</span><span class="sxs-lookup"><span data-stu-id="b1542-103">The **calculatedColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's data is calculated based on other columns in the site.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b1542-104">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b1542-104">JSON representation</span></span>

<span data-ttu-id="b1542-105">下面是 **calculatedColumn** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b1542-105">Here is a JSON representation of a **calculatedColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.calculatedColumn" } -->

```json
{
  "format": "dateOnly | dateTime",
  "formula": "=[Column1]+[Column2]+[Column3]",
  "outputType": "boolean | currency | dateTime | number | text",
}
```

## <a name="properties"></a><span data-ttu-id="b1542-106">属性</span><span class="sxs-lookup"><span data-stu-id="b1542-106">Properties</span></span>

| <span data-ttu-id="b1542-107">属性名称</span><span class="sxs-lookup"><span data-stu-id="b1542-107">Property name</span></span>  | <span data-ttu-id="b1542-108">类型</span><span class="sxs-lookup"><span data-stu-id="b1542-108">Type</span></span>    | <span data-ttu-id="b1542-109">说明</span><span class="sxs-lookup"><span data-stu-id="b1542-109">Description</span></span>
|:---------------|:--------|:--------------------------------------------------
| <span data-ttu-id="b1542-110">**format**</span><span class="sxs-lookup"><span data-stu-id="b1542-110">**format**</span></span>     | <span data-ttu-id="b1542-111">string</span><span class="sxs-lookup"><span data-stu-id="b1542-111">string</span></span>  | <span data-ttu-id="b1542-112">对于`dateTime` 输出类型，值的格式。</span><span class="sxs-lookup"><span data-stu-id="b1542-112">For `dateTime` output types, the format of the value.</span></span> <span data-ttu-id="b1542-113">必须为 `dateOnly` 或 `dateTime` 的其中一个。</span><span class="sxs-lookup"><span data-stu-id="b1542-113">Must be one of `dateOnly` or `dateTime`.</span></span>
| <span data-ttu-id="b1542-114">**formula**</span><span class="sxs-lookup"><span data-stu-id="b1542-114">**formula**</span></span>    | <span data-ttu-id="b1542-115">string</span><span class="sxs-lookup"><span data-stu-id="b1542-115">string</span></span>  | <span data-ttu-id="b1542-116">用于计算此列的值的公式。</span><span class="sxs-lookup"><span data-stu-id="b1542-116">The formula used to compute the value for this column.</span></span>
| <span data-ttu-id="b1542-117">**outputType**</span><span class="sxs-lookup"><span data-stu-id="b1542-117">**outputType**</span></span> | <span data-ttu-id="b1542-118">string</span><span class="sxs-lookup"><span data-stu-id="b1542-118">string</span></span>  | <span data-ttu-id="b1542-119">用于设置此列中值的格式的输出类型。</span><span class="sxs-lookup"><span data-stu-id="b1542-119">The output type used to format values in this column.</span></span> <span data-ttu-id="b1542-120">必须为 `boolean`、`currency`、`dateTime`、`number` 或 `text`.的其中一个。</span><span class="sxs-lookup"><span data-stu-id="b1542-120">Must be one of `boolean`, `currency`, `dateTime`, `number`, or `text`.</span></span>

<span data-ttu-id="b1542-121">SharePoint 公式使用一种类似于 Excel 公式的语法。</span><span class="sxs-lookup"><span data-stu-id="b1542-121">SharePoint formulas use a syntax similar to Excel formulas.</span></span>
<span data-ttu-id="b1542-122">请参阅 [SharePoint 列表中的常用公式示例][ SPFormulas]，了解详细信息。</span><span class="sxs-lookup"><span data-stu-id="b1542-122">See [Examples of common formulas in SharePoint Lists][SPFormulas] for more information.</span></span>

[SPFormulas]: https://support.office.com/en-us/article/Examples-of-common-formulas-in-SharePoint-Lists-d81f5f21-2b4e-45ce-b170-bf7ebf6988b3

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/CalculatedColumn",
  "suppressions": [
    "Error: /api-reference/beta/resources/calculatedColumn.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

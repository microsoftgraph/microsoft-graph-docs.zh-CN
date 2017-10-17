---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: CalculatedColumn
ms.openlocfilehash: 44700ba7606243002798ec0ec84c3be30d38ef1f
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/28/2017
---
# <a name="calculatedcolumn-resource-type"></a><span data-ttu-id="906e1-102">CalculatedColumn 资源类型</span><span class="sxs-lookup"><span data-stu-id="906e1-102">CalculatedColumn resource type</span></span>

<span data-ttu-id="906e1-103">[columnDefinition](columnDefinition.md) 资源上的 **calculatedColumn** 指示基于网站中的其他列计算的列数据。</span><span class="sxs-lookup"><span data-stu-id="906e1-103">The **calculatedColumn** on a [columnDefinition](columnDefinition.md) resource indicates that the column's data is calculated based on other columns in the site.</span></span>

## <a name="json-representation"></a><span data-ttu-id="906e1-104">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="906e1-104">JSON representation</span></span>

<span data-ttu-id="906e1-105">下面是 **calculatedColumn** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="906e1-105">Here is a JSON representation of a **driveItem** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.calculatedColumn" } -->

```json
{
  "format": "dateOnly | dateTime",
  "formula": "=[Column1]+[Column2]+[Column3]",
  "outputType": "boolean | currency | dateTime | number | text",
}
```

## <a name="properties"></a><span data-ttu-id="906e1-106">属性</span><span class="sxs-lookup"><span data-stu-id="906e1-106">Properties</span></span>

| <span data-ttu-id="906e1-107">属性名称</span><span class="sxs-lookup"><span data-stu-id="906e1-107">Property name</span></span>  | <span data-ttu-id="906e1-108">类型</span><span class="sxs-lookup"><span data-stu-id="906e1-108">Type</span></span>    | <span data-ttu-id="906e1-109">说明</span><span class="sxs-lookup"><span data-stu-id="906e1-109">Description</span></span>
|:---------------|:--------|:--------------------------------------------------
| <span data-ttu-id="906e1-110">**format**</span><span class="sxs-lookup"><span data-stu-id="906e1-110">**format**</span></span>     | <span data-ttu-id="906e1-111">string</span><span class="sxs-lookup"><span data-stu-id="906e1-111">string</span></span>  | <span data-ttu-id="906e1-112">对于 `dateTime` 输出类型，是值的格式。</span><span class="sxs-lookup"><span data-stu-id="906e1-112">For `dateTime` output types, the format of the value.</span></span> <span data-ttu-id="906e1-113">必须是 `dateOnly` 或 `dateTime` 的其中一个。</span><span class="sxs-lookup"><span data-stu-id="906e1-113">Must be one of `dateOnly` or `dateTime`.</span></span>
| <span data-ttu-id="906e1-114">**formula**</span><span class="sxs-lookup"><span data-stu-id="906e1-114">**formula**</span></span>    | <span data-ttu-id="906e1-115">string</span><span class="sxs-lookup"><span data-stu-id="906e1-115">string</span></span>  | <span data-ttu-id="906e1-116">用于计算此列的值的公式。</span><span class="sxs-lookup"><span data-stu-id="906e1-116">The formula used to compute the value for this column.</span></span>
| <span data-ttu-id="906e1-117">**outputType**</span><span class="sxs-lookup"><span data-stu-id="906e1-117">**outputType**</span></span> | <span data-ttu-id="906e1-118">string</span><span class="sxs-lookup"><span data-stu-id="906e1-118">string</span></span>  | <span data-ttu-id="906e1-119">用于设置此列中值的格式的输出类型。</span><span class="sxs-lookup"><span data-stu-id="906e1-119">The output type used to format values in this column.</span></span> <span data-ttu-id="906e1-120">必须为 `boolean`、`currency`、`dateTime`、`number` 或 `text` 的其中一个。</span><span class="sxs-lookup"><span data-stu-id="906e1-120">Must be one of `boolean`, `currency`, `dateTime`, `number`, or `text`.</span></span>

<span data-ttu-id="906e1-121">SharePoint 公式使用一种类似于 Excel 公式的语法。</span><span class="sxs-lookup"><span data-stu-id="906e1-121">SharePoint formulas use a syntax similar to Excel formulas.</span></span>
<span data-ttu-id="906e1-122">请参阅 [SharePoint 列表中的常用公式示例][SPFormulas]，了解详细信息。</span><span class="sxs-lookup"><span data-stu-id="906e1-122">See [Examples of common formulas in SharePoint Lists][SPFormulas] for more information.</span></span>

[SPFormulas]: https://support.office.com/en-us/article/Examples-of-common-formulas-in-SharePoint-Lists-d81f5f21-2b4e-45ce-b170-bf7ebf6988b3

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/CalculatedColumn"
} -->

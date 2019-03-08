---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: CalculatedColumn
localization_priority: Normal
ms.openlocfilehash: 66fbc59fa9fe4880c023086c9bd334e04650bc73
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2019
ms.locfileid: "30481711"
---
# <a name="calculatedcolumn-resource-type"></a><span data-ttu-id="c370b-102">CalculatedColumn 资源类型</span><span class="sxs-lookup"><span data-stu-id="c370b-102">CalculatedColumn resource type</span></span>

<span data-ttu-id="c370b-103">[columnDefinition](columndefinition.md) 资源上的 **calculatedColumn** 指出列数据基于站点中的其他列计算。</span><span class="sxs-lookup"><span data-stu-id="c370b-103">The **calculatedColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's data is calculated based on other columns in the site.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c370b-104">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c370b-104">JSON representation</span></span>

<span data-ttu-id="c370b-105">下面是 **calculatedColumn** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c370b-105">Here is a JSON representation of a **calculatedColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.calculatedColumn" } -->

```json
{
  "format": "dateOnly | dateTime",
  "formula": "=[Column1]+[Column2]+[Column3]",
  "outputType": "boolean | currency | dateTime | number | text",
}
```

## <a name="properties"></a><span data-ttu-id="c370b-106">属性</span><span class="sxs-lookup"><span data-stu-id="c370b-106">Properties</span></span>

| <span data-ttu-id="c370b-107">属性名称</span><span class="sxs-lookup"><span data-stu-id="c370b-107">Property name</span></span>  | <span data-ttu-id="c370b-108">类型</span><span class="sxs-lookup"><span data-stu-id="c370b-108">Type</span></span>    | <span data-ttu-id="c370b-109">说明</span><span class="sxs-lookup"><span data-stu-id="c370b-109">Description</span></span>
|:---------------|:--------|:--------------------------------------------------
| <span data-ttu-id="c370b-110">**format**</span><span class="sxs-lookup"><span data-stu-id="c370b-110">**format**</span></span>     | <span data-ttu-id="c370b-111">string</span><span class="sxs-lookup"><span data-stu-id="c370b-111">string</span></span>  | <span data-ttu-id="c370b-112">对于`dateTime` 输出类型，值的格式。</span><span class="sxs-lookup"><span data-stu-id="c370b-112">For `dateTime` output types, the format of the value.</span></span> <span data-ttu-id="c370b-113">必须为 `dateOnly` 或 `dateTime` 的其中一个。</span><span class="sxs-lookup"><span data-stu-id="c370b-113">Must be one of `dateOnly` or `dateTime`.</span></span>
| <span data-ttu-id="c370b-114">**formula**</span><span class="sxs-lookup"><span data-stu-id="c370b-114">**formula**</span></span>    | <span data-ttu-id="c370b-115">string</span><span class="sxs-lookup"><span data-stu-id="c370b-115">string</span></span>  | <span data-ttu-id="c370b-116">用于计算此列的值的公式。</span><span class="sxs-lookup"><span data-stu-id="c370b-116">The formula used to compute the value for this column.</span></span>
| <span data-ttu-id="c370b-117">**outputType**</span><span class="sxs-lookup"><span data-stu-id="c370b-117">**outputType**</span></span> | <span data-ttu-id="c370b-118">string</span><span class="sxs-lookup"><span data-stu-id="c370b-118">string</span></span>  | <span data-ttu-id="c370b-119">用于设置此列中值的格式的输出类型。</span><span class="sxs-lookup"><span data-stu-id="c370b-119">The output type used to format values in this column.</span></span> <span data-ttu-id="c370b-120">必须为 `boolean`、`currency`、`dateTime`、`number` 或 `text`.的其中一个。</span><span class="sxs-lookup"><span data-stu-id="c370b-120">Must be one of `boolean`, `currency`, `dateTime`, `number`, or `text`.</span></span>

<span data-ttu-id="c370b-121">SharePoint 公式使用一种类似于 Excel 公式的语法。</span><span class="sxs-lookup"><span data-stu-id="c370b-121">SharePoint formulas use a syntax similar to Excel formulas.</span></span>
<span data-ttu-id="c370b-122">请参阅 [SharePoint 列表中的常用公式示例][ SPFormulas]，了解详细信息。</span><span class="sxs-lookup"><span data-stu-id="c370b-122">See [Examples of common formulas in SharePoint Lists][SPFormulas] for more information.</span></span>

[SPFormulas]: https://support.office.com/en-us/article/Examples-of-common-formulas-in-SharePoint-Lists-d81f5f21-2b4e-45ce-b170-bf7ebf6988b3

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/calculatedcolumn.md:
      Found potential enums in resource example that weren't defined in a table:(dateOnly,dateTime) are in resource, but () are in table",
    "Warning: /api-reference/v1.0/resources/calculatedcolumn.md:
      Found potential enums in resource example that weren't defined in a table:(boolean,currency,dateTime,number,text) are in resource, but () are in table"
  ],
  "tocPath": "Resources/CalculatedColumn"
} -->

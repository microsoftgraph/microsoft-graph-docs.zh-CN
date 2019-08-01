---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: CalculatedColumn
localization_priority: Normal
description: columnDefinition 资源上的 calculatedColumn 指出列数据基于站点中的其他列计算。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 19f11c7033f03dbf4a190acbd6df54bbdfe1fa24
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029972"
---
# <a name="calculatedcolumn-resource-type"></a><span data-ttu-id="473a2-103">CalculatedColumn 资源类型</span><span class="sxs-lookup"><span data-stu-id="473a2-103">CalculatedColumn resource type</span></span>

<span data-ttu-id="473a2-104">[columnDefinition](columndefinition.md) 资源上的 **calculatedColumn** 指出列数据基于站点中的其他列计算。</span><span class="sxs-lookup"><span data-stu-id="473a2-104">The **calculatedColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's data is calculated based on other columns in the site.</span></span>

## <a name="json-representation"></a><span data-ttu-id="473a2-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="473a2-105">JSON representation</span></span>

<span data-ttu-id="473a2-106">下面是 **calculatedColumn** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="473a2-106">Here is a JSON representation of a **calculatedColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.calculatedColumn" } -->

```json
{
  "format": "dateOnly | dateTime",
  "formula": "=[Column1]+[Column2]+[Column3]",
  "outputType": "boolean | currency | dateTime | number | text",
}
```

## <a name="properties"></a><span data-ttu-id="473a2-107">属性</span><span class="sxs-lookup"><span data-stu-id="473a2-107">Properties</span></span>

| <span data-ttu-id="473a2-108">属性名称</span><span class="sxs-lookup"><span data-stu-id="473a2-108">Property name</span></span>  | <span data-ttu-id="473a2-109">类型</span><span class="sxs-lookup"><span data-stu-id="473a2-109">Type</span></span>    | <span data-ttu-id="473a2-110">说明</span><span class="sxs-lookup"><span data-stu-id="473a2-110">Description</span></span>
|:---------------|:--------|:--------------------------------------------------
| <span data-ttu-id="473a2-111">**format**</span><span class="sxs-lookup"><span data-stu-id="473a2-111">**format**</span></span>     | <span data-ttu-id="473a2-112">string</span><span class="sxs-lookup"><span data-stu-id="473a2-112">string</span></span>  | <span data-ttu-id="473a2-113">对于`dateTime` 输出类型，值的格式。</span><span class="sxs-lookup"><span data-stu-id="473a2-113">For `dateTime` output types, the format of the value.</span></span> <span data-ttu-id="473a2-114">必须为 `dateOnly` 或 `dateTime` 的其中一个。</span><span class="sxs-lookup"><span data-stu-id="473a2-114">Must be one of `dateOnly` or `dateTime`.</span></span>
| <span data-ttu-id="473a2-115">**formula**</span><span class="sxs-lookup"><span data-stu-id="473a2-115">**formula**</span></span>    | <span data-ttu-id="473a2-116">string</span><span class="sxs-lookup"><span data-stu-id="473a2-116">string</span></span>  | <span data-ttu-id="473a2-117">用于计算此列的值的公式。</span><span class="sxs-lookup"><span data-stu-id="473a2-117">The formula used to compute the value for this column.</span></span>
| <span data-ttu-id="473a2-118">**outputType**</span><span class="sxs-lookup"><span data-stu-id="473a2-118">**outputType**</span></span> | <span data-ttu-id="473a2-119">string</span><span class="sxs-lookup"><span data-stu-id="473a2-119">string</span></span>  | <span data-ttu-id="473a2-120">用于设置此列中值的格式的输出类型。</span><span class="sxs-lookup"><span data-stu-id="473a2-120">The output type used to format values in this column.</span></span> <span data-ttu-id="473a2-121">必须为 `boolean`、`currency`、`dateTime`、`number` 或 `text`.的其中一个。</span><span class="sxs-lookup"><span data-stu-id="473a2-121">Must be one of `boolean`, `currency`, `dateTime`, `number`, or `text`.</span></span>

<span data-ttu-id="473a2-122">SharePoint 公式使用一种类似于 Excel 公式的语法。</span><span class="sxs-lookup"><span data-stu-id="473a2-122">SharePoint formulas use a syntax similar to Excel formulas.</span></span>
<span data-ttu-id="473a2-123">有关详细信息, 请参阅[SharePoint 列表中常见公式的示例][SPFormulas]。</span><span class="sxs-lookup"><span data-stu-id="473a2-123">See [Examples of common formulas in SharePoint Lists][SPFormulas] for more information.</span></span>

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

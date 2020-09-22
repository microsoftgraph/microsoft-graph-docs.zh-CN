---
author: JeremyKelley
description: columnDefinition 资源上的 calculatedColumn 指出列数据基于站点中的其他列计算。
ms.date: 09/11/2017
title: CalculatedColumn
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: cc46a6987e6fbd2e1f1c77f026118b93b5974fe8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48071628"
---
# <a name="calculatedcolumn-resource-type"></a><span data-ttu-id="a8d5b-103">CalculatedColumn 资源类型</span><span class="sxs-lookup"><span data-stu-id="a8d5b-103">CalculatedColumn resource type</span></span>

<span data-ttu-id="a8d5b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a8d5b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a8d5b-105">[columnDefinition](columndefinition.md) 资源上的 **calculatedColumn** 指出列数据基于站点中的其他列计算。</span><span class="sxs-lookup"><span data-stu-id="a8d5b-105">The **calculatedColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's data is calculated based on other columns in the site.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a8d5b-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a8d5b-106">JSON representation</span></span>

<span data-ttu-id="a8d5b-107">下面是 **calculatedColumn** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a8d5b-107">Here is a JSON representation of a **calculatedColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.calculatedColumn" } -->

```json
{
  "format": "dateOnly | dateTime",
  "formula": "=[Column1]+[Column2]+[Column3]",
  "outputType": "boolean | currency | dateTime | number | text",
}
```

## <a name="properties"></a><span data-ttu-id="a8d5b-108">属性</span><span class="sxs-lookup"><span data-stu-id="a8d5b-108">Properties</span></span>

| <span data-ttu-id="a8d5b-109">属性名称</span><span class="sxs-lookup"><span data-stu-id="a8d5b-109">Property name</span></span>  | <span data-ttu-id="a8d5b-110">类型</span><span class="sxs-lookup"><span data-stu-id="a8d5b-110">Type</span></span>    | <span data-ttu-id="a8d5b-111">说明</span><span class="sxs-lookup"><span data-stu-id="a8d5b-111">Description</span></span>
|:---------------|:--------|:--------------------------------------------------
| <span data-ttu-id="a8d5b-112">**format**</span><span class="sxs-lookup"><span data-stu-id="a8d5b-112">**format**</span></span>     | <span data-ttu-id="a8d5b-113">string</span><span class="sxs-lookup"><span data-stu-id="a8d5b-113">string</span></span>  | <span data-ttu-id="a8d5b-114">对于`dateTime` 输出类型，值的格式。</span><span class="sxs-lookup"><span data-stu-id="a8d5b-114">For `dateTime` output types, the format of the value.</span></span> <span data-ttu-id="a8d5b-115">必须为 `dateOnly` 或 `dateTime` 的其中一个。</span><span class="sxs-lookup"><span data-stu-id="a8d5b-115">Must be one of `dateOnly` or `dateTime`.</span></span>
| <span data-ttu-id="a8d5b-116">**formula**</span><span class="sxs-lookup"><span data-stu-id="a8d5b-116">**formula**</span></span>    | <span data-ttu-id="a8d5b-117">string</span><span class="sxs-lookup"><span data-stu-id="a8d5b-117">string</span></span>  | <span data-ttu-id="a8d5b-118">用于计算此列的值的公式。</span><span class="sxs-lookup"><span data-stu-id="a8d5b-118">The formula used to compute the value for this column.</span></span>
| <span data-ttu-id="a8d5b-119">**outputType**</span><span class="sxs-lookup"><span data-stu-id="a8d5b-119">**outputType**</span></span> | <span data-ttu-id="a8d5b-120">string</span><span class="sxs-lookup"><span data-stu-id="a8d5b-120">string</span></span>  | <span data-ttu-id="a8d5b-121">用于设置此列中值的格式的输出类型。</span><span class="sxs-lookup"><span data-stu-id="a8d5b-121">The output type used to format values in this column.</span></span> <span data-ttu-id="a8d5b-122">必须为 `boolean`、`currency`、`dateTime`、`number` 或 `text`.的其中一个。</span><span class="sxs-lookup"><span data-stu-id="a8d5b-122">Must be one of `boolean`, `currency`, `dateTime`, `number`, or `text`.</span></span>

<span data-ttu-id="a8d5b-123">SharePoint 公式使用一种类似于 Excel 公式的语法。</span><span class="sxs-lookup"><span data-stu-id="a8d5b-123">SharePoint formulas use a syntax similar to Excel formulas.</span></span>
<span data-ttu-id="a8d5b-124">有关详细信息，请参阅 [SharePoint 列表中常见公式的示例][SPFormulas] 。</span><span class="sxs-lookup"><span data-stu-id="a8d5b-124">See [Examples of common formulas in SharePoint Lists][SPFormulas] for more information.</span></span>

[SPFormulas]: https://support.office.com/en-us/article/Examples-of-common-formulas-in-SharePoint-Lists-d81f5f21-2b4e-45ce-b170-bf7ebf6988b3

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/CalculatedColumn",
  "suppressions": []
}
-->



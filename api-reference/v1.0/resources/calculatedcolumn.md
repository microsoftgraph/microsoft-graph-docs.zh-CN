---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: CalculatedColumn
localization_priority: Normal
description: columnDefinition 资源上的 calculatedColumn 指出列数据基于站点中的其他列计算。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 77db50430d2d28eb8d23a7e45018b84734dcb77b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532002"
---
# <a name="calculatedcolumn-resource-type"></a><span data-ttu-id="0595d-103">CalculatedColumn 资源类型</span><span class="sxs-lookup"><span data-stu-id="0595d-103">CalculatedColumn resource type</span></span>

<span data-ttu-id="0595d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0595d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0595d-105">[columnDefinition](columndefinition.md) 资源上的 **calculatedColumn** 指出列数据基于站点中的其他列计算。</span><span class="sxs-lookup"><span data-stu-id="0595d-105">The **calculatedColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's data is calculated based on other columns in the site.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0595d-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0595d-106">JSON representation</span></span>

<span data-ttu-id="0595d-107">下面是 **calculatedColumn** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0595d-107">Here is a JSON representation of a **calculatedColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.calculatedColumn" } -->

```json
{
  "format": "dateOnly | dateTime",
  "formula": "=[Column1]+[Column2]+[Column3]",
  "outputType": "boolean | currency | dateTime | number | text",
}
```

## <a name="properties"></a><span data-ttu-id="0595d-108">属性</span><span class="sxs-lookup"><span data-stu-id="0595d-108">Properties</span></span>

| <span data-ttu-id="0595d-109">属性名称</span><span class="sxs-lookup"><span data-stu-id="0595d-109">Property name</span></span>  | <span data-ttu-id="0595d-110">类型</span><span class="sxs-lookup"><span data-stu-id="0595d-110">Type</span></span>    | <span data-ttu-id="0595d-111">说明</span><span class="sxs-lookup"><span data-stu-id="0595d-111">Description</span></span>
|:---------------|:--------|:--------------------------------------------------
| <span data-ttu-id="0595d-112">**format**</span><span class="sxs-lookup"><span data-stu-id="0595d-112">**format**</span></span>     | <span data-ttu-id="0595d-113">string</span><span class="sxs-lookup"><span data-stu-id="0595d-113">string</span></span>  | <span data-ttu-id="0595d-114">对于`dateTime` 输出类型，值的格式。</span><span class="sxs-lookup"><span data-stu-id="0595d-114">For `dateTime` output types, the format of the value.</span></span> <span data-ttu-id="0595d-115">必须为 `dateOnly` 或 `dateTime` 的其中一个。</span><span class="sxs-lookup"><span data-stu-id="0595d-115">Must be one of `dateOnly` or `dateTime`.</span></span>
| <span data-ttu-id="0595d-116">**formula**</span><span class="sxs-lookup"><span data-stu-id="0595d-116">**formula**</span></span>    | <span data-ttu-id="0595d-117">字符串</span><span class="sxs-lookup"><span data-stu-id="0595d-117">string</span></span>  | <span data-ttu-id="0595d-118">用于计算此列的值的公式。</span><span class="sxs-lookup"><span data-stu-id="0595d-118">The formula used to compute the value for this column.</span></span>
| <span data-ttu-id="0595d-119">**outputType**</span><span class="sxs-lookup"><span data-stu-id="0595d-119">**outputType**</span></span> | <span data-ttu-id="0595d-120">string</span><span class="sxs-lookup"><span data-stu-id="0595d-120">string</span></span>  | <span data-ttu-id="0595d-121">用于设置此列中值的格式的输出类型。</span><span class="sxs-lookup"><span data-stu-id="0595d-121">The output type used to format values in this column.</span></span> <span data-ttu-id="0595d-122">必须为 `boolean`、`currency`、`dateTime`、`number` 或 `text`.的其中一个。</span><span class="sxs-lookup"><span data-stu-id="0595d-122">Must be one of `boolean`, `currency`, `dateTime`, `number`, or `text`.</span></span>

<span data-ttu-id="0595d-123">SharePoint 公式使用一种类似于 Excel 公式的语法。</span><span class="sxs-lookup"><span data-stu-id="0595d-123">SharePoint formulas use a syntax similar to Excel formulas.</span></span>
<span data-ttu-id="0595d-124">有关详细信息，请参阅[SharePoint 列表中常见公式的示例][SPFormulas]。</span><span class="sxs-lookup"><span data-stu-id="0595d-124">See [Examples of common formulas in SharePoint Lists][SPFormulas] for more information.</span></span>

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

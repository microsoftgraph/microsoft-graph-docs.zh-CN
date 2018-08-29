---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: CalculatedColumn
ms.openlocfilehash: 7e26b3683c2c84d1c413f3214da39e0a3d016f40
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/21/2018
ms.locfileid: "23267841"
---
# <a name="calculatedcolumn-resource-type"></a><span data-ttu-id="50523-102">CalculatedColumn 资源类型</span><span class="sxs-lookup"><span data-stu-id="50523-102">CalculatedColumn resource type</span></span>

<span data-ttu-id="50523-103">[columnDefinition](columnDefinition.md) 资源上的 **calculatedColumn** 指出列数据基于站点中的其他列计算。</span><span class="sxs-lookup"><span data-stu-id="50523-103">The **calculatedColumn** on a [columnDefinition](columnDefinition.md) resource indicates that the column's data is calculated based on other columns in the site.</span></span>

## <a name="json-representation"></a><span data-ttu-id="50523-104">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="50523-104">JSON representation</span></span>

<span data-ttu-id="50523-105">下面是 **calculatedColumn** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="50523-105">Here is a JSON representation of a **calculatedColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.calculatedColumn" } -->

```json
{
  "format": "dateOnly | dateTime",
  "formula": "=[Column1]+[Column2]+[Column3]",
  "outputType": "boolean | currency | dateTime | number | text",
}
```

## <a name="properties"></a><span data-ttu-id="50523-106">属性</span><span class="sxs-lookup"><span data-stu-id="50523-106">Properties</span></span>

| <span data-ttu-id="50523-107">属性名称</span><span class="sxs-lookup"><span data-stu-id="50523-107">Property name</span></span>  | <span data-ttu-id="50523-108">类型</span><span class="sxs-lookup"><span data-stu-id="50523-108">Type</span></span>    | <span data-ttu-id="50523-109">说明</span><span class="sxs-lookup"><span data-stu-id="50523-109">Description</span></span>
|:---------------|:--------|:--------------------------------------------------
| <span data-ttu-id="50523-110">**format**</span><span class="sxs-lookup"><span data-stu-id="50523-110">**format**</span></span>     | <span data-ttu-id="50523-111">string</span><span class="sxs-lookup"><span data-stu-id="50523-111">string</span></span>  | <span data-ttu-id="50523-112">对于`dateTime` 输出类型，值的格式。</span><span class="sxs-lookup"><span data-stu-id="50523-112">For `dateTime` output types, the format of the value.</span></span> <span data-ttu-id="50523-113">必须为 `dateOnly` 或 `dateTime` 的其中一个。</span><span class="sxs-lookup"><span data-stu-id="50523-113">Must be one of `dateOnly` or `dateTime`.</span></span>
| <span data-ttu-id="50523-114">**formula**</span><span class="sxs-lookup"><span data-stu-id="50523-114">**formula**</span></span>    | <span data-ttu-id="50523-115">string</span><span class="sxs-lookup"><span data-stu-id="50523-115">string</span></span>  | <span data-ttu-id="50523-116">用于计算此列的值的公式。</span><span class="sxs-lookup"><span data-stu-id="50523-116">The formula used to compute the value for this column.</span></span>
| <span data-ttu-id="50523-117">**outputType**</span><span class="sxs-lookup"><span data-stu-id="50523-117">**outputType**</span></span> | <span data-ttu-id="50523-118">string</span><span class="sxs-lookup"><span data-stu-id="50523-118">string</span></span>  | <span data-ttu-id="50523-119">用于设置此列中值的格式的输出类型。</span><span class="sxs-lookup"><span data-stu-id="50523-119">The output type used to format values in this column.</span></span> <span data-ttu-id="50523-120">必须为 `boolean`、`currency`、`dateTime`、`number` 或 `text`.的其中一个。</span><span class="sxs-lookup"><span data-stu-id="50523-120">Must be one of `boolean`, `currency`, `dateTime`, `number`, or `text`.</span></span>

<span data-ttu-id="50523-121">SharePoint 公式使用一种类似于 Excel 公式的语法。</span><span class="sxs-lookup"><span data-stu-id="50523-121">SharePoint formulas use a syntax similar to Excel formulas.</span></span>
<span data-ttu-id="50523-122">请参阅 [SharePoint 列表中的常用公式示例][ SPFormulas]，了解详细信息。</span><span class="sxs-lookup"><span data-stu-id="50523-122">See [Examples of common formulas in SharePoint Lists][SPFormulas] for more information.</span></span>

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

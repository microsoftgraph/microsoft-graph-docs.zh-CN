---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: CalculatedColumn
ms.openlocfilehash: a5850961e680459af27f3e76965f0d3e1c97e923
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27047916"
---
# <a name="calculatedcolumn-resource-type"></a><span data-ttu-id="123b4-102">CalculatedColumn 资源类型</span><span class="sxs-lookup"><span data-stu-id="123b4-102">CalculatedColumn resource type</span></span>

> <span data-ttu-id="123b4-103">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="123b4-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="123b4-104">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="123b4-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="123b4-105">[columnDefinition](columndefinition.md) 资源上的 **calculatedColumn** 指出列数据基于站点中的其他列计算。</span><span class="sxs-lookup"><span data-stu-id="123b4-105">The **calculatedColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's data is calculated based on other columns in the site.</span></span>

## <a name="json-representation"></a><span data-ttu-id="123b4-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="123b4-106">JSON representation</span></span>

<span data-ttu-id="123b4-107">下面是 **calculatedColumn** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="123b4-107">Here is a JSON representation of a **calculatedColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.calculatedColumn" } -->

```json
{
  "format": "dateOnly | dateTime",
  "formula": "=[Column1]+[Column2]+[Column3]",
  "outputType": "boolean | currency | dateTime | number | text",
}
```

## <a name="properties"></a><span data-ttu-id="123b4-108">属性</span><span class="sxs-lookup"><span data-stu-id="123b4-108">Properties</span></span>

| <span data-ttu-id="123b4-109">属性名称</span><span class="sxs-lookup"><span data-stu-id="123b4-109">Property name</span></span>  | <span data-ttu-id="123b4-110">类型</span><span class="sxs-lookup"><span data-stu-id="123b4-110">Type</span></span>    | <span data-ttu-id="123b4-111">说明</span><span class="sxs-lookup"><span data-stu-id="123b4-111">Description</span></span>
|:---------------|:--------|:--------------------------------------------------
| <span data-ttu-id="123b4-112">**format**</span><span class="sxs-lookup"><span data-stu-id="123b4-112">**format**</span></span>     | <span data-ttu-id="123b4-113">string</span><span class="sxs-lookup"><span data-stu-id="123b4-113">string</span></span>  | <span data-ttu-id="123b4-114">对于`dateTime` 输出类型，值的格式。</span><span class="sxs-lookup"><span data-stu-id="123b4-114">For `dateTime` output types, the format of the value.</span></span> <span data-ttu-id="123b4-115">必须为 `dateOnly` 或 `dateTime` 的其中一个。</span><span class="sxs-lookup"><span data-stu-id="123b4-115">Must be one of `dateOnly` or `dateTime`.</span></span>
| <span data-ttu-id="123b4-116">**formula**</span><span class="sxs-lookup"><span data-stu-id="123b4-116">**formula**</span></span>    | <span data-ttu-id="123b4-117">string</span><span class="sxs-lookup"><span data-stu-id="123b4-117">string</span></span>  | <span data-ttu-id="123b4-118">用于计算此列的值的公式。</span><span class="sxs-lookup"><span data-stu-id="123b4-118">The formula used to compute the value for this column.</span></span>
| <span data-ttu-id="123b4-119">**outputType**</span><span class="sxs-lookup"><span data-stu-id="123b4-119">**outputType**</span></span> | <span data-ttu-id="123b4-120">string</span><span class="sxs-lookup"><span data-stu-id="123b4-120">string</span></span>  | <span data-ttu-id="123b4-121">用于设置此列中值的格式的输出类型。</span><span class="sxs-lookup"><span data-stu-id="123b4-121">The output type used to format values in this column.</span></span> <span data-ttu-id="123b4-122">必须为 `boolean`、`currency`、`dateTime`、`number` 或 `text`.的其中一个。</span><span class="sxs-lookup"><span data-stu-id="123b4-122">Must be one of `boolean`, `currency`, `dateTime`, `number`, or `text`.</span></span>

<span data-ttu-id="123b4-123">SharePoint 公式使用一种类似于 Excel 公式的语法。</span><span class="sxs-lookup"><span data-stu-id="123b4-123">SharePoint formulas use a syntax similar to Excel formulas.</span></span>
<span data-ttu-id="123b4-124">请参阅 [SharePoint 列表中的常用公式示例][ SPFormulas]，了解详细信息。</span><span class="sxs-lookup"><span data-stu-id="123b4-124">See [Examples of common formulas in SharePoint Lists][SPFormulas] for more information.</span></span>

[SPFormulas]: https://support.office.com/en-us/article/Examples-of-common-formulas-in-SharePoint-Lists-d81f5f21-2b4e-45ce-b170-bf7ebf6988b3

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/CalculatedColumn"
} -->

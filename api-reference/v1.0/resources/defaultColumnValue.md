---
author: daspek
ms.date: 09/12/2017
title: DefaultColumnValue
localization_priority: Normal
description: columnDefinition 资源上的 defaultColumnValue 指定此列的默认值。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 881927bdbd53936d7780fa7517b2d2428c524e78
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/14/2021
ms.locfileid: "50239637"
---
# <a name="defaultcolumnvalue-resource-type"></a><span data-ttu-id="1f2cf-103">DefaultColumnValue 资源类型</span><span class="sxs-lookup"><span data-stu-id="1f2cf-103">DefaultColumnValue resource type</span></span>

<span data-ttu-id="1f2cf-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1f2cf-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1f2cf-105">[columnDefinition](columndefinition.md) 资源上的 **defaultColumnValue** 指定此列的默认值。</span><span class="sxs-lookup"><span data-stu-id="1f2cf-105">The **defaultColumnValue** on a [columnDefinition](columndefinition.md) resource specifies the default value for this column.</span></span>
<span data-ttu-id="1f2cf-106">默认值可以直接指定或以公式形式指定。</span><span class="sxs-lookup"><span data-stu-id="1f2cf-106">The default value can either be specified directly or as a formula.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1f2cf-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1f2cf-107">JSON representation</span></span>

<span data-ttu-id="1f2cf-108">下面是 **defaultColumnValue** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1f2cf-108">Here is a JSON representation of a **defaultColumnValue** resource.</span></span>
<!-- { "blockType": "resource", "@type": "microsoft.graph.defaultColumnValue" } -->

```json
{
  "formula": "=[Column1]+[Column2]+[Column3]",
  "value": "defaultValueString"
}
```

## <a name="properties"></a><span data-ttu-id="1f2cf-109">属性</span><span class="sxs-lookup"><span data-stu-id="1f2cf-109">Properties</span></span>

| <span data-ttu-id="1f2cf-110">属性名称</span><span class="sxs-lookup"><span data-stu-id="1f2cf-110">Property name</span></span> | <span data-ttu-id="1f2cf-111">类型</span><span class="sxs-lookup"><span data-stu-id="1f2cf-111">Type</span></span>   | <span data-ttu-id="1f2cf-112">说明</span><span class="sxs-lookup"><span data-stu-id="1f2cf-112">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="1f2cf-113">**formula**</span><span class="sxs-lookup"><span data-stu-id="1f2cf-113">**formula**</span></span>   | <span data-ttu-id="1f2cf-114">string</span><span class="sxs-lookup"><span data-stu-id="1f2cf-114">string</span></span> | <span data-ttu-id="1f2cf-115">用于计算此列的默认值的公式。</span><span class="sxs-lookup"><span data-stu-id="1f2cf-115">The formula used to compute the default value for this column.</span></span>
| <span data-ttu-id="1f2cf-116">**value**</span><span class="sxs-lookup"><span data-stu-id="1f2cf-116">**value**</span></span>     | <span data-ttu-id="1f2cf-117">string</span><span class="sxs-lookup"><span data-stu-id="1f2cf-117">string</span></span> | <span data-ttu-id="1f2cf-118">用作此列的默认值的直接值。</span><span class="sxs-lookup"><span data-stu-id="1f2cf-118">The direct value to use as the default value for this column.</span></span>

<span data-ttu-id="1f2cf-119">一次只能指定 **formula** 或 **value** 两者之一。</span><span class="sxs-lookup"><span data-stu-id="1f2cf-119">Only one of **formula** or **value** may be specified at a time.</span></span>

<span data-ttu-id="1f2cf-120">SharePoint 公式使用一种类似于 Excel 公式的语法。</span><span class="sxs-lookup"><span data-stu-id="1f2cf-120">SharePoint formulas use a syntax similar to Excel formulas.</span></span>
<span data-ttu-id="1f2cf-121">有关详细信息 [，请参阅 SharePoint 列表中][SPFormulas] 常见公式的示例。</span><span class="sxs-lookup"><span data-stu-id="1f2cf-121">See [Examples of common formulas in SharePoint Lists][SPFormulas] for more information.</span></span>

[SPFormulas]: https://support.office.com/en-us/article/Examples-of-common-formulas-in-SharePoint-Lists-d81f5f21-2b4e-45ce-b170-bf7ebf6988b3


<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/DefaultColumnValue"
} -->


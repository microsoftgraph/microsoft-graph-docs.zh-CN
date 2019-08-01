---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: DefaultColumnValue
localization_priority: Normal
description: columnDefinition 资源上的 defaultColumnValue 指定此列的默认值。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 4a2ddff8de7efb2bb697ffae63d69376588e6ac9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029510"
---
# <a name="defaultcolumnvalue-resource-type"></a><span data-ttu-id="e004c-103">DefaultColumnValue 资源类型</span><span class="sxs-lookup"><span data-stu-id="e004c-103">DefaultColumnValue resource type</span></span>

<span data-ttu-id="e004c-104">[columnDefinition](columndefinition.md) 资源上的 **defaultColumnValue** 指定此列的默认值。</span><span class="sxs-lookup"><span data-stu-id="e004c-104">The **defaultColumnValue** on a [columnDefinition](columndefinition.md) resource specifies the default value for this column.</span></span>
<span data-ttu-id="e004c-105">默认值可以直接指定或以公式形式指定。</span><span class="sxs-lookup"><span data-stu-id="e004c-105">The default value can either be specified directly or as a formula.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e004c-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e004c-106">JSON representation</span></span>

<span data-ttu-id="e004c-107">下面是 **defaultColumnValue** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e004c-107">Here is a JSON representation of a **defaultColumnValue** resource.</span></span>
<!-- { "blockType": "resource", "@type": "microsoft.graph.defaultColumnValue" } -->

```json
{
  "formula": "=[Column1]+[Column2]+[Column3]",
  "value": "defaultValueString"
}
```

## <a name="properties"></a><span data-ttu-id="e004c-108">属性</span><span class="sxs-lookup"><span data-stu-id="e004c-108">Properties</span></span>

| <span data-ttu-id="e004c-109">属性名称</span><span class="sxs-lookup"><span data-stu-id="e004c-109">Property name</span></span> | <span data-ttu-id="e004c-110">类型</span><span class="sxs-lookup"><span data-stu-id="e004c-110">Type</span></span>   | <span data-ttu-id="e004c-111">说明</span><span class="sxs-lookup"><span data-stu-id="e004c-111">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="e004c-112">**formula**</span><span class="sxs-lookup"><span data-stu-id="e004c-112">**formula**</span></span>   | <span data-ttu-id="e004c-113">string</span><span class="sxs-lookup"><span data-stu-id="e004c-113">string</span></span> | <span data-ttu-id="e004c-114">用于计算此列的默认值的公式。</span><span class="sxs-lookup"><span data-stu-id="e004c-114">The formula used to compute the default value for this column.</span></span>
| <span data-ttu-id="e004c-115">**value**</span><span class="sxs-lookup"><span data-stu-id="e004c-115">**value**</span></span>     | <span data-ttu-id="e004c-116">string</span><span class="sxs-lookup"><span data-stu-id="e004c-116">string</span></span> | <span data-ttu-id="e004c-117">用作此列的默认值的直接值。</span><span class="sxs-lookup"><span data-stu-id="e004c-117">The direct value to use as the default value for this column.</span></span>

<span data-ttu-id="e004c-118">一次只能指定 **formula** 或 **value** 两者之一。</span><span class="sxs-lookup"><span data-stu-id="e004c-118">Only one of **formula** or **value** may be specified at a time.</span></span>

<span data-ttu-id="e004c-119">SharePoint 公式使用一种类似于 Excel 公式的语法。</span><span class="sxs-lookup"><span data-stu-id="e004c-119">SharePoint formulas use a syntax similar to Excel formulas.</span></span>
<span data-ttu-id="e004c-120">有关详细信息, 请参阅[SharePoint 列表中常见公式的示例][SPFormulas]。</span><span class="sxs-lookup"><span data-stu-id="e004c-120">See [Examples of common formulas in SharePoint Lists][SPFormulas] for more information.</span></span>

[SPFormulas]: https://support.office.com/en-us/article/Examples-of-common-formulas-in-SharePoint-Lists-d81f5f21-2b4e-45ce-b170-bf7ebf6988b3


<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/DefaultColumnValue"
} -->

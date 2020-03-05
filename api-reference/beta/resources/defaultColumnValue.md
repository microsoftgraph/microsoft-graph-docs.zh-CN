---
author: daspek
description: columnDefinition 资源上的 defaultColumnValue 指定此列的默认值。
ms.date: 09/12/2017
title: DefaultColumnValue
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 57c66b627a61c59f78166bd8d6a14aef41cdd36d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507280"
---
# <a name="defaultcolumnvalue-resource-type"></a><span data-ttu-id="a36d2-103">DefaultColumnValue 资源类型</span><span class="sxs-lookup"><span data-stu-id="a36d2-103">DefaultColumnValue resource type</span></span>

<span data-ttu-id="a36d2-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="a36d2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a36d2-105">[columnDefinition](columndefinition.md) 资源上的 **defaultColumnValue** 指定此列的默认值。</span><span class="sxs-lookup"><span data-stu-id="a36d2-105">The **defaultColumnValue** on a [columnDefinition](columndefinition.md) resource specifies the default value for this column.</span></span>
<span data-ttu-id="a36d2-106">默认值可以直接指定或以公式形式指定。</span><span class="sxs-lookup"><span data-stu-id="a36d2-106">The default value can either be specified directly or as a formula.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a36d2-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a36d2-107">JSON representation</span></span>

<span data-ttu-id="a36d2-108">下面是 **defaultColumnValue** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a36d2-108">Here is a JSON representation of a **defaultColumnValue** resource.</span></span>
<!-- { "blockType": "resource", "@type": "microsoft.graph.defaultColumnValue" } -->

```json
{
  "formula": "=[Column1]+[Column2]+[Column3]",
  "value": "defaultValueString"
}
```

## <a name="properties"></a><span data-ttu-id="a36d2-109">属性</span><span class="sxs-lookup"><span data-stu-id="a36d2-109">Properties</span></span>

| <span data-ttu-id="a36d2-110">属性名称</span><span class="sxs-lookup"><span data-stu-id="a36d2-110">Property name</span></span> | <span data-ttu-id="a36d2-111">类型</span><span class="sxs-lookup"><span data-stu-id="a36d2-111">Type</span></span>   | <span data-ttu-id="a36d2-112">说明</span><span class="sxs-lookup"><span data-stu-id="a36d2-112">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="a36d2-113">**formula**</span><span class="sxs-lookup"><span data-stu-id="a36d2-113">**formula**</span></span>   | <span data-ttu-id="a36d2-114">string</span><span class="sxs-lookup"><span data-stu-id="a36d2-114">string</span></span> | <span data-ttu-id="a36d2-115">用于计算此列的默认值的公式。</span><span class="sxs-lookup"><span data-stu-id="a36d2-115">The formula used to compute the default value for this column.</span></span>
| <span data-ttu-id="a36d2-116">**value**</span><span class="sxs-lookup"><span data-stu-id="a36d2-116">**value**</span></span>     | <span data-ttu-id="a36d2-117">string</span><span class="sxs-lookup"><span data-stu-id="a36d2-117">string</span></span> | <span data-ttu-id="a36d2-118">用作此列的默认值的直接值。</span><span class="sxs-lookup"><span data-stu-id="a36d2-118">The direct value to use as the default value for this column.</span></span>

<span data-ttu-id="a36d2-119">一次只能指定 **formula** 或 **value** 两者之一。</span><span class="sxs-lookup"><span data-stu-id="a36d2-119">Only one of **formula** or **value** may be specified at a time.</span></span>

<span data-ttu-id="a36d2-120">SharePoint 公式使用一种类似于 Excel 公式的语法。</span><span class="sxs-lookup"><span data-stu-id="a36d2-120">SharePoint formulas use a syntax similar to Excel formulas.</span></span>
<span data-ttu-id="a36d2-121">有关详细信息，请参阅[SharePoint 列表中常见公式的示例][SPFormulas]。</span><span class="sxs-lookup"><span data-stu-id="a36d2-121">See [Examples of common formulas in SharePoint Lists][SPFormulas] for more information.</span></span>

[SPFormulas]: https://support.office.com/en-us/article/Examples-of-common-formulas-in-SharePoint-Lists-d81f5f21-2b4e-45ce-b170-bf7ebf6988b3


<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/DefaultColumnValue",
  "suppressions": []
}
-->

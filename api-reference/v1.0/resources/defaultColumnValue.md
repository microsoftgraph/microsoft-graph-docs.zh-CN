---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: DefaultColumnValue
localization_priority: Normal
ms.openlocfilehash: 400fc25bf38f12db2be8cef21ddc351316d1265b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32574601"
---
# <a name="defaultcolumnvalue-resource-type"></a><span data-ttu-id="3f626-102">DefaultColumnValue 资源类型</span><span class="sxs-lookup"><span data-stu-id="3f626-102">DefaultColumnValue resource type</span></span>

<span data-ttu-id="3f626-103">[columnDefinition](columndefinition.md) 资源上的 **defaultColumnValue** 指定此列的默认值。</span><span class="sxs-lookup"><span data-stu-id="3f626-103">The **defaultColumnValue** on a [columnDefinition](columndefinition.md) resource specifies the default value for this column.</span></span>
<span data-ttu-id="3f626-104">默认值可以直接指定或以公式形式指定。</span><span class="sxs-lookup"><span data-stu-id="3f626-104">The default value can either be specified directly or as a formula.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3f626-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3f626-105">JSON representation</span></span>

<span data-ttu-id="3f626-106">下面是 **defaultColumnValue** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3f626-106">Here is a JSON representation of a **defaultColumnValue** resource.</span></span>
<!-- { "blockType": "resource", "@type": "microsoft.graph.defaultColumnValue" } -->

```json
{
  "formula": "=[Column1]+[Column2]+[Column3]",
  "value": "defaultValueString"
}
```

## <a name="properties"></a><span data-ttu-id="3f626-107">属性</span><span class="sxs-lookup"><span data-stu-id="3f626-107">Properties</span></span>

| <span data-ttu-id="3f626-108">属性名称</span><span class="sxs-lookup"><span data-stu-id="3f626-108">Property name</span></span> | <span data-ttu-id="3f626-109">类型</span><span class="sxs-lookup"><span data-stu-id="3f626-109">Type</span></span>   | <span data-ttu-id="3f626-110">说明</span><span class="sxs-lookup"><span data-stu-id="3f626-110">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="3f626-111">**formula**</span><span class="sxs-lookup"><span data-stu-id="3f626-111">**formula**</span></span>   | <span data-ttu-id="3f626-112">string</span><span class="sxs-lookup"><span data-stu-id="3f626-112">string</span></span> | <span data-ttu-id="3f626-113">用于计算此列的默认值的公式。</span><span class="sxs-lookup"><span data-stu-id="3f626-113">The formula used to compute the default value for this column.</span></span>
| <span data-ttu-id="3f626-114">**value**</span><span class="sxs-lookup"><span data-stu-id="3f626-114">**value**</span></span>     | <span data-ttu-id="3f626-115">string</span><span class="sxs-lookup"><span data-stu-id="3f626-115">string</span></span> | <span data-ttu-id="3f626-116">用作此列的默认值的直接值。</span><span class="sxs-lookup"><span data-stu-id="3f626-116">The direct value to use as the default value for this column.</span></span>

<span data-ttu-id="3f626-117">一次只能指定 **formula** 或 **value** 两者之一。</span><span class="sxs-lookup"><span data-stu-id="3f626-117">Only one of **formula** or **value** may be specified at a time.</span></span>

<span data-ttu-id="3f626-118">SharePoint 公式使用一种类似于 Excel 公式的语法。</span><span class="sxs-lookup"><span data-stu-id="3f626-118">SharePoint formulas use a syntax similar to Excel formulas.</span></span>
<span data-ttu-id="3f626-119">请参阅 [SharePoint 列表中的常用公式示例][ SPFormulas]，了解详细信息。</span><span class="sxs-lookup"><span data-stu-id="3f626-119">See [Examples of common formulas in SharePoint Lists][SPFormulas] for more information.</span></span>

[SPFormulas]: https://support.office.com/en-us/article/Examples-of-common-formulas-in-SharePoint-Lists-d81f5f21-2b4e-45ce-b170-bf7ebf6988b3


<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/DefaultColumnValue"
} -->

---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: DefaultColumnValue
ms.openlocfilehash: 3a486b6cc90dffb75343390102ecb3b17576e6fb
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27045791"
---
# <a name="defaultcolumnvalue-resource-type"></a><span data-ttu-id="19d72-102">DefaultColumnValue 资源类型</span><span class="sxs-lookup"><span data-stu-id="19d72-102">DefaultColumnValue resource type</span></span>

> <span data-ttu-id="19d72-103">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="19d72-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="19d72-104">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="19d72-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="19d72-105">[columnDefinition](columndefinition.md) 资源上的 **defaultColumnValue** 指定此列的默认值。</span><span class="sxs-lookup"><span data-stu-id="19d72-105">The **defaultColumnValue** on a [columnDefinition](columndefinition.md) resource specifies the default value for this column.</span></span>
<span data-ttu-id="19d72-106">默认值可以直接指定或以公式形式指定。</span><span class="sxs-lookup"><span data-stu-id="19d72-106">The default value can either be specified directly or as a formula.</span></span>

## <a name="json-representation"></a><span data-ttu-id="19d72-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="19d72-107">JSON representation</span></span>

<span data-ttu-id="19d72-108">下面是 **defaultColumnValue** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="19d72-108">Here is a JSON representation of a **defaultColumnValue** resource.</span></span>
<!-- { "blockType": "resource", "@type": "microsoft.graph.defaultColumnValue" } -->

```json
{
  "formula": "=[Column1]+[Column2]+[Column3]",
  "value": "defaultValueString"
}
```

## <a name="properties"></a><span data-ttu-id="19d72-109">属性</span><span class="sxs-lookup"><span data-stu-id="19d72-109">Properties</span></span>

| <span data-ttu-id="19d72-110">属性名称</span><span class="sxs-lookup"><span data-stu-id="19d72-110">Property name</span></span> | <span data-ttu-id="19d72-111">类型</span><span class="sxs-lookup"><span data-stu-id="19d72-111">Type</span></span>   | <span data-ttu-id="19d72-112">说明</span><span class="sxs-lookup"><span data-stu-id="19d72-112">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="19d72-113">**formula**</span><span class="sxs-lookup"><span data-stu-id="19d72-113">**formula**</span></span>   | <span data-ttu-id="19d72-114">string</span><span class="sxs-lookup"><span data-stu-id="19d72-114">string</span></span> | <span data-ttu-id="19d72-115">用于计算此列的默认值的公式。</span><span class="sxs-lookup"><span data-stu-id="19d72-115">The formula used to compute the default value for this column.</span></span>
| <span data-ttu-id="19d72-116">**value**</span><span class="sxs-lookup"><span data-stu-id="19d72-116">**value**</span></span>     | <span data-ttu-id="19d72-117">string</span><span class="sxs-lookup"><span data-stu-id="19d72-117">string</span></span> | <span data-ttu-id="19d72-118">用作此列的默认值的直接值。</span><span class="sxs-lookup"><span data-stu-id="19d72-118">The direct value to use as the default value for this column.</span></span>

<span data-ttu-id="19d72-119">一次只能指定 **formula** 或 **value** 两者之一。</span><span class="sxs-lookup"><span data-stu-id="19d72-119">Only one of **formula** or **value** may be specified at a time.</span></span>

<span data-ttu-id="19d72-120">SharePoint 公式使用一种类似于 Excel 公式的语法。</span><span class="sxs-lookup"><span data-stu-id="19d72-120">SharePoint formulas use a syntax similar to Excel formulas.</span></span>
<span data-ttu-id="19d72-121">请参阅 [SharePoint 列表中的常用公式示例][ SPFormulas]，了解详细信息。</span><span class="sxs-lookup"><span data-stu-id="19d72-121">See [Examples of common formulas in SharePoint Lists][SPFormulas] for more information.</span></span>

[SPFormulas]: https://support.office.com/en-us/article/Examples-of-common-formulas-in-SharePoint-Lists-d81f5f21-2b4e-45ce-b170-bf7ebf6988b3


<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/DefaultColumnValue"
} -->

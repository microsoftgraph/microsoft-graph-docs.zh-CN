---
author: JeremyKelley
description: columnDefinition 资源上的 currencyColumn 指示该列的值代表货币。
ms.date: 09/11/2017
title: CurrencyColumn
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 4cd887d4ca7e38ff6d22189760adf12e1479acb9
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48050017"
---
# <a name="currencycolumn-resource-type"></a><span data-ttu-id="a4dc9-103">CurrencyColumn 资源类型</span><span class="sxs-lookup"><span data-stu-id="a4dc9-103">CurrencyColumn resource type</span></span>

<span data-ttu-id="a4dc9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a4dc9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a4dc9-105">[columnDefinition](columndefinition.md) 资源上的 **currencyColumn** 指示该列的值代表货币。</span><span class="sxs-lookup"><span data-stu-id="a4dc9-105">The **currencyColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values represent currency.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a4dc9-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a4dc9-106">JSON representation</span></span>

<span data-ttu-id="a4dc9-107">下面是 **currencyColumn** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a4dc9-107">Here is a JSON representation of a **currencyColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.currencyColumn" } -->

```json
{
  "locale": "en-us"
}
```

## <a name="properties"></a><span data-ttu-id="a4dc9-108">属性</span><span class="sxs-lookup"><span data-stu-id="a4dc9-108">Properties</span></span>

| <span data-ttu-id="a4dc9-109">属性名称</span><span class="sxs-lookup"><span data-stu-id="a4dc9-109">Property name</span></span> | <span data-ttu-id="a4dc9-110">类型</span><span class="sxs-lookup"><span data-stu-id="a4dc9-110">Type</span></span>   | <span data-ttu-id="a4dc9-111">说明</span><span class="sxs-lookup"><span data-stu-id="a4dc9-111">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="a4dc9-112">**locale**</span><span class="sxs-lookup"><span data-stu-id="a4dc9-112">**locale**</span></span>    | <span data-ttu-id="a4dc9-113">string</span><span class="sxs-lookup"><span data-stu-id="a4dc9-113">string</span></span> | <span data-ttu-id="a4dc9-114">指定要从中推断货币符号的区域设置。</span><span class="sxs-lookup"><span data-stu-id="a4dc9-114">Specifies the locale from which to infer the currency symbol.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/CurrencyColumn",
  "suppressions": []
}
-->



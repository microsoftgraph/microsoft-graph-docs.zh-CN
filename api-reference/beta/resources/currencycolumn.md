---
author: JeremyKelley
description: columnDefinition 资源上的 currencyColumn 指示该列的值代表货币。
ms.date: 09/11/2017
title: CurrencyColumn
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 61a3c968ff48cd3bf59ec3611bc2e50a1a92a797
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973172"
---
# <a name="currencycolumn-resource-type"></a><span data-ttu-id="ac6f0-103">CurrencyColumn 资源类型</span><span class="sxs-lookup"><span data-stu-id="ac6f0-103">CurrencyColumn resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ac6f0-104">[columnDefinition](columndefinition.md) 资源上的 **currencyColumn** 指示该列的值代表货币。</span><span class="sxs-lookup"><span data-stu-id="ac6f0-104">The **currencyColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values represent currency.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ac6f0-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ac6f0-105">JSON representation</span></span>

<span data-ttu-id="ac6f0-106">下面是 **currencyColumn** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ac6f0-106">Here is a JSON representation of a **currencyColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.currencyColumn" } -->

```json
{
  "locale": "en-us"
}
```

## <a name="properties"></a><span data-ttu-id="ac6f0-107">属性</span><span class="sxs-lookup"><span data-stu-id="ac6f0-107">Properties</span></span>

| <span data-ttu-id="ac6f0-108">属性名称</span><span class="sxs-lookup"><span data-stu-id="ac6f0-108">Property name</span></span> | <span data-ttu-id="ac6f0-109">类型</span><span class="sxs-lookup"><span data-stu-id="ac6f0-109">Type</span></span>   | <span data-ttu-id="ac6f0-110">说明</span><span class="sxs-lookup"><span data-stu-id="ac6f0-110">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="ac6f0-111">**locale**</span><span class="sxs-lookup"><span data-stu-id="ac6f0-111">**locale**</span></span>    | <span data-ttu-id="ac6f0-112">string</span><span class="sxs-lookup"><span data-stu-id="ac6f0-112">string</span></span> | <span data-ttu-id="ac6f0-113">指定要从中推断货币符号的区域设置。</span><span class="sxs-lookup"><span data-stu-id="ac6f0-113">Specifies the locale from which to infer the currency symbol.</span></span>

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

---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: CurrencyColumn
localization_priority: Normal
ms.openlocfilehash: 065ac52a4d5216a4b3e62df892c8fe0a07a82ed0
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2019
ms.locfileid: "30481529"
---
# <a name="currencycolumn-resource-type"></a><span data-ttu-id="4b875-102">CurrencyColumn 资源类型</span><span class="sxs-lookup"><span data-stu-id="4b875-102">CurrencyColumn resource type</span></span>

<span data-ttu-id="4b875-103">[columnDefinition](columndefinition.md) 资源上的 **currencyColumn** 指示该列的值代表货币。</span><span class="sxs-lookup"><span data-stu-id="4b875-103">The **currencyColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values represent currency.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4b875-104">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4b875-104">JSON representation</span></span>

<span data-ttu-id="4b875-105">下面是 **currencyColumn** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4b875-105">Here is a JSON representation of a **currencyColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.currencyColumn" } -->

```json
{
  "locale": "en-us"
}
```

## <a name="properties"></a><span data-ttu-id="4b875-106">属性</span><span class="sxs-lookup"><span data-stu-id="4b875-106">Properties</span></span>

| <span data-ttu-id="4b875-107">属性名称</span><span class="sxs-lookup"><span data-stu-id="4b875-107">Property name</span></span> | <span data-ttu-id="4b875-108">类型</span><span class="sxs-lookup"><span data-stu-id="4b875-108">Type</span></span>   | <span data-ttu-id="4b875-109">说明</span><span class="sxs-lookup"><span data-stu-id="4b875-109">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="4b875-110">**locale**</span><span class="sxs-lookup"><span data-stu-id="4b875-110">**locale**</span></span>    | <span data-ttu-id="4b875-111">string</span><span class="sxs-lookup"><span data-stu-id="4b875-111">string</span></span> | <span data-ttu-id="4b875-112">指定要从中推断货币符号的区域设置。</span><span class="sxs-lookup"><span data-stu-id="4b875-112">Specifies the locale from which to infer the currency symbol.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/CurrencyColumn"
} -->

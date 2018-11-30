---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: CurrencyColumn
ms.openlocfilehash: 4f3ae97e5abfb84ad523caf74fa70b1f1ec0322a
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/28/2017
---
# <a name="currencycolumn-resource-type"></a><span data-ttu-id="6d10d-102">CurrencyColumn 资源类型</span><span class="sxs-lookup"><span data-stu-id="6d10d-102">CurrencyColumn resource type</span></span>

<span data-ttu-id="6d10d-103">[columnDefinition](columnDefinition.md) 资源上的 **currencyColumn** 指示该列的值代表货币。</span><span class="sxs-lookup"><span data-stu-id="6d10d-103">The **currencyColumn** on a [columnDefinition](columnDefinition.md) resource indicates that the column's values represent currency.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6d10d-104">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6d10d-104">JSON representation</span></span>

<span data-ttu-id="6d10d-105">下面是 **currencyColumn** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6d10d-105">Here is a JSON representation of a **baseItem** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.currencyColumn" } -->

```json
{
  "locale": "en-us"
}
```

## <a name="properties"></a><span data-ttu-id="6d10d-106">属性</span><span class="sxs-lookup"><span data-stu-id="6d10d-106">Properties</span></span>

| <span data-ttu-id="6d10d-107">属性名称</span><span class="sxs-lookup"><span data-stu-id="6d10d-107">Property name</span></span> | <span data-ttu-id="6d10d-108">类型</span><span class="sxs-lookup"><span data-stu-id="6d10d-108">Type</span></span>   | <span data-ttu-id="6d10d-109">说明</span><span class="sxs-lookup"><span data-stu-id="6d10d-109">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="6d10d-110">**locale**</span><span class="sxs-lookup"><span data-stu-id="6d10d-110">**Locale**</span></span>    | <span data-ttu-id="6d10d-111">string</span><span class="sxs-lookup"><span data-stu-id="6d10d-111">string</span></span> | <span data-ttu-id="6d10d-112">指定要从中推断货币符号的区域设置。</span><span class="sxs-lookup"><span data-stu-id="6d10d-112">Specifies the locale from which to infer the currency symbol.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/CurrencyColumn"
} -->

---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: CurrencyColumn
ms.openlocfilehash: 796bd9fc7bf379ea38dc2d2f602411740caf4b86
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27011403"
---
# <a name="currencycolumn-resource-type"></a><span data-ttu-id="ec49a-102">CurrencyColumn 资源类型</span><span class="sxs-lookup"><span data-stu-id="ec49a-102">CurrencyColumn resource type</span></span>

<span data-ttu-id="ec49a-103">[columnDefinition](columndefinition.md) 资源上的 **currencyColumn** 指示该列的值代表货币。</span><span class="sxs-lookup"><span data-stu-id="ec49a-103">The **currencyColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values represent currency.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ec49a-104">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ec49a-104">JSON representation</span></span>

<span data-ttu-id="ec49a-105">下面是 **currencyColumn** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ec49a-105">Here is a JSON representation of a **currencyColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.currencyColumn" } -->

```json
{
  "locale": "en-us"
}
```

## <a name="properties"></a><span data-ttu-id="ec49a-106">属性</span><span class="sxs-lookup"><span data-stu-id="ec49a-106">Properties</span></span>

| <span data-ttu-id="ec49a-107">属性名称</span><span class="sxs-lookup"><span data-stu-id="ec49a-107">Property name</span></span> | <span data-ttu-id="ec49a-108">类型</span><span class="sxs-lookup"><span data-stu-id="ec49a-108">Type</span></span>   | <span data-ttu-id="ec49a-109">说明</span><span class="sxs-lookup"><span data-stu-id="ec49a-109">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="ec49a-110">**locale**</span><span class="sxs-lookup"><span data-stu-id="ec49a-110">**locale**</span></span>    | <span data-ttu-id="ec49a-111">string</span><span class="sxs-lookup"><span data-stu-id="ec49a-111">string</span></span> | <span data-ttu-id="ec49a-112">指定要从中推断货币符号的区域设置。</span><span class="sxs-lookup"><span data-stu-id="ec49a-112">Specifies the locale from which to infer the currency symbol.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/CurrencyColumn"
} -->

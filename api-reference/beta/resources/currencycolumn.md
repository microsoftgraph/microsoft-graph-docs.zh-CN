---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: CurrencyColumn
ms.openlocfilehash: 21c95026eb61eb68c98010d8ac288be115e95ec8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27049188"
---
# <a name="currencycolumn-resource-type"></a><span data-ttu-id="f3c88-102">CurrencyColumn 资源类型</span><span class="sxs-lookup"><span data-stu-id="f3c88-102">CurrencyColumn resource type</span></span>

> <span data-ttu-id="f3c88-103">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="f3c88-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f3c88-104">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="f3c88-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f3c88-105">[columnDefinition](columndefinition.md) 资源上的 **currencyColumn** 指示该列的值代表货币。</span><span class="sxs-lookup"><span data-stu-id="f3c88-105">The **currencyColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values represent currency.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f3c88-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f3c88-106">JSON representation</span></span>

<span data-ttu-id="f3c88-107">下面是 **currencyColumn** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f3c88-107">Here is a JSON representation of a **currencyColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.currencyColumn" } -->

```json
{
  "locale": "en-us"
}
```

## <a name="properties"></a><span data-ttu-id="f3c88-108">属性</span><span class="sxs-lookup"><span data-stu-id="f3c88-108">Properties</span></span>

| <span data-ttu-id="f3c88-109">属性名称</span><span class="sxs-lookup"><span data-stu-id="f3c88-109">Property name</span></span> | <span data-ttu-id="f3c88-110">类型</span><span class="sxs-lookup"><span data-stu-id="f3c88-110">Type</span></span>   | <span data-ttu-id="f3c88-111">说明</span><span class="sxs-lookup"><span data-stu-id="f3c88-111">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="f3c88-112">**locale**</span><span class="sxs-lookup"><span data-stu-id="f3c88-112">**locale**</span></span>    | <span data-ttu-id="f3c88-113">string</span><span class="sxs-lookup"><span data-stu-id="f3c88-113">string</span></span> | <span data-ttu-id="f3c88-114">指定要从中推断货币符号的区域设置。</span><span class="sxs-lookup"><span data-stu-id="f3c88-114">Specifies the locale from which to infer the currency symbol.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/CurrencyColumn"
} -->

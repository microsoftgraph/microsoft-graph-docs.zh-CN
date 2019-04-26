---
title: bookingCurrency 资源类型
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。"
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 6ab74cff24e1f575166f6672523ecc5d94bc1826
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33328225"
---
# <a name="bookingcurrency-resource-type"></a><span data-ttu-id="3b422-104">bookingCurrency 资源类型</span><span class="sxs-lookup"><span data-stu-id="3b422-104">bookingCurrency resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="3b422-105">表示[bookingBusiness](bookingbusiness.md)支持的货币货币。</span><span class="sxs-lookup"><span data-stu-id="3b422-105">Represents a monetary currency supported by a [bookingBusiness](bookingbusiness.md).</span></span>


## <a name="methods"></a><span data-ttu-id="3b422-106">方法</span><span class="sxs-lookup"><span data-stu-id="3b422-106">Methods</span></span>

| <span data-ttu-id="3b422-107">方法</span><span class="sxs-lookup"><span data-stu-id="3b422-107">Method</span></span>           | <span data-ttu-id="3b422-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="3b422-108">Return Type</span></span>    |<span data-ttu-id="3b422-109">说明</span><span class="sxs-lookup"><span data-stu-id="3b422-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="3b422-110">列出 bookingCurrencies</span><span class="sxs-lookup"><span data-stu-id="3b422-110">List bookingCurrencies</span></span>](../api/bookingcurrency-list.md) | <span data-ttu-id="3b422-111">[bookingCurrency](bookingcurrency.md)集合</span><span class="sxs-lookup"><span data-stu-id="3b422-111">[bookingCurrency](bookingcurrency.md) collection</span></span> |<span data-ttu-id="3b422-112">获取可用于 Microsoft 预订业务的**bookingCurrency**对象的列表。</span><span class="sxs-lookup"><span data-stu-id="3b422-112">Get a list of **bookingCurrency** objects available to a Microsoft Bookings business.</span></span>|
|[<span data-ttu-id="3b422-113">获取 bookingCurrency</span><span class="sxs-lookup"><span data-stu-id="3b422-113">Get bookingCurrency</span></span>](../api/bookingcurrency-get.md) | [<span data-ttu-id="3b422-114">bookingCurrency</span><span class="sxs-lookup"><span data-stu-id="3b422-114">bookingCurrency</span></span>](bookingcurrency.md) |<span data-ttu-id="3b422-115">获取**bookingCurrency**对象的属性。</span><span class="sxs-lookup"><span data-stu-id="3b422-115">Get the properties of a **bookingCurrency** object.</span></span>|


## <a name="properties"></a><span data-ttu-id="3b422-116">属性</span><span class="sxs-lookup"><span data-stu-id="3b422-116">Properties</span></span>
| <span data-ttu-id="3b422-117">属性</span><span class="sxs-lookup"><span data-stu-id="3b422-117">Property</span></span>     | <span data-ttu-id="3b422-118">类型</span><span class="sxs-lookup"><span data-stu-id="3b422-118">Type</span></span>   |<span data-ttu-id="3b422-119">说明</span><span class="sxs-lookup"><span data-stu-id="3b422-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3b422-120">id</span><span class="sxs-lookup"><span data-stu-id="3b422-120">id</span></span>|<span data-ttu-id="3b422-121">String</span><span class="sxs-lookup"><span data-stu-id="3b422-121">String</span></span>| <span data-ttu-id="3b422-122">基于[ISO 4217](https://www.iso.org/iso-4217-currency-codes.html)的3个字符的货币代码。</span><span class="sxs-lookup"><span data-stu-id="3b422-122">A 3-character currency code, based on [ISO 4217](https://www.iso.org/iso-4217-currency-codes.html).</span></span> <span data-ttu-id="3b422-123">例如, 美元的货币代码是 USD, 而澳大利亚美元是 AUD。</span><span class="sxs-lookup"><span data-stu-id="3b422-123">For example, the currency code for the US dollar is USD, and for the Australian dollar is AUD.</span></span> <span data-ttu-id="3b422-124">只读。</span><span class="sxs-lookup"><span data-stu-id="3b422-124">Read-only.</span></span>|
|<span data-ttu-id="3b422-125">符号</span><span class="sxs-lookup"><span data-stu-id="3b422-125">symbol</span></span>|<span data-ttu-id="3b422-126">String</span><span class="sxs-lookup"><span data-stu-id="3b422-126">String</span></span>| <span data-ttu-id="3b422-127">货币符号。</span><span class="sxs-lookup"><span data-stu-id="3b422-127">The currency symbol.</span></span> <span data-ttu-id="3b422-128">例如, 美元的货币符号和澳大利亚美元为美元。</span><span class="sxs-lookup"><span data-stu-id="3b422-128">For example, the currency symbol for the US dollar and for the Australian dollar is $.</span></span>  |

## <a name="relationships"></a><span data-ttu-id="3b422-129">关系</span><span class="sxs-lookup"><span data-stu-id="3b422-129">Relationships</span></span>
<span data-ttu-id="3b422-130">无</span><span class="sxs-lookup"><span data-stu-id="3b422-130">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="3b422-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3b422-131">JSON representation</span></span>

<span data-ttu-id="3b422-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3b422-132">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bookingCurrency"
}-->

```json
{
  "id": "String (identifier)",
  "symbol": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "bookingCurrency resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

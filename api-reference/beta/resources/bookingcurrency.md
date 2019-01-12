---
title: bookingCurrency 资源类型
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 7e2289bfa6c6aac62f12d7321d06caaafbc41f8c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27956001"
---
# <a name="bookingcurrency-resource-type"></a><span data-ttu-id="4610d-104">bookingCurrency 资源类型</span><span class="sxs-lookup"><span data-stu-id="4610d-104">bookingCurrency resource type</span></span>

 > <span data-ttu-id="4610d-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="4610d-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4610d-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="4610d-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="4610d-107">代表货币货币[bookingBusiness](bookingbusiness.md)支持。</span><span class="sxs-lookup"><span data-stu-id="4610d-107">Represents a monetary currency supported by a [bookingBusiness](bookingbusiness.md).</span></span>


## <a name="methods"></a><span data-ttu-id="4610d-108">方法</span><span class="sxs-lookup"><span data-stu-id="4610d-108">Methods</span></span>

| <span data-ttu-id="4610d-109">方法</span><span class="sxs-lookup"><span data-stu-id="4610d-109">Method</span></span>           | <span data-ttu-id="4610d-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="4610d-110">Return Type</span></span>    |<span data-ttu-id="4610d-111">说明</span><span class="sxs-lookup"><span data-stu-id="4610d-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4610d-112">列表 bookingCurrencies</span><span class="sxs-lookup"><span data-stu-id="4610d-112">List bookingCurrencies</span></span>](../api/bookingcurrency-list.md) | <span data-ttu-id="4610d-113">[bookingCurrency](bookingcurrency.md)集合</span><span class="sxs-lookup"><span data-stu-id="4610d-113">[bookingCurrency](bookingcurrency.md) collection</span></span> |<span data-ttu-id="4610d-114">获取供 Microsoft 预订业务**bookingCurrency**对象的列表。</span><span class="sxs-lookup"><span data-stu-id="4610d-114">Get a list of **bookingCurrency** objects available to a Microsoft Bookings business.</span></span>|
|[<span data-ttu-id="4610d-115">获取 bookingCurrency</span><span class="sxs-lookup"><span data-stu-id="4610d-115">Get bookingCurrency</span></span>](../api/bookingcurrency-get.md) | [<span data-ttu-id="4610d-116">bookingCurrency</span><span class="sxs-lookup"><span data-stu-id="4610d-116">bookingCurrency</span></span>](bookingcurrency.md) |<span data-ttu-id="4610d-117">获取**bookingCurrency**对象的属性。</span><span class="sxs-lookup"><span data-stu-id="4610d-117">Get the properties of a **bookingCurrency** object.</span></span>|


## <a name="properties"></a><span data-ttu-id="4610d-118">属性</span><span class="sxs-lookup"><span data-stu-id="4610d-118">Properties</span></span>
| <span data-ttu-id="4610d-119">属性</span><span class="sxs-lookup"><span data-stu-id="4610d-119">Property</span></span>     | <span data-ttu-id="4610d-120">类型</span><span class="sxs-lookup"><span data-stu-id="4610d-120">Type</span></span>   |<span data-ttu-id="4610d-121">说明</span><span class="sxs-lookup"><span data-stu-id="4610d-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4610d-122">id</span><span class="sxs-lookup"><span data-stu-id="4610d-122">id</span></span>|<span data-ttu-id="4610d-123">字符串</span><span class="sxs-lookup"><span data-stu-id="4610d-123">String</span></span>| <span data-ttu-id="4610d-124">基于[ISO 4217](https://www.iso.org/iso-4217-currency-codes.html)3 个字符货币代码。</span><span class="sxs-lookup"><span data-stu-id="4610d-124">A 3-character currency code, based on [ISO 4217](https://www.iso.org/iso-4217-currency-codes.html).</span></span> <span data-ttu-id="4610d-125">例如，美国美元的货币代码是美元，而澳大利亚元为 AUD.</span><span class="sxs-lookup"><span data-stu-id="4610d-125">For example, the currency code for the US dollar is USD, and for the Australian dollar is AUD.</span></span> <span data-ttu-id="4610d-126">只读。</span><span class="sxs-lookup"><span data-stu-id="4610d-126">Read-only.</span></span>|
|<span data-ttu-id="4610d-127">符号</span><span class="sxs-lookup"><span data-stu-id="4610d-127">symbol</span></span>|<span data-ttu-id="4610d-128">字符串</span><span class="sxs-lookup"><span data-stu-id="4610d-128">String</span></span>| <span data-ttu-id="4610d-129">货币符号。</span><span class="sxs-lookup"><span data-stu-id="4610d-129">The currency symbol.</span></span> <span data-ttu-id="4610d-130">例如，美国美元和澳大利亚元的货币符号是 $。</span><span class="sxs-lookup"><span data-stu-id="4610d-130">For example, the currency symbol for the US dollar and for the Australian dollar is $.</span></span>  |

## <a name="relationships"></a><span data-ttu-id="4610d-131">Relationships</span><span class="sxs-lookup"><span data-stu-id="4610d-131">Relationships</span></span>
<span data-ttu-id="4610d-132">无</span><span class="sxs-lookup"><span data-stu-id="4610d-132">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="4610d-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4610d-133">JSON representation</span></span>

<span data-ttu-id="4610d-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4610d-134">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "bookingCurrency resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

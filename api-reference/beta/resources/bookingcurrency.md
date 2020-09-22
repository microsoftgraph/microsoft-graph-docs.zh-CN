---
title: bookingCurrency 资源类型
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: f4b5cc6a8fdb36c2e4543302ac32846a1b3c4388
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48071792"
---
# <a name="bookingcurrency-resource-type"></a><span data-ttu-id="a05d0-104">bookingCurrency 资源类型</span><span class="sxs-lookup"><span data-stu-id="a05d0-104">bookingCurrency resource type</span></span>

<span data-ttu-id="a05d0-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a05d0-105">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="a05d0-106">表示 [bookingBusiness](bookingbusiness.md)支持的货币货币。</span><span class="sxs-lookup"><span data-stu-id="a05d0-106">Represents a monetary currency supported by a [bookingBusiness](bookingbusiness.md).</span></span>


## <a name="methods"></a><span data-ttu-id="a05d0-107">方法</span><span class="sxs-lookup"><span data-stu-id="a05d0-107">Methods</span></span>

| <span data-ttu-id="a05d0-108">方法</span><span class="sxs-lookup"><span data-stu-id="a05d0-108">Method</span></span>           | <span data-ttu-id="a05d0-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="a05d0-109">Return Type</span></span>    |<span data-ttu-id="a05d0-110">说明</span><span class="sxs-lookup"><span data-stu-id="a05d0-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a05d0-111">列出 bookingCurrencies</span><span class="sxs-lookup"><span data-stu-id="a05d0-111">List bookingCurrencies</span></span>](../api/bookingcurrency-list.md) | <span data-ttu-id="a05d0-112">[bookingCurrency](bookingcurrency.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a05d0-112">[bookingCurrency](bookingcurrency.md) collection</span></span> |<span data-ttu-id="a05d0-113">获取可用于 Microsoft 预订业务的 **bookingCurrency** 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="a05d0-113">Get a list of **bookingCurrency** objects available to a Microsoft Bookings business.</span></span>|
|[<span data-ttu-id="a05d0-114">获取 bookingCurrency</span><span class="sxs-lookup"><span data-stu-id="a05d0-114">Get bookingCurrency</span></span>](../api/bookingcurrency-get.md) | [<span data-ttu-id="a05d0-115">bookingCurrency</span><span class="sxs-lookup"><span data-stu-id="a05d0-115">bookingCurrency</span></span>](bookingcurrency.md) |<span data-ttu-id="a05d0-116">获取 **bookingCurrency** 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="a05d0-116">Get the properties of a **bookingCurrency** object.</span></span>|


## <a name="properties"></a><span data-ttu-id="a05d0-117">属性</span><span class="sxs-lookup"><span data-stu-id="a05d0-117">Properties</span></span>
| <span data-ttu-id="a05d0-118">属性</span><span class="sxs-lookup"><span data-stu-id="a05d0-118">Property</span></span>     | <span data-ttu-id="a05d0-119">类型</span><span class="sxs-lookup"><span data-stu-id="a05d0-119">Type</span></span>   |<span data-ttu-id="a05d0-120">说明</span><span class="sxs-lookup"><span data-stu-id="a05d0-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a05d0-121">id</span><span class="sxs-lookup"><span data-stu-id="a05d0-121">id</span></span>|<span data-ttu-id="a05d0-122">String</span><span class="sxs-lookup"><span data-stu-id="a05d0-122">String</span></span>| <span data-ttu-id="a05d0-123">基于 [ISO 4217](https://www.iso.org/iso-4217-currency-codes.html)的3个字符的货币代码。</span><span class="sxs-lookup"><span data-stu-id="a05d0-123">A 3-character currency code, based on [ISO 4217](https://www.iso.org/iso-4217-currency-codes.html).</span></span> <span data-ttu-id="a05d0-124">例如，美元的货币代码是 USD，而澳大利亚美元是 AUD。</span><span class="sxs-lookup"><span data-stu-id="a05d0-124">For example, the currency code for the US dollar is USD, and for the Australian dollar is AUD.</span></span> <span data-ttu-id="a05d0-125">只读。</span><span class="sxs-lookup"><span data-stu-id="a05d0-125">Read-only.</span></span>|
|<span data-ttu-id="a05d0-126">符号</span><span class="sxs-lookup"><span data-stu-id="a05d0-126">symbol</span></span>|<span data-ttu-id="a05d0-127">String</span><span class="sxs-lookup"><span data-stu-id="a05d0-127">String</span></span>| <span data-ttu-id="a05d0-128">货币符号。</span><span class="sxs-lookup"><span data-stu-id="a05d0-128">The currency symbol.</span></span> <span data-ttu-id="a05d0-129">例如，美元的货币符号和澳大利亚美元为美元。</span><span class="sxs-lookup"><span data-stu-id="a05d0-129">For example, the currency symbol for the US dollar and for the Australian dollar is $.</span></span>  |

## <a name="relationships"></a><span data-ttu-id="a05d0-130">关系</span><span class="sxs-lookup"><span data-stu-id="a05d0-130">Relationships</span></span>
<span data-ttu-id="a05d0-131">无</span><span class="sxs-lookup"><span data-stu-id="a05d0-131">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="a05d0-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a05d0-132">JSON representation</span></span>

<span data-ttu-id="a05d0-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a05d0-133">The following is a JSON representation of the resource.</span></span>

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



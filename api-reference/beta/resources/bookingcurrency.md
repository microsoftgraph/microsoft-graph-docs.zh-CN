---
title: bookingCurrency 资源类型
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 9d4feac66e72c756173113101a88bf8bbe35563a
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518196"
---
# <a name="bookingcurrency-resource-type"></a><span data-ttu-id="bf0f4-104">bookingCurrency 资源类型</span><span class="sxs-lookup"><span data-stu-id="bf0f4-104">bookingCurrency resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="bf0f4-105">代表货币货币[bookingBusiness](bookingbusiness.md)支持。</span><span class="sxs-lookup"><span data-stu-id="bf0f4-105">Represents a monetary currency supported by a [bookingBusiness](bookingbusiness.md).</span></span>


## <a name="methods"></a><span data-ttu-id="bf0f4-106">方法</span><span class="sxs-lookup"><span data-stu-id="bf0f4-106">Methods</span></span>

| <span data-ttu-id="bf0f4-107">方法</span><span class="sxs-lookup"><span data-stu-id="bf0f4-107">Method</span></span>           | <span data-ttu-id="bf0f4-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="bf0f4-108">Return Type</span></span>    |<span data-ttu-id="bf0f4-109">说明</span><span class="sxs-lookup"><span data-stu-id="bf0f4-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="bf0f4-110">列表 bookingCurrencies</span><span class="sxs-lookup"><span data-stu-id="bf0f4-110">List bookingCurrencies</span></span>](../api/bookingcurrency-list.md) | <span data-ttu-id="bf0f4-111">[bookingCurrency](bookingcurrency.md)集合</span><span class="sxs-lookup"><span data-stu-id="bf0f4-111">[bookingCurrency](bookingcurrency.md) collection</span></span> |<span data-ttu-id="bf0f4-112">获取供 Microsoft 预订业务**bookingCurrency**对象的列表。</span><span class="sxs-lookup"><span data-stu-id="bf0f4-112">Get a list of **bookingCurrency** objects available to a Microsoft Bookings business.</span></span>|
|[<span data-ttu-id="bf0f4-113">获取 bookingCurrency</span><span class="sxs-lookup"><span data-stu-id="bf0f4-113">Get bookingCurrency</span></span>](../api/bookingcurrency-get.md) | [<span data-ttu-id="bf0f4-114">bookingCurrency</span><span class="sxs-lookup"><span data-stu-id="bf0f4-114">bookingCurrency</span></span>](bookingcurrency.md) |<span data-ttu-id="bf0f4-115">获取**bookingCurrency**对象的属性。</span><span class="sxs-lookup"><span data-stu-id="bf0f4-115">Get the properties of a **bookingCurrency** object.</span></span>|


## <a name="properties"></a><span data-ttu-id="bf0f4-116">属性</span><span class="sxs-lookup"><span data-stu-id="bf0f4-116">Properties</span></span>
| <span data-ttu-id="bf0f4-117">属性</span><span class="sxs-lookup"><span data-stu-id="bf0f4-117">Property</span></span>     | <span data-ttu-id="bf0f4-118">类型</span><span class="sxs-lookup"><span data-stu-id="bf0f4-118">Type</span></span>   |<span data-ttu-id="bf0f4-119">说明</span><span class="sxs-lookup"><span data-stu-id="bf0f4-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bf0f4-120">id</span><span class="sxs-lookup"><span data-stu-id="bf0f4-120">id</span></span>|<span data-ttu-id="bf0f4-121">String</span><span class="sxs-lookup"><span data-stu-id="bf0f4-121">String</span></span>| <span data-ttu-id="bf0f4-122">基于[ISO 4217](https://www.iso.org/iso-4217-currency-codes.html)3 个字符货币代码。</span><span class="sxs-lookup"><span data-stu-id="bf0f4-122">A 3-character currency code, based on [ISO 4217](https://www.iso.org/iso-4217-currency-codes.html).</span></span> <span data-ttu-id="bf0f4-123">例如，美国美元的货币代码是美元，而澳大利亚元为 AUD.</span><span class="sxs-lookup"><span data-stu-id="bf0f4-123">For example, the currency code for the US dollar is USD, and for the Australian dollar is AUD.</span></span> <span data-ttu-id="bf0f4-124">只读。</span><span class="sxs-lookup"><span data-stu-id="bf0f4-124">Read-only.</span></span>|
|<span data-ttu-id="bf0f4-125">Symbol</span><span class="sxs-lookup"><span data-stu-id="bf0f4-125">symbol</span></span>|<span data-ttu-id="bf0f4-126">String</span><span class="sxs-lookup"><span data-stu-id="bf0f4-126">String</span></span>| <span data-ttu-id="bf0f4-127">货币符号。</span><span class="sxs-lookup"><span data-stu-id="bf0f4-127">The currency symbol.</span></span> <span data-ttu-id="bf0f4-128">例如，美国美元和澳大利亚元的货币符号是 $。</span><span class="sxs-lookup"><span data-stu-id="bf0f4-128">For example, the currency symbol for the US dollar and for the Australian dollar is $.</span></span>  |

## <a name="relationships"></a><span data-ttu-id="bf0f4-129">关系</span><span class="sxs-lookup"><span data-stu-id="bf0f4-129">Relationships</span></span>
<span data-ttu-id="bf0f4-130">无</span><span class="sxs-lookup"><span data-stu-id="bf0f4-130">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="bf0f4-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bf0f4-131">JSON representation</span></span>

<span data-ttu-id="bf0f4-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bf0f4-132">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/bookingcurrency.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

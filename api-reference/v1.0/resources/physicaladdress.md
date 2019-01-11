---
title: physicalAddress 资源类型
description: 表示资源（例如联系人或事件）的街道地址。
localization_priority: Normal
ms.openlocfilehash: 2bbfc3f38d4d353d370b9c8ba859b06cc2e4398b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27866008"
---
# <a name="physicaladdress-resource-type"></a><span data-ttu-id="ec39f-103">physicalAddress 资源类型</span><span class="sxs-lookup"><span data-stu-id="ec39f-103">physicalAddress resource type</span></span>

<span data-ttu-id="ec39f-104">表示资源（例如联系人或事件）的街道地址。</span><span class="sxs-lookup"><span data-stu-id="ec39f-104">Represents the street address of a resource such as a contact or event.</span></span>


## <a name="properties"></a><span data-ttu-id="ec39f-105">属性</span><span class="sxs-lookup"><span data-stu-id="ec39f-105">Properties</span></span>
| <span data-ttu-id="ec39f-106">属性</span><span class="sxs-lookup"><span data-stu-id="ec39f-106">Property</span></span>     | <span data-ttu-id="ec39f-107">类型</span><span class="sxs-lookup"><span data-stu-id="ec39f-107">Type</span></span>   |<span data-ttu-id="ec39f-108">说明</span><span class="sxs-lookup"><span data-stu-id="ec39f-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ec39f-109">city</span><span class="sxs-lookup"><span data-stu-id="ec39f-109">city</span></span>|<span data-ttu-id="ec39f-110">String</span><span class="sxs-lookup"><span data-stu-id="ec39f-110">String</span></span>|<span data-ttu-id="ec39f-111">城市。</span><span class="sxs-lookup"><span data-stu-id="ec39f-111">The city.</span></span>|
|<span data-ttu-id="ec39f-112">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="ec39f-112">countryOrRegion</span></span>|<span data-ttu-id="ec39f-113">字符串</span><span class="sxs-lookup"><span data-stu-id="ec39f-113">String</span></span>|<span data-ttu-id="ec39f-p101">国家或地区。它是任意格式的字符串值，例如“United States”。</span><span class="sxs-lookup"><span data-stu-id="ec39f-p101">The country or region. It's a free-format string value, for example, "United States".</span></span>|
|<span data-ttu-id="ec39f-116">postalCode</span><span class="sxs-lookup"><span data-stu-id="ec39f-116">postalCode</span></span>|<span data-ttu-id="ec39f-117">String</span><span class="sxs-lookup"><span data-stu-id="ec39f-117">String</span></span>|<span data-ttu-id="ec39f-118">邮政编码。</span><span class="sxs-lookup"><span data-stu-id="ec39f-118">The postal code.</span></span>|
|<span data-ttu-id="ec39f-119">state</span><span class="sxs-lookup"><span data-stu-id="ec39f-119">state</span></span>|<span data-ttu-id="ec39f-120">String</span><span class="sxs-lookup"><span data-stu-id="ec39f-120">String</span></span>|<span data-ttu-id="ec39f-121">省/市/自治区。</span><span class="sxs-lookup"><span data-stu-id="ec39f-121">The state.</span></span>|
|<span data-ttu-id="ec39f-122">street</span><span class="sxs-lookup"><span data-stu-id="ec39f-122">street</span></span>|<span data-ttu-id="ec39f-123">String</span><span class="sxs-lookup"><span data-stu-id="ec39f-123">String</span></span>|<span data-ttu-id="ec39f-124">街道。</span><span class="sxs-lookup"><span data-stu-id="ec39f-124">The street.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ec39f-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ec39f-125">JSON representation</span></span>

<span data-ttu-id="ec39f-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ec39f-126">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.physicalAddress"
}-->

```json
{
  "city": "string",
  "countryOrRegion": "string",
  "postalCode": "string",
  "state": "string",
  "street": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "physicalAddress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

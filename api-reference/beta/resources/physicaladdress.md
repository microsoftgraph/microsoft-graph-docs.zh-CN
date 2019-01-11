---
title: physicalAddress 资源类型
description: 表示资源（例如联系人或事件）的街道地址。
localization_priority: Normal
ms.openlocfilehash: 3a656046cc23394fc8cff9100eb5ad2289050b25
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27823581"
---
# <a name="physicaladdress-resource-type"></a><span data-ttu-id="c2216-103">physicalAddress 资源类型</span><span class="sxs-lookup"><span data-stu-id="c2216-103">physicalAddress resource type</span></span>

<span data-ttu-id="c2216-104">表示资源（例如联系人或事件）的街道地址。</span><span class="sxs-lookup"><span data-stu-id="c2216-104">Represents the street address of a resource such as a contact or event.</span></span>


## <a name="properties"></a><span data-ttu-id="c2216-105">属性</span><span class="sxs-lookup"><span data-stu-id="c2216-105">Properties</span></span>
| <span data-ttu-id="c2216-106">属性</span><span class="sxs-lookup"><span data-stu-id="c2216-106">Property</span></span>     | <span data-ttu-id="c2216-107">类型</span><span class="sxs-lookup"><span data-stu-id="c2216-107">Type</span></span>   |<span data-ttu-id="c2216-108">说明</span><span class="sxs-lookup"><span data-stu-id="c2216-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c2216-109">type</span><span class="sxs-lookup"><span data-stu-id="c2216-109">type</span></span>|<span data-ttu-id="c2216-110">字符串</span><span class="sxs-lookup"><span data-stu-id="c2216-110">String</span></span>|<span data-ttu-id="c2216-111">地址类型。</span><span class="sxs-lookup"><span data-stu-id="c2216-111">The type of address.</span></span> <span data-ttu-id="c2216-112">可取值为：`unknown`、`home`、`business`、`other`。</span><span class="sxs-lookup"><span data-stu-id="c2216-112">Possible values are: `unknown`, `home`, `business`, `other`.</span></span>|
|<span data-ttu-id="c2216-113">postOfficeBox</span><span class="sxs-lookup"><span data-stu-id="c2216-113">postOfficeBox</span></span>|<span data-ttu-id="c2216-114">字符串</span><span class="sxs-lookup"><span data-stu-id="c2216-114">String</span></span>|<span data-ttu-id="c2216-115">邮政信箱号码。</span><span class="sxs-lookup"><span data-stu-id="c2216-115">The post office box number.</span></span>|
|<span data-ttu-id="c2216-116">城市</span><span class="sxs-lookup"><span data-stu-id="c2216-116">city</span></span>|<span data-ttu-id="c2216-117">String</span><span class="sxs-lookup"><span data-stu-id="c2216-117">String</span></span>|<span data-ttu-id="c2216-118">城市。</span><span class="sxs-lookup"><span data-stu-id="c2216-118">The city.</span></span>|
|<span data-ttu-id="c2216-119">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="c2216-119">countryOrRegion</span></span>|<span data-ttu-id="c2216-120">字符串</span><span class="sxs-lookup"><span data-stu-id="c2216-120">String</span></span>|<span data-ttu-id="c2216-p102">国家或地区。它是任意格式的字符串值，例如“United States”。</span><span class="sxs-lookup"><span data-stu-id="c2216-p102">The country or region. It's a free-format string value, for example, "United States".</span></span>|
|<span data-ttu-id="c2216-123">postalCode</span><span class="sxs-lookup"><span data-stu-id="c2216-123">postalCode</span></span>|<span data-ttu-id="c2216-124">String</span><span class="sxs-lookup"><span data-stu-id="c2216-124">String</span></span>|<span data-ttu-id="c2216-125">邮政编码。</span><span class="sxs-lookup"><span data-stu-id="c2216-125">The postal code.</span></span>|
|<span data-ttu-id="c2216-126">state</span><span class="sxs-lookup"><span data-stu-id="c2216-126">state</span></span>|<span data-ttu-id="c2216-127">String</span><span class="sxs-lookup"><span data-stu-id="c2216-127">String</span></span>|<span data-ttu-id="c2216-128">省/市/自治区。</span><span class="sxs-lookup"><span data-stu-id="c2216-128">The state.</span></span>|
|<span data-ttu-id="c2216-129">street</span><span class="sxs-lookup"><span data-stu-id="c2216-129">street</span></span>|<span data-ttu-id="c2216-130">String</span><span class="sxs-lookup"><span data-stu-id="c2216-130">String</span></span>|<span data-ttu-id="c2216-131">街道。</span><span class="sxs-lookup"><span data-stu-id="c2216-131">The street.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c2216-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c2216-132">JSON representation</span></span>

<span data-ttu-id="c2216-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c2216-133">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.physicalAddress"
}-->

```json
{
  "type": "string",
  "postOfficeBox": "string",
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

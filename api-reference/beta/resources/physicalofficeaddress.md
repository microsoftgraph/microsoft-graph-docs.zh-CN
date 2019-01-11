---
title: physicalOfficeAddress 资源类型
description: 代表资源如 contact 或事件的业务地址。
localization_priority: Normal
ms.openlocfilehash: bd4274e29b2ef0f9e7e8318528d18103be19fabc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27817785"
---
# <a name="physicalofficeaddress-resource-type"></a><span data-ttu-id="e1eb1-103">physicalOfficeAddress 资源类型</span><span class="sxs-lookup"><span data-stu-id="e1eb1-103">physicalOfficeAddress resource type</span></span>

<span data-ttu-id="e1eb1-104">表示业务地址的资源，如组织联系人。</span><span class="sxs-lookup"><span data-stu-id="e1eb1-104">Represents the business address of a resource such as an organizational contact.</span></span>

## <a name="properties"></a><span data-ttu-id="e1eb1-105">属性</span><span class="sxs-lookup"><span data-stu-id="e1eb1-105">Properties</span></span>

| <span data-ttu-id="e1eb1-106">属性</span><span class="sxs-lookup"><span data-stu-id="e1eb1-106">Property</span></span>     | <span data-ttu-id="e1eb1-107">类型</span><span class="sxs-lookup"><span data-stu-id="e1eb1-107">Type</span></span>   |<span data-ttu-id="e1eb1-108">说明</span><span class="sxs-lookup"><span data-stu-id="e1eb1-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e1eb1-109">city</span><span class="sxs-lookup"><span data-stu-id="e1eb1-109">city</span></span>|<span data-ttu-id="e1eb1-110">String</span><span class="sxs-lookup"><span data-stu-id="e1eb1-110">String</span></span>|<span data-ttu-id="e1eb1-111">城市。</span><span class="sxs-lookup"><span data-stu-id="e1eb1-111">The city.</span></span>|
|<span data-ttu-id="e1eb1-112">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="e1eb1-112">countryOrRegion</span></span>|<span data-ttu-id="e1eb1-113">字符串</span><span class="sxs-lookup"><span data-stu-id="e1eb1-113">String</span></span>|<span data-ttu-id="e1eb1-p101">国家或地区。它是任意格式的字符串值，例如“United States”。</span><span class="sxs-lookup"><span data-stu-id="e1eb1-p101">The country or region. It's a free-format string value, for example, "United States".</span></span>|
|<span data-ttu-id="e1eb1-116">officeLocation</span><span class="sxs-lookup"><span data-stu-id="e1eb1-116">officeLocation</span></span>  | <span data-ttu-id="e1eb1-117">String</span><span class="sxs-lookup"><span data-stu-id="e1eb1-117">String</span></span> | <span data-ttu-id="e1eb1-118">如构建和 office 号码为组织的联系人的办公室位置。</span><span class="sxs-lookup"><span data-stu-id="e1eb1-118">Office location such as building and office number for an organizational contact.</span></span>  |
|<span data-ttu-id="e1eb1-119">postalCode</span><span class="sxs-lookup"><span data-stu-id="e1eb1-119">postalCode</span></span>|<span data-ttu-id="e1eb1-120">String</span><span class="sxs-lookup"><span data-stu-id="e1eb1-120">String</span></span>|<span data-ttu-id="e1eb1-121">邮政编码。</span><span class="sxs-lookup"><span data-stu-id="e1eb1-121">The postal code.</span></span>|
|<span data-ttu-id="e1eb1-122">state</span><span class="sxs-lookup"><span data-stu-id="e1eb1-122">state</span></span>|<span data-ttu-id="e1eb1-123">String</span><span class="sxs-lookup"><span data-stu-id="e1eb1-123">String</span></span>|<span data-ttu-id="e1eb1-124">省/市/自治区。</span><span class="sxs-lookup"><span data-stu-id="e1eb1-124">The state.</span></span>|
|<span data-ttu-id="e1eb1-125">street</span><span class="sxs-lookup"><span data-stu-id="e1eb1-125">street</span></span>|<span data-ttu-id="e1eb1-126">String</span><span class="sxs-lookup"><span data-stu-id="e1eb1-126">String</span></span>|<span data-ttu-id="e1eb1-127">街道。</span><span class="sxs-lookup"><span data-stu-id="e1eb1-127">The street.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e1eb1-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e1eb1-128">JSON representation</span></span>

<span data-ttu-id="e1eb1-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e1eb1-129">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.physicalOfficeAddress"
}-->

```json
{
  "city": "string",
  "countryOrRegion": "string",
  "officeLocation": "string",
  "postalCode": "string",
  "state": "string",
  "street": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "physicalOfficeAddress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

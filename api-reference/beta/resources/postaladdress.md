---
title: 省略资源类型
description: 表示资源（例如联系人或事件）的街道地址。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 7d168e4f53dbd182e4dbd93d0a5b6342daf3339d
ms.sourcegitcommit: 539ed08adf3b7ad3253c98636d4ab303ce00176e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/15/2019
ms.locfileid: "30057341"
---
# <a name="postaladdress-resource-type"></a><span data-ttu-id="37200-103">省略资源类型</span><span class="sxs-lookup"><span data-stu-id="37200-103">postalAddress resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="37200-104">表示位置的街道地址。</span><span class="sxs-lookup"><span data-stu-id="37200-104">Represents the street address of a location.</span></span>


## <a name="properties"></a><span data-ttu-id="37200-105">属性</span><span class="sxs-lookup"><span data-stu-id="37200-105">Properties</span></span>
| <span data-ttu-id="37200-106">属性</span><span class="sxs-lookup"><span data-stu-id="37200-106">Property</span></span>     | <span data-ttu-id="37200-107">类型</span><span class="sxs-lookup"><span data-stu-id="37200-107">Type</span></span>   |<span data-ttu-id="37200-108">说明</span><span class="sxs-lookup"><span data-stu-id="37200-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="37200-109">city</span><span class="sxs-lookup"><span data-stu-id="37200-109">city</span></span>|<span data-ttu-id="37200-110">String</span><span class="sxs-lookup"><span data-stu-id="37200-110">String</span></span>|<span data-ttu-id="37200-111">城市。</span><span class="sxs-lookup"><span data-stu-id="37200-111">The city.</span></span>|
|<span data-ttu-id="37200-112">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="37200-112">countryOrRegion</span></span>|<span data-ttu-id="37200-113">字符串</span><span class="sxs-lookup"><span data-stu-id="37200-113">String</span></span>|<span data-ttu-id="37200-p101">国家或地区。它是任意格式的字符串值，例如“United States”。</span><span class="sxs-lookup"><span data-stu-id="37200-p101">The country or region. It's a free-format string value, for example, "United States".</span></span>|
|<span data-ttu-id="37200-116">isInferred</span><span class="sxs-lookup"><span data-stu-id="37200-116">isInferred</span></span>|<span data-ttu-id="37200-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="37200-117">Boolean</span></span>|<span data-ttu-id="37200-118">仅供内部使用。</span><span class="sxs-lookup"><span data-stu-id="37200-118">For internal use only.</span></span>|
|<span data-ttu-id="37200-119">postalCode</span><span class="sxs-lookup"><span data-stu-id="37200-119">postalCode</span></span>|<span data-ttu-id="37200-120">String</span><span class="sxs-lookup"><span data-stu-id="37200-120">String</span></span>|<span data-ttu-id="37200-121">邮政编码。</span><span class="sxs-lookup"><span data-stu-id="37200-121">The postal code.</span></span>|
|<span data-ttu-id="37200-122">state</span><span class="sxs-lookup"><span data-stu-id="37200-122">state</span></span>|<span data-ttu-id="37200-123">String</span><span class="sxs-lookup"><span data-stu-id="37200-123">String</span></span>|<span data-ttu-id="37200-124">省/市/自治区。</span><span class="sxs-lookup"><span data-stu-id="37200-124">The state.</span></span>|
|<span data-ttu-id="37200-125">street</span><span class="sxs-lookup"><span data-stu-id="37200-125">street</span></span>|<span data-ttu-id="37200-126">String</span><span class="sxs-lookup"><span data-stu-id="37200-126">String</span></span>|<span data-ttu-id="37200-127">街道。</span><span class="sxs-lookup"><span data-stu-id="37200-127">The street.</span></span>|
|<span data-ttu-id="37200-128">type</span><span class="sxs-lookup"><span data-stu-id="37200-128">type</span></span>|<span data-ttu-id="37200-129">addressType</span><span class="sxs-lookup"><span data-stu-id="37200-129">addressType</span></span>|<span data-ttu-id="37200-130">地址类型。</span><span class="sxs-lookup"><span data-stu-id="37200-130">The type of address.</span></span> <span data-ttu-id="37200-131">可能的值为: `unknown`、 `home`、 `business`、 `other`。</span><span class="sxs-lookup"><span data-stu-id="37200-131">The possible values are: `unknown`, `home`, `business`, `other`.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="37200-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="37200-132">JSON representation</span></span>

<span data-ttu-id="37200-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="37200-133">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.postalAddress"
}-->

```json
{
  "city": "string",
  "countryOrRegion": "string",
  "isInferred": "boolean",
  "postalCode": "string",
  "state": "string",
  "street": "string",
  "type": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "postaladdress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/postaladdress.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}-->

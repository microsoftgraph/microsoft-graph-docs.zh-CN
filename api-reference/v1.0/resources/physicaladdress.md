---
title: physicalAddress 资源类型
description: 表示资源（例如联系人或事件）的街道地址。
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: f301947d6d277cd4fd51b7db035ef4f7134a5e65
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035505"
---
# <a name="physicaladdress-resource-type"></a><span data-ttu-id="2c5da-103">physicalAddress 资源类型</span><span class="sxs-lookup"><span data-stu-id="2c5da-103">physicalAddress resource type</span></span>

<span data-ttu-id="2c5da-104">表示资源（例如联系人或事件）的街道地址。</span><span class="sxs-lookup"><span data-stu-id="2c5da-104">Represents the street address of a resource such as a contact or event.</span></span>


## <a name="properties"></a><span data-ttu-id="2c5da-105">属性</span><span class="sxs-lookup"><span data-stu-id="2c5da-105">Properties</span></span>
| <span data-ttu-id="2c5da-106">属性</span><span class="sxs-lookup"><span data-stu-id="2c5da-106">Property</span></span>     | <span data-ttu-id="2c5da-107">类型</span><span class="sxs-lookup"><span data-stu-id="2c5da-107">Type</span></span>   |<span data-ttu-id="2c5da-108">说明</span><span class="sxs-lookup"><span data-stu-id="2c5da-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2c5da-109">city</span><span class="sxs-lookup"><span data-stu-id="2c5da-109">city</span></span>|<span data-ttu-id="2c5da-110">String</span><span class="sxs-lookup"><span data-stu-id="2c5da-110">String</span></span>|<span data-ttu-id="2c5da-111">城市。</span><span class="sxs-lookup"><span data-stu-id="2c5da-111">The city.</span></span>|
|<span data-ttu-id="2c5da-112">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="2c5da-112">countryOrRegion</span></span>|<span data-ttu-id="2c5da-113">字符串</span><span class="sxs-lookup"><span data-stu-id="2c5da-113">String</span></span>|<span data-ttu-id="2c5da-p101">国家或地区。它是任意格式的字符串值，例如“United States”。</span><span class="sxs-lookup"><span data-stu-id="2c5da-p101">The country or region. It's a free-format string value, for example, "United States".</span></span>|
|<span data-ttu-id="2c5da-116">postalCode</span><span class="sxs-lookup"><span data-stu-id="2c5da-116">postalCode</span></span>|<span data-ttu-id="2c5da-117">String</span><span class="sxs-lookup"><span data-stu-id="2c5da-117">String</span></span>|<span data-ttu-id="2c5da-118">邮政编码。</span><span class="sxs-lookup"><span data-stu-id="2c5da-118">The postal code.</span></span>|
|<span data-ttu-id="2c5da-119">state</span><span class="sxs-lookup"><span data-stu-id="2c5da-119">state</span></span>|<span data-ttu-id="2c5da-120">String</span><span class="sxs-lookup"><span data-stu-id="2c5da-120">String</span></span>|<span data-ttu-id="2c5da-121">省/市/自治区。</span><span class="sxs-lookup"><span data-stu-id="2c5da-121">The state.</span></span>|
|<span data-ttu-id="2c5da-122">street</span><span class="sxs-lookup"><span data-stu-id="2c5da-122">street</span></span>|<span data-ttu-id="2c5da-123">String</span><span class="sxs-lookup"><span data-stu-id="2c5da-123">String</span></span>|<span data-ttu-id="2c5da-124">街道。</span><span class="sxs-lookup"><span data-stu-id="2c5da-124">The street.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2c5da-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2c5da-125">JSON representation</span></span>

<span data-ttu-id="2c5da-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2c5da-126">Here is a JSON representation of the resource</span></span>

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

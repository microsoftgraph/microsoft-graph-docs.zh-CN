---
title: physicalAddress 资源类型
description: 表示资源（例如联系人或事件）的街道地址。
localization_priority: Normal
author: kevinbellinger
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: e7729762a93e5185d45289b2377ecd961d894552
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46808856"
---
# <a name="physicaladdress-resource-type"></a><span data-ttu-id="1e4c3-103">physicalAddress 资源类型</span><span class="sxs-lookup"><span data-stu-id="1e4c3-103">physicalAddress resource type</span></span>

<span data-ttu-id="1e4c3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1e4c3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1e4c3-105">表示资源（例如联系人或事件）的街道地址。</span><span class="sxs-lookup"><span data-stu-id="1e4c3-105">Represents the street address of a resource such as a contact or event.</span></span>


## <a name="properties"></a><span data-ttu-id="1e4c3-106">属性</span><span class="sxs-lookup"><span data-stu-id="1e4c3-106">Properties</span></span>
| <span data-ttu-id="1e4c3-107">属性</span><span class="sxs-lookup"><span data-stu-id="1e4c3-107">Property</span></span>     | <span data-ttu-id="1e4c3-108">类型</span><span class="sxs-lookup"><span data-stu-id="1e4c3-108">Type</span></span>   |<span data-ttu-id="1e4c3-109">说明</span><span class="sxs-lookup"><span data-stu-id="1e4c3-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1e4c3-110">城市</span><span class="sxs-lookup"><span data-stu-id="1e4c3-110">city</span></span>|<span data-ttu-id="1e4c3-111">String</span><span class="sxs-lookup"><span data-stu-id="1e4c3-111">String</span></span>|<span data-ttu-id="1e4c3-112">城市。</span><span class="sxs-lookup"><span data-stu-id="1e4c3-112">The city.</span></span>|
|<span data-ttu-id="1e4c3-113">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="1e4c3-113">countryOrRegion</span></span>|<span data-ttu-id="1e4c3-114">String</span><span class="sxs-lookup"><span data-stu-id="1e4c3-114">String</span></span>|<span data-ttu-id="1e4c3-p101">国家或地区。它是任意格式的字符串值，例如“United States”。</span><span class="sxs-lookup"><span data-stu-id="1e4c3-p101">The country or region. It's a free-format string value, for example, "United States".</span></span>|
|<span data-ttu-id="1e4c3-117">postalCode</span><span class="sxs-lookup"><span data-stu-id="1e4c3-117">postalCode</span></span>|<span data-ttu-id="1e4c3-118">String</span><span class="sxs-lookup"><span data-stu-id="1e4c3-118">String</span></span>|<span data-ttu-id="1e4c3-119">邮政编码。</span><span class="sxs-lookup"><span data-stu-id="1e4c3-119">The postal code.</span></span>|
|<span data-ttu-id="1e4c3-120">state</span><span class="sxs-lookup"><span data-stu-id="1e4c3-120">state</span></span>|<span data-ttu-id="1e4c3-121">String</span><span class="sxs-lookup"><span data-stu-id="1e4c3-121">String</span></span>|<span data-ttu-id="1e4c3-122">省/市/自治区。</span><span class="sxs-lookup"><span data-stu-id="1e4c3-122">The state.</span></span>|
|<span data-ttu-id="1e4c3-123">street</span><span class="sxs-lookup"><span data-stu-id="1e4c3-123">street</span></span>|<span data-ttu-id="1e4c3-124">String</span><span class="sxs-lookup"><span data-stu-id="1e4c3-124">String</span></span>|<span data-ttu-id="1e4c3-125">街道。</span><span class="sxs-lookup"><span data-stu-id="1e4c3-125">The street.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1e4c3-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1e4c3-126">JSON representation</span></span>

<span data-ttu-id="1e4c3-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1e4c3-127">Here is a JSON representation of the resource</span></span>

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

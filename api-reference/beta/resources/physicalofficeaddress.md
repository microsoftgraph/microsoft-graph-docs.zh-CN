---
title: physicalOfficeAddress 资源类型
description: 表示某个资源 (如联系人或事件) 的业务地址。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 8299f72032cfb7910583fcd4dbefe914f054648e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966095"
---
# <a name="physicalofficeaddress-resource-type"></a><span data-ttu-id="1debf-103">physicalOfficeAddress 资源类型</span><span class="sxs-lookup"><span data-stu-id="1debf-103">physicalOfficeAddress resource type</span></span>

<span data-ttu-id="1debf-104">表示资源 (如组织联系人) 的业务地址。</span><span class="sxs-lookup"><span data-stu-id="1debf-104">Represents the business address of a resource such as an organizational contact.</span></span>

## <a name="properties"></a><span data-ttu-id="1debf-105">属性</span><span class="sxs-lookup"><span data-stu-id="1debf-105">Properties</span></span>

| <span data-ttu-id="1debf-106">属性</span><span class="sxs-lookup"><span data-stu-id="1debf-106">Property</span></span>     | <span data-ttu-id="1debf-107">类型</span><span class="sxs-lookup"><span data-stu-id="1debf-107">Type</span></span>   |<span data-ttu-id="1debf-108">说明</span><span class="sxs-lookup"><span data-stu-id="1debf-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1debf-109">city</span><span class="sxs-lookup"><span data-stu-id="1debf-109">city</span></span>|<span data-ttu-id="1debf-110">String</span><span class="sxs-lookup"><span data-stu-id="1debf-110">String</span></span>|<span data-ttu-id="1debf-111">城市。</span><span class="sxs-lookup"><span data-stu-id="1debf-111">The city.</span></span>|
|<span data-ttu-id="1debf-112">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="1debf-112">countryOrRegion</span></span>|<span data-ttu-id="1debf-113">字符串</span><span class="sxs-lookup"><span data-stu-id="1debf-113">String</span></span>|<span data-ttu-id="1debf-p101">国家或地区。它是任意格式的字符串值，例如“United States”。</span><span class="sxs-lookup"><span data-stu-id="1debf-p101">The country or region. It's a free-format string value, for example, "United States".</span></span>|
|<span data-ttu-id="1debf-116">officeLocation</span><span class="sxs-lookup"><span data-stu-id="1debf-116">officeLocation</span></span>  | <span data-ttu-id="1debf-117">String</span><span class="sxs-lookup"><span data-stu-id="1debf-117">String</span></span> | <span data-ttu-id="1debf-118">组织联系人的办公地点, 如建筑物和办公室号码。</span><span class="sxs-lookup"><span data-stu-id="1debf-118">Office location such as building and office number for an organizational contact.</span></span>  |
|<span data-ttu-id="1debf-119">postalCode</span><span class="sxs-lookup"><span data-stu-id="1debf-119">postalCode</span></span>|<span data-ttu-id="1debf-120">String</span><span class="sxs-lookup"><span data-stu-id="1debf-120">String</span></span>|<span data-ttu-id="1debf-121">邮政编码。</span><span class="sxs-lookup"><span data-stu-id="1debf-121">The postal code.</span></span>|
|<span data-ttu-id="1debf-122">state</span><span class="sxs-lookup"><span data-stu-id="1debf-122">state</span></span>|<span data-ttu-id="1debf-123">String</span><span class="sxs-lookup"><span data-stu-id="1debf-123">String</span></span>|<span data-ttu-id="1debf-124">省/市/自治区。</span><span class="sxs-lookup"><span data-stu-id="1debf-124">The state.</span></span>|
|<span data-ttu-id="1debf-125">street</span><span class="sxs-lookup"><span data-stu-id="1debf-125">street</span></span>|<span data-ttu-id="1debf-126">String</span><span class="sxs-lookup"><span data-stu-id="1debf-126">String</span></span>|<span data-ttu-id="1debf-127">街道。</span><span class="sxs-lookup"><span data-stu-id="1debf-127">The street.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1debf-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1debf-128">JSON representation</span></span>

<span data-ttu-id="1debf-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1debf-129">Here is a JSON representation of the resource</span></span>

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

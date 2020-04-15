---
title: physicalOfficeAddress 资源类型
description: 表示某个资源（如联系人或事件）的业务地址。
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 46674ad9be3e86fd36f5a5beb52829959bbd340b
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43445544"
---
# <a name="physicalofficeaddress-resource-type"></a><span data-ttu-id="baa3e-103">physicalOfficeAddress 资源类型</span><span class="sxs-lookup"><span data-stu-id="baa3e-103">physicalOfficeAddress resource type</span></span>

<span data-ttu-id="baa3e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="baa3e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="baa3e-105">表示资源（如组织联系人）的业务地址。</span><span class="sxs-lookup"><span data-stu-id="baa3e-105">Represents the business address of a resource such as an organizational contact.</span></span>

## <a name="properties"></a><span data-ttu-id="baa3e-106">属性</span><span class="sxs-lookup"><span data-stu-id="baa3e-106">Properties</span></span>

| <span data-ttu-id="baa3e-107">属性</span><span class="sxs-lookup"><span data-stu-id="baa3e-107">Property</span></span>     | <span data-ttu-id="baa3e-108">类型</span><span class="sxs-lookup"><span data-stu-id="baa3e-108">Type</span></span>   |<span data-ttu-id="baa3e-109">说明</span><span class="sxs-lookup"><span data-stu-id="baa3e-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="baa3e-110">city</span><span class="sxs-lookup"><span data-stu-id="baa3e-110">city</span></span>|<span data-ttu-id="baa3e-111">String</span><span class="sxs-lookup"><span data-stu-id="baa3e-111">String</span></span>|<span data-ttu-id="baa3e-112">城市。</span><span class="sxs-lookup"><span data-stu-id="baa3e-112">The city.</span></span>|
|<span data-ttu-id="baa3e-113">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="baa3e-113">countryOrRegion</span></span>|<span data-ttu-id="baa3e-114">字符串</span><span class="sxs-lookup"><span data-stu-id="baa3e-114">String</span></span>|<span data-ttu-id="baa3e-p101">国家或地区。它是任意格式的字符串值，例如“United States”。</span><span class="sxs-lookup"><span data-stu-id="baa3e-p101">The country or region. It's a free-format string value, for example, "United States".</span></span>|
|<span data-ttu-id="baa3e-117">officeLocation</span><span class="sxs-lookup"><span data-stu-id="baa3e-117">officeLocation</span></span>  | <span data-ttu-id="baa3e-118">String</span><span class="sxs-lookup"><span data-stu-id="baa3e-118">String</span></span> | <span data-ttu-id="baa3e-119">组织联系人的办公地点，如建筑物和办公室号码。</span><span class="sxs-lookup"><span data-stu-id="baa3e-119">Office location such as building and office number for an organizational contact.</span></span>  |
|<span data-ttu-id="baa3e-120">postalCode</span><span class="sxs-lookup"><span data-stu-id="baa3e-120">postalCode</span></span>|<span data-ttu-id="baa3e-121">String</span><span class="sxs-lookup"><span data-stu-id="baa3e-121">String</span></span>|<span data-ttu-id="baa3e-122">邮政编码。</span><span class="sxs-lookup"><span data-stu-id="baa3e-122">The postal code.</span></span>|
|<span data-ttu-id="baa3e-123">state</span><span class="sxs-lookup"><span data-stu-id="baa3e-123">state</span></span>|<span data-ttu-id="baa3e-124">String</span><span class="sxs-lookup"><span data-stu-id="baa3e-124">String</span></span>|<span data-ttu-id="baa3e-125">省/市/自治区。</span><span class="sxs-lookup"><span data-stu-id="baa3e-125">The state.</span></span>|
|<span data-ttu-id="baa3e-126">street</span><span class="sxs-lookup"><span data-stu-id="baa3e-126">street</span></span>|<span data-ttu-id="baa3e-127">String</span><span class="sxs-lookup"><span data-stu-id="baa3e-127">String</span></span>|<span data-ttu-id="baa3e-128">街道。</span><span class="sxs-lookup"><span data-stu-id="baa3e-128">The street.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="baa3e-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="baa3e-129">JSON representation</span></span>

<span data-ttu-id="baa3e-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="baa3e-130">Here is a JSON representation of the resource</span></span>

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

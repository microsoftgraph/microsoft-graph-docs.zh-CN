---
title: physicalAddress 资源类型
description: 表示资源（例如联系人或事件）的街道地址。
localization_priority: Normal
author: harini84
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 36edf38d16ca5e27fe5995eb59ec9150c3d76d87
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43455551"
---
# <a name="physicaladdress-resource-type"></a><span data-ttu-id="b8885-103">physicalAddress 资源类型</span><span class="sxs-lookup"><span data-stu-id="b8885-103">physicalAddress resource type</span></span>

<span data-ttu-id="b8885-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b8885-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b8885-105">表示资源（例如联系人或事件）的街道地址。</span><span class="sxs-lookup"><span data-stu-id="b8885-105">Represents the street address of a resource such as a contact or event.</span></span>


## <a name="properties"></a><span data-ttu-id="b8885-106">属性</span><span class="sxs-lookup"><span data-stu-id="b8885-106">Properties</span></span>
| <span data-ttu-id="b8885-107">属性</span><span class="sxs-lookup"><span data-stu-id="b8885-107">Property</span></span>     | <span data-ttu-id="b8885-108">类型</span><span class="sxs-lookup"><span data-stu-id="b8885-108">Type</span></span>   |<span data-ttu-id="b8885-109">说明</span><span class="sxs-lookup"><span data-stu-id="b8885-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b8885-110">city</span><span class="sxs-lookup"><span data-stu-id="b8885-110">city</span></span>|<span data-ttu-id="b8885-111">String</span><span class="sxs-lookup"><span data-stu-id="b8885-111">String</span></span>|<span data-ttu-id="b8885-112">城市。</span><span class="sxs-lookup"><span data-stu-id="b8885-112">The city.</span></span>|
|<span data-ttu-id="b8885-113">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="b8885-113">countryOrRegion</span></span>|<span data-ttu-id="b8885-114">字符串</span><span class="sxs-lookup"><span data-stu-id="b8885-114">String</span></span>|<span data-ttu-id="b8885-p101">国家或地区。它是任意格式的字符串值，例如“United States”。</span><span class="sxs-lookup"><span data-stu-id="b8885-p101">The country or region. It's a free-format string value, for example, "United States".</span></span>|
|<span data-ttu-id="b8885-117">postalCode</span><span class="sxs-lookup"><span data-stu-id="b8885-117">postalCode</span></span>|<span data-ttu-id="b8885-118">String</span><span class="sxs-lookup"><span data-stu-id="b8885-118">String</span></span>|<span data-ttu-id="b8885-119">邮政编码。</span><span class="sxs-lookup"><span data-stu-id="b8885-119">The postal code.</span></span>|
|<span data-ttu-id="b8885-120">postOfficeBox</span><span class="sxs-lookup"><span data-stu-id="b8885-120">postOfficeBox</span></span>|<span data-ttu-id="b8885-121">String</span><span class="sxs-lookup"><span data-stu-id="b8885-121">String</span></span>|<span data-ttu-id="b8885-122">邮局编号。</span><span class="sxs-lookup"><span data-stu-id="b8885-122">The post office box number.</span></span>|
|<span data-ttu-id="b8885-123">state</span><span class="sxs-lookup"><span data-stu-id="b8885-123">state</span></span>|<span data-ttu-id="b8885-124">String</span><span class="sxs-lookup"><span data-stu-id="b8885-124">String</span></span>|<span data-ttu-id="b8885-125">省/市/自治区。</span><span class="sxs-lookup"><span data-stu-id="b8885-125">The state.</span></span>|
|<span data-ttu-id="b8885-126">street</span><span class="sxs-lookup"><span data-stu-id="b8885-126">street</span></span>|<span data-ttu-id="b8885-127">String</span><span class="sxs-lookup"><span data-stu-id="b8885-127">String</span></span>|<span data-ttu-id="b8885-128">街道。</span><span class="sxs-lookup"><span data-stu-id="b8885-128">The street.</span></span>|
|<span data-ttu-id="b8885-129">type</span><span class="sxs-lookup"><span data-stu-id="b8885-129">type</span></span>|<span data-ttu-id="b8885-130">： Physicaladdresstype</span><span class="sxs-lookup"><span data-stu-id="b8885-130">physicalAddressType</span></span>|<span data-ttu-id="b8885-131">地址类型。</span><span class="sxs-lookup"><span data-stu-id="b8885-131">The type of address.</span></span> <span data-ttu-id="b8885-132">可取值为：`unknown`、`home`、`business`、`other`。</span><span class="sxs-lookup"><span data-stu-id="b8885-132">Possible values are: `unknown`, `home`, `business`, `other`.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="b8885-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b8885-133">JSON representation</span></span>

<span data-ttu-id="b8885-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b8885-134">Here is a JSON representation of the resource</span></span>

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
  "postOfficeBox": "string",
  "state": "string",
  "street": "string",
  "type": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "physicalAddress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

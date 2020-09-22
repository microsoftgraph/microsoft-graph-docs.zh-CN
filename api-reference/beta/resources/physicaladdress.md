---
title: physicalAddress 资源类型
description: 表示资源（例如联系人或事件）的街道地址。
localization_priority: Normal
author: harini84
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: d3d0a998f317a0fa19e7c29aabda5bc8e3908f85
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47997823"
---
# <a name="physicaladdress-resource-type"></a><span data-ttu-id="df879-103">physicalAddress 资源类型</span><span class="sxs-lookup"><span data-stu-id="df879-103">physicalAddress resource type</span></span>

<span data-ttu-id="df879-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="df879-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="df879-105">表示资源（例如联系人或事件）的街道地址。</span><span class="sxs-lookup"><span data-stu-id="df879-105">Represents the street address of a resource such as a contact or event.</span></span>


## <a name="properties"></a><span data-ttu-id="df879-106">属性</span><span class="sxs-lookup"><span data-stu-id="df879-106">Properties</span></span>
| <span data-ttu-id="df879-107">属性</span><span class="sxs-lookup"><span data-stu-id="df879-107">Property</span></span>     | <span data-ttu-id="df879-108">类型</span><span class="sxs-lookup"><span data-stu-id="df879-108">Type</span></span>   |<span data-ttu-id="df879-109">说明</span><span class="sxs-lookup"><span data-stu-id="df879-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="df879-110">城市</span><span class="sxs-lookup"><span data-stu-id="df879-110">city</span></span>|<span data-ttu-id="df879-111">String</span><span class="sxs-lookup"><span data-stu-id="df879-111">String</span></span>|<span data-ttu-id="df879-112">城市。</span><span class="sxs-lookup"><span data-stu-id="df879-112">The city.</span></span>|
|<span data-ttu-id="df879-113">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="df879-113">countryOrRegion</span></span>|<span data-ttu-id="df879-114">String</span><span class="sxs-lookup"><span data-stu-id="df879-114">String</span></span>|<span data-ttu-id="df879-p101">国家或地区。它是任意格式的字符串值，例如“United States”。</span><span class="sxs-lookup"><span data-stu-id="df879-p101">The country or region. It's a free-format string value, for example, "United States".</span></span>|
|<span data-ttu-id="df879-117">postalCode</span><span class="sxs-lookup"><span data-stu-id="df879-117">postalCode</span></span>|<span data-ttu-id="df879-118">String</span><span class="sxs-lookup"><span data-stu-id="df879-118">String</span></span>|<span data-ttu-id="df879-119">邮政编码。</span><span class="sxs-lookup"><span data-stu-id="df879-119">The postal code.</span></span>|
|<span data-ttu-id="df879-120">postOfficeBox</span><span class="sxs-lookup"><span data-stu-id="df879-120">postOfficeBox</span></span>|<span data-ttu-id="df879-121">String</span><span class="sxs-lookup"><span data-stu-id="df879-121">String</span></span>|<span data-ttu-id="df879-122">邮局编号。</span><span class="sxs-lookup"><span data-stu-id="df879-122">The post office box number.</span></span>|
|<span data-ttu-id="df879-123">state</span><span class="sxs-lookup"><span data-stu-id="df879-123">state</span></span>|<span data-ttu-id="df879-124">String</span><span class="sxs-lookup"><span data-stu-id="df879-124">String</span></span>|<span data-ttu-id="df879-125">省/市/自治区。</span><span class="sxs-lookup"><span data-stu-id="df879-125">The state.</span></span>|
|<span data-ttu-id="df879-126">street</span><span class="sxs-lookup"><span data-stu-id="df879-126">street</span></span>|<span data-ttu-id="df879-127">String</span><span class="sxs-lookup"><span data-stu-id="df879-127">String</span></span>|<span data-ttu-id="df879-128">街道。</span><span class="sxs-lookup"><span data-stu-id="df879-128">The street.</span></span>|
|<span data-ttu-id="df879-129">type</span><span class="sxs-lookup"><span data-stu-id="df879-129">type</span></span>|<span data-ttu-id="df879-130">： Physicaladdresstype</span><span class="sxs-lookup"><span data-stu-id="df879-130">physicalAddressType</span></span>|<span data-ttu-id="df879-131">地址类型。</span><span class="sxs-lookup"><span data-stu-id="df879-131">The type of address.</span></span> <span data-ttu-id="df879-132">可取值为：`unknown`、`home`、`business`、`other`。</span><span class="sxs-lookup"><span data-stu-id="df879-132">Possible values are: `unknown`, `home`, `business`, `other`.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="df879-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="df879-133">JSON representation</span></span>

<span data-ttu-id="df879-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="df879-134">Here is a JSON representation of the resource</span></span>

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



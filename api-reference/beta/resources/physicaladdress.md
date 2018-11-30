---
title: physicalAddress 资源类型
description: 表示资源（例如联系人或事件）的街道地址。
ms.openlocfilehash: 819240be3eb9a088fde43390fbb1d1d4af1fd30c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27048073"
---
# <a name="physicaladdress-resource-type"></a><span data-ttu-id="c9b60-103">physicalAddress 资源类型</span><span class="sxs-lookup"><span data-stu-id="c9b60-103">physicalAddress resource type</span></span>

<span data-ttu-id="c9b60-104">表示资源（例如联系人或事件）的街道地址。</span><span class="sxs-lookup"><span data-stu-id="c9b60-104">Represents the street address of a resource such as a contact or event.</span></span>


## <a name="properties"></a><span data-ttu-id="c9b60-105">属性</span><span class="sxs-lookup"><span data-stu-id="c9b60-105">Properties</span></span>
| <span data-ttu-id="c9b60-106">属性</span><span class="sxs-lookup"><span data-stu-id="c9b60-106">Property</span></span>     | <span data-ttu-id="c9b60-107">类型</span><span class="sxs-lookup"><span data-stu-id="c9b60-107">Type</span></span>   |<span data-ttu-id="c9b60-108">说明</span><span class="sxs-lookup"><span data-stu-id="c9b60-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c9b60-109">type</span><span class="sxs-lookup"><span data-stu-id="c9b60-109">type</span></span>|<span data-ttu-id="c9b60-110">字符串</span><span class="sxs-lookup"><span data-stu-id="c9b60-110">String</span></span>|<span data-ttu-id="c9b60-111">地址类型。</span><span class="sxs-lookup"><span data-stu-id="c9b60-111">The type of address.</span></span> <span data-ttu-id="c9b60-112">可取值为：`unknown`、`home`、`business`、`other`。</span><span class="sxs-lookup"><span data-stu-id="c9b60-112">Possible values are: `unknown`, `home`, `business`, `other`.</span></span>|
|<span data-ttu-id="c9b60-113">postOfficeBox</span><span class="sxs-lookup"><span data-stu-id="c9b60-113">postOfficeBox</span></span>|<span data-ttu-id="c9b60-114">字符串</span><span class="sxs-lookup"><span data-stu-id="c9b60-114">String</span></span>|<span data-ttu-id="c9b60-115">邮政信箱号码。</span><span class="sxs-lookup"><span data-stu-id="c9b60-115">The post office box number.</span></span>|
|<span data-ttu-id="c9b60-116">城市</span><span class="sxs-lookup"><span data-stu-id="c9b60-116">city</span></span>|<span data-ttu-id="c9b60-117">String</span><span class="sxs-lookup"><span data-stu-id="c9b60-117">String</span></span>|<span data-ttu-id="c9b60-118">城市。</span><span class="sxs-lookup"><span data-stu-id="c9b60-118">The city.</span></span>|
|<span data-ttu-id="c9b60-119">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="c9b60-119">countryOrRegion</span></span>|<span data-ttu-id="c9b60-120">字符串</span><span class="sxs-lookup"><span data-stu-id="c9b60-120">String</span></span>|<span data-ttu-id="c9b60-p102">国家或地区。它是任意格式的字符串值，例如“United States”。</span><span class="sxs-lookup"><span data-stu-id="c9b60-p102">The country or region. It's a free-format string value, for example, "United States".</span></span>|
|<span data-ttu-id="c9b60-123">postalCode</span><span class="sxs-lookup"><span data-stu-id="c9b60-123">postalCode</span></span>|<span data-ttu-id="c9b60-124">String</span><span class="sxs-lookup"><span data-stu-id="c9b60-124">String</span></span>|<span data-ttu-id="c9b60-125">邮政编码。</span><span class="sxs-lookup"><span data-stu-id="c9b60-125">The postal code.</span></span>|
|<span data-ttu-id="c9b60-126">state</span><span class="sxs-lookup"><span data-stu-id="c9b60-126">state</span></span>|<span data-ttu-id="c9b60-127">String</span><span class="sxs-lookup"><span data-stu-id="c9b60-127">String</span></span>|<span data-ttu-id="c9b60-128">省/市/自治区。</span><span class="sxs-lookup"><span data-stu-id="c9b60-128">The state.</span></span>|
|<span data-ttu-id="c9b60-129">street</span><span class="sxs-lookup"><span data-stu-id="c9b60-129">street</span></span>|<span data-ttu-id="c9b60-130">String</span><span class="sxs-lookup"><span data-stu-id="c9b60-130">String</span></span>|<span data-ttu-id="c9b60-131">街道。</span><span class="sxs-lookup"><span data-stu-id="c9b60-131">The street.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c9b60-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c9b60-132">JSON representation</span></span>

<span data-ttu-id="c9b60-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c9b60-133">Here is a JSON representation of the resource</span></span>

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

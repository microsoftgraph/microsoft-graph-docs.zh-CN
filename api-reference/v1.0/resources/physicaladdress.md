---
title: physicalAddress 资源类型
description: 表示资源（例如联系人或事件）的街道地址。
ms.openlocfilehash: eb2c1ea6a73d7f6eb5d3d43b877f50dc39a2b17e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27009503"
---
# <a name="physicaladdress-resource-type"></a><span data-ttu-id="d2c8c-103">physicalAddress 资源类型</span><span class="sxs-lookup"><span data-stu-id="d2c8c-103">physicalAddress resource type</span></span>

<span data-ttu-id="d2c8c-104">表示资源（例如联系人或事件）的街道地址。</span><span class="sxs-lookup"><span data-stu-id="d2c8c-104">Represents the street address of a resource such as a contact or event.</span></span>


## <a name="properties"></a><span data-ttu-id="d2c8c-105">属性</span><span class="sxs-lookup"><span data-stu-id="d2c8c-105">Properties</span></span>
| <span data-ttu-id="d2c8c-106">属性</span><span class="sxs-lookup"><span data-stu-id="d2c8c-106">Property</span></span>     | <span data-ttu-id="d2c8c-107">类型</span><span class="sxs-lookup"><span data-stu-id="d2c8c-107">Type</span></span>   |<span data-ttu-id="d2c8c-108">说明</span><span class="sxs-lookup"><span data-stu-id="d2c8c-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d2c8c-109">city</span><span class="sxs-lookup"><span data-stu-id="d2c8c-109">city</span></span>|<span data-ttu-id="d2c8c-110">String</span><span class="sxs-lookup"><span data-stu-id="d2c8c-110">String</span></span>|<span data-ttu-id="d2c8c-111">城市。</span><span class="sxs-lookup"><span data-stu-id="d2c8c-111">The city.</span></span>|
|<span data-ttu-id="d2c8c-112">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="d2c8c-112">countryOrRegion</span></span>|<span data-ttu-id="d2c8c-113">字符串</span><span class="sxs-lookup"><span data-stu-id="d2c8c-113">String</span></span>|<span data-ttu-id="d2c8c-p101">国家或地区。它是任意格式的字符串值，例如“United States”。</span><span class="sxs-lookup"><span data-stu-id="d2c8c-p101">The country or region. It's a free-format string value, for example, "United States".</span></span>|
|<span data-ttu-id="d2c8c-116">postalCode</span><span class="sxs-lookup"><span data-stu-id="d2c8c-116">postalCode</span></span>|<span data-ttu-id="d2c8c-117">String</span><span class="sxs-lookup"><span data-stu-id="d2c8c-117">String</span></span>|<span data-ttu-id="d2c8c-118">邮政编码。</span><span class="sxs-lookup"><span data-stu-id="d2c8c-118">The postal code.</span></span>|
|<span data-ttu-id="d2c8c-119">state</span><span class="sxs-lookup"><span data-stu-id="d2c8c-119">state</span></span>|<span data-ttu-id="d2c8c-120">String</span><span class="sxs-lookup"><span data-stu-id="d2c8c-120">String</span></span>|<span data-ttu-id="d2c8c-121">省/市/自治区。</span><span class="sxs-lookup"><span data-stu-id="d2c8c-121">The state.</span></span>|
|<span data-ttu-id="d2c8c-122">street</span><span class="sxs-lookup"><span data-stu-id="d2c8c-122">street</span></span>|<span data-ttu-id="d2c8c-123">String</span><span class="sxs-lookup"><span data-stu-id="d2c8c-123">String</span></span>|<span data-ttu-id="d2c8c-124">街道。</span><span class="sxs-lookup"><span data-stu-id="d2c8c-124">The street.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d2c8c-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d2c8c-125">JSON representation</span></span>

<span data-ttu-id="d2c8c-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d2c8c-126">Here is a JSON representation of the resource</span></span>

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

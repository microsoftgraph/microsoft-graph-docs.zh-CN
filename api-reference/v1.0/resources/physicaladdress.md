---
title: physicalAddress 资源类型
description: 表示资源（例如联系人或事件）的街道地址。
localization_priority: Normal
ms.openlocfilehash: 2bbfc3f38d4d353d370b9c8ba859b06cc2e4398b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32462464"
---
# <a name="physicaladdress-resource-type"></a><span data-ttu-id="463c5-103">physicalAddress 资源类型</span><span class="sxs-lookup"><span data-stu-id="463c5-103">physicalAddress resource type</span></span>

<span data-ttu-id="463c5-104">表示资源（例如联系人或事件）的街道地址。</span><span class="sxs-lookup"><span data-stu-id="463c5-104">Represents the street address of a resource such as a contact or event.</span></span>


## <a name="properties"></a><span data-ttu-id="463c5-105">属性</span><span class="sxs-lookup"><span data-stu-id="463c5-105">Properties</span></span>
| <span data-ttu-id="463c5-106">属性</span><span class="sxs-lookup"><span data-stu-id="463c5-106">Property</span></span>     | <span data-ttu-id="463c5-107">类型</span><span class="sxs-lookup"><span data-stu-id="463c5-107">Type</span></span>   |<span data-ttu-id="463c5-108">说明</span><span class="sxs-lookup"><span data-stu-id="463c5-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="463c5-109">city</span><span class="sxs-lookup"><span data-stu-id="463c5-109">city</span></span>|<span data-ttu-id="463c5-110">字符串</span><span class="sxs-lookup"><span data-stu-id="463c5-110">String</span></span>|<span data-ttu-id="463c5-111">城市。</span><span class="sxs-lookup"><span data-stu-id="463c5-111">The city.</span></span>|
|<span data-ttu-id="463c5-112">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="463c5-112">countryOrRegion</span></span>|<span data-ttu-id="463c5-113">字符串</span><span class="sxs-lookup"><span data-stu-id="463c5-113">String</span></span>|<span data-ttu-id="463c5-p101">国家或地区。它是任意格式的字符串值，例如“United States”。</span><span class="sxs-lookup"><span data-stu-id="463c5-p101">The country or region. It's a free-format string value, for example, "United States".</span></span>|
|<span data-ttu-id="463c5-116">postalCode</span><span class="sxs-lookup"><span data-stu-id="463c5-116">postalCode</span></span>|<span data-ttu-id="463c5-117">字符串</span><span class="sxs-lookup"><span data-stu-id="463c5-117">String</span></span>|<span data-ttu-id="463c5-118">邮政编码。</span><span class="sxs-lookup"><span data-stu-id="463c5-118">The postal code.</span></span>|
|<span data-ttu-id="463c5-119">state</span><span class="sxs-lookup"><span data-stu-id="463c5-119">state</span></span>|<span data-ttu-id="463c5-120">String</span><span class="sxs-lookup"><span data-stu-id="463c5-120">String</span></span>|<span data-ttu-id="463c5-121">省/市/自治区。</span><span class="sxs-lookup"><span data-stu-id="463c5-121">The state.</span></span>|
|<span data-ttu-id="463c5-122">street</span><span class="sxs-lookup"><span data-stu-id="463c5-122">street</span></span>|<span data-ttu-id="463c5-123">String</span><span class="sxs-lookup"><span data-stu-id="463c5-123">String</span></span>|<span data-ttu-id="463c5-124">街道。</span><span class="sxs-lookup"><span data-stu-id="463c5-124">The street.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="463c5-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="463c5-125">JSON representation</span></span>

<span data-ttu-id="463c5-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="463c5-126">Here is a JSON representation of the resource</span></span>

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

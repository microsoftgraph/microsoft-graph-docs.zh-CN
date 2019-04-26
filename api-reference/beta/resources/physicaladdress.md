---
title: physicalAddress 资源类型
description: 表示资源（例如联系人或事件）的街道地址。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: eb7bf1ee21a40517704f20176f5fbcf9ea2b276a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32573779"
---
# <a name="physicaladdress-resource-type"></a><span data-ttu-id="3e98c-103">physicalAddress 资源类型</span><span class="sxs-lookup"><span data-stu-id="3e98c-103">physicalAddress resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3e98c-104">表示资源（例如联系人或事件）的街道地址。</span><span class="sxs-lookup"><span data-stu-id="3e98c-104">Represents the street address of a resource such as a contact or event.</span></span>


## <a name="properties"></a><span data-ttu-id="3e98c-105">属性</span><span class="sxs-lookup"><span data-stu-id="3e98c-105">Properties</span></span>
| <span data-ttu-id="3e98c-106">属性</span><span class="sxs-lookup"><span data-stu-id="3e98c-106">Property</span></span>     | <span data-ttu-id="3e98c-107">类型</span><span class="sxs-lookup"><span data-stu-id="3e98c-107">Type</span></span>   |<span data-ttu-id="3e98c-108">说明</span><span class="sxs-lookup"><span data-stu-id="3e98c-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3e98c-109">city</span><span class="sxs-lookup"><span data-stu-id="3e98c-109">city</span></span>|<span data-ttu-id="3e98c-110">String</span><span class="sxs-lookup"><span data-stu-id="3e98c-110">String</span></span>|<span data-ttu-id="3e98c-111">城市。</span><span class="sxs-lookup"><span data-stu-id="3e98c-111">The city.</span></span>|
|<span data-ttu-id="3e98c-112">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="3e98c-112">countryOrRegion</span></span>|<span data-ttu-id="3e98c-113">字符串</span><span class="sxs-lookup"><span data-stu-id="3e98c-113">String</span></span>|<span data-ttu-id="3e98c-p101">国家或地区。它是任意格式的字符串值，例如“United States”。</span><span class="sxs-lookup"><span data-stu-id="3e98c-p101">The country or region. It's a free-format string value, for example, "United States".</span></span>|
|<span data-ttu-id="3e98c-116">postalCode</span><span class="sxs-lookup"><span data-stu-id="3e98c-116">postalCode</span></span>|<span data-ttu-id="3e98c-117">String</span><span class="sxs-lookup"><span data-stu-id="3e98c-117">String</span></span>|<span data-ttu-id="3e98c-118">邮政编码。</span><span class="sxs-lookup"><span data-stu-id="3e98c-118">The postal code.</span></span>|
|<span data-ttu-id="3e98c-119">postOfficeBox</span><span class="sxs-lookup"><span data-stu-id="3e98c-119">postOfficeBox</span></span>|<span data-ttu-id="3e98c-120">String</span><span class="sxs-lookup"><span data-stu-id="3e98c-120">String</span></span>|<span data-ttu-id="3e98c-121">邮局编号。</span><span class="sxs-lookup"><span data-stu-id="3e98c-121">The post office box number.</span></span>|
|<span data-ttu-id="3e98c-122">state</span><span class="sxs-lookup"><span data-stu-id="3e98c-122">state</span></span>|<span data-ttu-id="3e98c-123">String</span><span class="sxs-lookup"><span data-stu-id="3e98c-123">String</span></span>|<span data-ttu-id="3e98c-124">省/市/自治区。</span><span class="sxs-lookup"><span data-stu-id="3e98c-124">The state.</span></span>|
|<span data-ttu-id="3e98c-125">street</span><span class="sxs-lookup"><span data-stu-id="3e98c-125">street</span></span>|<span data-ttu-id="3e98c-126">String</span><span class="sxs-lookup"><span data-stu-id="3e98c-126">String</span></span>|<span data-ttu-id="3e98c-127">街道。</span><span class="sxs-lookup"><span data-stu-id="3e98c-127">The street.</span></span>|
|<span data-ttu-id="3e98c-128">type</span><span class="sxs-lookup"><span data-stu-id="3e98c-128">type</span></span>|<span data-ttu-id="3e98c-129">: physicaladdresstype</span><span class="sxs-lookup"><span data-stu-id="3e98c-129">physicalAddressType</span></span>|<span data-ttu-id="3e98c-130">地址类型。</span><span class="sxs-lookup"><span data-stu-id="3e98c-130">The type of address.</span></span> <span data-ttu-id="3e98c-131">可取值为：`unknown`、`home`、`business`、`other`。</span><span class="sxs-lookup"><span data-stu-id="3e98c-131">Possible values are: `unknown`, `home`, `business`, `other`.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="3e98c-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3e98c-132">JSON representation</span></span>

<span data-ttu-id="3e98c-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3e98c-133">Here is a JSON representation of the resource</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "physicalAddress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/physicaladdress.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}-->

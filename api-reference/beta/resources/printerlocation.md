---
title: printerLocation 资源类型
description: 表示打印机的物理和分层位置。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: ea54c7b3b572413be515aa728e18ae69f6f10fc3
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/21/2020
ms.locfileid: "42895609"
---
# <a name="printerlocation-resource-type"></a><span data-ttu-id="16dec-103">printerLocation 资源类型</span><span class="sxs-lookup"><span data-stu-id="16dec-103">printerLocation resource type</span></span>

<span data-ttu-id="16dec-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="16dec-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="16dec-105">表示打印机的物理和分层位置。</span><span class="sxs-lookup"><span data-stu-id="16dec-105">Represents the physical and hierarchical location of a printer.</span></span>

## <a name="properties"></a><span data-ttu-id="16dec-106">属性</span><span class="sxs-lookup"><span data-stu-id="16dec-106">Properties</span></span>
| <span data-ttu-id="16dec-107">属性</span><span class="sxs-lookup"><span data-stu-id="16dec-107">Property</span></span>     | <span data-ttu-id="16dec-108">类型</span><span class="sxs-lookup"><span data-stu-id="16dec-108">Type</span></span>        | <span data-ttu-id="16dec-109">说明</span><span class="sxs-lookup"><span data-stu-id="16dec-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="16dec-110">latitude</span><span class="sxs-lookup"><span data-stu-id="16dec-110">latitude</span></span>|<span data-ttu-id="16dec-111">双精度</span><span class="sxs-lookup"><span data-stu-id="16dec-111">Double</span></span>|<span data-ttu-id="16dec-112">打印机所在的纬度。</span><span class="sxs-lookup"><span data-stu-id="16dec-112">The latitude that the printer is located at.</span></span>|
|<span data-ttu-id="16dec-113">longitude</span><span class="sxs-lookup"><span data-stu-id="16dec-113">longitude</span></span>|<span data-ttu-id="16dec-114">Double</span><span class="sxs-lookup"><span data-stu-id="16dec-114">Double</span></span>|<span data-ttu-id="16dec-115">打印机所在的经度。</span><span class="sxs-lookup"><span data-stu-id="16dec-115">The longitude that the printer is located at.</span></span>|
|<span data-ttu-id="16dec-116">altitudeInMeters</span><span class="sxs-lookup"><span data-stu-id="16dec-116">altitudeInMeters</span></span>|<span data-ttu-id="16dec-117">Int32</span><span class="sxs-lookup"><span data-stu-id="16dec-117">Int32</span></span>|<span data-ttu-id="16dec-118">打印机所在的海拔高度（以米为单位）。</span><span class="sxs-lookup"><span data-stu-id="16dec-118">The altitude, in meters, that the printer is located at.</span></span>|
|<span data-ttu-id="16dec-119">streetAddress</span><span class="sxs-lookup"><span data-stu-id="16dec-119">streetAddress</span></span>|<span data-ttu-id="16dec-120">String</span><span class="sxs-lookup"><span data-stu-id="16dec-120">String</span></span>|<span data-ttu-id="16dec-121">打印机所在的街道地址。</span><span class="sxs-lookup"><span data-stu-id="16dec-121">The street address where the printer is located.</span></span>|
|<span data-ttu-id="16dec-122">子</span><span class="sxs-lookup"><span data-stu-id="16dec-122">subUnit</span></span>|<span data-ttu-id="16dec-123">String collection</span><span class="sxs-lookup"><span data-stu-id="16dec-123">String collection</span></span>|<span data-ttu-id="16dec-124">打印机所在的次级单位层次结构。</span><span class="sxs-lookup"><span data-stu-id="16dec-124">The subunit hierarchy where the printer is located.</span></span> <span data-ttu-id="16dec-125">元素应按层次结构顺序排列。</span><span class="sxs-lookup"><span data-stu-id="16dec-125">The elements should be in hierarchical order.</span></span> <span data-ttu-id="16dec-126">例如，如果一个校园分成不同的部分，则层次结构可能如下所示：`["East Wing", "Block A"]`</span><span class="sxs-lookup"><span data-stu-id="16dec-126">For example, if a campus is divided into different sections, the hierarchy might look like this: `["East Wing", "Block A"]`</span></span>
|<span data-ttu-id="16dec-127">城市</span><span class="sxs-lookup"><span data-stu-id="16dec-127">city</span></span>|<span data-ttu-id="16dec-128">String</span><span class="sxs-lookup"><span data-stu-id="16dec-128">String</span></span>|<span data-ttu-id="16dec-129">打印机所在的城市。</span><span class="sxs-lookup"><span data-stu-id="16dec-129">The city that the printer is located in.</span></span>
|<span data-ttu-id="16dec-130">postalCode</span><span class="sxs-lookup"><span data-stu-id="16dec-130">postalCode</span></span>|<span data-ttu-id="16dec-131">String</span><span class="sxs-lookup"><span data-stu-id="16dec-131">String</span></span>|<span data-ttu-id="16dec-132">打印机所在的邮政编码。</span><span class="sxs-lookup"><span data-stu-id="16dec-132">The postal code that the printer is located in.</span></span>
|<span data-ttu-id="16dec-133">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="16dec-133">countryOrRegion</span></span>|<span data-ttu-id="16dec-134">String</span><span class="sxs-lookup"><span data-stu-id="16dec-134">String</span></span>|<span data-ttu-id="16dec-135">打印机所在的国家或地区。</span><span class="sxs-lookup"><span data-stu-id="16dec-135">The country or region that the printer is located in.</span></span>|
|<span data-ttu-id="16dec-136">网站</span><span class="sxs-lookup"><span data-stu-id="16dec-136">site</span></span>|<span data-ttu-id="16dec-137">String</span><span class="sxs-lookup"><span data-stu-id="16dec-137">String</span></span>|<span data-ttu-id="16dec-138">打印机所在的网站。</span><span class="sxs-lookup"><span data-stu-id="16dec-138">The site that the printer is located in.</span></span>
|<span data-ttu-id="16dec-139">幢</span><span class="sxs-lookup"><span data-stu-id="16dec-139">building</span></span>|<span data-ttu-id="16dec-140">String</span><span class="sxs-lookup"><span data-stu-id="16dec-140">String</span></span>|<span data-ttu-id="16dec-141">打印机所在的建筑物。</span><span class="sxs-lookup"><span data-stu-id="16dec-141">The building that the printer is located in.</span></span>
|<span data-ttu-id="16dec-142">floorNumber</span><span class="sxs-lookup"><span data-stu-id="16dec-142">floorNumber</span></span>|<span data-ttu-id="16dec-143">Int32</span><span class="sxs-lookup"><span data-stu-id="16dec-143">Int32</span></span>|<span data-ttu-id="16dec-144">打印机所在的楼层号。</span><span class="sxs-lookup"><span data-stu-id="16dec-144">The floor number that the printer is located on.</span></span>
|<span data-ttu-id="16dec-145">floorDescription</span><span class="sxs-lookup"><span data-stu-id="16dec-145">floorDescription</span></span>|<span data-ttu-id="16dec-146">String</span><span class="sxs-lookup"><span data-stu-id="16dec-146">String</span></span>|<span data-ttu-id="16dec-147">打印机所在楼层的说明。</span><span class="sxs-lookup"><span data-stu-id="16dec-147">The description of the floor that the printer is located on.</span></span>
|<span data-ttu-id="16dec-148">roomNumber</span><span class="sxs-lookup"><span data-stu-id="16dec-148">roomNumber</span></span>|<span data-ttu-id="16dec-149">Int32</span><span class="sxs-lookup"><span data-stu-id="16dec-149">Int32</span></span>|<span data-ttu-id="16dec-150">打印机所在的房间号码。</span><span class="sxs-lookup"><span data-stu-id="16dec-150">The room number that the printer is located in.</span></span>
|<span data-ttu-id="16dec-151">roomDescription</span><span class="sxs-lookup"><span data-stu-id="16dec-151">roomDescription</span></span>|<span data-ttu-id="16dec-152">Int32</span><span class="sxs-lookup"><span data-stu-id="16dec-152">Int32</span></span>|<span data-ttu-id="16dec-153">打印机所在聊天室的说明。</span><span class="sxs-lookup"><span data-stu-id="16dec-153">The description of the room that the printer is located in.</span></span>
|<span data-ttu-id="16dec-154">组织</span><span class="sxs-lookup"><span data-stu-id="16dec-154">organization</span></span>|<span data-ttu-id="16dec-155">String collection</span><span class="sxs-lookup"><span data-stu-id="16dec-155">String collection</span></span>|<span data-ttu-id="16dec-156">打印机所属的组织层次结构。</span><span class="sxs-lookup"><span data-stu-id="16dec-156">The organizational hierarchy that the printer belongs to.</span></span> <span data-ttu-id="16dec-157">元素应按层次结构顺序排列。</span><span class="sxs-lookup"><span data-stu-id="16dec-157">The elements should be in hierarchical order.</span></span>
|<span data-ttu-id="16dec-158">细分</span><span class="sxs-lookup"><span data-stu-id="16dec-158">subdivision</span></span>|<span data-ttu-id="16dec-159">String collection</span><span class="sxs-lookup"><span data-stu-id="16dec-159">String collection</span></span>|<span data-ttu-id="16dec-160">打印机所在的细分。</span><span class="sxs-lookup"><span data-stu-id="16dec-160">The subdivision that the printer is located in.</span></span> <span data-ttu-id="16dec-161">元素应按层次结构顺序排列。</span><span class="sxs-lookup"><span data-stu-id="16dec-161">The elements should be in hierarchical order.</span></span>
|<span data-ttu-id="16dec-162">stateOrProvince</span><span class="sxs-lookup"><span data-stu-id="16dec-162">stateOrProvince</span></span>|<span data-ttu-id="16dec-163">String collection</span><span class="sxs-lookup"><span data-stu-id="16dec-163">String collection</span></span>|<span data-ttu-id="16dec-164">打印机所在的省/市/自治区。</span><span class="sxs-lookup"><span data-stu-id="16dec-164">The state or province that the printer is located in.</span></span>

## <a name="json-representation"></a><span data-ttu-id="16dec-165">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="16dec-165">JSON representation</span></span>

<span data-ttu-id="16dec-166">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="16dec-166">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printerLocation"
}-->

```json
{
    "latitude": 80.1,
    "longitude": -170.1,
    "altitudeInMeters": 123456,
    "streetAddress": "String",
    "subUnit": ["String"],
    "city": "String",
    "postalCode": "String",
    "countryOrRegion": "String",
    "site": "String",
    "building": "String",
    "floorNumber": 123456,
    "floorDescription": "String",
    "roomNumber": 123456,
    "roomDescription": "String",
    "organization": ["String"],
    "subdivision": ["String"],
    "stateOrProvince": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printerLocation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
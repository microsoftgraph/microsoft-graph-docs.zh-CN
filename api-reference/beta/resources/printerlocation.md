---
title: printerLocation 资源类型
description: 表示打印机的物理和分层位置。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: bfb082571ab1c5ddf2b46a06c6e66b9e31e47309
ms.sourcegitcommit: 7902607a1e5a030d46e907d08e16644a47a47006
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/12/2020
ms.locfileid: "49664056"
---
# <a name="printerlocation-resource-type"></a><span data-ttu-id="5daf4-103">printerLocation 资源类型</span><span class="sxs-lookup"><span data-stu-id="5daf4-103">printerLocation resource type</span></span>

<span data-ttu-id="5daf4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5daf4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5daf4-105">表示打印机的物理和分层位置。</span><span class="sxs-lookup"><span data-stu-id="5daf4-105">Represents the physical and hierarchical location of a printer.</span></span>

## <a name="properties"></a><span data-ttu-id="5daf4-106">属性</span><span class="sxs-lookup"><span data-stu-id="5daf4-106">Properties</span></span>
| <span data-ttu-id="5daf4-107">属性</span><span class="sxs-lookup"><span data-stu-id="5daf4-107">Property</span></span>     | <span data-ttu-id="5daf4-108">类型</span><span class="sxs-lookup"><span data-stu-id="5daf4-108">Type</span></span>        | <span data-ttu-id="5daf4-109">说明</span><span class="sxs-lookup"><span data-stu-id="5daf4-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="5daf4-110">latitude</span><span class="sxs-lookup"><span data-stu-id="5daf4-110">latitude</span></span>|<span data-ttu-id="5daf4-111">Double</span><span class="sxs-lookup"><span data-stu-id="5daf4-111">Double</span></span>|<span data-ttu-id="5daf4-112">打印机所在的纬度。</span><span class="sxs-lookup"><span data-stu-id="5daf4-112">The latitude that the printer is located at.</span></span>|
|<span data-ttu-id="5daf4-113">longitude</span><span class="sxs-lookup"><span data-stu-id="5daf4-113">longitude</span></span>|<span data-ttu-id="5daf4-114">Double</span><span class="sxs-lookup"><span data-stu-id="5daf4-114">Double</span></span>|<span data-ttu-id="5daf4-115">打印机所在的经度。</span><span class="sxs-lookup"><span data-stu-id="5daf4-115">The longitude that the printer is located at.</span></span>|
|<span data-ttu-id="5daf4-116">altitudeInMeters</span><span class="sxs-lookup"><span data-stu-id="5daf4-116">altitudeInMeters</span></span>|<span data-ttu-id="5daf4-117">Int32</span><span class="sxs-lookup"><span data-stu-id="5daf4-117">Int32</span></span>|<span data-ttu-id="5daf4-118">打印机所在的高度（以米为单位）。</span><span class="sxs-lookup"><span data-stu-id="5daf4-118">The altitude, in meters, that the printer is located at.</span></span>|
|<span data-ttu-id="5daf4-119">streetAddress</span><span class="sxs-lookup"><span data-stu-id="5daf4-119">streetAddress</span></span>|<span data-ttu-id="5daf4-120">String</span><span class="sxs-lookup"><span data-stu-id="5daf4-120">String</span></span>|<span data-ttu-id="5daf4-121">打印机所在的街道地址。</span><span class="sxs-lookup"><span data-stu-id="5daf4-121">The street address where the printer is located.</span></span>|
|<span data-ttu-id="5daf4-122">subUnit</span><span class="sxs-lookup"><span data-stu-id="5daf4-122">subUnit</span></span>|<span data-ttu-id="5daf4-123">String collection</span><span class="sxs-lookup"><span data-stu-id="5daf4-123">String collection</span></span>|<span data-ttu-id="5daf4-124">打印机所在的次级层次结构。</span><span class="sxs-lookup"><span data-stu-id="5daf4-124">The subunit hierarchy where the printer is located.</span></span> <span data-ttu-id="5daf4-125">元素应按层次结构顺序进行。</span><span class="sxs-lookup"><span data-stu-id="5daf4-125">The elements should be in hierarchical order.</span></span> <span data-ttu-id="5daf4-126">例如，如果校园分为不同的部分，则层次结构可能如下所示： `["East Wing", "Block A"]`</span><span class="sxs-lookup"><span data-stu-id="5daf4-126">For example, if a campus is divided into different sections, the hierarchy might look like this: `["East Wing", "Block A"]`</span></span>|
|<span data-ttu-id="5daf4-127">城市</span><span class="sxs-lookup"><span data-stu-id="5daf4-127">city</span></span>|<span data-ttu-id="5daf4-128">String</span><span class="sxs-lookup"><span data-stu-id="5daf4-128">String</span></span>|<span data-ttu-id="5daf4-129">打印机所在的城市。</span><span class="sxs-lookup"><span data-stu-id="5daf4-129">The city that the printer is located in.</span></span>|
|<span data-ttu-id="5daf4-130">postalCode</span><span class="sxs-lookup"><span data-stu-id="5daf4-130">postalCode</span></span>|<span data-ttu-id="5daf4-131">String</span><span class="sxs-lookup"><span data-stu-id="5daf4-131">String</span></span>|<span data-ttu-id="5daf4-132">打印机所在的邮政编码。</span><span class="sxs-lookup"><span data-stu-id="5daf4-132">The postal code that the printer is located in.</span></span>|
|<span data-ttu-id="5daf4-133">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="5daf4-133">countryOrRegion</span></span>|<span data-ttu-id="5daf4-134">String</span><span class="sxs-lookup"><span data-stu-id="5daf4-134">String</span></span>|<span data-ttu-id="5daf4-135">打印机所在的国家/地区。</span><span class="sxs-lookup"><span data-stu-id="5daf4-135">The country or region that the printer is located in.</span></span>|
|<span data-ttu-id="5daf4-136">网站</span><span class="sxs-lookup"><span data-stu-id="5daf4-136">site</span></span>|<span data-ttu-id="5daf4-137">String</span><span class="sxs-lookup"><span data-stu-id="5daf4-137">String</span></span>|<span data-ttu-id="5daf4-138">打印机所在的站点。</span><span class="sxs-lookup"><span data-stu-id="5daf4-138">The site that the printer is located in.</span></span>|
|<span data-ttu-id="5daf4-139">building</span><span class="sxs-lookup"><span data-stu-id="5daf4-139">building</span></span>|<span data-ttu-id="5daf4-140">String</span><span class="sxs-lookup"><span data-stu-id="5daf4-140">String</span></span>|<span data-ttu-id="5daf4-141">打印机所在的大楼。</span><span class="sxs-lookup"><span data-stu-id="5daf4-141">The building that the printer is located in.</span></span>|
|<span data-ttu-id="5daf4-142">floor</span><span class="sxs-lookup"><span data-stu-id="5daf4-142">floor</span></span>|<span data-ttu-id="5daf4-143">String</span><span class="sxs-lookup"><span data-stu-id="5daf4-143">String</span></span>|<span data-ttu-id="5daf4-144">打印机所在的楼层。</span><span class="sxs-lookup"><span data-stu-id="5daf4-144">The floor that the printer is located on.</span></span> <span data-ttu-id="5daf4-145">目前仅支持数值。</span><span class="sxs-lookup"><span data-stu-id="5daf4-145">Only numerical values are supported right now.</span></span>|
|<span data-ttu-id="5daf4-146">floorDescription</span><span class="sxs-lookup"><span data-stu-id="5daf4-146">floorDescription</span></span>|<span data-ttu-id="5daf4-147">String</span><span class="sxs-lookup"><span data-stu-id="5daf4-147">String</span></span>|<span data-ttu-id="5daf4-148">打印机所在的楼层的说明。</span><span class="sxs-lookup"><span data-stu-id="5daf4-148">The description of the floor that the printer is located on.</span></span>|
|<span data-ttu-id="5daf4-149">roomName</span><span class="sxs-lookup"><span data-stu-id="5daf4-149">roomName</span></span>|<span data-ttu-id="5daf4-150">String</span><span class="sxs-lookup"><span data-stu-id="5daf4-150">String</span></span>|<span data-ttu-id="5daf4-151">打印机所在的房间。</span><span class="sxs-lookup"><span data-stu-id="5daf4-151">The room that the printer is located in.</span></span> <span data-ttu-id="5daf4-152">目前仅支持数值。</span><span class="sxs-lookup"><span data-stu-id="5daf4-152">Only numerical values are supported right now.</span></span>|
|<span data-ttu-id="5daf4-153">roomDescription</span><span class="sxs-lookup"><span data-stu-id="5daf4-153">roomDescription</span></span>|<span data-ttu-id="5daf4-154">String</span><span class="sxs-lookup"><span data-stu-id="5daf4-154">String</span></span>|<span data-ttu-id="5daf4-155">打印机所在的房间的说明。</span><span class="sxs-lookup"><span data-stu-id="5daf4-155">The description of the room that the printer is located in.</span></span>|
|<span data-ttu-id="5daf4-156">组织</span><span class="sxs-lookup"><span data-stu-id="5daf4-156">organization</span></span>|<span data-ttu-id="5daf4-157">String collection</span><span class="sxs-lookup"><span data-stu-id="5daf4-157">String collection</span></span>|<span data-ttu-id="5daf4-158">打印机所属的组织层次结构。</span><span class="sxs-lookup"><span data-stu-id="5daf4-158">The organizational hierarchy that the printer belongs to.</span></span> <span data-ttu-id="5daf4-159">元素应按层次结构顺序进行。</span><span class="sxs-lookup"><span data-stu-id="5daf4-159">The elements should be in hierarchical order.</span></span>|
|<span data-ttu-id="5daf4-160">subdivision</span><span class="sxs-lookup"><span data-stu-id="5daf4-160">subdivision</span></span>|<span data-ttu-id="5daf4-161">String collection</span><span class="sxs-lookup"><span data-stu-id="5daf4-161">String collection</span></span>|<span data-ttu-id="5daf4-162">打印机所在的细分。</span><span class="sxs-lookup"><span data-stu-id="5daf4-162">The subdivision that the printer is located in.</span></span> <span data-ttu-id="5daf4-163">元素应按层次结构顺序进行。</span><span class="sxs-lookup"><span data-stu-id="5daf4-163">The elements should be in hierarchical order.</span></span>|
|<span data-ttu-id="5daf4-164">stateOrProvince</span><span class="sxs-lookup"><span data-stu-id="5daf4-164">stateOrProvince</span></span>|<span data-ttu-id="5daf4-165">String</span><span class="sxs-lookup"><span data-stu-id="5daf4-165">String</span></span>|<span data-ttu-id="5daf4-166">打印机所在的州或省。</span><span class="sxs-lookup"><span data-stu-id="5daf4-166">The state or province that the printer is located in.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5daf4-167">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5daf4-167">JSON representation</span></span>

<span data-ttu-id="5daf4-168">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5daf4-168">The following is a JSON representation of the resource.</span></span>

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
    "floor": "123456",
    "floorDescription": "String",
    "roomName": "123456",
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


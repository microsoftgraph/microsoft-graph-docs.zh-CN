---
title: printerLocation 资源类型
description: 表示打印机的物理和分层位置。
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: f357ab3b33182ac6ffb2f8ae705a359a0e955eed
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516957"
---
# <a name="printerlocation-resource-type"></a><span data-ttu-id="d3b1e-103">printerLocation 资源类型</span><span class="sxs-lookup"><span data-stu-id="d3b1e-103">printerLocation resource type</span></span>

<span data-ttu-id="d3b1e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d3b1e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="d3b1e-105">表示打印机的物理和分层位置。</span><span class="sxs-lookup"><span data-stu-id="d3b1e-105">Represents the physical and hierarchical location of a printer.</span></span>

## <a name="properties"></a><span data-ttu-id="d3b1e-106">属性</span><span class="sxs-lookup"><span data-stu-id="d3b1e-106">Properties</span></span>
|<span data-ttu-id="d3b1e-107">属性</span><span class="sxs-lookup"><span data-stu-id="d3b1e-107">Property</span></span>|<span data-ttu-id="d3b1e-108">类型</span><span class="sxs-lookup"><span data-stu-id="d3b1e-108">Type</span></span>|<span data-ttu-id="d3b1e-109">Description</span><span class="sxs-lookup"><span data-stu-id="d3b1e-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d3b1e-110">latitude</span><span class="sxs-lookup"><span data-stu-id="d3b1e-110">latitude</span></span>|<span data-ttu-id="d3b1e-111">Double</span><span class="sxs-lookup"><span data-stu-id="d3b1e-111">Double</span></span>|<span data-ttu-id="d3b1e-112">打印机所在的纬度。</span><span class="sxs-lookup"><span data-stu-id="d3b1e-112">The latitude that the printer is located at.</span></span>|
|<span data-ttu-id="d3b1e-113">longitude</span><span class="sxs-lookup"><span data-stu-id="d3b1e-113">longitude</span></span>|<span data-ttu-id="d3b1e-114">Double</span><span class="sxs-lookup"><span data-stu-id="d3b1e-114">Double</span></span>|<span data-ttu-id="d3b1e-115">打印机所在的经度。</span><span class="sxs-lookup"><span data-stu-id="d3b1e-115">The longitude that the printer is located at.</span></span>|
|<span data-ttu-id="d3b1e-116">altitudeInMeters</span><span class="sxs-lookup"><span data-stu-id="d3b1e-116">altitudeInMeters</span></span>|<span data-ttu-id="d3b1e-117">Int32</span><span class="sxs-lookup"><span data-stu-id="d3b1e-117">Int32</span></span>|<span data-ttu-id="d3b1e-118">打印机所在的高度（以米为单位）。</span><span class="sxs-lookup"><span data-stu-id="d3b1e-118">The altitude, in meters, that the printer is located at.</span></span>|
|<span data-ttu-id="d3b1e-119">streetAddress</span><span class="sxs-lookup"><span data-stu-id="d3b1e-119">streetAddress</span></span>|<span data-ttu-id="d3b1e-120">String</span><span class="sxs-lookup"><span data-stu-id="d3b1e-120">String</span></span>|<span data-ttu-id="d3b1e-121">打印机所在的街道地址。</span><span class="sxs-lookup"><span data-stu-id="d3b1e-121">The street address where the printer is located.</span></span>|
|<span data-ttu-id="d3b1e-122">subUnit</span><span class="sxs-lookup"><span data-stu-id="d3b1e-122">subUnit</span></span>|<span data-ttu-id="d3b1e-123">String collection</span><span class="sxs-lookup"><span data-stu-id="d3b1e-123">String collection</span></span>|<span data-ttu-id="d3b1e-124">打印机所在的次级单位层次结构。</span><span class="sxs-lookup"><span data-stu-id="d3b1e-124">The subunit hierarchy where the printer is located.</span></span> <span data-ttu-id="d3b1e-125">元素应按层次结构顺序进行。</span><span class="sxs-lookup"><span data-stu-id="d3b1e-125">The elements should be in hierarchical order.</span></span> <span data-ttu-id="d3b1e-126">例如，如果校园分为不同的部分，则层次结构可能如下所示： `["East Wing", "Block A"]`</span><span class="sxs-lookup"><span data-stu-id="d3b1e-126">For example, if a campus is divided into different sections, the hierarchy might look like this: `["East Wing", "Block A"]`</span></span>|
|<span data-ttu-id="d3b1e-127">城市</span><span class="sxs-lookup"><span data-stu-id="d3b1e-127">city</span></span>|<span data-ttu-id="d3b1e-128">String</span><span class="sxs-lookup"><span data-stu-id="d3b1e-128">String</span></span>|<span data-ttu-id="d3b1e-129">打印机所在的城市。</span><span class="sxs-lookup"><span data-stu-id="d3b1e-129">The city that the printer is located in.</span></span>|
|<span data-ttu-id="d3b1e-130">postalCode</span><span class="sxs-lookup"><span data-stu-id="d3b1e-130">postalCode</span></span>|<span data-ttu-id="d3b1e-131">String</span><span class="sxs-lookup"><span data-stu-id="d3b1e-131">String</span></span>|<span data-ttu-id="d3b1e-132">打印机所在的邮政编码。</span><span class="sxs-lookup"><span data-stu-id="d3b1e-132">The postal code that the printer is located in.</span></span>|
|<span data-ttu-id="d3b1e-133">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="d3b1e-133">countryOrRegion</span></span>|<span data-ttu-id="d3b1e-134">String</span><span class="sxs-lookup"><span data-stu-id="d3b1e-134">String</span></span>|<span data-ttu-id="d3b1e-135">打印机所在的国家/地区。</span><span class="sxs-lookup"><span data-stu-id="d3b1e-135">The country or region that the printer is located in.</span></span>|
|<span data-ttu-id="d3b1e-136">网站</span><span class="sxs-lookup"><span data-stu-id="d3b1e-136">site</span></span>|<span data-ttu-id="d3b1e-137">String</span><span class="sxs-lookup"><span data-stu-id="d3b1e-137">String</span></span>|<span data-ttu-id="d3b1e-138">打印机所在的站点。</span><span class="sxs-lookup"><span data-stu-id="d3b1e-138">The site that the printer is located in.</span></span>|
|<span data-ttu-id="d3b1e-139">building</span><span class="sxs-lookup"><span data-stu-id="d3b1e-139">building</span></span>|<span data-ttu-id="d3b1e-140">String</span><span class="sxs-lookup"><span data-stu-id="d3b1e-140">String</span></span>|<span data-ttu-id="d3b1e-141">打印机所在的建筑物。</span><span class="sxs-lookup"><span data-stu-id="d3b1e-141">The building that the printer is located in.</span></span>|
|<span data-ttu-id="d3b1e-142">floor</span><span class="sxs-lookup"><span data-stu-id="d3b1e-142">floor</span></span>|<span data-ttu-id="d3b1e-143">String</span><span class="sxs-lookup"><span data-stu-id="d3b1e-143">String</span></span>|<span data-ttu-id="d3b1e-144">打印机所在的楼层。</span><span class="sxs-lookup"><span data-stu-id="d3b1e-144">The floor that the printer is located on.</span></span> <span data-ttu-id="d3b1e-145">目前仅支持数值。</span><span class="sxs-lookup"><span data-stu-id="d3b1e-145">Only numerical values are supported right now.</span></span>|
|<span data-ttu-id="d3b1e-146">floorDescription</span><span class="sxs-lookup"><span data-stu-id="d3b1e-146">floorDescription</span></span>|<span data-ttu-id="d3b1e-147">String</span><span class="sxs-lookup"><span data-stu-id="d3b1e-147">String</span></span>|<span data-ttu-id="d3b1e-148">打印机所在的楼层的说明。</span><span class="sxs-lookup"><span data-stu-id="d3b1e-148">The description of the floor that the printer is located on.</span></span>|
|<span data-ttu-id="d3b1e-149">roomName</span><span class="sxs-lookup"><span data-stu-id="d3b1e-149">roomName</span></span>|<span data-ttu-id="d3b1e-150">String</span><span class="sxs-lookup"><span data-stu-id="d3b1e-150">String</span></span>|<span data-ttu-id="d3b1e-151">打印机所在的房间。</span><span class="sxs-lookup"><span data-stu-id="d3b1e-151">The room that the printer is located in.</span></span> <span data-ttu-id="d3b1e-152">目前仅支持数值。</span><span class="sxs-lookup"><span data-stu-id="d3b1e-152">Only numerical values are supported right now.</span></span>|
|<span data-ttu-id="d3b1e-153">roomDescription</span><span class="sxs-lookup"><span data-stu-id="d3b1e-153">roomDescription</span></span>|<span data-ttu-id="d3b1e-154">String</span><span class="sxs-lookup"><span data-stu-id="d3b1e-154">String</span></span>|<span data-ttu-id="d3b1e-155">打印机所在的房间的说明。</span><span class="sxs-lookup"><span data-stu-id="d3b1e-155">The description of the room that the printer is located in.</span></span>|
|<span data-ttu-id="d3b1e-156">组织</span><span class="sxs-lookup"><span data-stu-id="d3b1e-156">organization</span></span>|<span data-ttu-id="d3b1e-157">String collection</span><span class="sxs-lookup"><span data-stu-id="d3b1e-157">String collection</span></span>|<span data-ttu-id="d3b1e-158">打印机所属的组织层次结构。</span><span class="sxs-lookup"><span data-stu-id="d3b1e-158">The organizational hierarchy that the printer belongs to.</span></span> <span data-ttu-id="d3b1e-159">元素应按层次结构顺序进行。</span><span class="sxs-lookup"><span data-stu-id="d3b1e-159">The elements should be in hierarchical order.</span></span>|
|<span data-ttu-id="d3b1e-160">subdivision</span><span class="sxs-lookup"><span data-stu-id="d3b1e-160">subdivision</span></span>|<span data-ttu-id="d3b1e-161">String collection</span><span class="sxs-lookup"><span data-stu-id="d3b1e-161">String collection</span></span>|<span data-ttu-id="d3b1e-162">打印机所在的细分。</span><span class="sxs-lookup"><span data-stu-id="d3b1e-162">The subdivision that the printer is located in.</span></span> <span data-ttu-id="d3b1e-163">元素应按层次结构顺序进行。</span><span class="sxs-lookup"><span data-stu-id="d3b1e-163">The elements should be in hierarchical order.</span></span>|
|<span data-ttu-id="d3b1e-164">stateOrProvince</span><span class="sxs-lookup"><span data-stu-id="d3b1e-164">stateOrProvince</span></span>|<span data-ttu-id="d3b1e-165">String</span><span class="sxs-lookup"><span data-stu-id="d3b1e-165">String</span></span>|<span data-ttu-id="d3b1e-166">打印机所在的州或省。</span><span class="sxs-lookup"><span data-stu-id="d3b1e-166">The state or province that the printer is located in.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d3b1e-167">关系</span><span class="sxs-lookup"><span data-stu-id="d3b1e-167">Relationships</span></span>
<span data-ttu-id="d3b1e-168">无。</span><span class="sxs-lookup"><span data-stu-id="d3b1e-168">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d3b1e-169">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d3b1e-169">JSON representation</span></span>
<span data-ttu-id="d3b1e-170">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d3b1e-170">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.printerLocation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printerLocation",
  "latitude": "Double",
  "longitude": "Double",
  "altitudeInMeters": "Integer",
  "streetAddress": "String",
  "subunit": [
    "String"
  ],
  "city": "String",
  "postalCode": "String",
  "countryOrRegion": "String",
  "site": "String",
  "building": "String",
  "floor": "String",
  "floorDescription": "String",
  "roomName": "String",
  "roomDescription": "String",
  "organization": [
    "String"
  ],
  "subdivision": [
    "String"
  ],
  "stateOrProvince": "String"
}
```


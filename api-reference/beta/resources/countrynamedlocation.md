---
title: countryNamedLocation 资源类型
description: 表示由国家和地区定义的、名为 "位置" 的 Azure Active Directory。 "已命名位置" 是自定义规则，用于定义随后可在条件访问策略中使用的网络位置。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 7cb413aab72abe401152b67b985f023350f80f30
ms.sourcegitcommit: d189830649794365464e37539e02239f883011da
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/24/2019
ms.locfileid: "37653669"
---
# <a name="countrynamedlocation-resource-type"></a><span data-ttu-id="8aa8c-104">countryNamedLocation 资源类型</span><span class="sxs-lookup"><span data-stu-id="8aa8c-104">countryNamedLocation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8aa8c-105">表示由国家和地区定义的、名为 "位置" 的 Azure Active Directory。</span><span class="sxs-lookup"><span data-stu-id="8aa8c-105">Represents an Azure Active Directory named location defined by countries and regions.</span></span> <span data-ttu-id="8aa8c-106">"已命名位置" 是自定义规则，用于定义随后可在条件访问策略中使用的网络位置。</span><span class="sxs-lookup"><span data-stu-id="8aa8c-106">Named locations are custom rules that define network locations which can then be used in a Conditional Access policy.</span></span>

<span data-ttu-id="8aa8c-107">继承自[namedLocation](../resources/namedLocation.md)</span><span class="sxs-lookup"><span data-stu-id="8aa8c-107">Inherits from [namedLocation](../resources/namedLocation.md)</span></span>

## <a name="methods"></a><span data-ttu-id="8aa8c-108">方法</span><span class="sxs-lookup"><span data-stu-id="8aa8c-108">Methods</span></span>

| <span data-ttu-id="8aa8c-109">方法</span><span class="sxs-lookup"><span data-stu-id="8aa8c-109">Method</span></span>       | <span data-ttu-id="8aa8c-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="8aa8c-110">Return Type</span></span> | <span data-ttu-id="8aa8c-111">说明</span><span class="sxs-lookup"><span data-stu-id="8aa8c-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="8aa8c-112">列出 countryNamedLocations</span><span class="sxs-lookup"><span data-stu-id="8aa8c-112">List countryNamedLocations</span></span>](../api/conditionalaccessroot-list-namedlocations.md) | <span data-ttu-id="8aa8c-113">[countryNamedLocation](countryNamedLocation.md)集合</span><span class="sxs-lookup"><span data-stu-id="8aa8c-113">[countryNamedLocation](countryNamedLocation.md) collection</span></span> | <span data-ttu-id="8aa8c-114">获取组织中的所有**countryNamedLocation**对象。</span><span class="sxs-lookup"><span data-stu-id="8aa8c-114">Get all the **countryNamedLocation** objects in the organization.</span></span> |
| [<span data-ttu-id="8aa8c-115">创建 countryNamedLocation</span><span class="sxs-lookup"><span data-stu-id="8aa8c-115">Create countryNamedLocation</span></span>](../api/conditionalaccessroot-post-namedlocations.md) | [<span data-ttu-id="8aa8c-116">countryNamedLocation</span><span class="sxs-lookup"><span data-stu-id="8aa8c-116">countryNamedLocation</span></span>](countryNamedLocation.md) | <span data-ttu-id="8aa8c-117">创建新的**countryNamedLocation**对象。</span><span class="sxs-lookup"><span data-stu-id="8aa8c-117">Create a new **countryNamedLocation** object.</span></span> |
| [<span data-ttu-id="8aa8c-118">获取 countryNamedLocation</span><span class="sxs-lookup"><span data-stu-id="8aa8c-118">Get countryNamedLocation</span></span>](../api/countrynamedlocation-get.md) | [<span data-ttu-id="8aa8c-119">countryNamedLocation</span><span class="sxs-lookup"><span data-stu-id="8aa8c-119">countryNamedLocation</span></span>](countrynamedlocation.md) | <span data-ttu-id="8aa8c-120">读取**countryNamedLocation**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="8aa8c-120">Read the properties and relationships of a **countryNamedLocation** object.</span></span> |
| [<span data-ttu-id="8aa8c-121">更新 countryNamedLocation</span><span class="sxs-lookup"><span data-stu-id="8aa8c-121">Update countryNamedLocation</span></span>](../api/countrynamedlocation-update.md) | [<span data-ttu-id="8aa8c-122">countryNamedLocation</span><span class="sxs-lookup"><span data-stu-id="8aa8c-122">countryNamedLocation</span></span>](countrynamedlocation.md) | <span data-ttu-id="8aa8c-123">更新**countryNamedLocation**对象。</span><span class="sxs-lookup"><span data-stu-id="8aa8c-123">Update a **countryNamedLocation** object.</span></span> |
| [<span data-ttu-id="8aa8c-124">删除 countryNamedLocation</span><span class="sxs-lookup"><span data-stu-id="8aa8c-124">Delete countryNamedLocation</span></span>](../api/countrynamedlocation-delete.md) | <span data-ttu-id="8aa8c-125">无</span><span class="sxs-lookup"><span data-stu-id="8aa8c-125">None</span></span> | <span data-ttu-id="8aa8c-126">删除**countryNamedLocation**对象。</span><span class="sxs-lookup"><span data-stu-id="8aa8c-126">Delete a **countryNamedLocation** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="8aa8c-127">属性</span><span class="sxs-lookup"><span data-stu-id="8aa8c-127">Properties</span></span>

| <span data-ttu-id="8aa8c-128">属性</span><span class="sxs-lookup"><span data-stu-id="8aa8c-128">Property</span></span>     | <span data-ttu-id="8aa8c-129">类型</span><span class="sxs-lookup"><span data-stu-id="8aa8c-129">Type</span></span>        | <span data-ttu-id="8aa8c-130">说明</span><span class="sxs-lookup"><span data-stu-id="8aa8c-130">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8aa8c-131">countriesAndRegions</span><span class="sxs-lookup"><span data-stu-id="8aa8c-131">countriesAndRegions</span></span>|<span data-ttu-id="8aa8c-132">String collection</span><span class="sxs-lookup"><span data-stu-id="8aa8c-132">String collection</span></span>|<span data-ttu-id="8aa8c-133">由 ISO 3166-2 指定的两个字母格式的国家/地区和/或地区列表。</span><span class="sxs-lookup"><span data-stu-id="8aa8c-133">List of countries and/or regions in two-letter format specified by ISO 3166-2.</span></span>|
|<span data-ttu-id="8aa8c-134">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8aa8c-134">createdDateTime</span></span>|<span data-ttu-id="8aa8c-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8aa8c-135">DateTimeOffset</span></span>|<span data-ttu-id="8aa8c-136">时间戳类型表示使用 ISO 8601 格式的位置的创建日期和时间，并且始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="8aa8c-136">The Timestamp type represents creation date and time of the location using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="8aa8c-137">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="8aa8c-137">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="8aa8c-138">只读。</span><span class="sxs-lookup"><span data-stu-id="8aa8c-138">Read-only.</span></span> <span data-ttu-id="8aa8c-139">继承自[namedLocation](../resources/namedLocation.md)。</span><span class="sxs-lookup"><span data-stu-id="8aa8c-139">Inherited from [namedLocation](../resources/namedLocation.md).</span></span>|
|<span data-ttu-id="8aa8c-140">displayName</span><span class="sxs-lookup"><span data-stu-id="8aa8c-140">displayName</span></span>|<span data-ttu-id="8aa8c-141">String</span><span class="sxs-lookup"><span data-stu-id="8aa8c-141">String</span></span>|<span data-ttu-id="8aa8c-142">位置的人可读名称。</span><span class="sxs-lookup"><span data-stu-id="8aa8c-142">Human-readable name of the location.</span></span> <span data-ttu-id="8aa8c-143">继承自[namedLocation](../resources/namedLocation.md)。</span><span class="sxs-lookup"><span data-stu-id="8aa8c-143">Inherited from [namedLocation](../resources/namedLocation.md).</span></span>|
|<span data-ttu-id="8aa8c-144">id</span><span class="sxs-lookup"><span data-stu-id="8aa8c-144">id</span></span>|<span data-ttu-id="8aa8c-145">String</span><span class="sxs-lookup"><span data-stu-id="8aa8c-145">String</span></span>|<span data-ttu-id="8aa8c-146">NamedLocation 对象的标识符。</span><span class="sxs-lookup"><span data-stu-id="8aa8c-146">Identifier of a namedLocation object.</span></span> <span data-ttu-id="8aa8c-147">只读。</span><span class="sxs-lookup"><span data-stu-id="8aa8c-147">Read-only.</span></span> <span data-ttu-id="8aa8c-148">继承自[namedLocation](../resources/namedLocation.md)。</span><span class="sxs-lookup"><span data-stu-id="8aa8c-148">Inherited from [namedLocation](../resources/namedLocation.md).</span></span>|
|<span data-ttu-id="8aa8c-149">includeUnknownCountriesAndRegions</span><span class="sxs-lookup"><span data-stu-id="8aa8c-149">includeUnknownCountriesAndRegions</span></span>|<span data-ttu-id="8aa8c-150">Boolean</span><span class="sxs-lookup"><span data-stu-id="8aa8c-150">Boolean</span></span>|<span data-ttu-id="8aa8c-151">如此如果未映射到国家或地区的 IP 地址应包含在指定的位置。</span><span class="sxs-lookup"><span data-stu-id="8aa8c-151">True if IP addresses that don't map to a country or region should be included in the named location.</span></span>|
|<span data-ttu-id="8aa8c-152">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8aa8c-152">modifiedDateTime</span></span>|<span data-ttu-id="8aa8c-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8aa8c-153">DateTimeOffset</span></span>|<span data-ttu-id="8aa8c-154">时间戳类型表示上次修改的位置使用 ISO 8601 格式的日期和时间，并且始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="8aa8c-154">The Timestamp type represents last modified date and time of the location using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="8aa8c-155">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="8aa8c-155">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="8aa8c-156">只读。</span><span class="sxs-lookup"><span data-stu-id="8aa8c-156">Read-only.</span></span> <span data-ttu-id="8aa8c-157">继承自[namedLocation](../resources/namedLocation.md)。</span><span class="sxs-lookup"><span data-stu-id="8aa8c-157">Inherited from [namedLocation](../resources/namedLocation.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="8aa8c-158">关系</span><span class="sxs-lookup"><span data-stu-id="8aa8c-158">Relationships</span></span>

<span data-ttu-id="8aa8c-159">无。</span><span class="sxs-lookup"><span data-stu-id="8aa8c-159">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8aa8c-160">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8aa8c-160">JSON representation</span></span>

<span data-ttu-id="8aa8c-161">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8aa8c-161">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.countryNamedLocation",
  "baseType": ""
}-->

```json
{
  "countriesAndRegions": ["String"],
  "createdDateTime": "String (timestamp)",
  "displayName": "String",
  "id": "String (identifier)",
  "includeUnknownCountriesAndRegions": true,
  "modifiedDateTime": "String (timestamp)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "countryNamedLocation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

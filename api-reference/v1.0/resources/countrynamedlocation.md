---
title: countryNamedLocation 资源类型
description: 表示Azure Active Directory地区定义的命名位置。 命名位置是定义网络位置的自定义规则，这些位置随后可在条件访问策略中使用。
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 531942e5026e2fc3d4d9ed3311d9130275d5a853
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53443163"
---
# <a name="countrynamedlocation-resource-type"></a><span data-ttu-id="eb56b-104">countryNamedLocation 资源类型</span><span class="sxs-lookup"><span data-stu-id="eb56b-104">countryNamedLocation resource type</span></span>

<span data-ttu-id="eb56b-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eb56b-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="eb56b-106">表示Azure Active Directory地区定义的命名位置。</span><span class="sxs-lookup"><span data-stu-id="eb56b-106">Represents an Azure Active Directory named location defined by countries and regions.</span></span> <span data-ttu-id="eb56b-107">命名位置是定义网络位置的自定义规则，这些位置随后可在条件访问策略中使用。</span><span class="sxs-lookup"><span data-stu-id="eb56b-107">Named locations are custom rules that define network locations which can then be used in a Conditional Access policy.</span></span>

<span data-ttu-id="eb56b-108">继承自 [namedLocation](../resources/namedLocation.md)</span><span class="sxs-lookup"><span data-stu-id="eb56b-108">Inherits from [namedLocation](../resources/namedLocation.md)</span></span>

## <a name="methods"></a><span data-ttu-id="eb56b-109">方法</span><span class="sxs-lookup"><span data-stu-id="eb56b-109">Methods</span></span>

| <span data-ttu-id="eb56b-110">方法</span><span class="sxs-lookup"><span data-stu-id="eb56b-110">Method</span></span>       | <span data-ttu-id="eb56b-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="eb56b-111">Return Type</span></span> | <span data-ttu-id="eb56b-112">说明</span><span class="sxs-lookup"><span data-stu-id="eb56b-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="eb56b-113">列出 countryNamedLocations</span><span class="sxs-lookup"><span data-stu-id="eb56b-113">List countryNamedLocations</span></span>](../api/conditionalaccessroot-list-namedlocations.md) | <span data-ttu-id="eb56b-114">[countryNamedLocation](countryNamedLocation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="eb56b-114">[countryNamedLocation](countryNamedLocation.md) collection</span></span> | <span data-ttu-id="eb56b-115">获取 **组织的所有 countryNamedLocation** 对象。</span><span class="sxs-lookup"><span data-stu-id="eb56b-115">Get all the **countryNamedLocation** objects in the organization.</span></span> |
| [<span data-ttu-id="eb56b-116">创建 countryNamedLocation</span><span class="sxs-lookup"><span data-stu-id="eb56b-116">Create countryNamedLocation</span></span>](../api/conditionalaccessroot-post-namedlocations.md) | [<span data-ttu-id="eb56b-117">countryNamedLocation</span><span class="sxs-lookup"><span data-stu-id="eb56b-117">countryNamedLocation</span></span>](countryNamedLocation.md) | <span data-ttu-id="eb56b-118">创建新的 **countryNamedLocation** 对象。</span><span class="sxs-lookup"><span data-stu-id="eb56b-118">Create a new **countryNamedLocation** object.</span></span> |
| [<span data-ttu-id="eb56b-119">获取 countryNamedLocation</span><span class="sxs-lookup"><span data-stu-id="eb56b-119">Get countryNamedLocation</span></span>](../api/countrynamedlocation-get.md) | [<span data-ttu-id="eb56b-120">countryNamedLocation</span><span class="sxs-lookup"><span data-stu-id="eb56b-120">countryNamedLocation</span></span>](countrynamedlocation.md) | <span data-ttu-id="eb56b-121">读取 **countryNamedLocation** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="eb56b-121">Read the properties and relationships of a **countryNamedLocation** object.</span></span> |
| [<span data-ttu-id="eb56b-122">更新 countryNamedLocation</span><span class="sxs-lookup"><span data-stu-id="eb56b-122">Update countryNamedLocation</span></span>](../api/countrynamedlocation-update.md) | [<span data-ttu-id="eb56b-123">countryNamedLocation</span><span class="sxs-lookup"><span data-stu-id="eb56b-123">countryNamedLocation</span></span>](countrynamedlocation.md) | <span data-ttu-id="eb56b-124">更新 **countryNamedLocation** 对象。</span><span class="sxs-lookup"><span data-stu-id="eb56b-124">Update a **countryNamedLocation** object.</span></span> |
| [<span data-ttu-id="eb56b-125">删除 countryNamedLocation</span><span class="sxs-lookup"><span data-stu-id="eb56b-125">Delete countryNamedLocation</span></span>](../api/countrynamedlocation-delete.md) | <span data-ttu-id="eb56b-126">无</span><span class="sxs-lookup"><span data-stu-id="eb56b-126">None</span></span> | <span data-ttu-id="eb56b-127">删除 **countryNamedLocation** 对象。</span><span class="sxs-lookup"><span data-stu-id="eb56b-127">Delete a **countryNamedLocation** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="eb56b-128">属性</span><span class="sxs-lookup"><span data-stu-id="eb56b-128">Properties</span></span>

| <span data-ttu-id="eb56b-129">属性</span><span class="sxs-lookup"><span data-stu-id="eb56b-129">Property</span></span>     | <span data-ttu-id="eb56b-130">类型</span><span class="sxs-lookup"><span data-stu-id="eb56b-130">Type</span></span>        | <span data-ttu-id="eb56b-131">说明</span><span class="sxs-lookup"><span data-stu-id="eb56b-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="eb56b-132">countriesAndRegions</span><span class="sxs-lookup"><span data-stu-id="eb56b-132">countriesAndRegions</span></span>|<span data-ttu-id="eb56b-133">字符串集合</span><span class="sxs-lookup"><span data-stu-id="eb56b-133">String collection</span></span>|<span data-ttu-id="eb56b-134">ISO 3166-2 指定的两字母格式的国家/地区列表。</span><span class="sxs-lookup"><span data-stu-id="eb56b-134">List of countries and/or regions in two-letter format specified by ISO 3166-2.</span></span>|
|<span data-ttu-id="eb56b-135">countryLookupMethod</span><span class="sxs-lookup"><span data-stu-id="eb56b-135">countryLookupMethod</span></span>|<span data-ttu-id="eb56b-136">countryLookupMethodType</span><span class="sxs-lookup"><span data-stu-id="eb56b-136">countryLookupMethodType</span></span>|<span data-ttu-id="eb56b-137">确定用于确定用户所在的国家/地区的方法。</span><span class="sxs-lookup"><span data-stu-id="eb56b-137">Determines what method is used to decide which country the user is located in.</span></span> <span data-ttu-id="eb56b-138">可能的值为 `clientIpAddress` 和 `authenticatorAppGps`。</span><span class="sxs-lookup"><span data-stu-id="eb56b-138">Possible values are `clientIpAddress` and `authenticatorAppGps`.</span></span>|
|<span data-ttu-id="eb56b-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="eb56b-139">createdDateTime</span></span>|<span data-ttu-id="eb56b-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eb56b-140">DateTimeOffset</span></span>|<span data-ttu-id="eb56b-141">时间戳类型表示使用 ISO 8601 格式的位置的创建日期和时间，并且始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="eb56b-141">The Timestamp type represents creation date and time of the location using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="eb56b-142">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。</span><span class="sxs-lookup"><span data-stu-id="eb56b-142">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="eb56b-143">只读。</span><span class="sxs-lookup"><span data-stu-id="eb56b-143">Read-only.</span></span> <span data-ttu-id="eb56b-144">继承自 [namedLocation](../resources/namedLocation.md)。</span><span class="sxs-lookup"><span data-stu-id="eb56b-144">Inherited from [namedLocation](../resources/namedLocation.md).</span></span>|
|<span data-ttu-id="eb56b-145">displayName</span><span class="sxs-lookup"><span data-stu-id="eb56b-145">displayName</span></span>|<span data-ttu-id="eb56b-146">String</span><span class="sxs-lookup"><span data-stu-id="eb56b-146">String</span></span>|<span data-ttu-id="eb56b-147">位置的可读名称。</span><span class="sxs-lookup"><span data-stu-id="eb56b-147">Human-readable name of the location.</span></span> <span data-ttu-id="eb56b-148">继承自 [namedLocation](../resources/namedLocation.md)。</span><span class="sxs-lookup"><span data-stu-id="eb56b-148">Inherited from [namedLocation](../resources/namedLocation.md).</span></span>|
|<span data-ttu-id="eb56b-149">id</span><span class="sxs-lookup"><span data-stu-id="eb56b-149">id</span></span>|<span data-ttu-id="eb56b-150">String</span><span class="sxs-lookup"><span data-stu-id="eb56b-150">String</span></span>|<span data-ttu-id="eb56b-151">namedLocation 对象的标识符。</span><span class="sxs-lookup"><span data-stu-id="eb56b-151">Identifier of a namedLocation object.</span></span> <span data-ttu-id="eb56b-152">只读。</span><span class="sxs-lookup"><span data-stu-id="eb56b-152">Read-only.</span></span> <span data-ttu-id="eb56b-153">继承自 [namedLocation](../resources/namedLocation.md)。</span><span class="sxs-lookup"><span data-stu-id="eb56b-153">Inherited from [namedLocation](../resources/namedLocation.md).</span></span>|
|<span data-ttu-id="eb56b-154">includeUnknownCountriesAndRegions</span><span class="sxs-lookup"><span data-stu-id="eb56b-154">includeUnknownCountriesAndRegions</span></span>|<span data-ttu-id="eb56b-155">布尔</span><span class="sxs-lookup"><span data-stu-id="eb56b-155">Boolean</span></span>|<span data-ttu-id="eb56b-156">如此 如果未映射到国家/地区或地区的 IP 地址应包含在命名的位置。</span><span class="sxs-lookup"><span data-stu-id="eb56b-156">True if IP addresses that don't map to a country or region should be included in the named location.</span></span>|
|<span data-ttu-id="eb56b-157">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="eb56b-157">modifiedDateTime</span></span>|<span data-ttu-id="eb56b-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eb56b-158">DateTimeOffset</span></span>|<span data-ttu-id="eb56b-159">时间戳类型表示使用 ISO 8601 格式的位置的上次修改日期和时间，并且始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="eb56b-159">The Timestamp type represents last modified date and time of the location using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="eb56b-160">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。</span><span class="sxs-lookup"><span data-stu-id="eb56b-160">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="eb56b-161">只读。</span><span class="sxs-lookup"><span data-stu-id="eb56b-161">Read-only.</span></span> <span data-ttu-id="eb56b-162">继承自 [namedLocation](../resources/namedLocation.md)。</span><span class="sxs-lookup"><span data-stu-id="eb56b-162">Inherited from [namedLocation](../resources/namedLocation.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="eb56b-163">关系</span><span class="sxs-lookup"><span data-stu-id="eb56b-163">Relationships</span></span>

<span data-ttu-id="eb56b-164">无。</span><span class="sxs-lookup"><span data-stu-id="eb56b-164">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="eb56b-165">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="eb56b-165">JSON representation</span></span>

<span data-ttu-id="eb56b-166">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="eb56b-166">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.countryNamedLocation"
}-->

```json
{
  "countriesAndRegions": ["String"],
  "countryLookupMethod": "String",
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

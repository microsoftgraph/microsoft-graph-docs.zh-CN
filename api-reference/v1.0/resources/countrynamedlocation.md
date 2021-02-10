---
title: countryNamedLocation 资源类型
description: 表示由国家和地区定义的 Azure Active Directory 命名位置。 命名位置是定义网络位置的自定义规则，之后可在条件访问策略中使用。
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: e1cb97648d454277c1d778a28cd8e6ba9844db2f
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50157496"
---
# <a name="countrynamedlocation-resource-type"></a><span data-ttu-id="731cf-104">countryNamedLocation 资源类型</span><span class="sxs-lookup"><span data-stu-id="731cf-104">countryNamedLocation resource type</span></span>

<span data-ttu-id="731cf-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="731cf-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="731cf-106">表示由国家和地区定义的 Azure Active Directory 命名位置。</span><span class="sxs-lookup"><span data-stu-id="731cf-106">Represents an Azure Active Directory named location defined by countries and regions.</span></span> <span data-ttu-id="731cf-107">命名位置是定义网络位置的自定义规则，之后可在条件访问策略中使用。</span><span class="sxs-lookup"><span data-stu-id="731cf-107">Named locations are custom rules that define network locations which can then be used in a Conditional Access policy.</span></span>

<span data-ttu-id="731cf-108">继承自 [namedLocation](../resources/namedLocation.md)</span><span class="sxs-lookup"><span data-stu-id="731cf-108">Inherits from [namedLocation](../resources/namedLocation.md)</span></span>

## <a name="methods"></a><span data-ttu-id="731cf-109">方法</span><span class="sxs-lookup"><span data-stu-id="731cf-109">Methods</span></span>

| <span data-ttu-id="731cf-110">方法</span><span class="sxs-lookup"><span data-stu-id="731cf-110">Method</span></span>       | <span data-ttu-id="731cf-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="731cf-111">Return Type</span></span> | <span data-ttu-id="731cf-112">说明</span><span class="sxs-lookup"><span data-stu-id="731cf-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="731cf-113">列出 countryNamedLocations</span><span class="sxs-lookup"><span data-stu-id="731cf-113">List countryNamedLocations</span></span>](../api/conditionalaccessroot-list-namedlocations.md) | <span data-ttu-id="731cf-114">[countryNamedLocation](countryNamedLocation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="731cf-114">[countryNamedLocation](countryNamedLocation.md) collection</span></span> | <span data-ttu-id="731cf-115">获取 **组织的所有 countryNamedLocation** 对象。</span><span class="sxs-lookup"><span data-stu-id="731cf-115">Get all the **countryNamedLocation** objects in the organization.</span></span> |
| [<span data-ttu-id="731cf-116">创建 countryNamedLocation</span><span class="sxs-lookup"><span data-stu-id="731cf-116">Create countryNamedLocation</span></span>](../api/conditionalaccessroot-post-namedlocations.md) | [<span data-ttu-id="731cf-117">countryNamedLocation</span><span class="sxs-lookup"><span data-stu-id="731cf-117">countryNamedLocation</span></span>](countryNamedLocation.md) | <span data-ttu-id="731cf-118">创建新的 **countryNamedLocation** 对象。</span><span class="sxs-lookup"><span data-stu-id="731cf-118">Create a new **countryNamedLocation** object.</span></span> |
| [<span data-ttu-id="731cf-119">获取 countryNamedLocation</span><span class="sxs-lookup"><span data-stu-id="731cf-119">Get countryNamedLocation</span></span>](../api/countrynamedlocation-get.md) | [<span data-ttu-id="731cf-120">countryNamedLocation</span><span class="sxs-lookup"><span data-stu-id="731cf-120">countryNamedLocation</span></span>](countrynamedlocation.md) | <span data-ttu-id="731cf-121">读取 **countryNamedLocation 对象的属性和** 关系。</span><span class="sxs-lookup"><span data-stu-id="731cf-121">Read the properties and relationships of a **countryNamedLocation** object.</span></span> |
| [<span data-ttu-id="731cf-122">更新 countryNamedLocation</span><span class="sxs-lookup"><span data-stu-id="731cf-122">Update countryNamedLocation</span></span>](../api/countrynamedlocation-update.md) | [<span data-ttu-id="731cf-123">countryNamedLocation</span><span class="sxs-lookup"><span data-stu-id="731cf-123">countryNamedLocation</span></span>](countrynamedlocation.md) | <span data-ttu-id="731cf-124">更新 **countryNamedLocation** 对象。</span><span class="sxs-lookup"><span data-stu-id="731cf-124">Update a **countryNamedLocation** object.</span></span> |
| [<span data-ttu-id="731cf-125">删除 countryNamedLocation</span><span class="sxs-lookup"><span data-stu-id="731cf-125">Delete countryNamedLocation</span></span>](../api/countrynamedlocation-delete.md) | <span data-ttu-id="731cf-126">无</span><span class="sxs-lookup"><span data-stu-id="731cf-126">None</span></span> | <span data-ttu-id="731cf-127">删除 **countryNamedLocation** 对象。</span><span class="sxs-lookup"><span data-stu-id="731cf-127">Delete a **countryNamedLocation** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="731cf-128">属性</span><span class="sxs-lookup"><span data-stu-id="731cf-128">Properties</span></span>

| <span data-ttu-id="731cf-129">属性</span><span class="sxs-lookup"><span data-stu-id="731cf-129">Property</span></span>     | <span data-ttu-id="731cf-130">类型</span><span class="sxs-lookup"><span data-stu-id="731cf-130">Type</span></span>        | <span data-ttu-id="731cf-131">说明</span><span class="sxs-lookup"><span data-stu-id="731cf-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="731cf-132">countriesAndRegions</span><span class="sxs-lookup"><span data-stu-id="731cf-132">countriesAndRegions</span></span>|<span data-ttu-id="731cf-133">字符串集合</span><span class="sxs-lookup"><span data-stu-id="731cf-133">String collection</span></span>|<span data-ttu-id="731cf-134">ISO 3166-2 指定的两字母格式的国家/地区列表。</span><span class="sxs-lookup"><span data-stu-id="731cf-134">List of countries and/or regions in two-letter format specified by ISO 3166-2.</span></span>|
|<span data-ttu-id="731cf-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="731cf-135">createdDateTime</span></span>|<span data-ttu-id="731cf-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="731cf-136">DateTimeOffset</span></span>|<span data-ttu-id="731cf-137">时间戳类型表示使用 ISO 8601 格式的位置的创建日期和时间，并且始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="731cf-137">The Timestamp type represents creation date and time of the location using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="731cf-138">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="731cf-138">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="731cf-139">只读。</span><span class="sxs-lookup"><span data-stu-id="731cf-139">Read-only.</span></span> <span data-ttu-id="731cf-140">继承自 [namedLocation](../resources/namedLocation.md)。</span><span class="sxs-lookup"><span data-stu-id="731cf-140">Inherited from [namedLocation](../resources/namedLocation.md).</span></span>|
|<span data-ttu-id="731cf-141">displayName</span><span class="sxs-lookup"><span data-stu-id="731cf-141">displayName</span></span>|<span data-ttu-id="731cf-142">String</span><span class="sxs-lookup"><span data-stu-id="731cf-142">String</span></span>|<span data-ttu-id="731cf-143">位置的可读名称。</span><span class="sxs-lookup"><span data-stu-id="731cf-143">Human-readable name of the location.</span></span> <span data-ttu-id="731cf-144">继承自 [namedLocation](../resources/namedLocation.md)。</span><span class="sxs-lookup"><span data-stu-id="731cf-144">Inherited from [namedLocation](../resources/namedLocation.md).</span></span>|
|<span data-ttu-id="731cf-145">id</span><span class="sxs-lookup"><span data-stu-id="731cf-145">id</span></span>|<span data-ttu-id="731cf-146">String</span><span class="sxs-lookup"><span data-stu-id="731cf-146">String</span></span>|<span data-ttu-id="731cf-147">namedLocation 对象的标识符。</span><span class="sxs-lookup"><span data-stu-id="731cf-147">Identifier of a namedLocation object.</span></span> <span data-ttu-id="731cf-148">只读。</span><span class="sxs-lookup"><span data-stu-id="731cf-148">Read-only.</span></span> <span data-ttu-id="731cf-149">继承自 [namedLocation](../resources/namedLocation.md)。</span><span class="sxs-lookup"><span data-stu-id="731cf-149">Inherited from [namedLocation](../resources/namedLocation.md).</span></span>|
|<span data-ttu-id="731cf-150">includeUnknownCountriesAndRegions</span><span class="sxs-lookup"><span data-stu-id="731cf-150">includeUnknownCountriesAndRegions</span></span>|<span data-ttu-id="731cf-151">布尔值</span><span class="sxs-lookup"><span data-stu-id="731cf-151">Boolean</span></span>|<span data-ttu-id="731cf-152">如此 如果未映射到一个或多个国家/地区的 IP 地址应包含在命名的位置。</span><span class="sxs-lookup"><span data-stu-id="731cf-152">True if IP addresses that don't map to a country or region should be included in the named location.</span></span>|
|<span data-ttu-id="731cf-153">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="731cf-153">modifiedDateTime</span></span>|<span data-ttu-id="731cf-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="731cf-154">DateTimeOffset</span></span>|<span data-ttu-id="731cf-155">时间戳类型表示使用 ISO 8601 格式的位置的上次修改日期和时间，并且始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="731cf-155">The Timestamp type represents last modified date and time of the location using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="731cf-156">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="731cf-156">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="731cf-157">只读。</span><span class="sxs-lookup"><span data-stu-id="731cf-157">Read-only.</span></span> <span data-ttu-id="731cf-158">继承自 [namedLocation](../resources/namedLocation.md)。</span><span class="sxs-lookup"><span data-stu-id="731cf-158">Inherited from [namedLocation](../resources/namedLocation.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="731cf-159">关系</span><span class="sxs-lookup"><span data-stu-id="731cf-159">Relationships</span></span>

<span data-ttu-id="731cf-160">无。</span><span class="sxs-lookup"><span data-stu-id="731cf-160">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="731cf-161">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="731cf-161">JSON representation</span></span>

<span data-ttu-id="731cf-162">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="731cf-162">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.countryNamedLocation"
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


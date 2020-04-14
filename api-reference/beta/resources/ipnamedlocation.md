---
title: ipNamedLocation 资源类型
description: 表示由 IP 范围定义的 Azure Active Directory 的名称位置。 "已命名位置" 是自定义规则，用于定义随后可在条件访问策略中使用的网络位置。
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 067c77c6bc8a17d84252568548b44a3a44cd8f35
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43382526"
---
# <a name="ipnamedlocation-resource-type"></a><span data-ttu-id="d0d88-104">ipNamedLocation 资源类型</span><span class="sxs-lookup"><span data-stu-id="d0d88-104">ipNamedLocation resource type</span></span>

<span data-ttu-id="d0d88-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d0d88-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d0d88-106">表示由 IP 范围定义的 Azure Active Directory 的名称位置。</span><span class="sxs-lookup"><span data-stu-id="d0d88-106">Represents an Azure Active Directory named location defined by IP ranges.</span></span> <span data-ttu-id="d0d88-107">"已命名位置" 是自定义规则，用于定义随后可在条件访问策略中使用的网络位置。</span><span class="sxs-lookup"><span data-stu-id="d0d88-107">Named locations are custom rules that define network locations which can then be used in a Conditional Access policy.</span></span>

<span data-ttu-id="d0d88-108">继承自[namedLocation](../resources/namedLocation.md)</span><span class="sxs-lookup"><span data-stu-id="d0d88-108">Inherits from [namedLocation](../resources/namedLocation.md)</span></span>

## <a name="methods"></a><span data-ttu-id="d0d88-109">方法</span><span class="sxs-lookup"><span data-stu-id="d0d88-109">Methods</span></span>

| <span data-ttu-id="d0d88-110">方法</span><span class="sxs-lookup"><span data-stu-id="d0d88-110">Method</span></span>       | <span data-ttu-id="d0d88-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="d0d88-111">Return Type</span></span> | <span data-ttu-id="d0d88-112">说明</span><span class="sxs-lookup"><span data-stu-id="d0d88-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="d0d88-113">列出 ipNamedLocations</span><span class="sxs-lookup"><span data-stu-id="d0d88-113">List ipNamedLocations</span></span>](../api/conditionalaccessroot-list-namedlocations.md) | <span data-ttu-id="d0d88-114">[ipNamedLocation](ipNamedLocation.md)集合</span><span class="sxs-lookup"><span data-stu-id="d0d88-114">[ipNamedLocation](ipNamedLocation.md) collection</span></span> | <span data-ttu-id="d0d88-115">获取组织中的所有**ipNamedLocation**对象。</span><span class="sxs-lookup"><span data-stu-id="d0d88-115">Get all the **ipNamedLocation** objects in the organization.</span></span> |
| [<span data-ttu-id="d0d88-116">创建 ipNamedLocation</span><span class="sxs-lookup"><span data-stu-id="d0d88-116">Create ipNamedLocation</span></span>](../api/conditionalaccessroot-post-namedlocations.md) | [<span data-ttu-id="d0d88-117">ipNamedLocation</span><span class="sxs-lookup"><span data-stu-id="d0d88-117">ipNamedLocation</span></span>](ipNamedLocation.md) | <span data-ttu-id="d0d88-118">创建新的**ipNamedLocation**对象。</span><span class="sxs-lookup"><span data-stu-id="d0d88-118">Create a new **ipNamedLocation** object.</span></span> |
| [<span data-ttu-id="d0d88-119">获取 ipNamedLocation</span><span class="sxs-lookup"><span data-stu-id="d0d88-119">Get ipNamedLocation</span></span>](../api/ipnamedlocation-get.md) | [<span data-ttu-id="d0d88-120">ipNamedLocation</span><span class="sxs-lookup"><span data-stu-id="d0d88-120">ipNamedLocation</span></span>](ipnamedlocation.md) | <span data-ttu-id="d0d88-121">读取**ipNamedLocation**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d0d88-121">Read the properties and relationships of an **ipNamedLocation** object.</span></span> |
| [<span data-ttu-id="d0d88-122">更新 ipNamedLocation</span><span class="sxs-lookup"><span data-stu-id="d0d88-122">Update ipNamedLocation</span></span>](../api/ipnamedlocation-update.md) | [<span data-ttu-id="d0d88-123">ipNamedLocation</span><span class="sxs-lookup"><span data-stu-id="d0d88-123">ipNamedLocation</span></span>](ipnamedlocation.md) | <span data-ttu-id="d0d88-124">更新**ipNamedLocation**对象。</span><span class="sxs-lookup"><span data-stu-id="d0d88-124">Update an **ipNamedLocation** object.</span></span> |
| [<span data-ttu-id="d0d88-125">删除 ipNamedLocation</span><span class="sxs-lookup"><span data-stu-id="d0d88-125">Delete ipNamedLocation</span></span>](../api/ipnamedlocation-delete.md) | <span data-ttu-id="d0d88-126">无</span><span class="sxs-lookup"><span data-stu-id="d0d88-126">None</span></span> | <span data-ttu-id="d0d88-127">删除**ipNamedLocation**对象。</span><span class="sxs-lookup"><span data-stu-id="d0d88-127">Delete an **ipNamedLocation** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="d0d88-128">属性</span><span class="sxs-lookup"><span data-stu-id="d0d88-128">Properties</span></span>

| <span data-ttu-id="d0d88-129">属性</span><span class="sxs-lookup"><span data-stu-id="d0d88-129">Property</span></span>     | <span data-ttu-id="d0d88-130">类型</span><span class="sxs-lookup"><span data-stu-id="d0d88-130">Type</span></span>        | <span data-ttu-id="d0d88-131">说明</span><span class="sxs-lookup"><span data-stu-id="d0d88-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d0d88-132">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d0d88-132">createdDateTime</span></span>|<span data-ttu-id="d0d88-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d0d88-133">DateTimeOffset</span></span>|<span data-ttu-id="d0d88-134">时间戳类型表示使用 ISO 8601 格式的位置的创建日期和时间，并且始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="d0d88-134">The Timestamp type represents creation date and time of the location using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="d0d88-135">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="d0d88-135">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="d0d88-136">只读。</span><span class="sxs-lookup"><span data-stu-id="d0d88-136">Read-only.</span></span> <span data-ttu-id="d0d88-137">继承自[namedLocation](../resources/namedLocation.md)。</span><span class="sxs-lookup"><span data-stu-id="d0d88-137">Inherited from [namedLocation](../resources/namedLocation.md).</span></span>|
|<span data-ttu-id="d0d88-138">displayName</span><span class="sxs-lookup"><span data-stu-id="d0d88-138">displayName</span></span>|<span data-ttu-id="d0d88-139">String</span><span class="sxs-lookup"><span data-stu-id="d0d88-139">String</span></span>|<span data-ttu-id="d0d88-140">位置的人可读名称。</span><span class="sxs-lookup"><span data-stu-id="d0d88-140">Human-readable name of the location.</span></span>|
|<span data-ttu-id="d0d88-141">id</span><span class="sxs-lookup"><span data-stu-id="d0d88-141">id</span></span>|<span data-ttu-id="d0d88-142">字符串</span><span class="sxs-lookup"><span data-stu-id="d0d88-142">String</span></span>|<span data-ttu-id="d0d88-143">NamedLocation 对象的标识符。</span><span class="sxs-lookup"><span data-stu-id="d0d88-143">Identifier of a namedLocation object.</span></span> <span data-ttu-id="d0d88-144">只读。</span><span class="sxs-lookup"><span data-stu-id="d0d88-144">Read-only.</span></span> <span data-ttu-id="d0d88-145">继承自[namedLocation](../resources/namedLocation.md)。</span><span class="sxs-lookup"><span data-stu-id="d0d88-145">Inherited from [namedLocation](../resources/namedLocation.md).</span></span>|
|<span data-ttu-id="d0d88-146">ipRanges</span><span class="sxs-lookup"><span data-stu-id="d0d88-146">ipRanges</span></span>|<span data-ttu-id="d0d88-147">[ipRange](iprange.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d0d88-147">[ipRange](iprange.md) collection</span></span>|<span data-ttu-id="d0d88-148">IPv4 CIDR 格式的 IP 地址范围列表（例如，1.2.3.4/32）或来自 IETF RFC596 的任何允许的 IPv6 格式。</span><span class="sxs-lookup"><span data-stu-id="d0d88-148">List of IP address ranges in IPv4 CIDR format (e.g. 1.2.3.4/32) or any allowable IPv6 format from IETF RFC596.</span></span>|
|<span data-ttu-id="d0d88-149">isTrusted</span><span class="sxs-lookup"><span data-stu-id="d0d88-149">isTrusted</span></span>|<span data-ttu-id="d0d88-150">Boolean</span><span class="sxs-lookup"><span data-stu-id="d0d88-150">Boolean</span></span>|<span data-ttu-id="d0d88-151">如此如果此位置是明确信任的。</span><span class="sxs-lookup"><span data-stu-id="d0d88-151">True if this location is explicitly trusted.</span></span>|
|<span data-ttu-id="d0d88-152">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d0d88-152">modifiedDateTime</span></span>|<span data-ttu-id="d0d88-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d0d88-153">DateTimeOffset</span></span>|<span data-ttu-id="d0d88-154">时间戳类型表示上次修改的位置使用 ISO 8601 格式的日期和时间，并且始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="d0d88-154">The Timestamp type represents last modified date and time of the location using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="d0d88-155">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="d0d88-155">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="d0d88-156">只读。</span><span class="sxs-lookup"><span data-stu-id="d0d88-156">Read-only.</span></span> <span data-ttu-id="d0d88-157">继承自[namedLocation](../resources/namedLocation.md)。</span><span class="sxs-lookup"><span data-stu-id="d0d88-157">Inherited from [namedLocation](../resources/namedLocation.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="d0d88-158">关系</span><span class="sxs-lookup"><span data-stu-id="d0d88-158">Relationships</span></span>

<span data-ttu-id="d0d88-159">无。</span><span class="sxs-lookup"><span data-stu-id="d0d88-159">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d0d88-160">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d0d88-160">JSON representation</span></span>

<span data-ttu-id="d0d88-161">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d0d88-161">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.ipNamedLocation",
  "baseType": ""
}-->

```json
{
  "createdDateTime": "String (timestamp)",
  "displayName": "String",
  "id": "String (identifier)",
  "ipRanges": [{"@odata.type": "microsoft.graph.ipRange"}],
  "isTrusted": true,
  "modifiedDateTime": "String (timestamp)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ipNamedLocation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

---
title: ipNamedLocation 资源类型
description: 表示由 IP 范围定义的 Azure Active Directory 的名称位置。 "已命名位置" 是自定义规则，用于定义随后可在条件访问策略中使用的网络位置。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 10bdafb9894d822f345bb6fb23174fa7f7deee4c
ms.sourcegitcommit: d189830649794365464e37539e02239f883011da
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/24/2019
ms.locfileid: "37653816"
---
# <a name="ipnamedlocation-resource-type"></a><span data-ttu-id="9d0fa-104">ipNamedLocation 资源类型</span><span class="sxs-lookup"><span data-stu-id="9d0fa-104">ipNamedLocation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9d0fa-105">表示由 IP 范围定义的 Azure Active Directory 的名称位置。</span><span class="sxs-lookup"><span data-stu-id="9d0fa-105">Represents an Azure Active Directory named location defined by IP ranges.</span></span> <span data-ttu-id="9d0fa-106">"已命名位置" 是自定义规则，用于定义随后可在条件访问策略中使用的网络位置。</span><span class="sxs-lookup"><span data-stu-id="9d0fa-106">Named locations are custom rules that define network locations which can then be used in a Conditional Access policy.</span></span>

<span data-ttu-id="9d0fa-107">继承自[namedLocation](../resources/namedLocation.md)</span><span class="sxs-lookup"><span data-stu-id="9d0fa-107">Inherits from [namedLocation](../resources/namedLocation.md)</span></span>

## <a name="methods"></a><span data-ttu-id="9d0fa-108">方法</span><span class="sxs-lookup"><span data-stu-id="9d0fa-108">Methods</span></span>

| <span data-ttu-id="9d0fa-109">方法</span><span class="sxs-lookup"><span data-stu-id="9d0fa-109">Method</span></span>       | <span data-ttu-id="9d0fa-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="9d0fa-110">Return Type</span></span> | <span data-ttu-id="9d0fa-111">说明</span><span class="sxs-lookup"><span data-stu-id="9d0fa-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="9d0fa-112">列出 ipNamedLocations</span><span class="sxs-lookup"><span data-stu-id="9d0fa-112">List ipNamedLocations</span></span>](../api/conditionalaccessroot-list-namedlocations.md) | <span data-ttu-id="9d0fa-113">[ipNamedLocation](ipNamedLocation.md)集合</span><span class="sxs-lookup"><span data-stu-id="9d0fa-113">[ipNamedLocation](ipNamedLocation.md) collection</span></span> | <span data-ttu-id="9d0fa-114">获取组织中的所有**ipNamedLocation**对象。</span><span class="sxs-lookup"><span data-stu-id="9d0fa-114">Get all the **ipNamedLocation** objects in the organization.</span></span> |
| [<span data-ttu-id="9d0fa-115">创建 ipNamedLocation</span><span class="sxs-lookup"><span data-stu-id="9d0fa-115">Create ipNamedLocation</span></span>](../api/conditionalaccessroot-post-namedlocations.md) | [<span data-ttu-id="9d0fa-116">ipNamedLocation</span><span class="sxs-lookup"><span data-stu-id="9d0fa-116">ipNamedLocation</span></span>](ipNamedLocation.md) | <span data-ttu-id="9d0fa-117">创建新的**ipNamedLocation**对象。</span><span class="sxs-lookup"><span data-stu-id="9d0fa-117">Create a new **ipNamedLocation** object.</span></span> |
| [<span data-ttu-id="9d0fa-118">获取 ipNamedLocation</span><span class="sxs-lookup"><span data-stu-id="9d0fa-118">Get ipNamedLocation</span></span>](../api/ipnamedlocation-get.md) | [<span data-ttu-id="9d0fa-119">ipNamedLocation</span><span class="sxs-lookup"><span data-stu-id="9d0fa-119">ipNamedLocation</span></span>](ipnamedlocation.md) | <span data-ttu-id="9d0fa-120">读取**ipNamedLocation**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9d0fa-120">Read the properties and relationships of an **ipNamedLocation** object.</span></span> |
| [<span data-ttu-id="9d0fa-121">更新 ipNamedLocation</span><span class="sxs-lookup"><span data-stu-id="9d0fa-121">Update ipNamedLocation</span></span>](../api/ipnamedlocation-update.md) | [<span data-ttu-id="9d0fa-122">ipNamedLocation</span><span class="sxs-lookup"><span data-stu-id="9d0fa-122">ipNamedLocation</span></span>](ipnamedlocation.md) | <span data-ttu-id="9d0fa-123">更新**ipNamedLocation**对象。</span><span class="sxs-lookup"><span data-stu-id="9d0fa-123">Update an **ipNamedLocation** object.</span></span> |
| [<span data-ttu-id="9d0fa-124">删除 ipNamedLocation</span><span class="sxs-lookup"><span data-stu-id="9d0fa-124">Delete ipNamedLocation</span></span>](../api/ipnamedlocation-delete.md) | <span data-ttu-id="9d0fa-125">无</span><span class="sxs-lookup"><span data-stu-id="9d0fa-125">None</span></span> | <span data-ttu-id="9d0fa-126">删除**ipNamedLocation**对象。</span><span class="sxs-lookup"><span data-stu-id="9d0fa-126">Delete an **ipNamedLocation** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="9d0fa-127">属性</span><span class="sxs-lookup"><span data-stu-id="9d0fa-127">Properties</span></span>

| <span data-ttu-id="9d0fa-128">属性</span><span class="sxs-lookup"><span data-stu-id="9d0fa-128">Property</span></span>     | <span data-ttu-id="9d0fa-129">类型</span><span class="sxs-lookup"><span data-stu-id="9d0fa-129">Type</span></span>        | <span data-ttu-id="9d0fa-130">说明</span><span class="sxs-lookup"><span data-stu-id="9d0fa-130">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="9d0fa-131">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9d0fa-131">createdDateTime</span></span>|<span data-ttu-id="9d0fa-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9d0fa-132">DateTimeOffset</span></span>|<span data-ttu-id="9d0fa-133">时间戳类型表示使用 ISO 8601 格式的位置的创建日期和时间，并且始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="9d0fa-133">The Timestamp type represents creation date and time of the location using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="9d0fa-134">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="9d0fa-134">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="9d0fa-135">只读。</span><span class="sxs-lookup"><span data-stu-id="9d0fa-135">Read-only.</span></span> <span data-ttu-id="9d0fa-136">继承自[namedLocation](../resources/namedLocation.md)。</span><span class="sxs-lookup"><span data-stu-id="9d0fa-136">Inherited from [namedLocation](../resources/namedLocation.md).</span></span>|
|<span data-ttu-id="9d0fa-137">displayName</span><span class="sxs-lookup"><span data-stu-id="9d0fa-137">displayName</span></span>|<span data-ttu-id="9d0fa-138">String</span><span class="sxs-lookup"><span data-stu-id="9d0fa-138">String</span></span>|<span data-ttu-id="9d0fa-139">位置的人可读名称。</span><span class="sxs-lookup"><span data-stu-id="9d0fa-139">Human-readable name of the location.</span></span>|
|<span data-ttu-id="9d0fa-140">id</span><span class="sxs-lookup"><span data-stu-id="9d0fa-140">id</span></span>|<span data-ttu-id="9d0fa-141">String</span><span class="sxs-lookup"><span data-stu-id="9d0fa-141">String</span></span>|<span data-ttu-id="9d0fa-142">NamedLocation 对象的标识符。</span><span class="sxs-lookup"><span data-stu-id="9d0fa-142">Identifier of a namedLocation object.</span></span> <span data-ttu-id="9d0fa-143">只读。</span><span class="sxs-lookup"><span data-stu-id="9d0fa-143">Read-only.</span></span> <span data-ttu-id="9d0fa-144">继承自[namedLocation](../resources/namedLocation.md)。</span><span class="sxs-lookup"><span data-stu-id="9d0fa-144">Inherited from [namedLocation](../resources/namedLocation.md).</span></span>|
|<span data-ttu-id="9d0fa-145">ipRanges</span><span class="sxs-lookup"><span data-stu-id="9d0fa-145">ipRanges</span></span>|<span data-ttu-id="9d0fa-146">[ipRange](iprange.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9d0fa-146">[ipRange](iprange.md) collection</span></span>|<span data-ttu-id="9d0fa-147">IPv4 CIDR 格式的 IP 地址范围列表（例如，1.2.3.4/32）或来自 IETF RFC596 的任何允许的 IPv6 格式。</span><span class="sxs-lookup"><span data-stu-id="9d0fa-147">List of IP address ranges in IPv4 CIDR format (e.g. 1.2.3.4/32) or any allowable IPv6 format from IETF RFC596.</span></span>|
|<span data-ttu-id="9d0fa-148">isTrusted</span><span class="sxs-lookup"><span data-stu-id="9d0fa-148">isTrusted</span></span>|<span data-ttu-id="9d0fa-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="9d0fa-149">Boolean</span></span>|<span data-ttu-id="9d0fa-150">如此如果此位置是明确信任的。</span><span class="sxs-lookup"><span data-stu-id="9d0fa-150">True if this location is explicitly trusted.</span></span>|
|<span data-ttu-id="9d0fa-151">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9d0fa-151">modifiedDateTime</span></span>|<span data-ttu-id="9d0fa-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9d0fa-152">DateTimeOffset</span></span>|<span data-ttu-id="9d0fa-153">时间戳类型表示上次修改的位置使用 ISO 8601 格式的日期和时间，并且始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="9d0fa-153">The Timestamp type represents last modified date and time of the location using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="9d0fa-154">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="9d0fa-154">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="9d0fa-155">只读。</span><span class="sxs-lookup"><span data-stu-id="9d0fa-155">Read-only.</span></span> <span data-ttu-id="9d0fa-156">继承自[namedLocation](../resources/namedLocation.md)。</span><span class="sxs-lookup"><span data-stu-id="9d0fa-156">Inherited from [namedLocation](../resources/namedLocation.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="9d0fa-157">关系</span><span class="sxs-lookup"><span data-stu-id="9d0fa-157">Relationships</span></span>

<span data-ttu-id="9d0fa-158">无。</span><span class="sxs-lookup"><span data-stu-id="9d0fa-158">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9d0fa-159">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9d0fa-159">JSON representation</span></span>

<span data-ttu-id="9d0fa-160">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9d0fa-160">The following is a JSON representation of the resource.</span></span>

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

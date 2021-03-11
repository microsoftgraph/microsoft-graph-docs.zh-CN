---
title: ipNamedLocation 资源类型
description: 表示由 IP 范围定义的 Azure Active Directory 命名位置。 命名位置是定义网络位置的自定义规则，这些位置随后可在条件访问策略中使用。
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 02b704b1216c34f80155cf1ebf323e29f565c620
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720667"
---
# <a name="ipnamedlocation-resource-type"></a><span data-ttu-id="0e46f-104">ipNamedLocation 资源类型</span><span class="sxs-lookup"><span data-stu-id="0e46f-104">ipNamedLocation resource type</span></span>

<span data-ttu-id="0e46f-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0e46f-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0e46f-106">表示由 IP 范围定义的 Azure Active Directory 命名位置。</span><span class="sxs-lookup"><span data-stu-id="0e46f-106">Represents an Azure Active Directory named location defined by IP ranges.</span></span> <span data-ttu-id="0e46f-107">命名位置是定义网络位置的自定义规则，这些位置随后可在条件访问策略中使用。</span><span class="sxs-lookup"><span data-stu-id="0e46f-107">Named locations are custom rules that define network locations which can then be used in a Conditional Access policy.</span></span>

<span data-ttu-id="0e46f-108">继承自 [namedLocation](../resources/namedLocation.md)</span><span class="sxs-lookup"><span data-stu-id="0e46f-108">Inherits from [namedLocation](../resources/namedLocation.md)</span></span>

## <a name="methods"></a><span data-ttu-id="0e46f-109">方法</span><span class="sxs-lookup"><span data-stu-id="0e46f-109">Methods</span></span>

| <span data-ttu-id="0e46f-110">方法</span><span class="sxs-lookup"><span data-stu-id="0e46f-110">Method</span></span>       | <span data-ttu-id="0e46f-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="0e46f-111">Return Type</span></span> | <span data-ttu-id="0e46f-112">说明</span><span class="sxs-lookup"><span data-stu-id="0e46f-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="0e46f-113">列出 ipNamedLocations</span><span class="sxs-lookup"><span data-stu-id="0e46f-113">List ipNamedLocations</span></span>](../api/conditionalaccessroot-list-namedlocations.md) | <span data-ttu-id="0e46f-114">[ipNamedLocation](ipNamedLocation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0e46f-114">[ipNamedLocation](ipNamedLocation.md) collection</span></span> | <span data-ttu-id="0e46f-115">获取 **组织的所有 ipNamedLocation** 对象。</span><span class="sxs-lookup"><span data-stu-id="0e46f-115">Get all the **ipNamedLocation** objects in the organization.</span></span> |
| [<span data-ttu-id="0e46f-116">创建 ipNamedLocation</span><span class="sxs-lookup"><span data-stu-id="0e46f-116">Create ipNamedLocation</span></span>](../api/conditionalaccessroot-post-namedlocations.md) | [<span data-ttu-id="0e46f-117">ipNamedLocation</span><span class="sxs-lookup"><span data-stu-id="0e46f-117">ipNamedLocation</span></span>](ipNamedLocation.md) | <span data-ttu-id="0e46f-118">创建新的 **ipNamedLocation** 对象。</span><span class="sxs-lookup"><span data-stu-id="0e46f-118">Create a new **ipNamedLocation** object.</span></span> |
| [<span data-ttu-id="0e46f-119">获取 ipNamedLocation</span><span class="sxs-lookup"><span data-stu-id="0e46f-119">Get ipNamedLocation</span></span>](../api/ipnamedlocation-get.md) | [<span data-ttu-id="0e46f-120">ipNamedLocation</span><span class="sxs-lookup"><span data-stu-id="0e46f-120">ipNamedLocation</span></span>](ipnamedlocation.md) | <span data-ttu-id="0e46f-121">读取 **ipNamedLocation** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0e46f-121">Read the properties and relationships of an **ipNamedLocation** object.</span></span> |
| [<span data-ttu-id="0e46f-122">更新 ipNamedLocation</span><span class="sxs-lookup"><span data-stu-id="0e46f-122">Update ipNamedLocation</span></span>](../api/ipnamedlocation-update.md) | [<span data-ttu-id="0e46f-123">ipNamedLocation</span><span class="sxs-lookup"><span data-stu-id="0e46f-123">ipNamedLocation</span></span>](ipnamedlocation.md) | <span data-ttu-id="0e46f-124">更新 **ipNamedLocation** 对象。</span><span class="sxs-lookup"><span data-stu-id="0e46f-124">Update an **ipNamedLocation** object.</span></span> |
| [<span data-ttu-id="0e46f-125">删除 ipNamedLocation</span><span class="sxs-lookup"><span data-stu-id="0e46f-125">Delete ipNamedLocation</span></span>](../api/ipnamedlocation-delete.md) | <span data-ttu-id="0e46f-126">无</span><span class="sxs-lookup"><span data-stu-id="0e46f-126">None</span></span> | <span data-ttu-id="0e46f-127">删除 **ipNamedLocation** 对象。</span><span class="sxs-lookup"><span data-stu-id="0e46f-127">Delete an **ipNamedLocation** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="0e46f-128">属性</span><span class="sxs-lookup"><span data-stu-id="0e46f-128">Properties</span></span>

| <span data-ttu-id="0e46f-129">属性</span><span class="sxs-lookup"><span data-stu-id="0e46f-129">Property</span></span>     | <span data-ttu-id="0e46f-130">类型</span><span class="sxs-lookup"><span data-stu-id="0e46f-130">Type</span></span>        | <span data-ttu-id="0e46f-131">说明</span><span class="sxs-lookup"><span data-stu-id="0e46f-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0e46f-132">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0e46f-132">createdDateTime</span></span>|<span data-ttu-id="0e46f-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0e46f-133">DateTimeOffset</span></span>|<span data-ttu-id="0e46f-134">时间戳类型表示使用 ISO 8601 格式的位置的创建日期和时间，并且始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="0e46f-134">The Timestamp type represents creation date and time of the location using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="0e46f-135">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。</span><span class="sxs-lookup"><span data-stu-id="0e46f-135">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="0e46f-136">只读。</span><span class="sxs-lookup"><span data-stu-id="0e46f-136">Read-only.</span></span> <span data-ttu-id="0e46f-137">继承自 [namedLocation](../resources/namedLocation.md)。</span><span class="sxs-lookup"><span data-stu-id="0e46f-137">Inherited from [namedLocation](../resources/namedLocation.md).</span></span>|
|<span data-ttu-id="0e46f-138">displayName</span><span class="sxs-lookup"><span data-stu-id="0e46f-138">displayName</span></span>|<span data-ttu-id="0e46f-139">String</span><span class="sxs-lookup"><span data-stu-id="0e46f-139">String</span></span>|<span data-ttu-id="0e46f-140">位置的可读名称。</span><span class="sxs-lookup"><span data-stu-id="0e46f-140">Human-readable name of the location.</span></span>|
|<span data-ttu-id="0e46f-141">id</span><span class="sxs-lookup"><span data-stu-id="0e46f-141">id</span></span>|<span data-ttu-id="0e46f-142">String</span><span class="sxs-lookup"><span data-stu-id="0e46f-142">String</span></span>|<span data-ttu-id="0e46f-143">namedLocation 对象的标识符。</span><span class="sxs-lookup"><span data-stu-id="0e46f-143">Identifier of a namedLocation object.</span></span> <span data-ttu-id="0e46f-144">只读。</span><span class="sxs-lookup"><span data-stu-id="0e46f-144">Read-only.</span></span> <span data-ttu-id="0e46f-145">继承自 [namedLocation](../resources/namedLocation.md)。</span><span class="sxs-lookup"><span data-stu-id="0e46f-145">Inherited from [namedLocation](../resources/namedLocation.md).</span></span>|
|<span data-ttu-id="0e46f-146">ipRanges</span><span class="sxs-lookup"><span data-stu-id="0e46f-146">ipRanges</span></span>|<span data-ttu-id="0e46f-147">[ipRange](iprange.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0e46f-147">[ipRange](iprange.md) collection</span></span>|<span data-ttu-id="0e46f-148">IPv4 CIDR 格式的 IP 地址范围列表 (例如 1.2.3.4/32) IETF RFC596 中任何允许的 IPv6 格式。</span><span class="sxs-lookup"><span data-stu-id="0e46f-148">List of IP address ranges in IPv4 CIDR format (e.g. 1.2.3.4/32) or any allowable IPv6 format from IETF RFC596.</span></span>|
|<span data-ttu-id="0e46f-149">isTrusted</span><span class="sxs-lookup"><span data-stu-id="0e46f-149">isTrusted</span></span>|<span data-ttu-id="0e46f-150">布尔</span><span class="sxs-lookup"><span data-stu-id="0e46f-150">Boolean</span></span>|<span data-ttu-id="0e46f-151">如果明确信任此位置，则其为 True。</span><span class="sxs-lookup"><span data-stu-id="0e46f-151">True if this location is explicitly trusted.</span></span>|
|<span data-ttu-id="0e46f-152">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0e46f-152">modifiedDateTime</span></span>|<span data-ttu-id="0e46f-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0e46f-153">DateTimeOffset</span></span>|<span data-ttu-id="0e46f-154">时间戳类型表示使用 ISO 8601 格式的位置的上次修改日期和时间，并且始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="0e46f-154">The Timestamp type represents last modified date and time of the location using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="0e46f-155">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。</span><span class="sxs-lookup"><span data-stu-id="0e46f-155">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="0e46f-156">只读。</span><span class="sxs-lookup"><span data-stu-id="0e46f-156">Read-only.</span></span> <span data-ttu-id="0e46f-157">继承自 [namedLocation](../resources/namedLocation.md)。</span><span class="sxs-lookup"><span data-stu-id="0e46f-157">Inherited from [namedLocation](../resources/namedLocation.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="0e46f-158">关系</span><span class="sxs-lookup"><span data-stu-id="0e46f-158">Relationships</span></span>

<span data-ttu-id="0e46f-159">无。</span><span class="sxs-lookup"><span data-stu-id="0e46f-159">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0e46f-160">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0e46f-160">JSON representation</span></span>

<span data-ttu-id="0e46f-161">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0e46f-161">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.ipNamedLocation"
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



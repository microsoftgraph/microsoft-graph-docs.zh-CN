---
title: namedLocation 资源类型
description: 这是表示 Azure Active Directory （名为 location）的基类。 "已命名位置" 是自定义规则，用于定义随后可在条件访问策略中使用的网络位置。
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: dc92ba18f51f02f03713e43d0fbd4efe4e7cb227
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48022895"
---
# <a name="namedlocation-resource-type"></a><span data-ttu-id="39fa3-104">namedLocation 资源类型</span><span class="sxs-lookup"><span data-stu-id="39fa3-104">namedLocation resource type</span></span>

<span data-ttu-id="39fa3-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="39fa3-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="39fa3-106">这是表示 Azure Active Directory （名为 location）的基类。</span><span class="sxs-lookup"><span data-stu-id="39fa3-106">This is the base class that represents an Azure Active Directory named location.</span></span> <span data-ttu-id="39fa3-107">"已命名位置" 是自定义规则，用于定义随后可在条件访问策略中使用的网络位置。</span><span class="sxs-lookup"><span data-stu-id="39fa3-107">Named locations are custom rules that define network locations which can then be used in a Conditional Access policy.</span></span>

## <a name="methods"></a><span data-ttu-id="39fa3-108">方法</span><span class="sxs-lookup"><span data-stu-id="39fa3-108">Methods</span></span>

| <span data-ttu-id="39fa3-109">方法</span><span class="sxs-lookup"><span data-stu-id="39fa3-109">Method</span></span>       | <span data-ttu-id="39fa3-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="39fa3-110">Return Type</span></span> | <span data-ttu-id="39fa3-111">说明</span><span class="sxs-lookup"><span data-stu-id="39fa3-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="39fa3-112">列出 namedLocations</span><span class="sxs-lookup"><span data-stu-id="39fa3-112">List namedLocations</span></span>](../api/conditionalaccessroot-list-namedlocations.md) | <span data-ttu-id="39fa3-113">[namedLocation](namedLocation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="39fa3-113">[namedLocation](namedLocation.md) collection</span></span> | <span data-ttu-id="39fa3-114">获取组织中的所有 **namedLocation** 对象。</span><span class="sxs-lookup"><span data-stu-id="39fa3-114">Get all the **namedLocation** objects in the organization.</span></span> |
| [<span data-ttu-id="39fa3-115">获取 namedLocation</span><span class="sxs-lookup"><span data-stu-id="39fa3-115">Get namedLocation</span></span>](../api/namedlocation-get.md) | [<span data-ttu-id="39fa3-116">namedLocation</span><span class="sxs-lookup"><span data-stu-id="39fa3-116">namedLocation</span></span>](namedlocation.md) | <span data-ttu-id="39fa3-117">读取 **namedLocation** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="39fa3-117">Read the properties and relationships of a **namedLocation** object.</span></span> |
| [<span data-ttu-id="39fa3-118">删除 namedLocation</span><span class="sxs-lookup"><span data-stu-id="39fa3-118">Delete namedLocation</span></span>](../api/namedlocation-delete.md) | <span data-ttu-id="39fa3-119">无</span><span class="sxs-lookup"><span data-stu-id="39fa3-119">None</span></span> | <span data-ttu-id="39fa3-120">删除 **namedLocation** 对象。</span><span class="sxs-lookup"><span data-stu-id="39fa3-120">Delete a **namedLocation** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="39fa3-121">属性</span><span class="sxs-lookup"><span data-stu-id="39fa3-121">Properties</span></span>

| <span data-ttu-id="39fa3-122">属性</span><span class="sxs-lookup"><span data-stu-id="39fa3-122">Property</span></span>     | <span data-ttu-id="39fa3-123">类型</span><span class="sxs-lookup"><span data-stu-id="39fa3-123">Type</span></span>        | <span data-ttu-id="39fa3-124">说明</span><span class="sxs-lookup"><span data-stu-id="39fa3-124">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="39fa3-125">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="39fa3-125">createdDateTime</span></span>|<span data-ttu-id="39fa3-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="39fa3-126">DateTimeOffset</span></span>|<span data-ttu-id="39fa3-127">时间戳类型表示使用 ISO 8601 格式的位置的创建日期和时间，并且始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="39fa3-127">The Timestamp type represents creation date and time of the location using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="39fa3-128">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="39fa3-128">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="39fa3-129">只读。</span><span class="sxs-lookup"><span data-stu-id="39fa3-129">Read-only.</span></span>|
|<span data-ttu-id="39fa3-130">displayName</span><span class="sxs-lookup"><span data-stu-id="39fa3-130">displayName</span></span>|<span data-ttu-id="39fa3-131">String</span><span class="sxs-lookup"><span data-stu-id="39fa3-131">String</span></span>|<span data-ttu-id="39fa3-132">位置的人可读名称。</span><span class="sxs-lookup"><span data-stu-id="39fa3-132">Human-readable name of the location.</span></span>|
|<span data-ttu-id="39fa3-133">id</span><span class="sxs-lookup"><span data-stu-id="39fa3-133">id</span></span>|<span data-ttu-id="39fa3-134">String</span><span class="sxs-lookup"><span data-stu-id="39fa3-134">String</span></span>|<span data-ttu-id="39fa3-135">NamedLocation 对象的标识符。</span><span class="sxs-lookup"><span data-stu-id="39fa3-135">Identifier of a namedLocation object.</span></span> <span data-ttu-id="39fa3-136">只读。</span><span class="sxs-lookup"><span data-stu-id="39fa3-136">Read-only.</span></span>|
|<span data-ttu-id="39fa3-137">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="39fa3-137">modifiedDateTime</span></span>|<span data-ttu-id="39fa3-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="39fa3-138">DateTimeOffset</span></span>|<span data-ttu-id="39fa3-139">时间戳类型表示上次修改的位置使用 ISO 8601 格式的日期和时间，并且始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="39fa3-139">The Timestamp type represents last modified date and time of the location using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="39fa3-140">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="39fa3-140">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="39fa3-141">只读。</span><span class="sxs-lookup"><span data-stu-id="39fa3-141">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="39fa3-142">关系</span><span class="sxs-lookup"><span data-stu-id="39fa3-142">Relationships</span></span>

<span data-ttu-id="39fa3-143">无。</span><span class="sxs-lookup"><span data-stu-id="39fa3-143">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="39fa3-144">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="39fa3-144">JSON representation</span></span>

<span data-ttu-id="39fa3-145">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="39fa3-145">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.namedLocation",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "createdDateTime": "String (timestamp)",
  "displayName": "String",
  "id": "String (identifier)",
  "modifiedDateTime": "String (timestamp)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "namedLocation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


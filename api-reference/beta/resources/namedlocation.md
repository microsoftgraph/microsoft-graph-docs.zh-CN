---
title: namedLocation 资源类型
description: 这是表示 Azure Active Directory （名为 location）的基类。 "已命名位置" 是自定义规则，用于定义随后可在条件访问策略中使用的网络位置。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 1fda2606e24c6dda282835ada55fb3dfa91ab6ce
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522594"
---
# <a name="namedlocation-resource-type"></a><span data-ttu-id="14226-104">namedLocation 资源类型</span><span class="sxs-lookup"><span data-stu-id="14226-104">namedLocation resource type</span></span>

<span data-ttu-id="14226-105">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="14226-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="14226-106">这是表示 Azure Active Directory （名为 location）的基类。</span><span class="sxs-lookup"><span data-stu-id="14226-106">This is the base class that represents an Azure Active Directory named location.</span></span> <span data-ttu-id="14226-107">"已命名位置" 是自定义规则，用于定义随后可在条件访问策略中使用的网络位置。</span><span class="sxs-lookup"><span data-stu-id="14226-107">Named locations are custom rules that define network locations which can then be used in a Conditional Access policy.</span></span>

## <a name="methods"></a><span data-ttu-id="14226-108">方法</span><span class="sxs-lookup"><span data-stu-id="14226-108">Methods</span></span>

| <span data-ttu-id="14226-109">方法</span><span class="sxs-lookup"><span data-stu-id="14226-109">Method</span></span>       | <span data-ttu-id="14226-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="14226-110">Return Type</span></span> | <span data-ttu-id="14226-111">说明</span><span class="sxs-lookup"><span data-stu-id="14226-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="14226-112">列出 namedLocations</span><span class="sxs-lookup"><span data-stu-id="14226-112">List namedLocations</span></span>](../api/conditionalaccessroot-list-namedlocations.md) | <span data-ttu-id="14226-113">[namedLocation](namedLocation.md)集合</span><span class="sxs-lookup"><span data-stu-id="14226-113">[namedLocation](namedLocation.md) collection</span></span> | <span data-ttu-id="14226-114">获取组织中的所有**namedLocation**对象。</span><span class="sxs-lookup"><span data-stu-id="14226-114">Get all the **namedLocation** objects in the organization.</span></span> |
| [<span data-ttu-id="14226-115">获取 namedLocation</span><span class="sxs-lookup"><span data-stu-id="14226-115">Get namedLocation</span></span>](../api/namedlocation-get.md) | [<span data-ttu-id="14226-116">namedLocation</span><span class="sxs-lookup"><span data-stu-id="14226-116">namedLocation</span></span>](namedlocation.md) | <span data-ttu-id="14226-117">读取**namedLocation**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="14226-117">Read the properties and relationships of a **namedLocation** object.</span></span> |
| [<span data-ttu-id="14226-118">删除 namedLocation</span><span class="sxs-lookup"><span data-stu-id="14226-118">Delete namedLocation</span></span>](../api/namedlocation-delete.md) | <span data-ttu-id="14226-119">无</span><span class="sxs-lookup"><span data-stu-id="14226-119">None</span></span> | <span data-ttu-id="14226-120">删除**namedLocation**对象。</span><span class="sxs-lookup"><span data-stu-id="14226-120">Delete a **namedLocation** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="14226-121">属性</span><span class="sxs-lookup"><span data-stu-id="14226-121">Properties</span></span>

| <span data-ttu-id="14226-122">属性</span><span class="sxs-lookup"><span data-stu-id="14226-122">Property</span></span>     | <span data-ttu-id="14226-123">类型</span><span class="sxs-lookup"><span data-stu-id="14226-123">Type</span></span>        | <span data-ttu-id="14226-124">说明</span><span class="sxs-lookup"><span data-stu-id="14226-124">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="14226-125">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="14226-125">createdDateTime</span></span>|<span data-ttu-id="14226-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="14226-126">DateTimeOffset</span></span>|<span data-ttu-id="14226-127">时间戳类型表示使用 ISO 8601 格式的位置的创建日期和时间，并且始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="14226-127">The Timestamp type represents creation date and time of the location using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="14226-128">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="14226-128">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="14226-129">只读。</span><span class="sxs-lookup"><span data-stu-id="14226-129">Read-only.</span></span>|
|<span data-ttu-id="14226-130">displayName</span><span class="sxs-lookup"><span data-stu-id="14226-130">displayName</span></span>|<span data-ttu-id="14226-131">String</span><span class="sxs-lookup"><span data-stu-id="14226-131">String</span></span>|<span data-ttu-id="14226-132">位置的人可读名称。</span><span class="sxs-lookup"><span data-stu-id="14226-132">Human-readable name of the location.</span></span>|
|<span data-ttu-id="14226-133">id</span><span class="sxs-lookup"><span data-stu-id="14226-133">id</span></span>|<span data-ttu-id="14226-134">String</span><span class="sxs-lookup"><span data-stu-id="14226-134">String</span></span>|<span data-ttu-id="14226-135">NamedLocation 对象的标识符。</span><span class="sxs-lookup"><span data-stu-id="14226-135">Identifier of a namedLocation object.</span></span> <span data-ttu-id="14226-136">只读。</span><span class="sxs-lookup"><span data-stu-id="14226-136">Read-only.</span></span>|
|<span data-ttu-id="14226-137">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="14226-137">modifiedDateTime</span></span>|<span data-ttu-id="14226-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="14226-138">DateTimeOffset</span></span>|<span data-ttu-id="14226-139">时间戳类型表示上次修改的位置使用 ISO 8601 格式的日期和时间，并且始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="14226-139">The Timestamp type represents last modified date and time of the location using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="14226-140">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="14226-140">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="14226-141">只读。</span><span class="sxs-lookup"><span data-stu-id="14226-141">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="14226-142">关系</span><span class="sxs-lookup"><span data-stu-id="14226-142">Relationships</span></span>

<span data-ttu-id="14226-143">无。</span><span class="sxs-lookup"><span data-stu-id="14226-143">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="14226-144">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="14226-144">JSON representation</span></span>

<span data-ttu-id="14226-145">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="14226-145">The following is a JSON representation of the resource.</span></span>

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

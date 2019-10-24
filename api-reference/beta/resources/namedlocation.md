---
title: namedLocation 资源类型
description: 这是表示 Azure Active Directory （名为 location）的基类。 "已命名位置" 是自定义规则，用于定义随后可在条件访问策略中使用的网络位置。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 3f1e0b7c86a8b2c026c44b46fd833594aadad5a9
ms.sourcegitcommit: d189830649794365464e37539e02239f883011da
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/24/2019
ms.locfileid: "37653851"
---
# <a name="namedlocation-resource-type"></a><span data-ttu-id="aea11-104">namedLocation 资源类型</span><span class="sxs-lookup"><span data-stu-id="aea11-104">namedLocation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aea11-105">这是表示 Azure Active Directory （名为 location）的基类。</span><span class="sxs-lookup"><span data-stu-id="aea11-105">This is the base class that represents an Azure Active Directory named location.</span></span> <span data-ttu-id="aea11-106">"已命名位置" 是自定义规则，用于定义随后可在条件访问策略中使用的网络位置。</span><span class="sxs-lookup"><span data-stu-id="aea11-106">Named locations are custom rules that define network locations which can then be used in a Conditional Access policy.</span></span>

## <a name="methods"></a><span data-ttu-id="aea11-107">方法</span><span class="sxs-lookup"><span data-stu-id="aea11-107">Methods</span></span>

| <span data-ttu-id="aea11-108">方法</span><span class="sxs-lookup"><span data-stu-id="aea11-108">Method</span></span>       | <span data-ttu-id="aea11-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="aea11-109">Return Type</span></span> | <span data-ttu-id="aea11-110">说明</span><span class="sxs-lookup"><span data-stu-id="aea11-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="aea11-111">列出 namedLocations</span><span class="sxs-lookup"><span data-stu-id="aea11-111">List namedLocations</span></span>](../api/conditionalaccessroot-list-namedlocations.md) | <span data-ttu-id="aea11-112">[namedLocation](namedLocation.md)集合</span><span class="sxs-lookup"><span data-stu-id="aea11-112">[namedLocation](namedLocation.md) collection</span></span> | <span data-ttu-id="aea11-113">获取组织中的所有**namedLocation**对象。</span><span class="sxs-lookup"><span data-stu-id="aea11-113">Get all the **namedLocation** objects in the organization.</span></span> |
| [<span data-ttu-id="aea11-114">获取 namedLocation</span><span class="sxs-lookup"><span data-stu-id="aea11-114">Get namedLocation</span></span>](../api/namedlocation-get.md) | [<span data-ttu-id="aea11-115">namedLocation</span><span class="sxs-lookup"><span data-stu-id="aea11-115">namedLocation</span></span>](namedlocation.md) | <span data-ttu-id="aea11-116">读取**namedLocation**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="aea11-116">Read the properties and relationships of a **namedLocation** object.</span></span> |
| [<span data-ttu-id="aea11-117">删除 namedLocation</span><span class="sxs-lookup"><span data-stu-id="aea11-117">Delete namedLocation</span></span>](../api/namedlocation-delete.md) | <span data-ttu-id="aea11-118">无</span><span class="sxs-lookup"><span data-stu-id="aea11-118">None</span></span> | <span data-ttu-id="aea11-119">删除**namedLocation**对象。</span><span class="sxs-lookup"><span data-stu-id="aea11-119">Delete a **namedLocation** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="aea11-120">属性</span><span class="sxs-lookup"><span data-stu-id="aea11-120">Properties</span></span>

| <span data-ttu-id="aea11-121">属性</span><span class="sxs-lookup"><span data-stu-id="aea11-121">Property</span></span>     | <span data-ttu-id="aea11-122">类型</span><span class="sxs-lookup"><span data-stu-id="aea11-122">Type</span></span>        | <span data-ttu-id="aea11-123">说明</span><span class="sxs-lookup"><span data-stu-id="aea11-123">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="aea11-124">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="aea11-124">createdDateTime</span></span>|<span data-ttu-id="aea11-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aea11-125">DateTimeOffset</span></span>|<span data-ttu-id="aea11-126">时间戳类型表示使用 ISO 8601 格式的位置的创建日期和时间，并且始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="aea11-126">The Timestamp type represents creation date and time of the location using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="aea11-127">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="aea11-127">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="aea11-128">只读。</span><span class="sxs-lookup"><span data-stu-id="aea11-128">Read-only.</span></span>|
|<span data-ttu-id="aea11-129">displayName</span><span class="sxs-lookup"><span data-stu-id="aea11-129">displayName</span></span>|<span data-ttu-id="aea11-130">String</span><span class="sxs-lookup"><span data-stu-id="aea11-130">String</span></span>|<span data-ttu-id="aea11-131">位置的人可读名称。</span><span class="sxs-lookup"><span data-stu-id="aea11-131">Human-readable name of the location.</span></span>|
|<span data-ttu-id="aea11-132">id</span><span class="sxs-lookup"><span data-stu-id="aea11-132">id</span></span>|<span data-ttu-id="aea11-133">String</span><span class="sxs-lookup"><span data-stu-id="aea11-133">String</span></span>|<span data-ttu-id="aea11-134">NamedLocation 对象的标识符。</span><span class="sxs-lookup"><span data-stu-id="aea11-134">Identifier of a namedLocation object.</span></span> <span data-ttu-id="aea11-135">只读。</span><span class="sxs-lookup"><span data-stu-id="aea11-135">Read-only.</span></span>|
|<span data-ttu-id="aea11-136">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="aea11-136">modifiedDateTime</span></span>|<span data-ttu-id="aea11-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aea11-137">DateTimeOffset</span></span>|<span data-ttu-id="aea11-138">时间戳类型表示上次修改的位置使用 ISO 8601 格式的日期和时间，并且始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="aea11-138">The Timestamp type represents last modified date and time of the location using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="aea11-139">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="aea11-139">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="aea11-140">只读。</span><span class="sxs-lookup"><span data-stu-id="aea11-140">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="aea11-141">关系</span><span class="sxs-lookup"><span data-stu-id="aea11-141">Relationships</span></span>

<span data-ttu-id="aea11-142">无。</span><span class="sxs-lookup"><span data-stu-id="aea11-142">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="aea11-143">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="aea11-143">JSON representation</span></span>

<span data-ttu-id="aea11-144">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="aea11-144">The following is a JSON representation of the resource.</span></span>

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

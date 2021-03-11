---
title: namedLocation 资源类型
description: 这是表示 Azure Active Directory 命名位置的基类。 命名位置是定义网络位置的自定义规则，这些位置随后可在条件访问策略中使用。
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: ae3ec6235259001a453bac50e45d2b142cdbaa8f
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722116"
---
# <a name="namedlocation-resource-type"></a><span data-ttu-id="07e65-104">namedLocation 资源类型</span><span class="sxs-lookup"><span data-stu-id="07e65-104">namedLocation resource type</span></span>

<span data-ttu-id="07e65-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="07e65-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="07e65-106">这是表示 Azure Active Directory 命名位置的基类。</span><span class="sxs-lookup"><span data-stu-id="07e65-106">This is the base class that represents an Azure Active Directory named location.</span></span> <span data-ttu-id="07e65-107">命名位置是定义网络位置的自定义规则，这些位置随后可在条件访问策略中使用。</span><span class="sxs-lookup"><span data-stu-id="07e65-107">Named locations are custom rules that define network locations which can then be used in a Conditional Access policy.</span></span>

## <a name="methods"></a><span data-ttu-id="07e65-108">方法</span><span class="sxs-lookup"><span data-stu-id="07e65-108">Methods</span></span>

| <span data-ttu-id="07e65-109">方法</span><span class="sxs-lookup"><span data-stu-id="07e65-109">Method</span></span>       | <span data-ttu-id="07e65-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="07e65-110">Return Type</span></span> | <span data-ttu-id="07e65-111">说明</span><span class="sxs-lookup"><span data-stu-id="07e65-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="07e65-112">列出 namedLocations</span><span class="sxs-lookup"><span data-stu-id="07e65-112">List namedLocations</span></span>](../api/conditionalaccessroot-list-namedlocations.md) | <span data-ttu-id="07e65-113">[namedLocation](namedLocation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="07e65-113">[namedLocation](namedLocation.md) collection</span></span> | <span data-ttu-id="07e65-114">获取 **组织的所有 namedLocation** 对象。</span><span class="sxs-lookup"><span data-stu-id="07e65-114">Get all the **namedLocation** objects in the organization.</span></span> |
| [<span data-ttu-id="07e65-115">获取 namedLocation</span><span class="sxs-lookup"><span data-stu-id="07e65-115">Get namedLocation</span></span>](../api/namedlocation-get.md) | [<span data-ttu-id="07e65-116">namedLocation</span><span class="sxs-lookup"><span data-stu-id="07e65-116">namedLocation</span></span>](namedlocation.md) | <span data-ttu-id="07e65-117">读取 **namedLocation** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="07e65-117">Read the properties and relationships of a **namedLocation** object.</span></span> |
| [<span data-ttu-id="07e65-118">删除 namedLocation</span><span class="sxs-lookup"><span data-stu-id="07e65-118">Delete namedLocation</span></span>](../api/namedlocation-delete.md) | <span data-ttu-id="07e65-119">无</span><span class="sxs-lookup"><span data-stu-id="07e65-119">None</span></span> | <span data-ttu-id="07e65-120">删除 **namedLocation** 对象。</span><span class="sxs-lookup"><span data-stu-id="07e65-120">Delete a **namedLocation** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="07e65-121">属性</span><span class="sxs-lookup"><span data-stu-id="07e65-121">Properties</span></span>

| <span data-ttu-id="07e65-122">属性</span><span class="sxs-lookup"><span data-stu-id="07e65-122">Property</span></span>     | <span data-ttu-id="07e65-123">类型</span><span class="sxs-lookup"><span data-stu-id="07e65-123">Type</span></span>        | <span data-ttu-id="07e65-124">说明</span><span class="sxs-lookup"><span data-stu-id="07e65-124">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="07e65-125">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="07e65-125">createdDateTime</span></span>|<span data-ttu-id="07e65-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="07e65-126">DateTimeOffset</span></span>|<span data-ttu-id="07e65-127">时间戳类型表示使用 ISO 8601 格式的位置的创建日期和时间，并且始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="07e65-127">The Timestamp type represents creation date and time of the location using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="07e65-128">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。</span><span class="sxs-lookup"><span data-stu-id="07e65-128">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="07e65-129">只读。</span><span class="sxs-lookup"><span data-stu-id="07e65-129">Read-only.</span></span>|
|<span data-ttu-id="07e65-130">displayName</span><span class="sxs-lookup"><span data-stu-id="07e65-130">displayName</span></span>|<span data-ttu-id="07e65-131">String</span><span class="sxs-lookup"><span data-stu-id="07e65-131">String</span></span>|<span data-ttu-id="07e65-132">位置的可读名称。</span><span class="sxs-lookup"><span data-stu-id="07e65-132">Human-readable name of the location.</span></span>|
|<span data-ttu-id="07e65-133">id</span><span class="sxs-lookup"><span data-stu-id="07e65-133">id</span></span>|<span data-ttu-id="07e65-134">String</span><span class="sxs-lookup"><span data-stu-id="07e65-134">String</span></span>|<span data-ttu-id="07e65-135">namedLocation 对象的标识符。</span><span class="sxs-lookup"><span data-stu-id="07e65-135">Identifier of a namedLocation object.</span></span> <span data-ttu-id="07e65-136">只读。</span><span class="sxs-lookup"><span data-stu-id="07e65-136">Read-only.</span></span>|
|<span data-ttu-id="07e65-137">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="07e65-137">modifiedDateTime</span></span>|<span data-ttu-id="07e65-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="07e65-138">DateTimeOffset</span></span>|<span data-ttu-id="07e65-139">时间戳类型表示使用 ISO 8601 格式的位置的上次修改日期和时间，并且始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="07e65-139">The Timestamp type represents last modified date and time of the location using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="07e65-140">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。</span><span class="sxs-lookup"><span data-stu-id="07e65-140">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="07e65-141">只读。</span><span class="sxs-lookup"><span data-stu-id="07e65-141">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="07e65-142">关系</span><span class="sxs-lookup"><span data-stu-id="07e65-142">Relationships</span></span>

<span data-ttu-id="07e65-143">无。</span><span class="sxs-lookup"><span data-stu-id="07e65-143">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="07e65-144">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="07e65-144">JSON representation</span></span>

<span data-ttu-id="07e65-145">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="07e65-145">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.namedLocation",
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



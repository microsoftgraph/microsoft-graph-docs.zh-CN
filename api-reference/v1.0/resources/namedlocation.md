---
title: namedLocation 资源类型
description: 这是表示 Azure Active Directory 命名位置的基类。 命名位置是定义网络位置的自定义规则，这些位置随后可在条件访问策略中使用。
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 9a454855a5f1048ddfeab89c85be25e02a26f82b
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721906"
---
# <a name="namedlocation-resource-type"></a><span data-ttu-id="e33b0-104">namedLocation 资源类型</span><span class="sxs-lookup"><span data-stu-id="e33b0-104">namedLocation resource type</span></span>

<span data-ttu-id="e33b0-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e33b0-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e33b0-106">这是表示 Azure Active Directory 命名位置的基类。</span><span class="sxs-lookup"><span data-stu-id="e33b0-106">This is the base class that represents an Azure Active Directory named location.</span></span> <span data-ttu-id="e33b0-107">命名位置是定义网络位置的自定义规则，这些位置随后可在条件访问策略中使用。</span><span class="sxs-lookup"><span data-stu-id="e33b0-107">Named locations are custom rules that define network locations which can then be used in a Conditional Access policy.</span></span>

## <a name="methods"></a><span data-ttu-id="e33b0-108">Methods</span><span class="sxs-lookup"><span data-stu-id="e33b0-108">Methods</span></span>

| <span data-ttu-id="e33b0-109">方法</span><span class="sxs-lookup"><span data-stu-id="e33b0-109">Method</span></span>       | <span data-ttu-id="e33b0-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="e33b0-110">Return Type</span></span> | <span data-ttu-id="e33b0-111">说明</span><span class="sxs-lookup"><span data-stu-id="e33b0-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="e33b0-112">列出 namedLocations</span><span class="sxs-lookup"><span data-stu-id="e33b0-112">List namedLocations</span></span>](../api/conditionalaccessroot-list-namedlocations.md) | <span data-ttu-id="e33b0-113">[namedLocation](namedLocation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e33b0-113">[namedLocation](namedLocation.md) collection</span></span> | <span data-ttu-id="e33b0-114">获取 **组织的所有 namedLocation** 对象。</span><span class="sxs-lookup"><span data-stu-id="e33b0-114">Get all the **namedLocation** objects in the organization.</span></span> |
| [<span data-ttu-id="e33b0-115">获取 namedLocation</span><span class="sxs-lookup"><span data-stu-id="e33b0-115">Get namedLocation</span></span>](../api/namedlocation-get.md) | [<span data-ttu-id="e33b0-116">namedLocation</span><span class="sxs-lookup"><span data-stu-id="e33b0-116">namedLocation</span></span>](namedlocation.md) | <span data-ttu-id="e33b0-117">读取 **namedLocation** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e33b0-117">Read the properties and relationships of a **namedLocation** object.</span></span> |
| [<span data-ttu-id="e33b0-118">删除 namedLocation</span><span class="sxs-lookup"><span data-stu-id="e33b0-118">Delete namedLocation</span></span>](../api/namedlocation-delete.md) | <span data-ttu-id="e33b0-119">无</span><span class="sxs-lookup"><span data-stu-id="e33b0-119">None</span></span> | <span data-ttu-id="e33b0-120">删除 **namedLocation** 对象。</span><span class="sxs-lookup"><span data-stu-id="e33b0-120">Delete a **namedLocation** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="e33b0-121">属性</span><span class="sxs-lookup"><span data-stu-id="e33b0-121">Properties</span></span>

| <span data-ttu-id="e33b0-122">属性</span><span class="sxs-lookup"><span data-stu-id="e33b0-122">Property</span></span>     | <span data-ttu-id="e33b0-123">类型</span><span class="sxs-lookup"><span data-stu-id="e33b0-123">Type</span></span>        | <span data-ttu-id="e33b0-124">说明</span><span class="sxs-lookup"><span data-stu-id="e33b0-124">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e33b0-125">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e33b0-125">createdDateTime</span></span>|<span data-ttu-id="e33b0-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e33b0-126">DateTimeOffset</span></span>|<span data-ttu-id="e33b0-127">时间戳类型表示使用 ISO 8601 格式的位置的创建日期和时间，并且始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="e33b0-127">The Timestamp type represents creation date and time of the location using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="e33b0-128">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。</span><span class="sxs-lookup"><span data-stu-id="e33b0-128">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="e33b0-129">只读。</span><span class="sxs-lookup"><span data-stu-id="e33b0-129">Read-only.</span></span>|
|<span data-ttu-id="e33b0-130">displayName</span><span class="sxs-lookup"><span data-stu-id="e33b0-130">displayName</span></span>|<span data-ttu-id="e33b0-131">字符串</span><span class="sxs-lookup"><span data-stu-id="e33b0-131">String</span></span>|<span data-ttu-id="e33b0-132">位置的可读名称。</span><span class="sxs-lookup"><span data-stu-id="e33b0-132">Human-readable name of the location.</span></span>|
|<span data-ttu-id="e33b0-133">id</span><span class="sxs-lookup"><span data-stu-id="e33b0-133">id</span></span>|<span data-ttu-id="e33b0-134">字符串</span><span class="sxs-lookup"><span data-stu-id="e33b0-134">String</span></span>|<span data-ttu-id="e33b0-135">namedLocation 对象的标识符。</span><span class="sxs-lookup"><span data-stu-id="e33b0-135">Identifier of a namedLocation object.</span></span> <span data-ttu-id="e33b0-136">只读。</span><span class="sxs-lookup"><span data-stu-id="e33b0-136">Read-only.</span></span>|
|<span data-ttu-id="e33b0-137">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e33b0-137">modifiedDateTime</span></span>|<span data-ttu-id="e33b0-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e33b0-138">DateTimeOffset</span></span>|<span data-ttu-id="e33b0-139">时间戳类型表示使用 ISO 8601 格式的位置的上次修改日期和时间，并且始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="e33b0-139">The Timestamp type represents last modified date and time of the location using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="e33b0-140">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。</span><span class="sxs-lookup"><span data-stu-id="e33b0-140">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="e33b0-141">只读。</span><span class="sxs-lookup"><span data-stu-id="e33b0-141">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e33b0-142">关系</span><span class="sxs-lookup"><span data-stu-id="e33b0-142">Relationships</span></span>

<span data-ttu-id="e33b0-143">无。</span><span class="sxs-lookup"><span data-stu-id="e33b0-143">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e33b0-144">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e33b0-144">JSON representation</span></span>

<span data-ttu-id="e33b0-145">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e33b0-145">The following is a JSON representation of the resource.</span></span>

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


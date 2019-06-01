---
title: subscribedSku 资源类型
description: 包含有关公司订阅的服务 SKU 的信息。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 9ed1a9dc5b12cf1e3b3a01b31d7a990fa7fd562c
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/31/2019
ms.locfileid: "34656466"
---
# <a name="subscribedsku-resource-type"></a><span data-ttu-id="e5053-103">subscribedSku 资源类型</span><span class="sxs-lookup"><span data-stu-id="e5053-103">subscribedSku resource type</span></span>

<span data-ttu-id="e5053-104">包含有关公司订阅的服务 SKU 的信息。</span><span class="sxs-lookup"><span data-stu-id="e5053-104">Contains information about a service SKU that a company is subscribed to.</span></span>

<span data-ttu-id="e5053-p101">只支持在订阅的 SKU 上执行读取操作；不支持执行创建、更新和删除操作。不支持查询筛选表达式。继承自 [directoryObject](directoryobject.md)。</span><span class="sxs-lookup"><span data-stu-id="e5053-p101">Only the read operation is supported on subscribed SKUs; create, update, and delete are not supported. Query filter expressions are not supported. Inherits from [directoryObject](directoryobject.md).</span></span>

## <a name="methods"></a><span data-ttu-id="e5053-108">方法</span><span class="sxs-lookup"><span data-stu-id="e5053-108">Methods</span></span>
| <span data-ttu-id="e5053-109">方法</span><span class="sxs-lookup"><span data-stu-id="e5053-109">Method</span></span>           | <span data-ttu-id="e5053-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="e5053-110">Return Type</span></span>    |<span data-ttu-id="e5053-111">说明</span><span class="sxs-lookup"><span data-stu-id="e5053-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e5053-112">获取 subscribedSku</span><span class="sxs-lookup"><span data-stu-id="e5053-112">Get subscribedSku</span></span>](../api/subscribedsku-get.md) | [<span data-ttu-id="e5053-113">subscribedSku</span><span class="sxs-lookup"><span data-stu-id="e5053-113">subscribedSku</span></span>](subscribedsku.md) |<span data-ttu-id="e5053-114">读取 subscribedSku 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e5053-114">Read properties and relationships of subscribedSku object.</span></span>|
|[<span data-ttu-id="e5053-115">列出 subscribedsku</span><span class="sxs-lookup"><span data-stu-id="e5053-115">List subscribedsku</span></span>](../api/subscribedsku-list.md) | <span data-ttu-id="e5053-116">[subscribedSku](subscribedsku.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e5053-116">[subscribedSku](subscribedsku.md) collection</span></span> |<span data-ttu-id="e5053-117">检索组织已获取的商业订阅列表。</span><span class="sxs-lookup"><span data-stu-id="e5053-117">Retrieve the list of commercial subscriptions that an organization has acquired.</span></span>|

## <a name="properties"></a><span data-ttu-id="e5053-118">属性</span><span class="sxs-lookup"><span data-stu-id="e5053-118">Properties</span></span>
| <span data-ttu-id="e5053-119">属性</span><span class="sxs-lookup"><span data-stu-id="e5053-119">Property</span></span>     | <span data-ttu-id="e5053-120">类型</span><span class="sxs-lookup"><span data-stu-id="e5053-120">Type</span></span>   |<span data-ttu-id="e5053-121">说明</span><span class="sxs-lookup"><span data-stu-id="e5053-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e5053-122">appliesTo</span><span class="sxs-lookup"><span data-stu-id="e5053-122">appliesTo</span></span>|<span data-ttu-id="e5053-123">String</span><span class="sxs-lookup"><span data-stu-id="e5053-123">String</span></span>| <span data-ttu-id="e5053-124">例如，“用户”或“公司”。</span><span class="sxs-lookup"><span data-stu-id="e5053-124">For example, "User" or "Company".</span></span> |
|<span data-ttu-id="e5053-125">capabilityStatus</span><span class="sxs-lookup"><span data-stu-id="e5053-125">capabilityStatus</span></span>|<span data-ttu-id="e5053-126">String</span><span class="sxs-lookup"><span data-stu-id="e5053-126">String</span></span>| <span data-ttu-id="e5053-127">例如, "Enabled"。</span><span class="sxs-lookup"><span data-stu-id="e5053-127">For example, "Enabled".</span></span> |
|<span data-ttu-id="e5053-128">consumedUnits</span><span class="sxs-lookup"><span data-stu-id="e5053-128">consumedUnits</span></span>|<span data-ttu-id="e5053-129">Int32</span><span class="sxs-lookup"><span data-stu-id="e5053-129">Int32</span></span>| <span data-ttu-id="e5053-130">已分配的许可证数量。</span><span class="sxs-lookup"><span data-stu-id="e5053-130">The number of licenses that have been assigned.</span></span> |
|<span data-ttu-id="e5053-131">id</span><span class="sxs-lookup"><span data-stu-id="e5053-131">id</span></span>|<span data-ttu-id="e5053-132">String</span><span class="sxs-lookup"><span data-stu-id="e5053-132">String</span></span>| <span data-ttu-id="e5053-133">订阅的 sku 对象的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="e5053-133">The unique identifier for the subscribed sku object.</span></span> <span data-ttu-id="e5053-134">键, 不可为 null。</span><span class="sxs-lookup"><span data-stu-id="e5053-134">Key, not nullable.</span></span> |
|<span data-ttu-id="e5053-135">prepaidUnits</span><span class="sxs-lookup"><span data-stu-id="e5053-135">prepaidUnits</span></span>|[<span data-ttu-id="e5053-136">licenseUnitsDetail</span><span class="sxs-lookup"><span data-stu-id="e5053-136">licenseUnitsDetail</span></span>](licenseunitsdetail.md)| <span data-ttu-id="e5053-137">有关预付许可证的数量和状态的信息。</span><span class="sxs-lookup"><span data-stu-id="e5053-137">Information about the number and status of prepaid licenses.</span></span> |
|<span data-ttu-id="e5053-138">servicePlans</span><span class="sxs-lookup"><span data-stu-id="e5053-138">servicePlans</span></span>|<span data-ttu-id="e5053-139">[servicePlanInfo](serviceplaninfo.md) collection</span><span class="sxs-lookup"><span data-stu-id="e5053-139">[servicePlanInfo](serviceplaninfo.md) collection</span></span>| <span data-ttu-id="e5053-140">有关 SKU 可用服务计划的信息。</span><span class="sxs-lookup"><span data-stu-id="e5053-140">Information about the service plans that are available with the SKU.</span></span> <span data-ttu-id="e5053-141">不可为 null</span><span class="sxs-lookup"><span data-stu-id="e5053-141">Not nullable</span></span> |
|<span data-ttu-id="e5053-142">skuId</span><span class="sxs-lookup"><span data-stu-id="e5053-142">skuId</span></span>|<span data-ttu-id="e5053-143">Guid</span><span class="sxs-lookup"><span data-stu-id="e5053-143">Guid</span></span>| <span data-ttu-id="e5053-144">服务 SKU 的唯一标识符 (GUID)。</span><span class="sxs-lookup"><span data-stu-id="e5053-144">The unique identifier (GUID) for the service SKU.</span></span> |
|<span data-ttu-id="e5053-145">skuPartNumber</span><span class="sxs-lookup"><span data-stu-id="e5053-145">skuPartNumber</span></span>|<span data-ttu-id="e5053-146">String</span><span class="sxs-lookup"><span data-stu-id="e5053-146">String</span></span>| <span data-ttu-id="e5053-147">SKU 商品编号；例如：“AAD_PREMIUM”或“RMSBASIC”。</span><span class="sxs-lookup"><span data-stu-id="e5053-147">The SKU part number; for example: "AAD_PREMIUM" or "RMSBASIC".</span></span> |

## <a name="relationships"></a><span data-ttu-id="e5053-148">关系</span><span class="sxs-lookup"><span data-stu-id="e5053-148">Relationships</span></span>
<span data-ttu-id="e5053-149">无</span><span class="sxs-lookup"><span data-stu-id="e5053-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e5053-150">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e5053-150">JSON representation</span></span>

<span data-ttu-id="e5053-151">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e5053-151">Here is a JSON representation of the resource</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.subscribedSku",
  "@odata.annotations": [
    {
      "capabilities": {
        "skippable": false,
        "toppable": false,
        "countable": false,
        "expandable": false,
        "filterable": false,
        "referenceable": false,
        "selectable": false
      }
    }
  ]
}-->

```json
{
  "appliesTo": "string",
  "capabilityStatus": "string",
  "consumedUnits": 1024,
  "id": "string (identifier)",
  "prepaidUnits": {"@odata.type": "microsoft.graph.licenseUnitsDetail"},
  "servicePlans": [{"@odata.type": "microsoft.graph.servicePlanInfo"}],
  "skuId": "guid",
  "skuPartNumber": "string"
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "subscribedSku resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

---
title: subscribedSku 资源类型
description: 包含有关公司订阅的服务 SKU 的信息。
localization_priority: Normal
author: SumitParikh
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: b0dbb255bced328b6b3d40e675ee53e6cf3fbece
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48094153"
---
# <a name="subscribedsku-resource-type"></a><span data-ttu-id="e07cf-103">subscribedSku 资源类型</span><span class="sxs-lookup"><span data-stu-id="e07cf-103">subscribedSku resource type</span></span>

<span data-ttu-id="e07cf-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e07cf-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e07cf-105">包含有关公司订阅的服务 SKU 的信息。</span><span class="sxs-lookup"><span data-stu-id="e07cf-105">Contains information about a service SKU that a company is subscribed to.</span></span>

<span data-ttu-id="e07cf-p101">只支持在订阅的 SKU 上执行读取操作；不支持执行创建、更新和删除操作。不支持查询筛选表达式。继承自 [directoryObject](directoryobject.md)。</span><span class="sxs-lookup"><span data-stu-id="e07cf-p101">Only the read operation is supported on subscribed SKUs; create, update, and delete are not supported. Query filter expressions are not supported. Inherits from [directoryObject](directoryobject.md).</span></span>

## <a name="methods"></a><span data-ttu-id="e07cf-109">方法</span><span class="sxs-lookup"><span data-stu-id="e07cf-109">Methods</span></span>
| <span data-ttu-id="e07cf-110">方法</span><span class="sxs-lookup"><span data-stu-id="e07cf-110">Method</span></span>           | <span data-ttu-id="e07cf-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="e07cf-111">Return Type</span></span>    |<span data-ttu-id="e07cf-112">说明</span><span class="sxs-lookup"><span data-stu-id="e07cf-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e07cf-113">获取 subscribedSku</span><span class="sxs-lookup"><span data-stu-id="e07cf-113">Get subscribedSku</span></span>](../api/subscribedsku-get.md) | [<span data-ttu-id="e07cf-114">subscribedSku</span><span class="sxs-lookup"><span data-stu-id="e07cf-114">subscribedSku</span></span>](subscribedsku.md) |<span data-ttu-id="e07cf-115">获取组织已获取的特定商业订阅。</span><span class="sxs-lookup"><span data-stu-id="e07cf-115">Get a specific commercial subscription that an organization has acquired.</span></span>|
|[<span data-ttu-id="e07cf-116">列出 subscribedsku</span><span class="sxs-lookup"><span data-stu-id="e07cf-116">List subscribedsku</span></span>](../api/subscribedsku-list.md) | <span data-ttu-id="e07cf-117">[subscribedSku](subscribedsku.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e07cf-117">[subscribedSku](subscribedsku.md) collection</span></span> |<span data-ttu-id="e07cf-118">获取组织已获取的商业版订阅的列表。</span><span class="sxs-lookup"><span data-stu-id="e07cf-118">Get the list of commercial subscriptions that an organization has acquired.</span></span>|

## <a name="properties"></a><span data-ttu-id="e07cf-119">属性</span><span class="sxs-lookup"><span data-stu-id="e07cf-119">Properties</span></span>
| <span data-ttu-id="e07cf-120">属性</span><span class="sxs-lookup"><span data-stu-id="e07cf-120">Property</span></span>     | <span data-ttu-id="e07cf-121">类型</span><span class="sxs-lookup"><span data-stu-id="e07cf-121">Type</span></span>   |<span data-ttu-id="e07cf-122">说明</span><span class="sxs-lookup"><span data-stu-id="e07cf-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e07cf-123">appliesTo</span><span class="sxs-lookup"><span data-stu-id="e07cf-123">appliesTo</span></span>|<span data-ttu-id="e07cf-124">String</span><span class="sxs-lookup"><span data-stu-id="e07cf-124">String</span></span>| <span data-ttu-id="e07cf-125">例如，“用户”或“公司”。</span><span class="sxs-lookup"><span data-stu-id="e07cf-125">For example, "User" or "Company".</span></span> |
|<span data-ttu-id="e07cf-126">capabilityStatus</span><span class="sxs-lookup"><span data-stu-id="e07cf-126">capabilityStatus</span></span>|<span data-ttu-id="e07cf-127">String</span><span class="sxs-lookup"><span data-stu-id="e07cf-127">String</span></span>|  <span data-ttu-id="e07cf-128">可取值为：`Enabled`、`Warning`、`Suspended`、`Deleted`、`LockedOut`。</span><span class="sxs-lookup"><span data-stu-id="e07cf-128">Possible values are: `Enabled`, `Warning`, `Suspended`, `Deleted`, `LockedOut`.</span></span> |
|<span data-ttu-id="e07cf-129">consumedUnits</span><span class="sxs-lookup"><span data-stu-id="e07cf-129">consumedUnits</span></span>|<span data-ttu-id="e07cf-130">Int32</span><span class="sxs-lookup"><span data-stu-id="e07cf-130">Int32</span></span>| <span data-ttu-id="e07cf-131">已分配的许可证数量。</span><span class="sxs-lookup"><span data-stu-id="e07cf-131">The number of licenses that have been assigned.</span></span> |
|<span data-ttu-id="e07cf-132">id</span><span class="sxs-lookup"><span data-stu-id="e07cf-132">id</span></span>|<span data-ttu-id="e07cf-133">String</span><span class="sxs-lookup"><span data-stu-id="e07cf-133">String</span></span>| <span data-ttu-id="e07cf-134">订阅的 sku 对象的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="e07cf-134">The unique identifier for the subscribed sku object.</span></span> <span data-ttu-id="e07cf-135">键，不可为 null。</span><span class="sxs-lookup"><span data-stu-id="e07cf-135">Key, not nullable.</span></span> |
|<span data-ttu-id="e07cf-136">prepaidUnits</span><span class="sxs-lookup"><span data-stu-id="e07cf-136">prepaidUnits</span></span>|[<span data-ttu-id="e07cf-137">licenseUnitsDetail</span><span class="sxs-lookup"><span data-stu-id="e07cf-137">licenseUnitsDetail</span></span>](licenseunitsdetail.md)| <span data-ttu-id="e07cf-138">有关预付许可证的数量和状态的信息。</span><span class="sxs-lookup"><span data-stu-id="e07cf-138">Information about the number and status of prepaid licenses.</span></span> |
|<span data-ttu-id="e07cf-139">servicePlans</span><span class="sxs-lookup"><span data-stu-id="e07cf-139">servicePlans</span></span>|<span data-ttu-id="e07cf-140">[servicePlanInfo](serviceplaninfo.md) collection</span><span class="sxs-lookup"><span data-stu-id="e07cf-140">[servicePlanInfo](serviceplaninfo.md) collection</span></span>| <span data-ttu-id="e07cf-141">有关 SKU 可用服务计划的信息。</span><span class="sxs-lookup"><span data-stu-id="e07cf-141">Information about the service plans that are available with the SKU.</span></span> <span data-ttu-id="e07cf-142">不可为 null</span><span class="sxs-lookup"><span data-stu-id="e07cf-142">Not nullable</span></span> |
|<span data-ttu-id="e07cf-143">skuId</span><span class="sxs-lookup"><span data-stu-id="e07cf-143">skuId</span></span>|<span data-ttu-id="e07cf-144">Guid</span><span class="sxs-lookup"><span data-stu-id="e07cf-144">Guid</span></span>| <span data-ttu-id="e07cf-145">服务 SKU 的唯一标识符 (GUID)。</span><span class="sxs-lookup"><span data-stu-id="e07cf-145">The unique identifier (GUID) for the service SKU.</span></span> |
|<span data-ttu-id="e07cf-146">skuPartNumber</span><span class="sxs-lookup"><span data-stu-id="e07cf-146">skuPartNumber</span></span>|<span data-ttu-id="e07cf-147">String</span><span class="sxs-lookup"><span data-stu-id="e07cf-147">String</span></span>| <span data-ttu-id="e07cf-148">SKU 商品编号；例如：“AAD_PREMIUM”或“RMSBASIC”。</span><span class="sxs-lookup"><span data-stu-id="e07cf-148">The SKU part number; for example: "AAD_PREMIUM" or "RMSBASIC".</span></span> <span data-ttu-id="e07cf-149">若要获取组织获取的商业订阅的列表，请参阅 [List subscribedsku](../api/subscribedsku-list.md)。</span><span class="sxs-lookup"><span data-stu-id="e07cf-149">To get a list of commercial subscriptions that an organization has acquired, see [List subscribedSkus](../api/subscribedsku-list.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="e07cf-150">关系</span><span class="sxs-lookup"><span data-stu-id="e07cf-150">Relationships</span></span>
<span data-ttu-id="e07cf-151">无</span><span class="sxs-lookup"><span data-stu-id="e07cf-151">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e07cf-152">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e07cf-152">JSON representation</span></span>

<span data-ttu-id="e07cf-153">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e07cf-153">Here is a JSON representation of the resource</span></span>

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


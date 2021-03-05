---
title: subscribedSku 资源类型
description: 包含有关公司订阅的服务 SKU 的信息。
localization_priority: Normal
author: SumitParikh
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: d3a5ea5a5792f1e55e3f5d1ff9b053b35eadd2aa
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50432830"
---
# <a name="subscribedsku-resource-type"></a><span data-ttu-id="cfd8d-103">subscribedSku 资源类型</span><span class="sxs-lookup"><span data-stu-id="cfd8d-103">subscribedSku resource type</span></span>

<span data-ttu-id="cfd8d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cfd8d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="cfd8d-105">包含有关公司订阅的服务 SKU 的信息。</span><span class="sxs-lookup"><span data-stu-id="cfd8d-105">Contains information about a service SKU that a company is subscribed to.</span></span>

<span data-ttu-id="cfd8d-p101">只支持在订阅的 SKU 上执行读取操作；不支持执行创建、更新和删除操作。不支持查询筛选表达式。继承自 [directoryObject](directoryobject.md)。</span><span class="sxs-lookup"><span data-stu-id="cfd8d-p101">Only the read operation is supported on subscribed SKUs; create, update, and delete are not supported. Query filter expressions are not supported. Inherits from [directoryObject](directoryobject.md).</span></span>

## <a name="methods"></a><span data-ttu-id="cfd8d-109">Methods</span><span class="sxs-lookup"><span data-stu-id="cfd8d-109">Methods</span></span>
| <span data-ttu-id="cfd8d-110">方法</span><span class="sxs-lookup"><span data-stu-id="cfd8d-110">Method</span></span>           | <span data-ttu-id="cfd8d-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="cfd8d-111">Return Type</span></span>    |<span data-ttu-id="cfd8d-112">说明</span><span class="sxs-lookup"><span data-stu-id="cfd8d-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="cfd8d-113">获取 subscribedSku</span><span class="sxs-lookup"><span data-stu-id="cfd8d-113">Get subscribedSku</span></span>](../api/subscribedsku-get.md) | [<span data-ttu-id="cfd8d-114">subscribedSku</span><span class="sxs-lookup"><span data-stu-id="cfd8d-114">subscribedSku</span></span>](subscribedsku.md) |<span data-ttu-id="cfd8d-115">获取组织已获取的特定商业订阅。</span><span class="sxs-lookup"><span data-stu-id="cfd8d-115">Get a specific commercial subscription that an organization has acquired.</span></span>|
|[<span data-ttu-id="cfd8d-116">列出 subscribedsku</span><span class="sxs-lookup"><span data-stu-id="cfd8d-116">List subscribedsku</span></span>](../api/subscribedsku-list.md) | <span data-ttu-id="cfd8d-117">[subscribedSku](subscribedsku.md) 集合</span><span class="sxs-lookup"><span data-stu-id="cfd8d-117">[subscribedSku](subscribedsku.md) collection</span></span> |<span data-ttu-id="cfd8d-118">获取组织已获取的商业版订阅的列表。</span><span class="sxs-lookup"><span data-stu-id="cfd8d-118">Get the list of commercial subscriptions that an organization has acquired.</span></span>|

## <a name="properties"></a><span data-ttu-id="cfd8d-119">属性</span><span class="sxs-lookup"><span data-stu-id="cfd8d-119">Properties</span></span>
| <span data-ttu-id="cfd8d-120">属性</span><span class="sxs-lookup"><span data-stu-id="cfd8d-120">Property</span></span>     | <span data-ttu-id="cfd8d-121">类型</span><span class="sxs-lookup"><span data-stu-id="cfd8d-121">Type</span></span>   |<span data-ttu-id="cfd8d-122">说明</span><span class="sxs-lookup"><span data-stu-id="cfd8d-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cfd8d-123">appliesTo</span><span class="sxs-lookup"><span data-stu-id="cfd8d-123">appliesTo</span></span>|<span data-ttu-id="cfd8d-124">String</span><span class="sxs-lookup"><span data-stu-id="cfd8d-124">String</span></span>| <span data-ttu-id="cfd8d-125">例如，“用户”或“公司”。</span><span class="sxs-lookup"><span data-stu-id="cfd8d-125">For example, "User" or "Company".</span></span> |
|<span data-ttu-id="cfd8d-126">capabilityStatus</span><span class="sxs-lookup"><span data-stu-id="cfd8d-126">capabilityStatus</span></span>|<span data-ttu-id="cfd8d-127">String</span><span class="sxs-lookup"><span data-stu-id="cfd8d-127">String</span></span>|  <span data-ttu-id="cfd8d-128">可取值为：`Enabled`、`Warning`、`Suspended`、`Deleted`、`LockedOut`。</span><span class="sxs-lookup"><span data-stu-id="cfd8d-128">Possible values are: `Enabled`, `Warning`, `Suspended`, `Deleted`, `LockedOut`.</span></span> |
|<span data-ttu-id="cfd8d-129">consumedUnits</span><span class="sxs-lookup"><span data-stu-id="cfd8d-129">consumedUnits</span></span>|<span data-ttu-id="cfd8d-130">Int32</span><span class="sxs-lookup"><span data-stu-id="cfd8d-130">Int32</span></span>| <span data-ttu-id="cfd8d-131">已分配的许可证数量。</span><span class="sxs-lookup"><span data-stu-id="cfd8d-131">The number of licenses that have been assigned.</span></span> |
|<span data-ttu-id="cfd8d-132">id</span><span class="sxs-lookup"><span data-stu-id="cfd8d-132">id</span></span>|<span data-ttu-id="cfd8d-133">String</span><span class="sxs-lookup"><span data-stu-id="cfd8d-133">String</span></span>| <span data-ttu-id="cfd8d-134">订阅的 sku 对象的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="cfd8d-134">The unique identifier for the subscribed sku object.</span></span> <span data-ttu-id="cfd8d-135">键，不可为 null。</span><span class="sxs-lookup"><span data-stu-id="cfd8d-135">Key, not nullable.</span></span> |
|<span data-ttu-id="cfd8d-136">prepaidUnits</span><span class="sxs-lookup"><span data-stu-id="cfd8d-136">prepaidUnits</span></span>|[<span data-ttu-id="cfd8d-137">licenseUnitsDetail</span><span class="sxs-lookup"><span data-stu-id="cfd8d-137">licenseUnitsDetail</span></span>](licenseunitsdetail.md)| <span data-ttu-id="cfd8d-138">有关预付许可证的数量和状态的信息。</span><span class="sxs-lookup"><span data-stu-id="cfd8d-138">Information about the number and status of prepaid licenses.</span></span> |
|<span data-ttu-id="cfd8d-139">servicePlans</span><span class="sxs-lookup"><span data-stu-id="cfd8d-139">servicePlans</span></span>|<span data-ttu-id="cfd8d-140">[servicePlanInfo](serviceplaninfo.md) collection</span><span class="sxs-lookup"><span data-stu-id="cfd8d-140">[servicePlanInfo](serviceplaninfo.md) collection</span></span>| <span data-ttu-id="cfd8d-141">有关 SKU 可用服务计划的信息。</span><span class="sxs-lookup"><span data-stu-id="cfd8d-141">Information about the service plans that are available with the SKU.</span></span> <span data-ttu-id="cfd8d-142">不可为 null</span><span class="sxs-lookup"><span data-stu-id="cfd8d-142">Not nullable</span></span> |
|<span data-ttu-id="cfd8d-143">skuId</span><span class="sxs-lookup"><span data-stu-id="cfd8d-143">skuId</span></span>|<span data-ttu-id="cfd8d-144">Guid</span><span class="sxs-lookup"><span data-stu-id="cfd8d-144">Guid</span></span>| <span data-ttu-id="cfd8d-145">服务 SKU 的唯一标识符 (GUID)。</span><span class="sxs-lookup"><span data-stu-id="cfd8d-145">The unique identifier (GUID) for the service SKU.</span></span> |
|<span data-ttu-id="cfd8d-146">skuPartNumber</span><span class="sxs-lookup"><span data-stu-id="cfd8d-146">skuPartNumber</span></span>|<span data-ttu-id="cfd8d-147">String</span><span class="sxs-lookup"><span data-stu-id="cfd8d-147">String</span></span>| <span data-ttu-id="cfd8d-148">SKU 商品编号；例如：“AAD_PREMIUM”或“RMSBASIC”。</span><span class="sxs-lookup"><span data-stu-id="cfd8d-148">The SKU part number; for example: "AAD_PREMIUM" or "RMSBASIC".</span></span> <span data-ttu-id="cfd8d-149">若要获取组织已获取的商业订阅的列表，请参阅[List subscribedSkus。](../api/subscribedsku-list.md)</span><span class="sxs-lookup"><span data-stu-id="cfd8d-149">To get a list of commercial subscriptions that an organization has acquired, see [List subscribedSkus](../api/subscribedsku-list.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="cfd8d-150">关系</span><span class="sxs-lookup"><span data-stu-id="cfd8d-150">Relationships</span></span>
<span data-ttu-id="cfd8d-151">无</span><span class="sxs-lookup"><span data-stu-id="cfd8d-151">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cfd8d-152">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cfd8d-152">JSON representation</span></span>

<span data-ttu-id="cfd8d-153">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cfd8d-153">Here is a JSON representation of the resource</span></span>

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


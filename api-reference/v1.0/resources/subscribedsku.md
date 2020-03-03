---
title: subscribedSku 资源类型
description: 包含有关公司订阅的服务 SKU 的信息。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: bcd9e9b9cf32b3bfc35c5c10cb43a2a748b32041
ms.sourcegitcommit: d3b6e4d11012e6b4c775afcec4fe5444e3a99bd3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/03/2020
ms.locfileid: "42394615"
---
# <a name="subscribedsku-resource-type"></a><span data-ttu-id="f034f-103">subscribedSku 资源类型</span><span class="sxs-lookup"><span data-stu-id="f034f-103">subscribedSku resource type</span></span>

<span data-ttu-id="f034f-104">包含有关公司订阅的服务 SKU 的信息。</span><span class="sxs-lookup"><span data-stu-id="f034f-104">Contains information about a service SKU that a company is subscribed to.</span></span>

<span data-ttu-id="f034f-p101">只支持在订阅的 SKU 上执行读取操作；不支持执行创建、更新和删除操作。不支持查询筛选表达式。继承自 [directoryObject](directoryobject.md)。</span><span class="sxs-lookup"><span data-stu-id="f034f-p101">Only the read operation is supported on subscribed SKUs; create, update, and delete are not supported. Query filter expressions are not supported. Inherits from [directoryObject](directoryobject.md).</span></span>

## <a name="methods"></a><span data-ttu-id="f034f-108">方法</span><span class="sxs-lookup"><span data-stu-id="f034f-108">Methods</span></span>
| <span data-ttu-id="f034f-109">方法</span><span class="sxs-lookup"><span data-stu-id="f034f-109">Method</span></span>           | <span data-ttu-id="f034f-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="f034f-110">Return Type</span></span>    |<span data-ttu-id="f034f-111">说明</span><span class="sxs-lookup"><span data-stu-id="f034f-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f034f-112">获取 subscribedSku</span><span class="sxs-lookup"><span data-stu-id="f034f-112">Get subscribedSku</span></span>](../api/subscribedsku-get.md) | [<span data-ttu-id="f034f-113">subscribedSku</span><span class="sxs-lookup"><span data-stu-id="f034f-113">subscribedSku</span></span>](subscribedsku.md) |<span data-ttu-id="f034f-114">获取组织已获取的特定商业订阅。</span><span class="sxs-lookup"><span data-stu-id="f034f-114">Get a specific commercial subscription that an organization has acquired.</span></span>|
|[<span data-ttu-id="f034f-115">列出 subscribedsku</span><span class="sxs-lookup"><span data-stu-id="f034f-115">List subscribedsku</span></span>](../api/subscribedsku-list.md) | <span data-ttu-id="f034f-116">[subscribedSku](subscribedsku.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f034f-116">[subscribedSku](subscribedsku.md) collection</span></span> |<span data-ttu-id="f034f-117">获取组织已获取的商业版订阅的列表。</span><span class="sxs-lookup"><span data-stu-id="f034f-117">Get the list of commercial subscriptions that an organization has acquired.</span></span>|

## <a name="properties"></a><span data-ttu-id="f034f-118">属性</span><span class="sxs-lookup"><span data-stu-id="f034f-118">Properties</span></span>
| <span data-ttu-id="f034f-119">属性</span><span class="sxs-lookup"><span data-stu-id="f034f-119">Property</span></span>     | <span data-ttu-id="f034f-120">类型</span><span class="sxs-lookup"><span data-stu-id="f034f-120">Type</span></span>   |<span data-ttu-id="f034f-121">说明</span><span class="sxs-lookup"><span data-stu-id="f034f-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f034f-122">appliesTo</span><span class="sxs-lookup"><span data-stu-id="f034f-122">appliesTo</span></span>|<span data-ttu-id="f034f-123">String</span><span class="sxs-lookup"><span data-stu-id="f034f-123">String</span></span>| <span data-ttu-id="f034f-124">例如，“用户”或“公司”。</span><span class="sxs-lookup"><span data-stu-id="f034f-124">For example, "User" or "Company".</span></span> |
|<span data-ttu-id="f034f-125">capabilityStatus</span><span class="sxs-lookup"><span data-stu-id="f034f-125">capabilityStatus</span></span>|<span data-ttu-id="f034f-126">String</span><span class="sxs-lookup"><span data-stu-id="f034f-126">String</span></span>|  <span data-ttu-id="f034f-127">可取值为：`Enabled`、`Warning`、`Suspended`、`Deleted`、`LockedOut`。</span><span class="sxs-lookup"><span data-stu-id="f034f-127">Possible values are: `Enabled`, `Warning`, `Suspended`, `Deleted`, `LockedOut`.</span></span> |
|<span data-ttu-id="f034f-128">consumedUnits</span><span class="sxs-lookup"><span data-stu-id="f034f-128">consumedUnits</span></span>|<span data-ttu-id="f034f-129">Int32</span><span class="sxs-lookup"><span data-stu-id="f034f-129">Int32</span></span>| <span data-ttu-id="f034f-130">已分配的许可证数量。</span><span class="sxs-lookup"><span data-stu-id="f034f-130">The number of licenses that have been assigned.</span></span> |
|<span data-ttu-id="f034f-131">id</span><span class="sxs-lookup"><span data-stu-id="f034f-131">id</span></span>|<span data-ttu-id="f034f-132">String</span><span class="sxs-lookup"><span data-stu-id="f034f-132">String</span></span>| <span data-ttu-id="f034f-133">订阅的 sku 对象的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="f034f-133">The unique identifier for the subscribed sku object.</span></span> <span data-ttu-id="f034f-134">键，不可为 null。</span><span class="sxs-lookup"><span data-stu-id="f034f-134">Key, not nullable.</span></span> |
|<span data-ttu-id="f034f-135">prepaidUnits</span><span class="sxs-lookup"><span data-stu-id="f034f-135">prepaidUnits</span></span>|[<span data-ttu-id="f034f-136">licenseUnitsDetail</span><span class="sxs-lookup"><span data-stu-id="f034f-136">licenseUnitsDetail</span></span>](licenseunitsdetail.md)| <span data-ttu-id="f034f-137">有关预付许可证的数量和状态的信息。</span><span class="sxs-lookup"><span data-stu-id="f034f-137">Information about the number and status of prepaid licenses.</span></span> |
|<span data-ttu-id="f034f-138">servicePlans</span><span class="sxs-lookup"><span data-stu-id="f034f-138">servicePlans</span></span>|<span data-ttu-id="f034f-139">[servicePlanInfo](serviceplaninfo.md) collection</span><span class="sxs-lookup"><span data-stu-id="f034f-139">[servicePlanInfo](serviceplaninfo.md) collection</span></span>| <span data-ttu-id="f034f-140">有关 SKU 可用服务计划的信息。</span><span class="sxs-lookup"><span data-stu-id="f034f-140">Information about the service plans that are available with the SKU.</span></span> <span data-ttu-id="f034f-141">不可为 null</span><span class="sxs-lookup"><span data-stu-id="f034f-141">Not nullable</span></span> |
|<span data-ttu-id="f034f-142">skuId</span><span class="sxs-lookup"><span data-stu-id="f034f-142">skuId</span></span>|<span data-ttu-id="f034f-143">Guid</span><span class="sxs-lookup"><span data-stu-id="f034f-143">Guid</span></span>| <span data-ttu-id="f034f-144">服务 SKU 的唯一标识符 (GUID)。</span><span class="sxs-lookup"><span data-stu-id="f034f-144">The unique identifier (GUID) for the service SKU.</span></span> |
|<span data-ttu-id="f034f-145">skuPartNumber</span><span class="sxs-lookup"><span data-stu-id="f034f-145">skuPartNumber</span></span>|<span data-ttu-id="f034f-146">String</span><span class="sxs-lookup"><span data-stu-id="f034f-146">String</span></span>| <span data-ttu-id="f034f-147">SKU 商品编号；例如：“AAD_PREMIUM”或“RMSBASIC”。</span><span class="sxs-lookup"><span data-stu-id="f034f-147">The SKU part number; for example: "AAD_PREMIUM" or "RMSBASIC".</span></span> <span data-ttu-id="f034f-148">若要获取组织获取的商业订阅的列表，请参阅[List subscribedsku](../api/subscribedsku-list.md)。</span><span class="sxs-lookup"><span data-stu-id="f034f-148">To get a list of commercial subscriptions that an organization has acquired, see [List subscribedSkus](../api/subscribedsku-list.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="f034f-149">关系</span><span class="sxs-lookup"><span data-stu-id="f034f-149">Relationships</span></span>
<span data-ttu-id="f034f-150">无</span><span class="sxs-lookup"><span data-stu-id="f034f-150">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f034f-151">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f034f-151">JSON representation</span></span>

<span data-ttu-id="f034f-152">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f034f-152">Here is a JSON representation of the resource</span></span>

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

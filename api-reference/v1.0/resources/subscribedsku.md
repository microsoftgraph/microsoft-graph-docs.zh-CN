---
title: subscribedSku 资源类型
description: 包含有关公司订阅的服务 SKU 的信息。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: f0e99acd1cfead36cd4f0591591cfbe7cee9d1e6
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034018"
---
# <a name="subscribedsku-resource-type"></a><span data-ttu-id="58a04-103">subscribedSku 资源类型</span><span class="sxs-lookup"><span data-stu-id="58a04-103">subscribedSku resource type</span></span>

<span data-ttu-id="58a04-104">包含有关公司订阅的服务 SKU 的信息。</span><span class="sxs-lookup"><span data-stu-id="58a04-104">Contains information about a service SKU that a company is subscribed to.</span></span>

<span data-ttu-id="58a04-p101">只支持在订阅的 SKU 上执行读取操作；不支持执行创建、更新和删除操作。不支持查询筛选表达式。继承自 [directoryObject](directoryobject.md)。</span><span class="sxs-lookup"><span data-stu-id="58a04-p101">Only the read operation is supported on subscribed SKUs; create, update, and delete are not supported. Query filter expressions are not supported. Inherits from [directoryObject](directoryobject.md).</span></span>

## <a name="methods"></a><span data-ttu-id="58a04-108">方法</span><span class="sxs-lookup"><span data-stu-id="58a04-108">Methods</span></span>
| <span data-ttu-id="58a04-109">方法</span><span class="sxs-lookup"><span data-stu-id="58a04-109">Method</span></span>           | <span data-ttu-id="58a04-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="58a04-110">Return Type</span></span>    |<span data-ttu-id="58a04-111">说明</span><span class="sxs-lookup"><span data-stu-id="58a04-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="58a04-112">获取 subscribedSku</span><span class="sxs-lookup"><span data-stu-id="58a04-112">Get subscribedSku</span></span>](../api/subscribedsku-get.md) | [<span data-ttu-id="58a04-113">subscribedSku</span><span class="sxs-lookup"><span data-stu-id="58a04-113">subscribedSku</span></span>](subscribedsku.md) |<span data-ttu-id="58a04-114">获取组织已获取的特定商业订阅。</span><span class="sxs-lookup"><span data-stu-id="58a04-114">Get a specific commercial subscription that an organization has acquired.</span></span>|
|[<span data-ttu-id="58a04-115">列出 subscribedsku</span><span class="sxs-lookup"><span data-stu-id="58a04-115">List subscribedsku</span></span>](../api/subscribedsku-list.md) | <span data-ttu-id="58a04-116">[subscribedSku](subscribedsku.md) 集合</span><span class="sxs-lookup"><span data-stu-id="58a04-116">[subscribedSku](subscribedsku.md) collection</span></span> |<span data-ttu-id="58a04-117">获取组织获取的商业订阅的列表。</span><span class="sxs-lookup"><span data-stu-id="58a04-117">Get the list of commercial subscriptions that an organization has acquired.</span></span>|

## <a name="properties"></a><span data-ttu-id="58a04-118">属性</span><span class="sxs-lookup"><span data-stu-id="58a04-118">Properties</span></span>
| <span data-ttu-id="58a04-119">属性</span><span class="sxs-lookup"><span data-stu-id="58a04-119">Property</span></span>     | <span data-ttu-id="58a04-120">类型</span><span class="sxs-lookup"><span data-stu-id="58a04-120">Type</span></span>   |<span data-ttu-id="58a04-121">说明</span><span class="sxs-lookup"><span data-stu-id="58a04-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="58a04-122">appliesTo</span><span class="sxs-lookup"><span data-stu-id="58a04-122">appliesTo</span></span>|<span data-ttu-id="58a04-123">String</span><span class="sxs-lookup"><span data-stu-id="58a04-123">String</span></span>| <span data-ttu-id="58a04-124">例如，“用户”或“公司”。</span><span class="sxs-lookup"><span data-stu-id="58a04-124">For example, "User" or "Company".</span></span> |
|<span data-ttu-id="58a04-125">capabilityStatus</span><span class="sxs-lookup"><span data-stu-id="58a04-125">capabilityStatus</span></span>|<span data-ttu-id="58a04-126">String</span><span class="sxs-lookup"><span data-stu-id="58a04-126">String</span></span>| <span data-ttu-id="58a04-127">例如, "Enabled"。</span><span class="sxs-lookup"><span data-stu-id="58a04-127">For example, "Enabled".</span></span> |
|<span data-ttu-id="58a04-128">consumedUnits</span><span class="sxs-lookup"><span data-stu-id="58a04-128">consumedUnits</span></span>|<span data-ttu-id="58a04-129">Int32</span><span class="sxs-lookup"><span data-stu-id="58a04-129">Int32</span></span>| <span data-ttu-id="58a04-130">已分配的许可证数量。</span><span class="sxs-lookup"><span data-stu-id="58a04-130">The number of licenses that have been assigned.</span></span> |
|<span data-ttu-id="58a04-131">id</span><span class="sxs-lookup"><span data-stu-id="58a04-131">id</span></span>|<span data-ttu-id="58a04-132">String</span><span class="sxs-lookup"><span data-stu-id="58a04-132">String</span></span>| <span data-ttu-id="58a04-133">订阅的 sku 对象的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="58a04-133">The unique identifier for the subscribed sku object.</span></span> <span data-ttu-id="58a04-134">键, 不可为 null。</span><span class="sxs-lookup"><span data-stu-id="58a04-134">Key, not nullable.</span></span> |
|<span data-ttu-id="58a04-135">prepaidUnits</span><span class="sxs-lookup"><span data-stu-id="58a04-135">prepaidUnits</span></span>|[<span data-ttu-id="58a04-136">licenseUnitsDetail</span><span class="sxs-lookup"><span data-stu-id="58a04-136">licenseUnitsDetail</span></span>](licenseunitsdetail.md)| <span data-ttu-id="58a04-137">有关预付许可证的数量和状态的信息。</span><span class="sxs-lookup"><span data-stu-id="58a04-137">Information about the number and status of prepaid licenses.</span></span> |
|<span data-ttu-id="58a04-138">servicePlans</span><span class="sxs-lookup"><span data-stu-id="58a04-138">servicePlans</span></span>|<span data-ttu-id="58a04-139">[servicePlanInfo](serviceplaninfo.md) collection</span><span class="sxs-lookup"><span data-stu-id="58a04-139">[servicePlanInfo](serviceplaninfo.md) collection</span></span>| <span data-ttu-id="58a04-140">有关 SKU 可用服务计划的信息。</span><span class="sxs-lookup"><span data-stu-id="58a04-140">Information about the service plans that are available with the SKU.</span></span> <span data-ttu-id="58a04-141">不可为 null</span><span class="sxs-lookup"><span data-stu-id="58a04-141">Not nullable</span></span> |
|<span data-ttu-id="58a04-142">skuId</span><span class="sxs-lookup"><span data-stu-id="58a04-142">skuId</span></span>|<span data-ttu-id="58a04-143">Guid</span><span class="sxs-lookup"><span data-stu-id="58a04-143">Guid</span></span>| <span data-ttu-id="58a04-144">服务 SKU 的唯一标识符 (GUID)。</span><span class="sxs-lookup"><span data-stu-id="58a04-144">The unique identifier (GUID) for the service SKU.</span></span> |
|<span data-ttu-id="58a04-145">skuPartNumber</span><span class="sxs-lookup"><span data-stu-id="58a04-145">skuPartNumber</span></span>|<span data-ttu-id="58a04-146">String</span><span class="sxs-lookup"><span data-stu-id="58a04-146">String</span></span>| <span data-ttu-id="58a04-147">SKU 商品编号；例如：“AAD_PREMIUM”或“RMSBASIC”。</span><span class="sxs-lookup"><span data-stu-id="58a04-147">The SKU part number; for example: "AAD_PREMIUM" or "RMSBASIC".</span></span> |

## <a name="relationships"></a><span data-ttu-id="58a04-148">关系</span><span class="sxs-lookup"><span data-stu-id="58a04-148">Relationships</span></span>
<span data-ttu-id="58a04-149">无</span><span class="sxs-lookup"><span data-stu-id="58a04-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="58a04-150">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="58a04-150">JSON representation</span></span>

<span data-ttu-id="58a04-151">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="58a04-151">Here is a JSON representation of the resource</span></span>

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

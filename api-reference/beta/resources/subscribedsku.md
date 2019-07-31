---
title: subscribedSku 资源类型
description: " 不支持创建、更新和删除。 不支持查询筛选表达式。 继承自 directoryObject。"
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 9e57ff1e59c7caf5b29e582b7381492a7eee5b4c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964815"
---
# <a name="subscribedsku-resource-type"></a><span data-ttu-id="b8b97-105">subscribedSku 资源类型</span><span class="sxs-lookup"><span data-stu-id="b8b97-105">subscribedSku resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b8b97-p102">只支持在订阅的 SKU 上执行读取操作；不支持执行创建、更新和删除操作。不支持查询筛选表达式。继承自 [directoryObject](directoryobject.md)。</span><span class="sxs-lookup"><span data-stu-id="b8b97-p102">Only the read operation is supported on subscribed SKUs; create, update, and delete are not supported. Query filter expressions are not supported. Inherits from [directoryObject](directoryobject.md).</span></span>


## <a name="methods"></a><span data-ttu-id="b8b97-109">方法</span><span class="sxs-lookup"><span data-stu-id="b8b97-109">Methods</span></span>
| <span data-ttu-id="b8b97-110">方法</span><span class="sxs-lookup"><span data-stu-id="b8b97-110">Method</span></span>           | <span data-ttu-id="b8b97-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="b8b97-111">Return Type</span></span>    |<span data-ttu-id="b8b97-112">说明</span><span class="sxs-lookup"><span data-stu-id="b8b97-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b8b97-113">获取 subscribedSku</span><span class="sxs-lookup"><span data-stu-id="b8b97-113">Get subscribedSku</span></span>](../api/subscribedsku-get.md) | [<span data-ttu-id="b8b97-114">subscribedSku</span><span class="sxs-lookup"><span data-stu-id="b8b97-114">subscribedSku</span></span>](subscribedsku.md) |<span data-ttu-id="b8b97-115">获取组织已获取的特定商业订阅。</span><span class="sxs-lookup"><span data-stu-id="b8b97-115">Get a specific commercial subscription that an organization has acquired.</span></span>|
|[<span data-ttu-id="b8b97-116">列出 subscribedsku</span><span class="sxs-lookup"><span data-stu-id="b8b97-116">List subscribedsku</span></span>](../api/subscribedsku-list.md) | <span data-ttu-id="b8b97-117">[subscribedSku](subscribedsku.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b8b97-117">[subscribedSku](subscribedsku.md) collection</span></span> |<span data-ttu-id="b8b97-118">获取组织获取的商业订阅的列表。</span><span class="sxs-lookup"><span data-stu-id="b8b97-118">Get the list of commercial subscriptions that an organization has acquired.</span></span>|

## <a name="properties"></a><span data-ttu-id="b8b97-119">属性</span><span class="sxs-lookup"><span data-stu-id="b8b97-119">Properties</span></span>
| <span data-ttu-id="b8b97-120">属性</span><span class="sxs-lookup"><span data-stu-id="b8b97-120">Property</span></span>     | <span data-ttu-id="b8b97-121">类型</span><span class="sxs-lookup"><span data-stu-id="b8b97-121">Type</span></span>   |<span data-ttu-id="b8b97-122">说明</span><span class="sxs-lookup"><span data-stu-id="b8b97-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b8b97-123">appliesTo</span><span class="sxs-lookup"><span data-stu-id="b8b97-123">appliesTo</span></span>|<span data-ttu-id="b8b97-124">String</span><span class="sxs-lookup"><span data-stu-id="b8b97-124">String</span></span>| <span data-ttu-id="b8b97-125">例如，“用户”或“公司”。</span><span class="sxs-lookup"><span data-stu-id="b8b97-125">For example, "User" or "Company".</span></span> |
|<span data-ttu-id="b8b97-126">capabilityStatus</span><span class="sxs-lookup"><span data-stu-id="b8b97-126">capabilityStatus</span></span>|<span data-ttu-id="b8b97-127">String</span><span class="sxs-lookup"><span data-stu-id="b8b97-127">String</span></span>| <span data-ttu-id="b8b97-128">例如, "Enabled"。</span><span class="sxs-lookup"><span data-stu-id="b8b97-128">For example, "Enabled".</span></span> |
|<span data-ttu-id="b8b97-129">consumedUnits</span><span class="sxs-lookup"><span data-stu-id="b8b97-129">consumedUnits</span></span>|<span data-ttu-id="b8b97-130">Int32</span><span class="sxs-lookup"><span data-stu-id="b8b97-130">Int32</span></span>| <span data-ttu-id="b8b97-131">已分配的许可证数量。</span><span class="sxs-lookup"><span data-stu-id="b8b97-131">The number of licenses that have been assigned.</span></span> |
|<span data-ttu-id="b8b97-132">id</span><span class="sxs-lookup"><span data-stu-id="b8b97-132">id</span></span>|<span data-ttu-id="b8b97-133">String</span><span class="sxs-lookup"><span data-stu-id="b8b97-133">String</span></span>| <span data-ttu-id="b8b97-134">订阅的 sku 对象的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="b8b97-134">The unique identifier for the subscribed sku object.</span></span> <span data-ttu-id="b8b97-135">键, 不可为 null。</span><span class="sxs-lookup"><span data-stu-id="b8b97-135">Key, not nullable.</span></span> |
|<span data-ttu-id="b8b97-136">prepaidUnits</span><span class="sxs-lookup"><span data-stu-id="b8b97-136">prepaidUnits</span></span>|[<span data-ttu-id="b8b97-137">licenseUnitsDetail</span><span class="sxs-lookup"><span data-stu-id="b8b97-137">licenseUnitsDetail</span></span>](licenseunitsdetail.md)| <span data-ttu-id="b8b97-138">有关预付许可证的数量和状态的信息。</span><span class="sxs-lookup"><span data-stu-id="b8b97-138">Information about the number and status of prepaid licenses.</span></span> |
|<span data-ttu-id="b8b97-139">servicePlans</span><span class="sxs-lookup"><span data-stu-id="b8b97-139">servicePlans</span></span>|<span data-ttu-id="b8b97-140">[servicePlanInfo](serviceplaninfo.md) collection</span><span class="sxs-lookup"><span data-stu-id="b8b97-140">[servicePlanInfo](serviceplaninfo.md) collection</span></span>| <span data-ttu-id="b8b97-141">有关 SKU 可用服务计划的信息。</span><span class="sxs-lookup"><span data-stu-id="b8b97-141">Information about the service plans that are available with the SKU.</span></span> <span data-ttu-id="b8b97-142">不可为 null</span><span class="sxs-lookup"><span data-stu-id="b8b97-142">Not nullable</span></span> |
|<span data-ttu-id="b8b97-143">skuId</span><span class="sxs-lookup"><span data-stu-id="b8b97-143">skuId</span></span>|<span data-ttu-id="b8b97-144">Guid</span><span class="sxs-lookup"><span data-stu-id="b8b97-144">Guid</span></span>| <span data-ttu-id="b8b97-145">服务 SKU 的唯一标识符 (GUID)。</span><span class="sxs-lookup"><span data-stu-id="b8b97-145">The unique identifier (GUID) for the service SKU.</span></span> |
|<span data-ttu-id="b8b97-146">skuPartNumber</span><span class="sxs-lookup"><span data-stu-id="b8b97-146">skuPartNumber</span></span>|<span data-ttu-id="b8b97-147">String</span><span class="sxs-lookup"><span data-stu-id="b8b97-147">String</span></span>| <span data-ttu-id="b8b97-148">SKU 商品编号；例如：“AAD_PREMIUM”或“RMSBASIC”。</span><span class="sxs-lookup"><span data-stu-id="b8b97-148">The SKU part number; for example: "AAD_PREMIUM" or "RMSBASIC".</span></span> |

## <a name="relationships"></a><span data-ttu-id="b8b97-149">关系</span><span class="sxs-lookup"><span data-stu-id="b8b97-149">Relationships</span></span>
<span data-ttu-id="b8b97-150">无</span><span class="sxs-lookup"><span data-stu-id="b8b97-150">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b8b97-151">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b8b97-151">JSON representation</span></span>

<span data-ttu-id="b8b97-152">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b8b97-152">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.subscribedSku"
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
<!--
{
  "type": "#page.annotation",
  "description": "subscribedSku resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

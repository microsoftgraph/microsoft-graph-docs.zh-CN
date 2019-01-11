---
title: subscribedSku 资源类型
description: 包含有关公司订阅的服务 SKU 的信息。
localization_priority: Normal
ms.openlocfilehash: 17290890ff27fded1aaf5d7fdb2c0cdacee09b0c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27873715"
---
# <a name="subscribedsku-resource-type"></a><span data-ttu-id="cfc7f-103">subscribedSku 资源类型</span><span class="sxs-lookup"><span data-stu-id="cfc7f-103">subscribedSku resource type</span></span>

<span data-ttu-id="cfc7f-104">包含有关公司订阅的服务 SKU 的信息。</span><span class="sxs-lookup"><span data-stu-id="cfc7f-104">Contains information about a service SKU that a company is subscribed to.</span></span>

<span data-ttu-id="cfc7f-p101">只支持在订阅的 SKU 上执行读取操作；不支持执行创建、更新和删除操作。不支持查询筛选表达式。继承自 [directoryObject](directoryobject.md)。</span><span class="sxs-lookup"><span data-stu-id="cfc7f-p101">Only the read operation is supported on subscribed SKUs; create, update, and delete are not supported. Query filter expressions are not supported. Inherits from [directoryObject](directoryobject.md).</span></span>

## <a name="methods"></a><span data-ttu-id="cfc7f-108">方法</span><span class="sxs-lookup"><span data-stu-id="cfc7f-108">Methods</span></span>
| <span data-ttu-id="cfc7f-109">方法</span><span class="sxs-lookup"><span data-stu-id="cfc7f-109">Method</span></span>           | <span data-ttu-id="cfc7f-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="cfc7f-110">Return Type</span></span>    |<span data-ttu-id="cfc7f-111">说明</span><span class="sxs-lookup"><span data-stu-id="cfc7f-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="cfc7f-112">获取 subscribedSku</span><span class="sxs-lookup"><span data-stu-id="cfc7f-112">Get subscribedSku</span></span>](../api/subscribedsku-get.md) | [<span data-ttu-id="cfc7f-113">subscribedSku</span><span class="sxs-lookup"><span data-stu-id="cfc7f-113">subscribedSku</span></span>](subscribedsku.md) |<span data-ttu-id="cfc7f-114">读取 subscribedSku 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="cfc7f-114">Read properties and relationships of subscribedSku object.</span></span>|
|[<span data-ttu-id="cfc7f-115">列表 subscribedsku</span><span class="sxs-lookup"><span data-stu-id="cfc7f-115">List subscribedsku</span></span>](../api/subscribedsku-list.md) | <span data-ttu-id="cfc7f-116">[subscribedSku](subscribedsku.md) 集合</span><span class="sxs-lookup"><span data-stu-id="cfc7f-116">[subscribedSku](subscribedsku.md) collection</span></span> |<span data-ttu-id="cfc7f-117">检索组织已获取的商业订阅列表。</span><span class="sxs-lookup"><span data-stu-id="cfc7f-117">Retrieve the list of commercial subscriptions that an organization has acquired.</span></span>|

## <a name="properties"></a><span data-ttu-id="cfc7f-118">属性</span><span class="sxs-lookup"><span data-stu-id="cfc7f-118">Properties</span></span>
| <span data-ttu-id="cfc7f-119">属性</span><span class="sxs-lookup"><span data-stu-id="cfc7f-119">Property</span></span>     | <span data-ttu-id="cfc7f-120">类型</span><span class="sxs-lookup"><span data-stu-id="cfc7f-120">Type</span></span>   |<span data-ttu-id="cfc7f-121">说明</span><span class="sxs-lookup"><span data-stu-id="cfc7f-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cfc7f-122">appliesTo</span><span class="sxs-lookup"><span data-stu-id="cfc7f-122">appliesTo</span></span>|<span data-ttu-id="cfc7f-123">String</span><span class="sxs-lookup"><span data-stu-id="cfc7f-123">String</span></span>| <span data-ttu-id="cfc7f-124">例如，“用户”或“公司”。</span><span class="sxs-lookup"><span data-stu-id="cfc7f-124">For example, "User" or "Company".</span></span> |
|<span data-ttu-id="cfc7f-125">capabilityStatus</span><span class="sxs-lookup"><span data-stu-id="cfc7f-125">capabilityStatus</span></span>|<span data-ttu-id="cfc7f-126">String</span><span class="sxs-lookup"><span data-stu-id="cfc7f-126">String</span></span>| <span data-ttu-id="cfc7f-127">例如，“Enabled”。</span><span class="sxs-lookup"><span data-stu-id="cfc7f-127">For example, "Enabled".</span></span> |
|<span data-ttu-id="cfc7f-128">consumedUnits</span><span class="sxs-lookup"><span data-stu-id="cfc7f-128">consumedUnits</span></span>|<span data-ttu-id="cfc7f-129">Int32</span><span class="sxs-lookup"><span data-stu-id="cfc7f-129">Int32</span></span>| <span data-ttu-id="cfc7f-130">已分配的许可证数量。</span><span class="sxs-lookup"><span data-stu-id="cfc7f-130">The number of licenses that have been assigned.</span></span> |
|<span data-ttu-id="cfc7f-131">id</span><span class="sxs-lookup"><span data-stu-id="cfc7f-131">id</span></span>|<span data-ttu-id="cfc7f-132">String</span><span class="sxs-lookup"><span data-stu-id="cfc7f-132">String</span></span>| <span data-ttu-id="cfc7f-p102">订阅的 sku 对象的唯一标识符。密钥，不可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="cfc7f-p102">The unique identifier for the subscribed sku object. Key, not nullable.</span></span> |
|<span data-ttu-id="cfc7f-135">prepaidUnits</span><span class="sxs-lookup"><span data-stu-id="cfc7f-135">prepaidUnits</span></span>|[<span data-ttu-id="cfc7f-136">licenseUnitsDetail</span><span class="sxs-lookup"><span data-stu-id="cfc7f-136">licenseUnitsDetail</span></span>](licenseunitsdetail.md)| <span data-ttu-id="cfc7f-137">有关预付许可证的数量和状态的信息。</span><span class="sxs-lookup"><span data-stu-id="cfc7f-137">Information about the number and status of prepaid licenses.</span></span> |
|<span data-ttu-id="cfc7f-138">servicePlans</span><span class="sxs-lookup"><span data-stu-id="cfc7f-138">servicePlans</span></span>|<span data-ttu-id="cfc7f-139">[servicePlanInfo](serviceplaninfo.md) collection</span><span class="sxs-lookup"><span data-stu-id="cfc7f-139">[servicePlanInfo](serviceplaninfo.md) collection</span></span>| <span data-ttu-id="cfc7f-p103">有关 SKU 可用服务计划的信息。不可为 null</span><span class="sxs-lookup"><span data-stu-id="cfc7f-p103">Information about the service plans that are available with the SKU. Not nullable</span></span> |
|<span data-ttu-id="cfc7f-142">skuId</span><span class="sxs-lookup"><span data-stu-id="cfc7f-142">skuId</span></span>|<span data-ttu-id="cfc7f-143">Guid</span><span class="sxs-lookup"><span data-stu-id="cfc7f-143">Guid</span></span>| <span data-ttu-id="cfc7f-144">服务 SKU 的唯一标识符 (GUID)。</span><span class="sxs-lookup"><span data-stu-id="cfc7f-144">The unique identifier (GUID) for the service SKU.</span></span> |
|<span data-ttu-id="cfc7f-145">skuPartNumber</span><span class="sxs-lookup"><span data-stu-id="cfc7f-145">skuPartNumber</span></span>|<span data-ttu-id="cfc7f-146">字符串</span><span class="sxs-lookup"><span data-stu-id="cfc7f-146">String</span></span>| <span data-ttu-id="cfc7f-147">SKU 商品编号；例如：“AAD_PREMIUM”或“RMSBASIC”。</span><span class="sxs-lookup"><span data-stu-id="cfc7f-147">The SKU part number; for example: "AAD_PREMIUM" or "RMSBASIC".</span></span> |

## <a name="relationships"></a><span data-ttu-id="cfc7f-148">关系</span><span class="sxs-lookup"><span data-stu-id="cfc7f-148">Relationships</span></span>
<span data-ttu-id="cfc7f-149">无</span><span class="sxs-lookup"><span data-stu-id="cfc7f-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cfc7f-150">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cfc7f-150">JSON representation</span></span>

<span data-ttu-id="cfc7f-151">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cfc7f-151">Here is a JSON representation of the resource</span></span>

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

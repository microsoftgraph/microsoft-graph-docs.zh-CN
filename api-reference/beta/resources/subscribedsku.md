---
title: subscribedSku 资源类型
description: " 不支持创建、更新和删除。 不支持查询筛选表达式。 继承自 directoryObject。"
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 528ec916edf049ef48b057afabad943bbb2182cf
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520294"
---
# <a name="subscribedsku-resource-type"></a><span data-ttu-id="99b18-105">subscribedSku 资源类型</span><span class="sxs-lookup"><span data-stu-id="99b18-105">subscribedSku resource type</span></span>

<span data-ttu-id="99b18-106">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="99b18-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="99b18-p102">只支持在订阅的 SKU 上执行读取操作；不支持执行创建、更新和删除操作。不支持查询筛选表达式。继承自 [directoryObject](directoryobject.md)。</span><span class="sxs-lookup"><span data-stu-id="99b18-p102">Only the read operation is supported on subscribed SKUs; create, update, and delete are not supported. Query filter expressions are not supported. Inherits from [directoryObject](directoryobject.md).</span></span>


## <a name="methods"></a><span data-ttu-id="99b18-110">方法</span><span class="sxs-lookup"><span data-stu-id="99b18-110">Methods</span></span>
| <span data-ttu-id="99b18-111">方法</span><span class="sxs-lookup"><span data-stu-id="99b18-111">Method</span></span>           | <span data-ttu-id="99b18-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="99b18-112">Return Type</span></span>    |<span data-ttu-id="99b18-113">说明</span><span class="sxs-lookup"><span data-stu-id="99b18-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="99b18-114">获取 subscribedSku</span><span class="sxs-lookup"><span data-stu-id="99b18-114">Get subscribedSku</span></span>](../api/subscribedsku-get.md) | [<span data-ttu-id="99b18-115">subscribedSku</span><span class="sxs-lookup"><span data-stu-id="99b18-115">subscribedSku</span></span>](subscribedsku.md) |<span data-ttu-id="99b18-116">获取组织已获取的特定商业订阅。</span><span class="sxs-lookup"><span data-stu-id="99b18-116">Get a specific commercial subscription that an organization has acquired.</span></span>|
|[<span data-ttu-id="99b18-117">列出 subscribedsku</span><span class="sxs-lookup"><span data-stu-id="99b18-117">List subscribedsku</span></span>](../api/subscribedsku-list.md) | <span data-ttu-id="99b18-118">[subscribedSku](subscribedsku.md) 集合</span><span class="sxs-lookup"><span data-stu-id="99b18-118">[subscribedSku](subscribedsku.md) collection</span></span> |<span data-ttu-id="99b18-119">获取组织已获取的商业版订阅的列表。</span><span class="sxs-lookup"><span data-stu-id="99b18-119">Get the list of commercial subscriptions that an organization has acquired.</span></span>|

## <a name="properties"></a><span data-ttu-id="99b18-120">属性</span><span class="sxs-lookup"><span data-stu-id="99b18-120">Properties</span></span>
| <span data-ttu-id="99b18-121">属性</span><span class="sxs-lookup"><span data-stu-id="99b18-121">Property</span></span>     | <span data-ttu-id="99b18-122">类型</span><span class="sxs-lookup"><span data-stu-id="99b18-122">Type</span></span>   |<span data-ttu-id="99b18-123">说明</span><span class="sxs-lookup"><span data-stu-id="99b18-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="99b18-124">appliesTo</span><span class="sxs-lookup"><span data-stu-id="99b18-124">appliesTo</span></span>|<span data-ttu-id="99b18-125">String</span><span class="sxs-lookup"><span data-stu-id="99b18-125">String</span></span>| <span data-ttu-id="99b18-126">例如，“用户”或“公司”。</span><span class="sxs-lookup"><span data-stu-id="99b18-126">For example, "User" or "Company".</span></span> |
|<span data-ttu-id="99b18-127">capabilityStatus</span><span class="sxs-lookup"><span data-stu-id="99b18-127">capabilityStatus</span></span>|<span data-ttu-id="99b18-128">String</span><span class="sxs-lookup"><span data-stu-id="99b18-128">String</span></span>| <span data-ttu-id="99b18-129">可取值为：`Enabled`、`Warning`、`Suspended`、`Deleted`、`LockedOut`。</span><span class="sxs-lookup"><span data-stu-id="99b18-129">Possible values are: `Enabled`, `Warning`, `Suspended`, `Deleted`, `LockedOut`.</span></span> |
|<span data-ttu-id="99b18-130">consumedUnits</span><span class="sxs-lookup"><span data-stu-id="99b18-130">consumedUnits</span></span>|<span data-ttu-id="99b18-131">Int32</span><span class="sxs-lookup"><span data-stu-id="99b18-131">Int32</span></span>| <span data-ttu-id="99b18-132">已分配的许可证数量。</span><span class="sxs-lookup"><span data-stu-id="99b18-132">The number of licenses that have been assigned.</span></span> |
|<span data-ttu-id="99b18-133">id</span><span class="sxs-lookup"><span data-stu-id="99b18-133">id</span></span>|<span data-ttu-id="99b18-134">String</span><span class="sxs-lookup"><span data-stu-id="99b18-134">String</span></span>| <span data-ttu-id="99b18-135">订阅的 sku 对象的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="99b18-135">The unique identifier for the subscribed sku object.</span></span> <span data-ttu-id="99b18-136">键，不可为 null。</span><span class="sxs-lookup"><span data-stu-id="99b18-136">Key, not nullable.</span></span> |
|<span data-ttu-id="99b18-137">prepaidUnits</span><span class="sxs-lookup"><span data-stu-id="99b18-137">prepaidUnits</span></span>|[<span data-ttu-id="99b18-138">licenseUnitsDetail</span><span class="sxs-lookup"><span data-stu-id="99b18-138">licenseUnitsDetail</span></span>](licenseunitsdetail.md)| <span data-ttu-id="99b18-139">有关预付许可证的数量和状态的信息。</span><span class="sxs-lookup"><span data-stu-id="99b18-139">Information about the number and status of prepaid licenses.</span></span> |
|<span data-ttu-id="99b18-140">servicePlans</span><span class="sxs-lookup"><span data-stu-id="99b18-140">servicePlans</span></span>|<span data-ttu-id="99b18-141">[servicePlanInfo](serviceplaninfo.md) collection</span><span class="sxs-lookup"><span data-stu-id="99b18-141">[servicePlanInfo](serviceplaninfo.md) collection</span></span>| <span data-ttu-id="99b18-142">有关 SKU 可用服务计划的信息。</span><span class="sxs-lookup"><span data-stu-id="99b18-142">Information about the service plans that are available with the SKU.</span></span> <span data-ttu-id="99b18-143">不可为 null</span><span class="sxs-lookup"><span data-stu-id="99b18-143">Not nullable</span></span> |
|<span data-ttu-id="99b18-144">skuId</span><span class="sxs-lookup"><span data-stu-id="99b18-144">skuId</span></span>|<span data-ttu-id="99b18-145">Guid</span><span class="sxs-lookup"><span data-stu-id="99b18-145">Guid</span></span>| <span data-ttu-id="99b18-146">服务 SKU 的唯一标识符 (GUID)。</span><span class="sxs-lookup"><span data-stu-id="99b18-146">The unique identifier (GUID) for the service SKU.</span></span> |
|<span data-ttu-id="99b18-147">skuPartNumber</span><span class="sxs-lookup"><span data-stu-id="99b18-147">skuPartNumber</span></span>|<span data-ttu-id="99b18-148">String</span><span class="sxs-lookup"><span data-stu-id="99b18-148">String</span></span>| <span data-ttu-id="99b18-149">SKU 商品编号；例如：“AAD_PREMIUM”或“RMSBASIC”。</span><span class="sxs-lookup"><span data-stu-id="99b18-149">The SKU part number; for example: "AAD_PREMIUM" or "RMSBASIC".</span></span> <span data-ttu-id="99b18-150">若要获取组织获取的商业订阅的列表，请参阅[List subscribedsku](../api/subscribedsku-list.md)。</span><span class="sxs-lookup"><span data-stu-id="99b18-150">To get a list of commercial subscriptions that an organization has acquired, see [List subscribedSkus](../api/subscribedsku-list.md).</span></span> |

## <a name="relationships"></a><span data-ttu-id="99b18-151">关系</span><span class="sxs-lookup"><span data-stu-id="99b18-151">Relationships</span></span>
<span data-ttu-id="99b18-152">无</span><span class="sxs-lookup"><span data-stu-id="99b18-152">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="99b18-153">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="99b18-153">JSON representation</span></span>

<span data-ttu-id="99b18-154">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="99b18-154">Here is a JSON representation of the resource</span></span>

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

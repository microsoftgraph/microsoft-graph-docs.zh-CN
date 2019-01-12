---
title: subscribedSku 资源类型
description: " 创建、 更新和删除不受支持。 不支持查询筛选器表达式。 继承自 directoryObject。"
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 01dbbf8727ab361b3763e2343e7cc72a3676848b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27960152"
---
# <a name="subscribedsku-resource-type"></a><span data-ttu-id="ff263-105">subscribedSku 资源类型</span><span class="sxs-lookup"><span data-stu-id="ff263-105">subscribedSku resource type</span></span>

> <span data-ttu-id="ff263-106">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="ff263-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ff263-107">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ff263-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ff263-p103">只支持在订阅的 SKU 上执行读取操作；不支持执行创建、更新和删除操作。不支持查询筛选表达式。继承自 [directoryObject](directoryobject.md)。</span><span class="sxs-lookup"><span data-stu-id="ff263-p103">Only the read operation is supported on subscribed SKUs; create, update, and delete are not supported. Query filter expressions are not supported. Inherits from [directoryObject](directoryobject.md).</span></span>


## <a name="methods"></a><span data-ttu-id="ff263-111">方法</span><span class="sxs-lookup"><span data-stu-id="ff263-111">Methods</span></span>
| <span data-ttu-id="ff263-112">方法</span><span class="sxs-lookup"><span data-stu-id="ff263-112">Method</span></span>           | <span data-ttu-id="ff263-113">返回类型</span><span class="sxs-lookup"><span data-stu-id="ff263-113">Return Type</span></span>    |<span data-ttu-id="ff263-114">说明</span><span class="sxs-lookup"><span data-stu-id="ff263-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ff263-115">获取 subscribedSku</span><span class="sxs-lookup"><span data-stu-id="ff263-115">Get subscribedSku</span></span>](../api/subscribedsku-get.md) | [<span data-ttu-id="ff263-116">subscribedSku</span><span class="sxs-lookup"><span data-stu-id="ff263-116">subscribedSku</span></span>](subscribedsku.md) |<span data-ttu-id="ff263-117">读取 subscribedSku 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ff263-117">Read properties and relationships of subscribedSku object.</span></span>|
|[<span data-ttu-id="ff263-118">列表 subscribedsku</span><span class="sxs-lookup"><span data-stu-id="ff263-118">List subscribedsku</span></span>](../api/subscribedsku-list.md) | <span data-ttu-id="ff263-119">[subscribedSku](subscribedsku.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ff263-119">[subscribedSku](subscribedsku.md) collection</span></span> |<span data-ttu-id="ff263-120">检索组织已获取的商业订阅列表。</span><span class="sxs-lookup"><span data-stu-id="ff263-120">Retrieve the list of commercial subscriptions that an organization has acquired.</span></span>|

## <a name="properties"></a><span data-ttu-id="ff263-121">属性</span><span class="sxs-lookup"><span data-stu-id="ff263-121">Properties</span></span>
| <span data-ttu-id="ff263-122">属性</span><span class="sxs-lookup"><span data-stu-id="ff263-122">Property</span></span>     | <span data-ttu-id="ff263-123">类型</span><span class="sxs-lookup"><span data-stu-id="ff263-123">Type</span></span>   |<span data-ttu-id="ff263-124">说明</span><span class="sxs-lookup"><span data-stu-id="ff263-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ff263-125">appliesTo</span><span class="sxs-lookup"><span data-stu-id="ff263-125">appliesTo</span></span>|<span data-ttu-id="ff263-126">String</span><span class="sxs-lookup"><span data-stu-id="ff263-126">String</span></span>| <span data-ttu-id="ff263-127">例如，“用户”或“公司”。</span><span class="sxs-lookup"><span data-stu-id="ff263-127">For example, "User" or "Company".</span></span> |
|<span data-ttu-id="ff263-128">capabilityStatus</span><span class="sxs-lookup"><span data-stu-id="ff263-128">capabilityStatus</span></span>|<span data-ttu-id="ff263-129">String</span><span class="sxs-lookup"><span data-stu-id="ff263-129">String</span></span>| <span data-ttu-id="ff263-130">例如，“Enabled”。</span><span class="sxs-lookup"><span data-stu-id="ff263-130">For example, "Enabled".</span></span> |
|<span data-ttu-id="ff263-131">consumedUnits</span><span class="sxs-lookup"><span data-stu-id="ff263-131">consumedUnits</span></span>|<span data-ttu-id="ff263-132">Int32</span><span class="sxs-lookup"><span data-stu-id="ff263-132">Int32</span></span>| <span data-ttu-id="ff263-133">已分配的许可证数量。</span><span class="sxs-lookup"><span data-stu-id="ff263-133">The number of licenses that have been assigned.</span></span> |
|<span data-ttu-id="ff263-134">id</span><span class="sxs-lookup"><span data-stu-id="ff263-134">id</span></span>|<span data-ttu-id="ff263-135">String</span><span class="sxs-lookup"><span data-stu-id="ff263-135">String</span></span>| <span data-ttu-id="ff263-p104">订阅的 sku 对象的唯一标识符。密钥，不可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="ff263-p104">The unique identifier for the subscribed sku object. Key, not nullable.</span></span> |
|<span data-ttu-id="ff263-138">prepaidUnits</span><span class="sxs-lookup"><span data-stu-id="ff263-138">prepaidUnits</span></span>|[<span data-ttu-id="ff263-139">licenseUnitsDetail</span><span class="sxs-lookup"><span data-stu-id="ff263-139">licenseUnitsDetail</span></span>](licenseunitsdetail.md)| <span data-ttu-id="ff263-140">有关预付许可证的数量和状态的信息。</span><span class="sxs-lookup"><span data-stu-id="ff263-140">Information about the number and status of prepaid licenses.</span></span> |
|<span data-ttu-id="ff263-141">servicePlans</span><span class="sxs-lookup"><span data-stu-id="ff263-141">servicePlans</span></span>|<span data-ttu-id="ff263-142">[servicePlanInfo](serviceplaninfo.md) collection</span><span class="sxs-lookup"><span data-stu-id="ff263-142">[servicePlanInfo](serviceplaninfo.md) collection</span></span>| <span data-ttu-id="ff263-p105">有关 SKU 可用服务计划的信息。不可为 null</span><span class="sxs-lookup"><span data-stu-id="ff263-p105">Information about the service plans that are available with the SKU. Not nullable</span></span> |
|<span data-ttu-id="ff263-145">skuId</span><span class="sxs-lookup"><span data-stu-id="ff263-145">skuId</span></span>|<span data-ttu-id="ff263-146">Guid</span><span class="sxs-lookup"><span data-stu-id="ff263-146">Guid</span></span>| <span data-ttu-id="ff263-147">服务 SKU 的唯一标识符 (GUID)。</span><span class="sxs-lookup"><span data-stu-id="ff263-147">The unique identifier (GUID) for the service SKU.</span></span> |
|<span data-ttu-id="ff263-148">skuPartNumber</span><span class="sxs-lookup"><span data-stu-id="ff263-148">skuPartNumber</span></span>|<span data-ttu-id="ff263-149">字符串</span><span class="sxs-lookup"><span data-stu-id="ff263-149">String</span></span>| <span data-ttu-id="ff263-150">SKU 商品编号；例如：“AAD_PREMIUM”或“RMSBASIC”。</span><span class="sxs-lookup"><span data-stu-id="ff263-150">The SKU part number; for example: "AAD_PREMIUM" or "RMSBASIC".</span></span> |

## <a name="relationships"></a><span data-ttu-id="ff263-151">关系</span><span class="sxs-lookup"><span data-stu-id="ff263-151">Relationships</span></span>
<span data-ttu-id="ff263-152">无</span><span class="sxs-lookup"><span data-stu-id="ff263-152">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ff263-153">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ff263-153">JSON representation</span></span>

<span data-ttu-id="ff263-154">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ff263-154">Here is a JSON representation of the resource</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "subscribedSku resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

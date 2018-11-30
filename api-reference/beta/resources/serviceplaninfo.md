---
title: servicePlanInfo 资源类型
description: 包含与订阅的 SKU 相关的服务计划有关的信息。subscribedSku 实体的 **servicePlans** 属性是一个 **servicePlanInfo** 集合。
ms.openlocfilehash: 86246de74caef6bf0c778f5b6b38e185841394b1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27046869"
---
# <a name="serviceplaninfo-resource-type"></a><span data-ttu-id="09682-104">servicePlanInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="09682-104">servicePlanInfo resource type</span></span>

> <span data-ttu-id="09682-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="09682-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="09682-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="09682-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="09682-p103">包含与订阅的 SKU 相关的服务计划有关的信息。[subscribedSku](subscribedsku.md) 实体的 **servicePlans** 属性是一个 **servicePlanInfo** 集合。</span><span class="sxs-lookup"><span data-stu-id="09682-p103">Contains information about a service plan associated with a subscribed SKU. The **servicePlans** property of the [subscribedSku](subscribedsku.md) entity is a collection of **servicePlanInfo**.</span></span>


## <a name="properties"></a><span data-ttu-id="09682-109">属性</span><span class="sxs-lookup"><span data-stu-id="09682-109">Properties</span></span>
| <span data-ttu-id="09682-110">属性</span><span class="sxs-lookup"><span data-stu-id="09682-110">Property</span></span>     | <span data-ttu-id="09682-111">类型</span><span class="sxs-lookup"><span data-stu-id="09682-111">Type</span></span>   |<span data-ttu-id="09682-112">说明</span><span class="sxs-lookup"><span data-stu-id="09682-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="09682-113">servicePlanId</span><span class="sxs-lookup"><span data-stu-id="09682-113">servicePlanId</span></span>|<span data-ttu-id="09682-114">Guid</span><span class="sxs-lookup"><span data-stu-id="09682-114">Guid</span></span>|<span data-ttu-id="09682-115">服务计划的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="09682-115">The unique identifier of the service plan.</span></span>|
|<span data-ttu-id="09682-116">servicePlanName</span><span class="sxs-lookup"><span data-stu-id="09682-116">servicePlanName</span></span>|<span data-ttu-id="09682-117">String</span><span class="sxs-lookup"><span data-stu-id="09682-117">String</span></span>|<span data-ttu-id="09682-118">服务计划的名称。</span><span class="sxs-lookup"><span data-stu-id="09682-118">The name of the service plan.</span></span>|
|<span data-ttu-id="09682-119">provisioningStatus</span><span class="sxs-lookup"><span data-stu-id="09682-119">provisioningStatus</span></span>|<span data-ttu-id="09682-120">字符串</span><span class="sxs-lookup"><span data-stu-id="09682-120">String</span></span>|<span data-ttu-id="09682-p104">服务计划的预配状态。可能的值：</span><span class="sxs-lookup"><span data-stu-id="09682-p104">The provisioning status of the service plan. Possible values:</span></span><br/><span data-ttu-id="09682-123">“Success” - 服务已完全预配。</span><span class="sxs-lookup"><span data-stu-id="09682-123">"Success" - Service is fully provisioned.</span></span><br/><span data-ttu-id="09682-124">“Disabled” - 服务已禁用。</span><span class="sxs-lookup"><span data-stu-id="09682-124">"Disabled" - Service has been disabled.</span></span><br/><span data-ttu-id="09682-125">“PendingInput” - 服务尚未预配；等待服务确认。</span><span class="sxs-lookup"><span data-stu-id="09682-125">"PendingInput" - Service is not yet provisioned; awaiting service confirmation.</span></span><br/><span data-ttu-id="09682-126">"PendingActivation"-服务设置，但需要由管理员 （例如，Intune_O365 服务计划） 的显式激活。</span><span class="sxs-lookup"><span data-stu-id="09682-126">"PendingActivation" - Service is provisioned but requires explicit activation by administrator (for example, Intune_O365 service plan).</span></span><br/><span data-ttu-id="09682-127">“PendingProvisioning” - Microsoft 已将新服务添加到产品 SKU，但它尚未在租户中激活。</span><span class="sxs-lookup"><span data-stu-id="09682-127">"PendingProvisioning" - Microsoft has added a new service to the product SKU and it has not been activated in the tenant, yet.</span></span>|
|<span data-ttu-id="09682-128">appliesTo</span><span class="sxs-lookup"><span data-stu-id="09682-128">appliesTo</span></span>|<span data-ttu-id="09682-129">字符串</span><span class="sxs-lookup"><span data-stu-id="09682-129">String</span></span>|<span data-ttu-id="09682-p105">可以向其分配服务计划的对象。可能的值：</span><span class="sxs-lookup"><span data-stu-id="09682-p105">The object the service plan can be assigned to. Possible values:</span></span><br/><span data-ttu-id="09682-132">“User” - 服务计划可分配给各个用户。</span><span class="sxs-lookup"><span data-stu-id="09682-132">"User" - service plan can be assigned to individual users.</span></span><br/><span data-ttu-id="09682-133">“Company” - 服务计划可分配给整个租户。</span><span class="sxs-lookup"><span data-stu-id="09682-133">"Company" - service plan can be assigned to the entire tenant.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="09682-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="09682-134">JSON representation</span></span>

<span data-ttu-id="09682-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="09682-135">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.servicePlanInfo"
}-->

```json
{
  "appliesTo": "string",
  "provisioningStatus": "string",
  "servicePlanId": "guid",
  "servicePlanName": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "servicePlanInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

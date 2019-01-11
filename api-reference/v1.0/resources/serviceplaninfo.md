---
title: servicePlanInfo 资源类型
description: 包含与订阅的 SKU 相关的服务计划有关的信息。subscribedSku 实体的 **servicePlans** 属性是一个 **servicePlanInfo** 集合。
localization_priority: Normal
ms.openlocfilehash: 837170881c7c093d26c5b59662e20e87b399a029
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845449"
---
# <a name="serviceplaninfo-resource-type"></a><span data-ttu-id="f1bb5-104">servicePlanInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="f1bb5-104">servicePlanInfo resource type</span></span>

<span data-ttu-id="f1bb5-p102">包含与订阅的 SKU 相关的服务计划有关的信息。[subscribedSku](subscribedsku.md) 实体的 **servicePlans** 属性是一个 **servicePlanInfo** 集合。</span><span class="sxs-lookup"><span data-stu-id="f1bb5-p102">Contains information about a service plan associated with a subscribed SKU. The **servicePlans** property of the [subscribedSku](subscribedsku.md) entity is a collection of **servicePlanInfo**.</span></span>


## <a name="properties"></a><span data-ttu-id="f1bb5-107">属性</span><span class="sxs-lookup"><span data-stu-id="f1bb5-107">Properties</span></span>
| <span data-ttu-id="f1bb5-108">属性</span><span class="sxs-lookup"><span data-stu-id="f1bb5-108">Property</span></span>     | <span data-ttu-id="f1bb5-109">类型</span><span class="sxs-lookup"><span data-stu-id="f1bb5-109">Type</span></span>   |<span data-ttu-id="f1bb5-110">说明</span><span class="sxs-lookup"><span data-stu-id="f1bb5-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f1bb5-111">servicePlanId</span><span class="sxs-lookup"><span data-stu-id="f1bb5-111">servicePlanId</span></span>|<span data-ttu-id="f1bb5-112">Guid</span><span class="sxs-lookup"><span data-stu-id="f1bb5-112">Guid</span></span>|<span data-ttu-id="f1bb5-113">服务计划的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="f1bb5-113">The unique identifier of the service plan.</span></span>|
|<span data-ttu-id="f1bb5-114">servicePlanName</span><span class="sxs-lookup"><span data-stu-id="f1bb5-114">servicePlanName</span></span>|<span data-ttu-id="f1bb5-115">String</span><span class="sxs-lookup"><span data-stu-id="f1bb5-115">String</span></span>|<span data-ttu-id="f1bb5-116">服务计划的名称。</span><span class="sxs-lookup"><span data-stu-id="f1bb5-116">The name of the service plan.</span></span>|
|<span data-ttu-id="f1bb5-117">provisioningStatus</span><span class="sxs-lookup"><span data-stu-id="f1bb5-117">provisioningStatus</span></span>|<span data-ttu-id="f1bb5-118">字符串</span><span class="sxs-lookup"><span data-stu-id="f1bb5-118">String</span></span>|<span data-ttu-id="f1bb5-p103">服务计划的预配状态。可能的值：</span><span class="sxs-lookup"><span data-stu-id="f1bb5-p103">The provisioning status of the service plan. Possible values:</span></span><br/><span data-ttu-id="f1bb5-121">“Success” - 服务已完全预配。</span><span class="sxs-lookup"><span data-stu-id="f1bb5-121">"Success" - Service is fully provisioned.</span></span><br/><span data-ttu-id="f1bb5-122">“Disabled” - 服务已禁用。</span><span class="sxs-lookup"><span data-stu-id="f1bb5-122">"Disabled" - Service has been disabled.</span></span><br/><span data-ttu-id="f1bb5-123">“PendingInput” - 服务尚未预配；等待服务确认。</span><span class="sxs-lookup"><span data-stu-id="f1bb5-123">"PendingInput" - Service is not yet provisioned; awaiting service confirmation.</span></span><br/><span data-ttu-id="f1bb5-124">“PendingActivation” - 服务已预配，但需要由管理员显式激活（例如，Intune_O365 服务计划）</span><span class="sxs-lookup"><span data-stu-id="f1bb5-124">"PendingActivation" - Service is provisioned but requires explicit activation by administrator (for example, Intune_O365 service plan)</span></span><br/><span data-ttu-id="f1bb5-125">“PendingProvisioning” - Microsoft 已将新服务添加到产品 SKU，但它尚未在租户中激活。</span><span class="sxs-lookup"><span data-stu-id="f1bb5-125">"PendingProvisioning" - Microsoft has added a new service to the product SKU and it has not been activated in the tenant, yet.</span></span>|
|<span data-ttu-id="f1bb5-126">appliesTo</span><span class="sxs-lookup"><span data-stu-id="f1bb5-126">appliesTo</span></span>|<span data-ttu-id="f1bb5-127">字符串</span><span class="sxs-lookup"><span data-stu-id="f1bb5-127">String</span></span>|<span data-ttu-id="f1bb5-p104">可以向其分配服务计划的对象。可能的值：</span><span class="sxs-lookup"><span data-stu-id="f1bb5-p104">The object the service plan can be assigned to. Possible values:</span></span><br/><span data-ttu-id="f1bb5-130">“User” - 服务计划可分配给各个用户。</span><span class="sxs-lookup"><span data-stu-id="f1bb5-130">"User" - service plan can be assigned to individual users.</span></span><br/><span data-ttu-id="f1bb5-131">“Company” - 服务计划可分配给整个租户。</span><span class="sxs-lookup"><span data-stu-id="f1bb5-131">"Company" - service plan can be assigned to the entire tenant.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f1bb5-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f1bb5-132">JSON representation</span></span>

<span data-ttu-id="f1bb5-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f1bb5-133">Here is a JSON representation of the resource</span></span>

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

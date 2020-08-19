---
title: servicePlanInfo 资源类型
description: 包含与订阅的 SKU 相关联的服务计划的相关信息。 SubscribedSku 实体的 **servicePlans** 属性是 **servicePlanInfo**的集合。
localization_priority: Normal
author: krbain
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 1f776f667ae45e362b6e70b76ed3758f4553f167
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46812616"
---
# <a name="serviceplaninfo-resource-type"></a><span data-ttu-id="d782b-104">servicePlanInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="d782b-104">servicePlanInfo resource type</span></span>

<span data-ttu-id="d782b-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d782b-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d782b-106">包含与订阅的 SKU 相关联的服务计划的相关信息。</span><span class="sxs-lookup"><span data-stu-id="d782b-106">Contains information about a service plan associated with a subscribed SKU.</span></span> <span data-ttu-id="d782b-107">[SubscribedSku](subscribedsku.md)实体的**ServicePlans**属性是**servicePlanInfo**的集合。</span><span class="sxs-lookup"><span data-stu-id="d782b-107">The **servicePlans** property of the [subscribedSku](subscribedsku.md) entity is a collection of **servicePlanInfo**.</span></span>


## <a name="properties"></a><span data-ttu-id="d782b-108">属性</span><span class="sxs-lookup"><span data-stu-id="d782b-108">Properties</span></span>
| <span data-ttu-id="d782b-109">属性</span><span class="sxs-lookup"><span data-stu-id="d782b-109">Property</span></span>     | <span data-ttu-id="d782b-110">类型</span><span class="sxs-lookup"><span data-stu-id="d782b-110">Type</span></span>   |<span data-ttu-id="d782b-111">说明</span><span class="sxs-lookup"><span data-stu-id="d782b-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d782b-112">servicePlanId</span><span class="sxs-lookup"><span data-stu-id="d782b-112">servicePlanId</span></span>|<span data-ttu-id="d782b-113">Guid</span><span class="sxs-lookup"><span data-stu-id="d782b-113">Guid</span></span>|<span data-ttu-id="d782b-114">服务计划的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="d782b-114">The unique identifier of the service plan.</span></span>|
|<span data-ttu-id="d782b-115">servicePlanName</span><span class="sxs-lookup"><span data-stu-id="d782b-115">servicePlanName</span></span>|<span data-ttu-id="d782b-116">String</span><span class="sxs-lookup"><span data-stu-id="d782b-116">String</span></span>|<span data-ttu-id="d782b-117">服务计划的名称。</span><span class="sxs-lookup"><span data-stu-id="d782b-117">The name of the service plan.</span></span>|
|<span data-ttu-id="d782b-118">provisioningStatus</span><span class="sxs-lookup"><span data-stu-id="d782b-118">provisioningStatus</span></span>|<span data-ttu-id="d782b-119">String</span><span class="sxs-lookup"><span data-stu-id="d782b-119">String</span></span>|<span data-ttu-id="d782b-120">服务计划的预配状态。</span><span class="sxs-lookup"><span data-stu-id="d782b-120">The provisioning status of the service plan.</span></span> <span data-ttu-id="d782b-121">可能的值：</span><span class="sxs-lookup"><span data-stu-id="d782b-121">Possible values:</span></span><br/><span data-ttu-id="d782b-122">"成功"-服务已完全预配。</span><span class="sxs-lookup"><span data-stu-id="d782b-122">"Success" - Service is fully provisioned.</span></span><br/><span data-ttu-id="d782b-123">"已禁用"-服务已禁用。</span><span class="sxs-lookup"><span data-stu-id="d782b-123">"Disabled" - Service has been disabled.</span></span><br/><span data-ttu-id="d782b-124">"PendingInput"-服务尚未预配;等待服务确认。</span><span class="sxs-lookup"><span data-stu-id="d782b-124">"PendingInput" - Service is not yet provisioned; awaiting service confirmation.</span></span><br/><span data-ttu-id="d782b-125">"PendingActivation"-服务已预配，但需要管理员进行显式激活 (例如，Intune_O365 Service plan) </span><span class="sxs-lookup"><span data-stu-id="d782b-125">"PendingActivation" - Service is provisioned but requires explicit activation by administrator (for example, Intune_O365 service plan)</span></span><br/><span data-ttu-id="d782b-126">"PendingProvisioning"-Microsoft 已向产品 SKU 添加了新服务，但尚未在租户中激活。</span><span class="sxs-lookup"><span data-stu-id="d782b-126">"PendingProvisioning" - Microsoft has added a new service to the product SKU and it has not been activated in the tenant, yet.</span></span>|
|<span data-ttu-id="d782b-127">appliesTo</span><span class="sxs-lookup"><span data-stu-id="d782b-127">appliesTo</span></span>|<span data-ttu-id="d782b-128">String</span><span class="sxs-lookup"><span data-stu-id="d782b-128">String</span></span>|<span data-ttu-id="d782b-129">可将服务计划分配到的对象。</span><span class="sxs-lookup"><span data-stu-id="d782b-129">The object the service plan can be assigned to.</span></span> <span data-ttu-id="d782b-130">可能的值：</span><span class="sxs-lookup"><span data-stu-id="d782b-130">Possible values:</span></span><br/><span data-ttu-id="d782b-131">"User"-服务计划可分配给单个用户。</span><span class="sxs-lookup"><span data-stu-id="d782b-131">"User" - service plan can be assigned to individual users.</span></span><br/><span data-ttu-id="d782b-132">"Company"-服务计划可分配给整个租户。</span><span class="sxs-lookup"><span data-stu-id="d782b-132">"Company" - service plan can be assigned to the entire tenant.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d782b-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d782b-133">JSON representation</span></span>

<span data-ttu-id="d782b-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d782b-134">Here is a JSON representation of the resource</span></span>

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

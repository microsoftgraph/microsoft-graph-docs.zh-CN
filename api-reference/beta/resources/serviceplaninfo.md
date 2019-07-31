---
title: servicePlanInfo 资源类型
description: 包含与订阅的 SKU 相关联的服务计划的相关信息。 SubscribedSku 实体的**servicePlans**属性是**servicePlanInfo**的集合。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 3b74ddbb26e61dd1c97342a61b30a3fff9ee1851
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008479"
---
# <a name="serviceplaninfo-resource-type"></a><span data-ttu-id="0ad30-104">servicePlanInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="0ad30-104">servicePlanInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0ad30-105">包含与订阅的 SKU 相关联的服务计划的相关信息。</span><span class="sxs-lookup"><span data-stu-id="0ad30-105">Contains information about a service plan associated with a subscribed SKU.</span></span> <span data-ttu-id="0ad30-106">[SubscribedSku](subscribedsku.md)实体的**ServicePlans**属性是**servicePlanInfo**的集合。</span><span class="sxs-lookup"><span data-stu-id="0ad30-106">The **servicePlans** property of the [subscribedSku](subscribedsku.md) entity is a collection of **servicePlanInfo**.</span></span>


## <a name="properties"></a><span data-ttu-id="0ad30-107">属性</span><span class="sxs-lookup"><span data-stu-id="0ad30-107">Properties</span></span>
| <span data-ttu-id="0ad30-108">属性</span><span class="sxs-lookup"><span data-stu-id="0ad30-108">Property</span></span>     | <span data-ttu-id="0ad30-109">类型</span><span class="sxs-lookup"><span data-stu-id="0ad30-109">Type</span></span>   |<span data-ttu-id="0ad30-110">说明</span><span class="sxs-lookup"><span data-stu-id="0ad30-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0ad30-111">servicePlanId</span><span class="sxs-lookup"><span data-stu-id="0ad30-111">servicePlanId</span></span>|<span data-ttu-id="0ad30-112">Guid</span><span class="sxs-lookup"><span data-stu-id="0ad30-112">Guid</span></span>|<span data-ttu-id="0ad30-113">服务计划的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="0ad30-113">The unique identifier of the service plan.</span></span>|
|<span data-ttu-id="0ad30-114">servicePlanName</span><span class="sxs-lookup"><span data-stu-id="0ad30-114">servicePlanName</span></span>|<span data-ttu-id="0ad30-115">String</span><span class="sxs-lookup"><span data-stu-id="0ad30-115">String</span></span>|<span data-ttu-id="0ad30-116">服务计划的名称。</span><span class="sxs-lookup"><span data-stu-id="0ad30-116">The name of the service plan.</span></span>|
|<span data-ttu-id="0ad30-117">provisioningStatus</span><span class="sxs-lookup"><span data-stu-id="0ad30-117">provisioningStatus</span></span>|<span data-ttu-id="0ad30-118">String</span><span class="sxs-lookup"><span data-stu-id="0ad30-118">String</span></span>|<span data-ttu-id="0ad30-119">服务计划的预配状态。</span><span class="sxs-lookup"><span data-stu-id="0ad30-119">The provisioning status of the service plan.</span></span> <span data-ttu-id="0ad30-120">可能的值：</span><span class="sxs-lookup"><span data-stu-id="0ad30-120">Possible values:</span></span><br/><span data-ttu-id="0ad30-121">"成功"-服务已完全预配。</span><span class="sxs-lookup"><span data-stu-id="0ad30-121">"Success" - Service is fully provisioned.</span></span><br/><span data-ttu-id="0ad30-122">"已禁用"-服务已禁用。</span><span class="sxs-lookup"><span data-stu-id="0ad30-122">"Disabled" - Service has been disabled.</span></span><br/><span data-ttu-id="0ad30-123">"PendingInput"-服务尚未预配;等待服务确认。</span><span class="sxs-lookup"><span data-stu-id="0ad30-123">"PendingInput" - Service is not yet provisioned; awaiting service confirmation.</span></span><br/><span data-ttu-id="0ad30-124">"PendingActivation"-服务已预配, 但需要管理员显式激活 (例如, Intune_O365 Service plan)。</span><span class="sxs-lookup"><span data-stu-id="0ad30-124">"PendingActivation" - Service is provisioned but requires explicit activation by administrator (for example, Intune_O365 service plan).</span></span><br/><span data-ttu-id="0ad30-125">"PendingProvisioning"-Microsoft 已向产品 SKU 添加了新服务, 但尚未在租户中激活。</span><span class="sxs-lookup"><span data-stu-id="0ad30-125">"PendingProvisioning" - Microsoft has added a new service to the product SKU and it has not been activated in the tenant, yet.</span></span>|
|<span data-ttu-id="0ad30-126">appliesTo</span><span class="sxs-lookup"><span data-stu-id="0ad30-126">appliesTo</span></span>|<span data-ttu-id="0ad30-127">String</span><span class="sxs-lookup"><span data-stu-id="0ad30-127">String</span></span>|<span data-ttu-id="0ad30-128">可将服务计划分配到的对象。</span><span class="sxs-lookup"><span data-stu-id="0ad30-128">The object the service plan can be assigned to.</span></span> <span data-ttu-id="0ad30-129">可能的值：</span><span class="sxs-lookup"><span data-stu-id="0ad30-129">Possible values:</span></span><br/><span data-ttu-id="0ad30-130">"User"-服务计划可分配给单个用户。</span><span class="sxs-lookup"><span data-stu-id="0ad30-130">"User" - service plan can be assigned to individual users.</span></span><br/><span data-ttu-id="0ad30-131">"Company"-服务计划可分配给整个租户。</span><span class="sxs-lookup"><span data-stu-id="0ad30-131">"Company" - service plan can be assigned to the entire tenant.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0ad30-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0ad30-132">JSON representation</span></span>

<span data-ttu-id="0ad30-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0ad30-133">Here is a JSON representation of the resource</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "servicePlanInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

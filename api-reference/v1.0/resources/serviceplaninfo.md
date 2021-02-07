---
title: servicePlanInfo 资源类型
description: 包含有关与订阅的 SKU 关联的服务计划的信息。 **subscribedSku** 实体的 servicePlans 属性是 **servicePlanInfo 的集合**。
localization_priority: Normal
author: krbain
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 0fe4ff98fd06932ee6f46ce2489c36cd2a524bc0
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50130169"
---
# <a name="serviceplaninfo-resource-type"></a><span data-ttu-id="6b926-104">servicePlanInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="6b926-104">servicePlanInfo resource type</span></span>

<span data-ttu-id="6b926-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6b926-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6b926-106">包含有关与订阅的 SKU 关联的服务计划的信息。</span><span class="sxs-lookup"><span data-stu-id="6b926-106">Contains information about a service plan associated with a subscribed SKU.</span></span> <span data-ttu-id="6b926-107">**subscribedSku** 实体的 [servicePlans](subscribedsku.md)属性是 **servicePlanInfo 的集合**。</span><span class="sxs-lookup"><span data-stu-id="6b926-107">The **servicePlans** property of the [subscribedSku](subscribedsku.md) entity is a collection of **servicePlanInfo**.</span></span>


## <a name="properties"></a><span data-ttu-id="6b926-108">属性</span><span class="sxs-lookup"><span data-stu-id="6b926-108">Properties</span></span>
| <span data-ttu-id="6b926-109">属性</span><span class="sxs-lookup"><span data-stu-id="6b926-109">Property</span></span>     | <span data-ttu-id="6b926-110">类型</span><span class="sxs-lookup"><span data-stu-id="6b926-110">Type</span></span>   |<span data-ttu-id="6b926-111">说明</span><span class="sxs-lookup"><span data-stu-id="6b926-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6b926-112">servicePlanId</span><span class="sxs-lookup"><span data-stu-id="6b926-112">servicePlanId</span></span>|<span data-ttu-id="6b926-113">Guid</span><span class="sxs-lookup"><span data-stu-id="6b926-113">Guid</span></span>|<span data-ttu-id="6b926-114">服务计划的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="6b926-114">The unique identifier of the service plan.</span></span>|
|<span data-ttu-id="6b926-115">servicePlanName</span><span class="sxs-lookup"><span data-stu-id="6b926-115">servicePlanName</span></span>|<span data-ttu-id="6b926-116">String</span><span class="sxs-lookup"><span data-stu-id="6b926-116">String</span></span>|<span data-ttu-id="6b926-117">服务计划的名称。</span><span class="sxs-lookup"><span data-stu-id="6b926-117">The name of the service plan.</span></span>|
|<span data-ttu-id="6b926-118">provisioningStatus</span><span class="sxs-lookup"><span data-stu-id="6b926-118">provisioningStatus</span></span>|<span data-ttu-id="6b926-119">String</span><span class="sxs-lookup"><span data-stu-id="6b926-119">String</span></span>|<span data-ttu-id="6b926-120">服务计划的预配状态。</span><span class="sxs-lookup"><span data-stu-id="6b926-120">The provisioning status of the service plan.</span></span> <span data-ttu-id="6b926-121">可能的值：</span><span class="sxs-lookup"><span data-stu-id="6b926-121">Possible values:</span></span><br/><span data-ttu-id="6b926-122">"成功"- 服务已完全预配。</span><span class="sxs-lookup"><span data-stu-id="6b926-122">"Success" - Service is fully provisioned.</span></span><br/><span data-ttu-id="6b926-123">"已禁用"- 服务已禁用。</span><span class="sxs-lookup"><span data-stu-id="6b926-123">"Disabled" - Service has been disabled.</span></span><br/><span data-ttu-id="6b926-124">"PendingInput"- 尚未设置服务;等待服务确认。</span><span class="sxs-lookup"><span data-stu-id="6b926-124">"PendingInput" - Service is not yet provisioned; awaiting service confirmation.</span></span><br/><span data-ttu-id="6b926-125">"PendingActivation"- 服务已设置，但需要管理员 (，例如，Intune_O365计划) </span><span class="sxs-lookup"><span data-stu-id="6b926-125">"PendingActivation" - Service is provisioned but requires explicit activation by administrator (for example, Intune_O365 service plan)</span></span><br/><span data-ttu-id="6b926-126">"PendingProvisioning"- Microsoft 向产品 SKU 添加了一个新服务，但尚未在租户中激活它。</span><span class="sxs-lookup"><span data-stu-id="6b926-126">"PendingProvisioning" - Microsoft has added a new service to the product SKU and it has not been activated in the tenant, yet.</span></span>|
|<span data-ttu-id="6b926-127">appliesTo</span><span class="sxs-lookup"><span data-stu-id="6b926-127">appliesTo</span></span>|<span data-ttu-id="6b926-128">String</span><span class="sxs-lookup"><span data-stu-id="6b926-128">String</span></span>|<span data-ttu-id="6b926-129">可以为其分配服务计划的对象。</span><span class="sxs-lookup"><span data-stu-id="6b926-129">The object the service plan can be assigned to.</span></span> <span data-ttu-id="6b926-130">可能的值：</span><span class="sxs-lookup"><span data-stu-id="6b926-130">Possible values:</span></span><br/><span data-ttu-id="6b926-131">"用户"- 可以将服务计划分配给单个用户。</span><span class="sxs-lookup"><span data-stu-id="6b926-131">"User" - service plan can be assigned to individual users.</span></span><br/><span data-ttu-id="6b926-132">"公司"- 可以将服务计划分配给整个租户。</span><span class="sxs-lookup"><span data-stu-id="6b926-132">"Company" - service plan can be assigned to the entire tenant.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6b926-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6b926-133">JSON representation</span></span>

<span data-ttu-id="6b926-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6b926-134">Here is a JSON representation of the resource</span></span>

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


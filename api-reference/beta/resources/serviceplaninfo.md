---
title: servicePlanInfo 资源类型
description: 包含与订阅的 SKU 相关的服务计划有关的信息。**subscribedSku** 实体的 **servicePlans** 属性是一个 servicePlanInfo 集合。
localization_priority: Normal
ms.openlocfilehash: e759082984cc66f7d3efec3cbb7cbee11561f253
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512603"
---
# <a name="serviceplaninfo-resource-type"></a><span data-ttu-id="97454-104">servicePlanInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="97454-104">servicePlanInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="97454-p102">包含与订阅的 SKU 相关的服务计划有关的信息。[subscribedSku](subscribedsku.md) 实体的 **servicePlans** 属性是一个 **servicePlanInfo** 集合。</span><span class="sxs-lookup"><span data-stu-id="97454-p102">Contains information about a service plan associated with a subscribed SKU. The **servicePlans** property of the [subscribedSku](subscribedsku.md) entity is a collection of **servicePlanInfo**.</span></span>


## <a name="properties"></a><span data-ttu-id="97454-107">属性</span><span class="sxs-lookup"><span data-stu-id="97454-107">Properties</span></span>
| <span data-ttu-id="97454-108">属性</span><span class="sxs-lookup"><span data-stu-id="97454-108">Property</span></span>     | <span data-ttu-id="97454-109">类型</span><span class="sxs-lookup"><span data-stu-id="97454-109">Type</span></span>   |<span data-ttu-id="97454-110">说明</span><span class="sxs-lookup"><span data-stu-id="97454-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="97454-111">servicePlanId</span><span class="sxs-lookup"><span data-stu-id="97454-111">servicePlanId</span></span>|<span data-ttu-id="97454-112">Guid</span><span class="sxs-lookup"><span data-stu-id="97454-112">Guid</span></span>|<span data-ttu-id="97454-113">服务计划的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="97454-113">The unique identifier of the service plan.</span></span>|
|<span data-ttu-id="97454-114">servicePlanName</span><span class="sxs-lookup"><span data-stu-id="97454-114">servicePlanName</span></span>|<span data-ttu-id="97454-115">String</span><span class="sxs-lookup"><span data-stu-id="97454-115">String</span></span>|<span data-ttu-id="97454-116">服务计划的名称。</span><span class="sxs-lookup"><span data-stu-id="97454-116">The name of the service plan.</span></span>|
|<span data-ttu-id="97454-117">provisioningStatus</span><span class="sxs-lookup"><span data-stu-id="97454-117">provisioningStatus</span></span>|<span data-ttu-id="97454-118">字符串</span><span class="sxs-lookup"><span data-stu-id="97454-118">String</span></span>|<span data-ttu-id="97454-p103">服务计划的预配状态。可能的值：</span><span class="sxs-lookup"><span data-stu-id="97454-p103">The provisioning status of the service plan. Possible values:</span></span><br/><span data-ttu-id="97454-121">“Success” - 服务已完全预配。</span><span class="sxs-lookup"><span data-stu-id="97454-121">"Success" - Service is fully provisioned.</span></span><br/><span data-ttu-id="97454-122">“Disabled” - 服务已禁用。</span><span class="sxs-lookup"><span data-stu-id="97454-122">"Disabled" - Service has been disabled.</span></span><br/><span data-ttu-id="97454-123">“PendingInput” - 服务尚未预配；等待服务确认。</span><span class="sxs-lookup"><span data-stu-id="97454-123">"PendingInput" - Service is not yet provisioned; awaiting service confirmation.</span></span><br/><span data-ttu-id="97454-124">"PendingActivation"-服务设置，但需要由管理员 （例如，Intune_O365 服务计划） 的显式激活。</span><span class="sxs-lookup"><span data-stu-id="97454-124">"PendingActivation" - Service is provisioned but requires explicit activation by administrator (for example, Intune_O365 service plan).</span></span><br/><span data-ttu-id="97454-125">“PendingProvisioning” - Microsoft 已将新服务添加到产品 SKU，但它尚未在租户中激活。</span><span class="sxs-lookup"><span data-stu-id="97454-125">"PendingProvisioning" - Microsoft has added a new service to the product SKU and it has not been activated in the tenant, yet.</span></span>|
|<span data-ttu-id="97454-126">appliesTo</span><span class="sxs-lookup"><span data-stu-id="97454-126">appliesTo</span></span>|<span data-ttu-id="97454-127">String</span><span class="sxs-lookup"><span data-stu-id="97454-127">String</span></span>|<span data-ttu-id="97454-p104">可以向其分配服务计划的对象。可能的值：</span><span class="sxs-lookup"><span data-stu-id="97454-p104">The object the service plan can be assigned to. Possible values:</span></span><br/><span data-ttu-id="97454-130">“User” - 服务计划可分配给各个用户。</span><span class="sxs-lookup"><span data-stu-id="97454-130">"User" - service plan can be assigned to individual users.</span></span><br/><span data-ttu-id="97454-131">“Company” - 服务计划可分配给整个租户。</span><span class="sxs-lookup"><span data-stu-id="97454-131">"Company" - service plan can be assigned to the entire tenant.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="97454-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="97454-132">JSON representation</span></span>

<span data-ttu-id="97454-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="97454-133">Here is a JSON representation of the resource</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/serviceplaninfo.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

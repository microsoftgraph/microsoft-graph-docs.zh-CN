# <a name="serviceplaninfo-resource-type"></a><span data-ttu-id="0874b-101">servicePlanInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="0874b-101">servicePlanInfo resource type</span></span>

<span data-ttu-id="0874b-p101">包含与订阅的 SKU 相关的服务计划有关的信息。[subscribedSku](subscribedsku.md) 实体的 **servicePlans** 属性是一个 **servicePlanInfo** 集合。</span><span class="sxs-lookup"><span data-stu-id="0874b-p101">Contains information about a service plan associated with a subscribed SKU. The **servicePlans** property of the [subscribedSku](subscribedsku.md) entity is a collection of **servicePlanInfo**.</span></span>


## <a name="properties"></a><span data-ttu-id="0874b-104">属性</span><span class="sxs-lookup"><span data-stu-id="0874b-104">Properties</span></span>
| <span data-ttu-id="0874b-105">属性</span><span class="sxs-lookup"><span data-stu-id="0874b-105">Property</span></span>     | <span data-ttu-id="0874b-106">类型</span><span class="sxs-lookup"><span data-stu-id="0874b-106">Type</span></span>   |<span data-ttu-id="0874b-107">说明</span><span class="sxs-lookup"><span data-stu-id="0874b-107">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0874b-108">servicePlanId</span><span class="sxs-lookup"><span data-stu-id="0874b-108">servicePlanId</span></span>|<span data-ttu-id="0874b-109">Guid</span><span class="sxs-lookup"><span data-stu-id="0874b-109">Guid</span></span>|<span data-ttu-id="0874b-110">服务计划的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="0874b-110">The unique identifier of the service plan.</span></span>|
|<span data-ttu-id="0874b-111">servicePlanName</span><span class="sxs-lookup"><span data-stu-id="0874b-111">servicePlanName</span></span>|<span data-ttu-id="0874b-112">String</span><span class="sxs-lookup"><span data-stu-id="0874b-112">String</span></span>|<span data-ttu-id="0874b-113">服务计划的名称。</span><span class="sxs-lookup"><span data-stu-id="0874b-113">The name of the service plan.</span></span>|
|<span data-ttu-id="0874b-114">provisioningStatus</span><span class="sxs-lookup"><span data-stu-id="0874b-114">provisioningStatus</span></span>|<span data-ttu-id="0874b-115">字符串</span><span class="sxs-lookup"><span data-stu-id="0874b-115">String</span></span>|<span data-ttu-id="0874b-p102">服务计划的预配状态。可能的值：</span><span class="sxs-lookup"><span data-stu-id="0874b-p102">The provisioning status of the service plan. Possible values:</span></span><br/><span data-ttu-id="0874b-118">“Success” - 服务已完全预配。</span><span class="sxs-lookup"><span data-stu-id="0874b-118">"Success" - Service is fully provisioned.</span></span><br/><span data-ttu-id="0874b-119">“Disabled” - 服务已禁用。</span><span class="sxs-lookup"><span data-stu-id="0874b-119">"Disabled" - Service has been disabled.</span></span><br/><span data-ttu-id="0874b-120">“PendingInput” - 服务尚未预配；等待服务确认。</span><span class="sxs-lookup"><span data-stu-id="0874b-120">"PendingInput" - Service is not yet provisioned; awaiting service confirmation.</span></span><br/><span data-ttu-id="0874b-121">“PendingActivation” - 服务已预配，但需要由管理员显式激活（例如，Intune_O365 服务计划）</span><span class="sxs-lookup"><span data-stu-id="0874b-121">"PendingActivation" - Service is provisioned but requires explicit activation by administrator (for example, Intune_O365 service plan)</span></span><br/><span data-ttu-id="0874b-122">“PendingProvisioning” - Microsoft 已将新服务添加到产品 SKU，但它尚未在租户中激活。</span><span class="sxs-lookup"><span data-stu-id="0874b-122">"PendingProvisioning" - Microsoft has added a new service to the product SKU and it has not been activated in the tenant, yet.</span></span>|
|<span data-ttu-id="0874b-123">appliesTo</span><span class="sxs-lookup"><span data-stu-id="0874b-123">appliesTo</span></span>|<span data-ttu-id="0874b-124">字符串</span><span class="sxs-lookup"><span data-stu-id="0874b-124">String</span></span>|<span data-ttu-id="0874b-p103">可以向其分配服务计划的对象。可能的值：</span><span class="sxs-lookup"><span data-stu-id="0874b-p103">The object the service plan can be assigned to. Possible values:</span></span><br/><span data-ttu-id="0874b-127">“User” - 服务计划可分配给各个用户。</span><span class="sxs-lookup"><span data-stu-id="0874b-127">"User" - service plan can be assigned to individual users.</span></span><br/><span data-ttu-id="0874b-128">“Company” - 服务计划可分配给整个租户。</span><span class="sxs-lookup"><span data-stu-id="0874b-128">"Company" - service plan can be assigned to the entire tenant.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0874b-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0874b-129">JSON representation</span></span>

<span data-ttu-id="0874b-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0874b-130">Here is a JSON representation of the resource</span></span>

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

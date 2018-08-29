# <a name="subscribedsku-resource-type"></a><span data-ttu-id="8030f-101">subscribedSku 资源类型</span><span class="sxs-lookup"><span data-stu-id="8030f-101">subscribedSku resource type</span></span>

<span data-ttu-id="8030f-102">包含有关公司订阅的服务 SKU 的信息。</span><span class="sxs-lookup"><span data-stu-id="8030f-102">Contains information about a service SKU that a company is subscribed to.</span></span>

<span data-ttu-id="8030f-p101">只支持在订阅的 SKU 上执行读取操作；不支持执行创建、更新和删除操作。不支持查询筛选表达式。继承自 [directoryObject](directoryobject.md)。</span><span class="sxs-lookup"><span data-stu-id="8030f-p101">Only the read operation is supported on subscribed SKUs; create, update, and delete are not supported. Query filter expressions are not supported. Inherits from [directoryObject](directoryobject.md).</span></span>

## <a name="methods"></a><span data-ttu-id="8030f-106">方法</span><span class="sxs-lookup"><span data-stu-id="8030f-106">Methods</span></span>
| <span data-ttu-id="8030f-107">方法</span><span class="sxs-lookup"><span data-stu-id="8030f-107">Method</span></span>           | <span data-ttu-id="8030f-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="8030f-108">Return Type</span></span>    |<span data-ttu-id="8030f-109">说明</span><span class="sxs-lookup"><span data-stu-id="8030f-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8030f-110">Get subscribedSku</span><span class="sxs-lookup"><span data-stu-id="8030f-110">Get subscribedSku</span></span>](../api/subscribedsku_get.md) | [<span data-ttu-id="8030f-111">subscribedSku</span><span class="sxs-lookup"><span data-stu-id="8030f-111">subscribedSku</span></span>](subscribedsku.md) |<span data-ttu-id="8030f-112">读取 subscribedSku 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="8030f-112">Read properties and relationships of subscribedSku object.</span></span>|
|[<span data-ttu-id="8030f-113">List subscribedsku</span><span class="sxs-lookup"><span data-stu-id="8030f-113">List subscribedSku</span></span>](../api/subscribedsku_list.md) | <span data-ttu-id="8030f-114">[subscribedSku](subscribedsku.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8030f-114">[subscribedSku](subscribedsku.md) collection</span></span> |<span data-ttu-id="8030f-115">检索组织已获取的商业订阅列表。</span><span class="sxs-lookup"><span data-stu-id="8030f-115">Retrieve the list of commercial subscriptions that an organization has acquired.</span></span>|

## <a name="properties"></a><span data-ttu-id="8030f-116">属性</span><span class="sxs-lookup"><span data-stu-id="8030f-116">Properties</span></span>
| <span data-ttu-id="8030f-117">属性</span><span class="sxs-lookup"><span data-stu-id="8030f-117">Property</span></span>     | <span data-ttu-id="8030f-118">类型</span><span class="sxs-lookup"><span data-stu-id="8030f-118">Type</span></span>   |<span data-ttu-id="8030f-119">说明</span><span class="sxs-lookup"><span data-stu-id="8030f-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8030f-120">appliesTo</span><span class="sxs-lookup"><span data-stu-id="8030f-120">appliesTo</span></span>|<span data-ttu-id="8030f-121">字符串</span><span class="sxs-lookup"><span data-stu-id="8030f-121">String</span></span>| <span data-ttu-id="8030f-122">例如，“用户”或“公司”。</span><span class="sxs-lookup"><span data-stu-id="8030f-122">For example, "User" or "Company".</span></span> |
|<span data-ttu-id="8030f-123">capabilityStatus</span><span class="sxs-lookup"><span data-stu-id="8030f-123">capabilityStatus</span></span>|<span data-ttu-id="8030f-124">字符串</span><span class="sxs-lookup"><span data-stu-id="8030f-124">String</span></span>| <span data-ttu-id="8030f-125">例如，“Enabled”。</span><span class="sxs-lookup"><span data-stu-id="8030f-125">For example, "Enabled".</span></span> |
|<span data-ttu-id="8030f-126">consumedUnits</span><span class="sxs-lookup"><span data-stu-id="8030f-126">consumedUnits</span></span>|<span data-ttu-id="8030f-127">Int32</span><span class="sxs-lookup"><span data-stu-id="8030f-127">Int32</span></span>| <span data-ttu-id="8030f-128">已分配的许可证数量。</span><span class="sxs-lookup"><span data-stu-id="8030f-128">The number of licenses that have been assigned.</span></span> |
|<span data-ttu-id="8030f-129">id</span><span class="sxs-lookup"><span data-stu-id="8030f-129">id</span></span>|<span data-ttu-id="8030f-130">字符串</span><span class="sxs-lookup"><span data-stu-id="8030f-130">String</span></span>| <span data-ttu-id="8030f-p102">订阅的 sku 对象的唯一标识符。密钥，不可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="8030f-p102">The unique identifier for the subscribed sku object. Key, not nullable.</span></span> |
|<span data-ttu-id="8030f-133">prepaidUnits</span><span class="sxs-lookup"><span data-stu-id="8030f-133">prepaidUnits</span></span>|[<span data-ttu-id="8030f-134">licenseUnitsDetail</span><span class="sxs-lookup"><span data-stu-id="8030f-134">licenseUnitsDetail</span></span>](licenseunitsdetail.md)| <span data-ttu-id="8030f-135">有关预付许可证的数量和状态的信息。</span><span class="sxs-lookup"><span data-stu-id="8030f-135">Information about the number and status of prepaid licenses.</span></span> |
|<span data-ttu-id="8030f-136">servicePlans</span><span class="sxs-lookup"><span data-stu-id="8030f-136">servicePlans</span></span>|<span data-ttu-id="8030f-137">[servicePlanInfo](serviceplaninfo.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8030f-137">[servicePlanInfo](serviceplaninfo.md) collection</span></span>| <span data-ttu-id="8030f-p103">有关 SKU 可用服务计划的信息。不可为 null</span><span class="sxs-lookup"><span data-stu-id="8030f-p103">Information about the service plans that are available with the SKU. Not nullable</span></span> |
|<span data-ttu-id="8030f-140">skuId</span><span class="sxs-lookup"><span data-stu-id="8030f-140">skuId</span></span>|<span data-ttu-id="8030f-141">Guid</span><span class="sxs-lookup"><span data-stu-id="8030f-141">Guid</span></span>| <span data-ttu-id="8030f-142">服务 SKU 的唯一标识符 (GUID)。</span><span class="sxs-lookup"><span data-stu-id="8030f-142">The unique identifier (GUID) for the service SKU.</span></span> |
|<span data-ttu-id="8030f-143">skuPartNumber</span><span class="sxs-lookup"><span data-stu-id="8030f-143">skuPartNumber</span></span>|<span data-ttu-id="8030f-144">字符串</span><span class="sxs-lookup"><span data-stu-id="8030f-144">String</span></span>| <span data-ttu-id="8030f-145">SKU 商品编号；例如：“AAD_PREMIUM”或“RMSBASIC”。</span><span class="sxs-lookup"><span data-stu-id="8030f-145">The SKU part number; for example: "AAD_PREMIUM" or "RMSBASIC".</span></span> |

## <a name="relationships"></a><span data-ttu-id="8030f-146">关系</span><span class="sxs-lookup"><span data-stu-id="8030f-146">Relationships</span></span>
<span data-ttu-id="8030f-147">无</span><span class="sxs-lookup"><span data-stu-id="8030f-147">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8030f-148">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8030f-148">JSON representation</span></span>

<span data-ttu-id="8030f-149">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8030f-149">Here is a JSON representation of the resource</span></span>

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

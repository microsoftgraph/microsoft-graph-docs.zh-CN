# <a name="licensedetails-resource-type"></a><span data-ttu-id="1b788-101">licenseDetails 资源类型</span><span class="sxs-lookup"><span data-stu-id="1b788-101">licenseDetails resource type</span></span>

<span data-ttu-id="1b788-102">包含已分配给用户的许可证的相关信息。</span><span class="sxs-lookup"><span data-stu-id="1b788-102">Contains information about a license assigned to a user.</span></span>

## <a name="methods"></a><span data-ttu-id="1b788-103">方法</span><span class="sxs-lookup"><span data-stu-id="1b788-103">Methods</span></span>

| <span data-ttu-id="1b788-104">方法</span><span class="sxs-lookup"><span data-stu-id="1b788-104">Method</span></span>           | <span data-ttu-id="1b788-105">返回类型</span><span class="sxs-lookup"><span data-stu-id="1b788-105">Return Type</span></span>    |<span data-ttu-id="1b788-106">说明</span><span class="sxs-lookup"><span data-stu-id="1b788-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1b788-107">列举 licenseDetails</span><span class="sxs-lookup"><span data-stu-id="1b788-107">List licenseDetails</span></span>](../api/user_list_licensedetails.md) | <span data-ttu-id="1b788-108">licenseDetails 集合</span><span class="sxs-lookup"><span data-stu-id="1b788-108">licenseDetails collection</span></span> |<span data-ttu-id="1b788-109">检索用户的 licenseDetails 对象列表。</span><span class="sxs-lookup"><span data-stu-id="1b788-109">Retrieve a list of licenseDetails objects for a user.</span></span>|

<!--|[Get licenseDetails](../api/licensedetails_get.md) | licenseDetails |Read properties and relationships of a licenseDetails object.|-->

## <a name="properties"></a><span data-ttu-id="1b788-110">属性</span><span class="sxs-lookup"><span data-stu-id="1b788-110">Properties</span></span>
| <span data-ttu-id="1b788-111">属性</span><span class="sxs-lookup"><span data-stu-id="1b788-111">Property</span></span>     | <span data-ttu-id="1b788-112">类型</span><span class="sxs-lookup"><span data-stu-id="1b788-112">Type</span></span>   |<span data-ttu-id="1b788-113">说明</span><span class="sxs-lookup"><span data-stu-id="1b788-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1b788-114">ID</span><span class="sxs-lookup"><span data-stu-id="1b788-114">id</span></span>|<span data-ttu-id="1b788-115">字符串</span><span class="sxs-lookup"><span data-stu-id="1b788-115">String</span></span>| <span data-ttu-id="1b788-p101">许可证详细信息对象的唯一标识符。只读，密钥，不可为 NULL</span><span class="sxs-lookup"><span data-stu-id="1b788-p101">The unique identifier for the license detail object. Read-only, Key, Not nullable</span></span> |
|<span data-ttu-id="1b788-118">servicePlans</span><span class="sxs-lookup"><span data-stu-id="1b788-118">servicePlans</span></span>|<span data-ttu-id="1b788-119">[servicePlanInfo](serviceplaninfo.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1b788-119">[servicePlanInfo](serviceplaninfo.md) collection</span></span>| <span data-ttu-id="1b788-p102">许可证分配的服务计划的相关信息。只读，不可为 Null</span><span class="sxs-lookup"><span data-stu-id="1b788-p102">Information about the service plans assigned with the license. Read-only, Not nullable</span></span> |
|<span data-ttu-id="1b788-122">skuId</span><span class="sxs-lookup"><span data-stu-id="1b788-122">skuId</span></span>|<span data-ttu-id="1b788-123">全局唯一标识符</span><span class="sxs-lookup"><span data-stu-id="1b788-123">Guid</span></span>| <span data-ttu-id="1b788-p103">服务 SKU 的唯一标识符 (GUID)。等同于相关的 [SubscribedSku](subscribedsku.md) 对象上的 skuId 属性。只读</span><span class="sxs-lookup"><span data-stu-id="1b788-p103">Unique identifier (GUID) for the service SKU. Equal to the skuId property on the related [SubscribedSku](subscribedsku.md) object. Read-only</span></span> |
|<span data-ttu-id="1b788-127">skuPartNumber</span><span class="sxs-lookup"><span data-stu-id="1b788-127">skuPartNumber</span></span>|<span data-ttu-id="1b788-128">字符串</span><span class="sxs-lookup"><span data-stu-id="1b788-128">String</span></span>| <span data-ttu-id="1b788-p104">唯一的 SKU 显示名称。等同于相关的 [SubscribedSku](subscribedsku.md) 对象上的 skuPartNumber；例如：“AAD_Premium”。只读</span><span class="sxs-lookup"><span data-stu-id="1b788-p104">Unique SKU display name. Equal to the skuPartNumber on the related [SubscribedSku](subscribedsku.md) object; for example: "AAD_Premium". Read-only</span></span> |

## <a name="relationships"></a><span data-ttu-id="1b788-132">关系</span><span class="sxs-lookup"><span data-stu-id="1b788-132">Relationships</span></span>
<span data-ttu-id="1b788-133">无</span><span class="sxs-lookup"><span data-stu-id="1b788-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1b788-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1b788-134">JSON representation</span></span>
<span data-ttu-id="1b788-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1b788-135">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.licenseDetails"
}-->

```json
{
  "id": "String (identifier)",
  "servicePlans": [{"@odata.type": "microsoft.graph.servicePlanInfo"}],
  "skuId": "Guid",
  "skuPartNumber": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "licenseDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
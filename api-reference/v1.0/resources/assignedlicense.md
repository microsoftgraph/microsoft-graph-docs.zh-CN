# <a name="assignedlicense-resource-type"></a><span data-ttu-id="73831-101">assignedLicense 资源类型</span><span class="sxs-lookup"><span data-stu-id="73831-101">assignedLicense resource type</span></span>

<span data-ttu-id="73831-p101">表示分配给用户的许可证。[用户](user.md) 实体的 **AssignedLicenses** 属性是一个 **assignedLicense** 集合。</span><span class="sxs-lookup"><span data-stu-id="73831-p101">Represents a license assigned to a user. The **assignedLicenses** property of the [user](user.md) entity is a collection of **assignedLicense**.</span></span>

## <a name="properties"></a><span data-ttu-id="73831-104">属性</span><span class="sxs-lookup"><span data-stu-id="73831-104">Properties</span></span>
| <span data-ttu-id="73831-105">属性</span><span class="sxs-lookup"><span data-stu-id="73831-105">Property</span></span>     | <span data-ttu-id="73831-106">类型</span><span class="sxs-lookup"><span data-stu-id="73831-106">Type</span></span>   |<span data-ttu-id="73831-107">说明</span><span class="sxs-lookup"><span data-stu-id="73831-107">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="73831-108">disabledPlans</span><span class="sxs-lookup"><span data-stu-id="73831-108">disabledPlans</span></span>|<span data-ttu-id="73831-109">Guid 集合</span><span class="sxs-lookup"><span data-stu-id="73831-109">Guid collection</span></span>|<span data-ttu-id="73831-110">已禁用的计划的唯一标识符的集合。</span><span class="sxs-lookup"><span data-stu-id="73831-110">A collection of the unique identifiers for plans that have been disabled.</span></span>|
|<span data-ttu-id="73831-111">skuId</span><span class="sxs-lookup"><span data-stu-id="73831-111">skuId</span></span>|<span data-ttu-id="73831-112">Guid</span><span class="sxs-lookup"><span data-stu-id="73831-112">Guid</span></span>|<span data-ttu-id="73831-113">此 SKU 的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="73831-113">The unique identifier for the SKU.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="73831-114">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="73831-114">JSON representation</span></span>

<span data-ttu-id="73831-115">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="73831-115">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.assignedLicense"
}-->

```json
{
  "disabledPlans": ["guid"],
  "skuId": "guid"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "assignedLicense resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

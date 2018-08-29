# <a name="provisionedplan-resource-type"></a><span data-ttu-id="d57e8-101">provisionedPlan 资源类型</span><span class="sxs-lookup"><span data-stu-id="d57e8-101">provisionedPlan resource type</span></span>

<span data-ttu-id="d57e8-102">[用户](user.md) 实体和 [组织](organization.md) 实体的 **provisionedPlans** 属性都是一个 **provisionedPlan** 集合。</span><span class="sxs-lookup"><span data-stu-id="d57e8-102">The **provisionedPlans** property of the [user](user.md) entity and the [organization](organization.md) entity is a collection of **provisionedPlan**.</span></span>


## <a name="properties"></a><span data-ttu-id="d57e8-103">属性</span><span class="sxs-lookup"><span data-stu-id="d57e8-103">Properties</span></span>
| <span data-ttu-id="d57e8-104">属性</span><span class="sxs-lookup"><span data-stu-id="d57e8-104">Property</span></span>     | <span data-ttu-id="d57e8-105">类型</span><span class="sxs-lookup"><span data-stu-id="d57e8-105">Type</span></span>   |<span data-ttu-id="d57e8-106">说明</span><span class="sxs-lookup"><span data-stu-id="d57e8-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d57e8-107">capabilityStatus</span><span class="sxs-lookup"><span data-stu-id="d57e8-107">capabilityStatus</span></span>|<span data-ttu-id="d57e8-108">String</span><span class="sxs-lookup"><span data-stu-id="d57e8-108">String</span></span>|<span data-ttu-id="d57e8-109">例如，“Enabled”。</span><span class="sxs-lookup"><span data-stu-id="d57e8-109">For example, “Enabled”.</span></span>|
|<span data-ttu-id="d57e8-110">provisioningStatus</span><span class="sxs-lookup"><span data-stu-id="d57e8-110">provisioningStatus</span></span>|<span data-ttu-id="d57e8-111">String</span><span class="sxs-lookup"><span data-stu-id="d57e8-111">String</span></span>|<span data-ttu-id="d57e8-112">例如，“Success”。</span><span class="sxs-lookup"><span data-stu-id="d57e8-112">For example, “Success”.</span></span>|
|<span data-ttu-id="d57e8-113">service</span><span class="sxs-lookup"><span data-stu-id="d57e8-113">service</span></span>|<span data-ttu-id="d57e8-114">String</span><span class="sxs-lookup"><span data-stu-id="d57e8-114">String</span></span>|<span data-ttu-id="d57e8-115">服务名称；例如，“AccessControlS2S”</span><span class="sxs-lookup"><span data-stu-id="d57e8-115">The name of the service; for example, “AccessControlS2S”</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d57e8-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d57e8-116">JSON representation</span></span>

<span data-ttu-id="d57e8-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d57e8-117">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.provisionedPlan"
}-->

```json
{
  "capabilityStatus": "string",
  "provisioningStatus": "string",
  "service": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "provisionedPlan resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
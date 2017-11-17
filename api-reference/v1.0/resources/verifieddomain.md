# <a name="verifieddomain-resource-type"></a><span data-ttu-id="00890-101">verifiedDomain 资源类型</span><span class="sxs-lookup"><span data-stu-id="00890-101">verifiedDomain resource type</span></span>

<span data-ttu-id="00890-p101">指定租户的域。[组织](organization.md) 实体的 **verifiedDomains** 属性是一个 **VerifiedDomain** 集合。</span><span class="sxs-lookup"><span data-stu-id="00890-p101">Specifies a domain for a tenant. The **verifiedDomains** property of the [organization](organization.md) entity is a collection of **VerifiedDomain**.</span></span>


## <a name="properties"></a><span data-ttu-id="00890-104">属性</span><span class="sxs-lookup"><span data-stu-id="00890-104">Properties</span></span>
| <span data-ttu-id="00890-105">属性</span><span class="sxs-lookup"><span data-stu-id="00890-105">Property</span></span>     | <span data-ttu-id="00890-106">类型</span><span class="sxs-lookup"><span data-stu-id="00890-106">Type</span></span>   |<span data-ttu-id="00890-107">说明</span><span class="sxs-lookup"><span data-stu-id="00890-107">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="00890-108">capabilities</span><span class="sxs-lookup"><span data-stu-id="00890-108">capabilities</span></span>|<span data-ttu-id="00890-109">String</span><span class="sxs-lookup"><span data-stu-id="00890-109">String</span></span>|<span data-ttu-id="00890-110">例如，“Email”、“OfficeCommunicationsOnline”。</span><span class="sxs-lookup"><span data-stu-id="00890-110">For example, “Email”, “OfficeCommunicationsOnline”.</span></span>|
|<span data-ttu-id="00890-111">isDefault</span><span class="sxs-lookup"><span data-stu-id="00890-111">isDefault</span></span>|<span data-ttu-id="00890-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="00890-112">Boolean</span></span>|                <span data-ttu-id="00890-113">如果这是与租户关联的默认域，则为 **true**；否则为 **false**。</span><span class="sxs-lookup"><span data-stu-id="00890-113">**true** if this is the default domain associated with the tenant; otherwise, **false**.</span></span>            |
|<span data-ttu-id="00890-114">isInitial</span><span class="sxs-lookup"><span data-stu-id="00890-114">isInitial</span></span>|<span data-ttu-id="00890-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="00890-115">Boolean</span></span>|<span data-ttu-id="00890-116">如果这是与租户关联的初始域，则为 **true**；否则为 **false**</span><span class="sxs-lookup"><span data-stu-id="00890-116">**true** if this is the initial domain associated with the tenant; otherwise, **false**</span></span>|
|<span data-ttu-id="00890-117">name</span><span class="sxs-lookup"><span data-stu-id="00890-117">name</span></span>|<span data-ttu-id="00890-118">String</span><span class="sxs-lookup"><span data-stu-id="00890-118">String</span></span>|<span data-ttu-id="00890-119">域名；例如，“contoso.onmicrosoft.com”</span><span class="sxs-lookup"><span data-stu-id="00890-119">The domain name; for example, “contoso.onmicrosoft.com”</span></span>|
|<span data-ttu-id="00890-120">type</span><span class="sxs-lookup"><span data-stu-id="00890-120">type</span></span>|<span data-ttu-id="00890-121">String</span><span class="sxs-lookup"><span data-stu-id="00890-121">String</span></span>|<span data-ttu-id="00890-122">例如，“Managed”。</span><span class="sxs-lookup"><span data-stu-id="00890-122">For example, “Managed”.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="00890-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="00890-123">JSON representation</span></span>

<span data-ttu-id="00890-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="00890-124">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.verifieddomain"
}-->

```json
{
  "capabilities": "string",
  "isDefault": true,
  "isInitial": true,
  "name": "string",
  "type": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "verifiedDomain resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

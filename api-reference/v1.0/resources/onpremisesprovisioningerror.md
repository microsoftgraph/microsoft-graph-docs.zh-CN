# <a name="onpremisesprovisioningerror-resource-type"></a><span data-ttu-id="486d0-101">onPremisesProvisioningError 资源类型</span><span class="sxs-lookup"><span data-stu-id="486d0-101">onPremisesProvisioningError resource type</span></span>

<span data-ttu-id="486d0-102">表示同步本地目录到 Azure Active Directory 目录时 [user](user.md) 和 [group](group.md) 实体的目录同步错误。</span><span class="sxs-lookup"><span data-stu-id="486d0-102">Represents directory synchronization errors for the [user](user.md) and [group](group.md) entities when synchronizing on-premises directories to Azure Active Directory.</span></span>

## <a name="properties"></a><span data-ttu-id="486d0-103">属性</span><span class="sxs-lookup"><span data-stu-id="486d0-103">Properties</span></span>

| <span data-ttu-id="486d0-104">属性</span><span class="sxs-lookup"><span data-stu-id="486d0-104">Property</span></span> | <span data-ttu-id="486d0-105">类型</span><span class="sxs-lookup"><span data-stu-id="486d0-105">Type</span></span> | <span data-ttu-id="486d0-106">说明</span><span class="sxs-lookup"><span data-stu-id="486d0-106">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="486d0-107">category</span><span class="sxs-lookup"><span data-stu-id="486d0-107">category</span></span>|<span data-ttu-id="486d0-108">字符串</span><span class="sxs-lookup"><span data-stu-id="486d0-108">String</span></span>| <span data-ttu-id="486d0-109">设置错误的类别。</span><span class="sxs-lookup"><span data-stu-id="486d0-109">Category of the provisioning error.</span></span> <span data-ttu-id="486d0-110">注意：当前只有一个可能的值。</span><span class="sxs-lookup"><span data-stu-id="486d0-110">Note: Currently, there is only one possible value.</span></span> <span data-ttu-id="486d0-111">可能的值：*PropertyConflict* - 指示属性值不唯一。</span><span class="sxs-lookup"><span data-stu-id="486d0-111">Possible value: *PropertyConflict* - indicates a property value is not unique.</span></span> <span data-ttu-id="486d0-112">其他对象包含属性的相同值。</span><span class="sxs-lookup"><span data-stu-id="486d0-112">Other objects contain the same value for the property.</span></span> |
|<span data-ttu-id="486d0-113">occurredDateTime</span><span class="sxs-lookup"><span data-stu-id="486d0-113">occurredDateTime</span></span>|<span data-ttu-id="486d0-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="486d0-114">DateTimeOffset</span></span>| <span data-ttu-id="486d0-115">发生错误的日期 和时间。</span><span class="sxs-lookup"><span data-stu-id="486d0-115">The time at which the error occurred.</span></span> |
|<span data-ttu-id="486d0-116">propertyCausingError</span><span class="sxs-lookup"><span data-stu-id="486d0-116">propertyCausingError</span></span>|<span data-ttu-id="486d0-117">字符串</span><span class="sxs-lookup"><span data-stu-id="486d0-117">String</span></span>| <span data-ttu-id="486d0-118">导致此错误的目录属性的名称。</span><span class="sxs-lookup"><span data-stu-id="486d0-118">Name of the directory property causing the error.</span></span> <span data-ttu-id="486d0-119">当前的可能值：*UserPrincipalName* 或 *ProxyAddress*</span><span class="sxs-lookup"><span data-stu-id="486d0-119">Current possible values: *UserPrincipalName* or *ProxyAddress*</span></span> |
|<span data-ttu-id="486d0-120">value</span><span class="sxs-lookup"><span data-stu-id="486d0-120">value</span></span>|<span data-ttu-id="486d0-121">字符串</span><span class="sxs-lookup"><span data-stu-id="486d0-121">String</span></span>| <span data-ttu-id="486d0-122">导致错误的属性的值。</span><span class="sxs-lookup"><span data-stu-id="486d0-122">Value of the property causing the error.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="486d0-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="486d0-123">JSON representation</span></span>
<span data-ttu-id="486d0-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="486d0-124">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onPremisesProvisioningError"
}-->

```json
{
  "category": "String",
  "occurredDateTime": "String (timestamp)",
  "propertyCausingError": "String",
  "value": "String"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onPremisesProvisioningError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
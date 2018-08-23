# <a name="educationorganization-resource-type"></a><span data-ttu-id="77a6d-101">educationOrganization 资源类型</span><span class="sxs-lookup"><span data-stu-id="77a6d-101">educationOrganization resource type</span></span>

<span data-ttu-id="77a6d-102">用于模拟教育扇区中不同组织类型之间的通用性的抽象实体。</span><span class="sxs-lookup"><span data-stu-id="77a6d-102">Abstract entity used to model the commonality between different organization types within the education sector.</span></span>

## <a name="properties"></a><span data-ttu-id="77a6d-103">属性</span><span class="sxs-lookup"><span data-stu-id="77a6d-103">Properties</span></span>
| <span data-ttu-id="77a6d-104">属性</span><span class="sxs-lookup"><span data-stu-id="77a6d-104">Property</span></span>     | <span data-ttu-id="77a6d-105">类型</span><span class="sxs-lookup"><span data-stu-id="77a6d-105">Type</span></span>   |<span data-ttu-id="77a6d-106">说明</span><span class="sxs-lookup"><span data-stu-id="77a6d-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="77a6d-107">说明</span><span class="sxs-lookup"><span data-stu-id="77a6d-107">description</span></span>|<span data-ttu-id="77a6d-108">字符串</span><span class="sxs-lookup"><span data-stu-id="77a6d-108">String</span></span>| <span data-ttu-id="77a6d-109">组织说明。</span><span class="sxs-lookup"><span data-stu-id="77a6d-109">Organization description.</span></span>|
|<span data-ttu-id="77a6d-110">displayName</span><span class="sxs-lookup"><span data-stu-id="77a6d-110">displayName</span></span>|<span data-ttu-id="77a6d-111">字符串</span><span class="sxs-lookup"><span data-stu-id="77a6d-111">String</span></span>| <span data-ttu-id="77a6d-112">组织的显示名称。</span><span class="sxs-lookup"><span data-stu-id="77a6d-112">Organization display name.</span></span>|
|<span data-ttu-id="77a6d-113">externalSource</span><span class="sxs-lookup"><span data-stu-id="77a6d-113">externalSource</span></span>|<span data-ttu-id="77a6d-114">educationExternalSource</span><span class="sxs-lookup"><span data-stu-id="77a6d-114">educationExternalSource</span></span>| <span data-ttu-id="77a6d-115">创建此组织的来源。</span><span class="sxs-lookup"><span data-stu-id="77a6d-115">Source where this organization was created from.</span></span> <span data-ttu-id="77a6d-116">可取值为：`sis`、`manual`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="77a6d-116">The possible values are:</span></span>|

## <a name="relationships"></a><span data-ttu-id="77a6d-117">关系</span><span class="sxs-lookup"><span data-stu-id="77a6d-117">Relationships</span></span>
<span data-ttu-id="77a6d-118">无。</span><span class="sxs-lookup"><span data-stu-id="77a6d-118">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="77a6d-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="77a6d-119">JSON representation</span></span>

<span data-ttu-id="77a6d-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="77a6d-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "abstract": true,
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationOrganization"
}-->

```json
{
  "description": "String",
  "displayName": "String",
  "externalSource": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationOrganization resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
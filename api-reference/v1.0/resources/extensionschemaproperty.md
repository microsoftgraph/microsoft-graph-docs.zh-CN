# <a name="extensionschemaproperty-resource-type"></a><span data-ttu-id="35c2d-101">extensionSchemaProperty 资源类型</span><span class="sxs-lookup"><span data-stu-id="35c2d-101">extensionSchemaProperty resource type</span></span>

<span data-ttu-id="35c2d-102">使用 **extensionSchemaProperty** 资源将属性的名称及其类型定义为 [schemaExtension](schemaextension.md) 定义的一部分。</span><span class="sxs-lookup"><span data-stu-id="35c2d-102">Use the **extensionSchemaProperty** resource to define a property's name and its type, as part of a [schemaExtension](schemaextension.md) definition.</span></span>


## <a name="properties"></a><span data-ttu-id="35c2d-103">属性</span><span class="sxs-lookup"><span data-stu-id="35c2d-103">Properties</span></span>
| <span data-ttu-id="35c2d-104">属性</span><span class="sxs-lookup"><span data-stu-id="35c2d-104">Property</span></span>     | <span data-ttu-id="35c2d-105">类型</span><span class="sxs-lookup"><span data-stu-id="35c2d-105">Type</span></span>   |<span data-ttu-id="35c2d-106">说明</span><span class="sxs-lookup"><span data-stu-id="35c2d-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="35c2d-107">名称</span><span class="sxs-lookup"><span data-stu-id="35c2d-107">name</span></span>|<span data-ttu-id="35c2d-108">String</span><span class="sxs-lookup"><span data-stu-id="35c2d-108">String</span></span>| <span data-ttu-id="35c2d-109">被定义为架构扩展组成部分的强类型属性的名称。</span><span class="sxs-lookup"><span data-stu-id="35c2d-109">The name of the strongly-typed property defined as part of a schema extension.</span></span>|
|<span data-ttu-id="35c2d-110">type</span><span class="sxs-lookup"><span data-stu-id="35c2d-110">type</span></span>|<span data-ttu-id="35c2d-111">String</span><span class="sxs-lookup"><span data-stu-id="35c2d-111">String</span></span>| <span data-ttu-id="35c2d-p101">被定义为架构扩展组成部分的属性的类型。允许的值为 *Binary、Boolean、DateTime、Integer* 或 *String*。请参阅下表获取更多详细信息。</span><span class="sxs-lookup"><span data-stu-id="35c2d-p101">The type of the property that is defined as part of a schema extension.  Allowed values are *Binary, Boolean, DateTime, Integer* or *String*.  See the table below for more details.</span></span>|

#### <a name="supported-property-data-types"></a><span data-ttu-id="35c2d-115">受支持的属性数据类型</span><span class="sxs-lookup"><span data-stu-id="35c2d-115">Supported property data types</span></span> 
<span data-ttu-id="35c2d-116">在架构扩展中定义属性时，支持以下数据类型：</span><span class="sxs-lookup"><span data-stu-id="35c2d-116">The following data types are supported when defining a property in a schema extension:</span></span>

| <span data-ttu-id="35c2d-117">属性类型</span><span class="sxs-lookup"><span data-stu-id="35c2d-117">Property Type</span></span> | <span data-ttu-id="35c2d-118">备注</span><span class="sxs-lookup"><span data-stu-id="35c2d-118">Remarks</span></span> |
|-------------|------------|
| <span data-ttu-id="35c2d-119">Binary</span><span class="sxs-lookup"><span data-stu-id="35c2d-119">Binary</span></span> | <span data-ttu-id="35c2d-120">最多 256 字节。</span><span class="sxs-lookup"><span data-stu-id="35c2d-120">256 bytes maximum.</span></span> |
| <span data-ttu-id="35c2d-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="35c2d-121">Boolean</span></span> | <span data-ttu-id="35c2d-122">不受联系人、邮件、活动和帖子支持。</span><span class="sxs-lookup"><span data-stu-id="35c2d-122">Not supported for messages, events and posts.</span></span> |
| <span data-ttu-id="35c2d-123">DateTime</span><span class="sxs-lookup"><span data-stu-id="35c2d-123">DateTime</span></span> | <span data-ttu-id="35c2d-p102">必须以 ISO 8601 格式进行指定。存储为 UTC 格式。</span><span class="sxs-lookup"><span data-stu-id="35c2d-p102">Must be specified in ISO 8601 format. Will be stored in UTC.</span></span> |
| <span data-ttu-id="35c2d-126">Integer</span><span class="sxs-lookup"><span data-stu-id="35c2d-126">Integer</span></span> | <span data-ttu-id="35c2d-127">32 位值。</span><span class="sxs-lookup"><span data-stu-id="35c2d-127">A 32-bit integer value.</span></span> <span data-ttu-id="35c2d-128">不受联系人、邮件、活动和帖子支持。</span><span class="sxs-lookup"><span data-stu-id="35c2d-128">Not supported for messages, events and posts.</span></span> |
| <span data-ttu-id="35c2d-129">String</span><span class="sxs-lookup"><span data-stu-id="35c2d-129">String</span></span> | <span data-ttu-id="35c2d-130">最多 256 个字符。</span><span class="sxs-lookup"><span data-stu-id="35c2d-130">256 characters maximum.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="35c2d-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="35c2d-131">JSON representation</span></span>
<span data-ttu-id="35c2d-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="35c2d-132">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.extensionSchemaProperty"
}-->

```json
{
  "name": "String",
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "extensionSchemaProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

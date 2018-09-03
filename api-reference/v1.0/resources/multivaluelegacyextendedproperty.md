# <a name="multivaluelegacyextendedproperty-resource-type"></a><span data-ttu-id="89f8b-101">multiValueLegacyExtendedProperty 资源类型</span><span class="sxs-lookup"><span data-stu-id="89f8b-101">multiValueLegacyExtendedProperty resource type</span></span>

<span data-ttu-id="89f8b-102">包含值集合的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="89f8b-102">An extended property that contains a collection of values.</span></span>

<span data-ttu-id="89f8b-103">有关何时使用开放扩展或扩展属性，以及如何指定扩展属性的详细信息，请参阅[扩展属性概述](../resources/extended-properties-overview.md)。</span><span class="sxs-lookup"><span data-stu-id="89f8b-103">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="methods"></a><span data-ttu-id="89f8b-104">方法</span><span class="sxs-lookup"><span data-stu-id="89f8b-104">Methods</span></span>

| <span data-ttu-id="89f8b-105">方法</span><span class="sxs-lookup"><span data-stu-id="89f8b-105">Method</span></span>           | <span data-ttu-id="89f8b-106">返回类型</span><span class="sxs-lookup"><span data-stu-id="89f8b-106">Return Type</span></span>    |<span data-ttu-id="89f8b-107">说明</span><span class="sxs-lookup"><span data-stu-id="89f8b-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="89f8b-108">发布</span><span class="sxs-lookup"><span data-stu-id="89f8b-108">Post</span></span>](../api/multivaluelegacyextendedproperty_post_multivalueextendedproperties.md) | <span data-ttu-id="89f8b-p101">支持的资源实例有：[message](../resources/message.md)、[mailFolder](../resources/mailfolder.md)、[event](../resources/event.md)、[calendar](../resources/calendar.md)、[contact](../resources/contact.md) 或 [contactFolder](../resources/contactfolder.md)。请注意，不支持 [post](../resources/post.md) 组。</span><span class="sxs-lookup"><span data-stu-id="89f8b-p101">A supported resource instance: [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), or [contactFolder](../resources/contactfolder.md). Note that group [post](../resources/post.md) is not supported.</span></span> | <span data-ttu-id="89f8b-111">在新建或现有的支持资源实例中创建 **multiValueLegacyExtendedProperty**。</span><span class="sxs-lookup"><span data-stu-id="89f8b-111">Create a **multiValueLegacyExtendedProperty** in a new or existing instance of a supported resource.</span></span> |
|[<span data-ttu-id="89f8b-112">获取</span><span class="sxs-lookup"><span data-stu-id="89f8b-112">Get</span></span>](../api/multivaluelegacyextendedproperty_get.md) |<span data-ttu-id="89f8b-113">通过 [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) 对象扩展的受支持的资源实例（[message](../resources/message.md)、[mailFolder](../resources/mailfolder.md)、[event](../resources/event.md)、[calendar](../resources/calendar.md)、[contact](../resources/contact.md)、[contactFolder](../resources/contactfolder.md) 或 [post](../resources/post.md) 组）。</span><span class="sxs-lookup"><span data-stu-id="89f8b-113">A supported resource instance ([message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), or group [post](../resources/post.md)) expanded with a [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) object.</span></span> |<span data-ttu-id="89f8b-114">使用 `$expand` 获取具有扩展属性的资源实例。</span><span class="sxs-lookup"><span data-stu-id="89f8b-114">Get a resource instance with an extended property using `$expand`.</span></span>|

## <a name="properties"></a><span data-ttu-id="89f8b-115">属性</span><span class="sxs-lookup"><span data-stu-id="89f8b-115">Properties</span></span>
| <span data-ttu-id="89f8b-116">属性</span><span class="sxs-lookup"><span data-stu-id="89f8b-116">Property</span></span>     | <span data-ttu-id="89f8b-117">类型</span><span class="sxs-lookup"><span data-stu-id="89f8b-117">Type</span></span>   |<span data-ttu-id="89f8b-118">说明</span><span class="sxs-lookup"><span data-stu-id="89f8b-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="89f8b-119">ID</span><span class="sxs-lookup"><span data-stu-id="89f8b-119">id</span></span>|<span data-ttu-id="89f8b-120">字符串</span><span class="sxs-lookup"><span data-stu-id="89f8b-120">string</span></span>|<span data-ttu-id="89f8b-p102">属性标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="89f8b-p102">The property identifier. Read-only.</span></span>|
|<span data-ttu-id="89f8b-123">值</span><span class="sxs-lookup"><span data-stu-id="89f8b-123">value</span></span>|<span data-ttu-id="89f8b-124">字符串集合</span><span class="sxs-lookup"><span data-stu-id="89f8b-124">string collection</span></span>|<span data-ttu-id="89f8b-125">属性值的集合。</span><span class="sxs-lookup"><span data-stu-id="89f8b-125">A collection of property values.</span></span>|

## <a name="relationships"></a><span data-ttu-id="89f8b-126">关系</span><span class="sxs-lookup"><span data-stu-id="89f8b-126">Relationships</span></span>
<span data-ttu-id="89f8b-127">无</span><span class="sxs-lookup"><span data-stu-id="89f8b-127">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="89f8b-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="89f8b-128">JSON representation</span></span>

<span data-ttu-id="89f8b-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="89f8b-129">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.multiValueLegacyExtendedProperty"
}-->

```json
{
  "id": "string (identifier)",
  "value": ["string"]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "multiValueLegacyExtendedProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
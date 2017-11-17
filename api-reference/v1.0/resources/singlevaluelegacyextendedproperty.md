# <a name="singlevaluelegacyextendedproperty-resource-type"></a><span data-ttu-id="66f7d-101">singleValueLegacyExtendedProperty 资源类型</span><span class="sxs-lookup"><span data-stu-id="66f7d-101">singleValueLegacyExtendedProperty resource type</span></span>

<span data-ttu-id="66f7d-102">包含单个值的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="66f7d-102">An extended property that contains a single value.</span></span> 

<span data-ttu-id="66f7d-103">有关何时使用开放扩展或扩展属性，以及如何指定扩展属性的详细信息，请参阅[扩展属性概述](../resources/extended-properties-overview.md)。</span><span class="sxs-lookup"><span data-stu-id="66f7d-103">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span> 


## <a name="methods"></a><span data-ttu-id="66f7d-104">方法</span><span class="sxs-lookup"><span data-stu-id="66f7d-104">Methods</span></span>

| <span data-ttu-id="66f7d-105">方法</span><span class="sxs-lookup"><span data-stu-id="66f7d-105">Method</span></span>           | <span data-ttu-id="66f7d-106">返回类型</span><span class="sxs-lookup"><span data-stu-id="66f7d-106">Return Type</span></span>    |<span data-ttu-id="66f7d-107">说明</span><span class="sxs-lookup"><span data-stu-id="66f7d-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="66f7d-108">帖子</span><span class="sxs-lookup"><span data-stu-id="66f7d-108">Post</span></span>](../api/singlevaluelegacyextendedproperty_post_singlevalueextendedproperties.md) | <span data-ttu-id="66f7d-109">受支持的资源实例有：[message](../resources/message.md)、[mailFolder](../resources/mailfolder.md)、[event](../resources/event.md)、[calendar](../resources/calendar.md)、[contact](../resources/contact.md) 或 [contactFolder](../resources/contactfolder.md)，但没有 [post](../resources/post.md) 组。</span><span class="sxs-lookup"><span data-stu-id="66f7d-109">A supported resource instance: [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), or [contactFolder](../resources/contactfolder.md), but not group [post](../resources/post.md).</span></span> | <span data-ttu-id="66f7d-110">在新建或现有的支持资源实例中创建 **singleValueLegacyExtendedProperty**。</span><span class="sxs-lookup"><span data-stu-id="66f7d-110">Create a **singleValueLegacyExtendedProperty** in a new or existing instance of a supported resource.</span></span> |
|[<span data-ttu-id="66f7d-111">获取</span><span class="sxs-lookup"><span data-stu-id="66f7d-111">Get</span></span>](../api/singlevaluelegacyextendedproperty_get.md) |<span data-ttu-id="66f7d-112">一个或多个受支持的资源实例（[message](../resources/message.md)、[mailFolder](../resources/mailfolder.md)、[event](../resources/event.md)、[calendar](../resources/calendar.md)、[contact](../resources/contact.md)、[contactFolder](../resources/contactfolder.md) 或[post](../resources/post.md) 组），或通过 [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) 对象扩展的一个此类的实例。</span><span class="sxs-lookup"><span data-stu-id="66f7d-112">One or a collection of supported resource instance ([message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), or group [post](../resources/post.md)), or one such instance expanded with a [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) object.</span></span> |<span data-ttu-id="66f7d-113">使用 `$expand` 或 `$filter` 获取具有扩展属性的资源实例。</span><span class="sxs-lookup"><span data-stu-id="66f7d-113">Get a resource instance with an extended property using `$expand` or `$filter`.</span></span>|

## <a name="properties"></a><span data-ttu-id="66f7d-114">属性</span><span class="sxs-lookup"><span data-stu-id="66f7d-114">Properties</span></span>
| <span data-ttu-id="66f7d-115">属性</span><span class="sxs-lookup"><span data-stu-id="66f7d-115">Property</span></span>     | <span data-ttu-id="66f7d-116">类型</span><span class="sxs-lookup"><span data-stu-id="66f7d-116">Type</span></span>   |<span data-ttu-id="66f7d-117">说明</span><span class="sxs-lookup"><span data-stu-id="66f7d-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="66f7d-118">id</span><span class="sxs-lookup"><span data-stu-id="66f7d-118">id</span></span>|<span data-ttu-id="66f7d-119">string</span><span class="sxs-lookup"><span data-stu-id="66f7d-119">string</span></span>|<span data-ttu-id="66f7d-p101">用于标识属性的属性 ID。只读。</span><span class="sxs-lookup"><span data-stu-id="66f7d-p101">The property ID used to identify the property. Read-only.</span></span>|
|<span data-ttu-id="66f7d-122">value</span><span class="sxs-lookup"><span data-stu-id="66f7d-122">value</span></span>|<span data-ttu-id="66f7d-123">string</span><span class="sxs-lookup"><span data-stu-id="66f7d-123">string</span></span>|<span data-ttu-id="66f7d-124">属性值。</span><span class="sxs-lookup"><span data-stu-id="66f7d-124">A property value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="66f7d-125">关系</span><span class="sxs-lookup"><span data-stu-id="66f7d-125">Relationships</span></span>
<span data-ttu-id="66f7d-126">无</span><span class="sxs-lookup"><span data-stu-id="66f7d-126">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="66f7d-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="66f7d-127">JSON representation</span></span>

<span data-ttu-id="66f7d-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="66f7d-128">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.singleValueLegacyExtendedProperty"
}-->

```json
{
  "id": "string (identifier)",
  "value": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "singleValueLegacyExtendedProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
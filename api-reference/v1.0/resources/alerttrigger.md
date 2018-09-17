# <a name="alerttrigger-resource-type"></a><span data-ttu-id="00fbb-101">alertTrigger 资源类型</span><span class="sxs-lookup"><span data-stu-id="00fbb-101">alertTrigger resource type</span></span>

<span data-ttu-id="00fbb-102">包含有关触发检测属性的信息 （警报实体中存在属性）。</span><span class="sxs-lookup"><span data-stu-id="00fbb-102">Contains information about the properties that triggered a detection (properties exist in the alert entity).</span></span>

## <a name="properties"></a><span data-ttu-id="00fbb-103">属性</span><span class="sxs-lookup"><span data-stu-id="00fbb-103">Properties</span></span>

| <span data-ttu-id="00fbb-104">属性</span><span class="sxs-lookup"><span data-stu-id="00fbb-104">Property</span></span>   | <span data-ttu-id="00fbb-105">类型</span><span class="sxs-lookup"><span data-stu-id="00fbb-105">Type</span></span>|<span data-ttu-id="00fbb-106">说明</span><span class="sxs-lookup"><span data-stu-id="00fbb-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="00fbb-107">name</span><span class="sxs-lookup"><span data-stu-id="00fbb-107">name</span></span>|<span data-ttu-id="00fbb-108">字符串</span><span class="sxs-lookup"><span data-stu-id="00fbb-108">String</span></span>|<span data-ttu-id="00fbb-109">充当检测触发器属性的名称。</span><span class="sxs-lookup"><span data-stu-id="00fbb-109">Name of the property serving as a detection trigger.</span></span>|
|<span data-ttu-id="00fbb-110">类型</span><span class="sxs-lookup"><span data-stu-id="00fbb-110">type</span></span>|<span data-ttu-id="00fbb-111">字符串</span><span class="sxs-lookup"><span data-stu-id="00fbb-111">String</span></span>|<span data-ttu-id="00fbb-112">用于解释：键值对中属性的类型。</span><span class="sxs-lookup"><span data-stu-id="00fbb-112">Type of the property in the key:value pair for interpretation.</span></span> <span data-ttu-id="00fbb-113">例如，字符串、布尔值、等。</span><span class="sxs-lookup"><span data-stu-id="00fbb-113">For example, String, Boolean, etc.</span></span>|
|<span data-ttu-id="00fbb-114">value</span><span class="sxs-lookup"><span data-stu-id="00fbb-114">value</span></span>|<span data-ttu-id="00fbb-115">字符串</span><span class="sxs-lookup"><span data-stu-id="00fbb-115">String</span></span>|<span data-ttu-id="00fbb-116">充当检测触发器属性的名称。</span><span class="sxs-lookup"><span data-stu-id="00fbb-116">Value of the property serving as a detection trigger.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="00fbb-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="00fbb-117">JSON representation</span></span>

<span data-ttu-id="00fbb-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="00fbb-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.alertTrigger"
}-->

```json
{
  "name": "String",
  "type": "String",
  "value": "String"
}

```

## <a name="example"></a><span data-ttu-id="00fbb-119">示例</span><span class="sxs-lookup"><span data-stu-id="00fbb-119">Example</span></span>

```json
{
  "name": "endpointAddress",
  "type": "networkConnection.sourceAddress",
  "value": "10.154.9.40"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "alertTrigger resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
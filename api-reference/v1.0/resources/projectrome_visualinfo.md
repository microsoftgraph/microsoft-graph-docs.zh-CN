# <a name="visualinfo-resource-type"></a><span data-ttu-id="5442c-101">visualInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="5442c-101">visualInfo resource type</span></span>

<span data-ttu-id="5442c-102">代表 activity 对象中 \*\*visual \*\* Elements[ visualElements](../resources/projectrome_activity.md) 属性的复杂类型。</span><span class="sxs-lookup"><span data-stu-id="5442c-102">A complex type for representing the **attribution** property in the [visualInfo part of the activity](../resources/projectrome_activity.md) object.</span></span>

<span data-ttu-id="5442c-103">每个用户活动都将作为自适应卡片在日程表中显示。</span><span class="sxs-lookup"><span data-stu-id="5442c-103">Each user activity will be shown in Timeline as an Adaptive Card.</span></span> <span data-ttu-id="5442c-104">鼓励应用程序开发人员提供自定义卡片，用于捕获应用程序中发生的活动的本质。</span><span class="sxs-lookup"><span data-stu-id="5442c-104">App developers are encouraged to provide a custom Card which captures the essence of the activity which took place in your app.</span></span> <span data-ttu-id="5442c-105">这可以通过在内容属性中提供自定义 JSON 卡来实现。</span><span class="sxs-lookup"><span data-stu-id="5442c-105">This is possible by providing a custom JSON card in the content property.</span></span>

<span data-ttu-id="5442c-106">除了具有自适应卡的可视元数据，应用还可以指定内容元数据，该数据可用于根据用户活动生成推断，以此提供可用于未来重新使用的新活动。</span><span class="sxs-lookup"><span data-stu-id="5442c-106">In addition to visual metadata with an Adaptive Card, app can specify content metadata – data that be used to build inferences on the user’s activity in order to offer new activities for future re-engagement.</span></span> <span data-ttu-id="5442c-107">可通过使用活动的 contentInfo 属性提供一个 JSON 对象来实现，该 JSON 对象利用 schema.org 属性描述内容。</span><span class="sxs-lookup"><span data-stu-id="5442c-107">This is possible by using the activity's contentInfo property to provide a JSON object which leverages schema.org properties to describe the content.</span></span>

<span data-ttu-id="5442c-108">如果未提供自定义卡片，则使用 displayText 和说明属性生成简单卡片。</span><span class="sxs-lookup"><span data-stu-id="5442c-108">If a custom card is not provided, a simple card will be generated using displayText and description properties.</span></span> <span data-ttu-id="5442c-109">建议使用自定义卡片展示应用程序中的最佳内容。</span><span class="sxs-lookup"><span data-stu-id="5442c-109">Custom cards are recommended to showcase the best content from within your app.</span></span>

## <a name="properties"></a><span data-ttu-id="5442c-110">属性</span><span class="sxs-lookup"><span data-stu-id="5442c-110">Properties</span></span>

|<span data-ttu-id="5442c-111">名称</span><span class="sxs-lookup"><span data-stu-id="5442c-111">Name</span></span> | <span data-ttu-id="5442c-112">类型</span><span class="sxs-lookup"><span data-stu-id="5442c-112">Type</span></span> | <span data-ttu-id="5442c-113">说明</span><span class="sxs-lookup"><span data-stu-id="5442c-113">Description</span></span>|
|:----|:------|:-----------|
|<span data-ttu-id="5442c-114">displayText</span><span class="sxs-lookup"><span data-stu-id="5442c-114">displayText</span></span> | <span data-ttu-id="5442c-115">String</span><span class="sxs-lookup"><span data-stu-id="5442c-115">String</span></span> | <span data-ttu-id="5442c-116">必需。</span><span class="sxs-lookup"><span data-stu-id="5442c-116">Required.</span></span> <span data-ttu-id="5442c-117">用户唯一活动的简短文本说明（例如，在活动引用文档创建的情况下的文档名称）</span><span class="sxs-lookup"><span data-stu-id="5442c-117">Short text description of the user's unique activity (for example, document name in cases where an activity refers to document creation)</span></span>|
|<span data-ttu-id="5442c-118">description</span><span class="sxs-lookup"><span data-stu-id="5442c-118">description</span></span> | <span data-ttu-id="5442c-119">字符串</span><span class="sxs-lookup"><span data-stu-id="5442c-119">String</span></span> | <span data-ttu-id="5442c-120">可选。</span><span class="sxs-lookup"><span data-stu-id="5442c-120">Optional.</span></span> <span data-ttu-id="5442c-121">用户唯一活动的详细文本说明（例如，文档名称、第一句和/或元数据）</span><span class="sxs-lookup"><span data-stu-id="5442c-121">Longer text description of the user's unique activity (example: document name, first sentence, and/or metadata)</span></span>|
|<span data-ttu-id="5442c-122">backgroundColor</span><span class="sxs-lookup"><span data-stu-id="5442c-122">background-color</span></span> | <span data-ttu-id="5442c-123">String</span><span class="sxs-lookup"><span data-stu-id="5442c-123">String</span></span> | <span data-ttu-id="5442c-124">可选。</span><span class="sxs-lookup"><span data-stu-id="5442c-124">Optional.</span></span> <span data-ttu-id="5442c-125">用于在 UI 中呈现活动的背景颜色 - 活动的应用程序源中的品牌颜色。</span><span class="sxs-lookup"><span data-stu-id="5442c-125">Background color used to render the activity in the UI - brand color for the application source of the activity.</span></span> <span data-ttu-id="5442c-126">必须是有效的十六进制颜色</span><span class="sxs-lookup"><span data-stu-id="5442c-126">Must be a valid hex color</span></span>|
|<span data-ttu-id="5442c-127">content</span><span class="sxs-lookup"><span data-stu-id="5442c-127">content</span></span> | <span data-ttu-id="5442c-128">无类型的 JSON 对象</span><span class="sxs-lookup"><span data-stu-id="5442c-128">Untyped JSON object</span></span> | <span data-ttu-id="5442c-129">可选。</span><span class="sxs-lookup"><span data-stu-id="5442c-129">Optional.</span></span> <span data-ttu-id="5442c-130">自定义的数据 - 用于提供自定义内容，以在 Windows  Shell UI 中呈现活动的 JSON 对象</span><span class="sxs-lookup"><span data-stu-id="5442c-130">Custom piece of data - JSON object used to provide custom content to render the activity in the Windows Shell UI</span></span>|
|<span data-ttu-id="5442c-131">attribution</span><span class="sxs-lookup"><span data-stu-id="5442c-131">attribution</span></span> | <span data-ttu-id="5442c-132">[imageInfo](../resources/projectrome_imageinfo.md)</span><span class="sxs-lookup"><span data-stu-id="5442c-132">Added [imageInfo](../resources/projectrome_imageinfo.md)</span></span> | <span data-ttu-id="5442c-133">可选。</span><span class="sxs-lookup"><span data-stu-id="5442c-133">Optional.</span></span> <span data-ttu-id="5442c-134">JSON 对象，用于表示一个图标，代表用于生成活动的应用程序</span><span class="sxs-lookup"><span data-stu-id="5442c-134">Optional; URI that points to an icon which represents the application used to generate the activity</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5442c-135">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5442c-135">JSON Representation</span></span>

<span data-ttu-id="5442c-136">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5442c-136">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "attribution",
    "description",
    "backgroundColor",
    "content"
  ],
  "@odata.type": "microsoft.graph.visualInfo"
}-->

```json
{
    "@odata.type": "microsoft.graph.visualInfo",
    "attribution": {
        "@odata.type": "microsoft.graph.imageInfo",
        "iconUrl": "String (URL)",
        "alternateText": "String",
        "addImageQuery": "boolean"
    },
    "description": "String",
    "backgroundColor": "String",
    "displayText": "String",
    "content": {
        "@odata.type": "microsoft.graph.Json"
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "visualinfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

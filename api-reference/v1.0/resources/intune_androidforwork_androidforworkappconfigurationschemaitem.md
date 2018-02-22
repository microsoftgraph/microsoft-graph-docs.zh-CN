# <a name="androidforworkappconfigurationschemaitem-resource-type"></a><span data-ttu-id="5aa59-101">androidForWorkAppConfigurationSchemaItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="5aa59-101">androidForWorkAppConfigurationSchemaItem resource type</span></span>

> <span data-ttu-id="5aa59-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="5aa59-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5aa59-103">Android for Work 应用程序的自定义配置架构内的单个配置项。</span><span class="sxs-lookup"><span data-stu-id="5aa59-103">Single configuration item inside an Android for Work application's custom configuration schema.</span></span>
## <a name="properties"></a><span data-ttu-id="5aa59-104">属性</span><span class="sxs-lookup"><span data-stu-id="5aa59-104">Properties</span></span>
|<span data-ttu-id="5aa59-105">属性</span><span class="sxs-lookup"><span data-stu-id="5aa59-105">Property</span></span>|<span data-ttu-id="5aa59-106">类型</span><span class="sxs-lookup"><span data-stu-id="5aa59-106">Type</span></span>|<span data-ttu-id="5aa59-107">说明</span><span class="sxs-lookup"><span data-stu-id="5aa59-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5aa59-108">schemaItemKey</span><span class="sxs-lookup"><span data-stu-id="5aa59-108">schemaItemKey</span></span>|<span data-ttu-id="5aa59-109">String</span><span class="sxs-lookup"><span data-stu-id="5aa59-109">String</span></span>|<span data-ttu-id="5aa59-110">应用程序用于标识项的唯一键</span><span class="sxs-lookup"><span data-stu-id="5aa59-110">Unique key the application uses to identify the item</span></span>|
|<span data-ttu-id="5aa59-111">displayName</span><span class="sxs-lookup"><span data-stu-id="5aa59-111">displayName</span></span>|<span data-ttu-id="5aa59-112">String</span><span class="sxs-lookup"><span data-stu-id="5aa59-112">String</span></span>|<span data-ttu-id="5aa59-113">用户可读的名称</span><span class="sxs-lookup"><span data-stu-id="5aa59-113">Human readable name</span></span>|
|<span data-ttu-id="5aa59-114">说明</span><span class="sxs-lookup"><span data-stu-id="5aa59-114">description</span></span>|<span data-ttu-id="5aa59-115">String</span><span class="sxs-lookup"><span data-stu-id="5aa59-115">String</span></span>|<span data-ttu-id="5aa59-116">项在应用程序内所控制内容的说明</span><span class="sxs-lookup"><span data-stu-id="5aa59-116">Description of what the item controls within the application</span></span>|
|<span data-ttu-id="5aa59-117">defaultBoolValue</span><span class="sxs-lookup"><span data-stu-id="5aa59-117">defaultBoolValue</span></span>|<span data-ttu-id="5aa59-118">布尔值</span><span class="sxs-lookup"><span data-stu-id="5aa59-118">Boolean</span></span>|<span data-ttu-id="5aa59-119">如果由应用开发人员指定，则为布尔类型项的默认值</span><span class="sxs-lookup"><span data-stu-id="5aa59-119">Default value for boolean type items, if specified by the app developer</span></span>|
|<span data-ttu-id="5aa59-120">defaultIntValue</span><span class="sxs-lookup"><span data-stu-id="5aa59-120">defaultIntValue</span></span>|<span data-ttu-id="5aa59-121">Int32</span><span class="sxs-lookup"><span data-stu-id="5aa59-121">Int32</span></span>|<span data-ttu-id="5aa59-122">如果由应用开发人员指定，则为整数类型项的默认值</span><span class="sxs-lookup"><span data-stu-id="5aa59-122">Default value for integer type items, if specified by the app developer</span></span>|
|<span data-ttu-id="5aa59-123">defaultStringValue</span><span class="sxs-lookup"><span data-stu-id="5aa59-123">defaultStringValue</span></span>|<span data-ttu-id="5aa59-124">String</span><span class="sxs-lookup"><span data-stu-id="5aa59-124">String</span></span>|<span data-ttu-id="5aa59-125">如果由应用开发人员指定，则为字符串类型项的默认值</span><span class="sxs-lookup"><span data-stu-id="5aa59-125">Default value for string type items, if specified by the app developer</span></span>|
|<span data-ttu-id="5aa59-126">defaultStringArrayValue</span><span class="sxs-lookup"><span data-stu-id="5aa59-126">defaultStringArrayValue</span></span>|<span data-ttu-id="5aa59-127">String collection</span><span class="sxs-lookup"><span data-stu-id="5aa59-127">String collection</span></span>|<span data-ttu-id="5aa59-128">如果由应用开发人员指定，则为字符串数组类型项的默认值</span><span class="sxs-lookup"><span data-stu-id="5aa59-128">Default value for string array type items, if specified by the app developer</span></span>|
|<span data-ttu-id="5aa59-129">DataType</span><span class="sxs-lookup"><span data-stu-id="5aa59-129">DataType</span></span>|<span data-ttu-id="5aa59-130">String</span><span class="sxs-lookup"><span data-stu-id="5aa59-130">String</span></span>|<span data-ttu-id="5aa59-131">此项介绍的值类型 可取值为：`bool`、`integer`、`string`、`choice`、`multiselect`、`bundle`、`bundleArray`、`hidden`。</span><span class="sxs-lookup"><span data-stu-id="5aa59-131">The type of value this item describes Possible values are: `bool`, `integer`, `string`, `choice`, `multiselect`, `bundle`, `bundleArray`, `hidden`.</span></span>|
|<span data-ttu-id="5aa59-132">选择</span><span class="sxs-lookup"><span data-stu-id="5aa59-132">selections</span></span>|<span data-ttu-id="5aa59-133">[keyValuePair](../resources/intune_androidforwork_keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5aa59-133">[keyValuePair](../resources/intune_androidforwork_keyvaluepair.md) collection</span></span>|<span data-ttu-id="5aa59-134">可为此项（仅 Choice 和 Multiselect 项）设置的有效值的用于可读名称/值对列表</span><span class="sxs-lookup"><span data-stu-id="5aa59-134">List of human readable name/value pairs for the valid values that can be set for this item (Choice and Multiselect items only)</span></span>|

## <a name="relationships"></a><span data-ttu-id="5aa59-135">关系</span><span class="sxs-lookup"><span data-stu-id="5aa59-135">Relationships</span></span>
<span data-ttu-id="5aa59-136">无</span><span class="sxs-lookup"><span data-stu-id="5aa59-136">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="5aa59-137">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5aa59-137">JSON Representation</span></span>
<span data-ttu-id="5aa59-138">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5aa59-138">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidForWorkAppConfigurationSchemaItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidForWorkAppConfigurationSchemaItem",
  "schemaItemKey": "String",
  "displayName": "String",
  "description": "String",
  "defaultBoolValue": true,
  "defaultIntValue": 1024,
  "defaultStringValue": "String",
  "defaultStringArrayValue": [
    "String"
  ],
  "dataType": "String",
  "selections": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "String",
      "value": "String"
    }
  ]
}
```




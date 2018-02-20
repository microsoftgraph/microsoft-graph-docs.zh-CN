# <a name="managedappconfiguration-resource-type"></a><span data-ttu-id="bdadb-101">managedAppConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="bdadb-101">managedAppConfiguration resource type</span></span>

> <span data-ttu-id="bdadb-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="bdadb-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bdadb-103">用于将一组自定义设置按原样提供给配置范围确定的用户应用的配置。</span><span class="sxs-lookup"><span data-stu-id="bdadb-103">Configuration used to deliver a set of custom settings as-is to apps for users to whom the configuration is scoped</span></span>

<span data-ttu-id="bdadb-104">继承自 [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="bdadb-104">Inherits from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>

## <a name="methods"></a><span data-ttu-id="bdadb-105">方法</span><span class="sxs-lookup"><span data-stu-id="bdadb-105">Methods</span></span>
|<span data-ttu-id="bdadb-106">方法</span><span class="sxs-lookup"><span data-stu-id="bdadb-106">Method</span></span>|<span data-ttu-id="bdadb-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="bdadb-107">Return Type</span></span>|<span data-ttu-id="bdadb-108">说明</span><span class="sxs-lookup"><span data-stu-id="bdadb-108">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="bdadb-109">List managedAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="bdadb-109">List managedAppConfigurations</span></span>](../api/intune_mam_managedappconfiguration_list.md)|<span data-ttu-id="bdadb-110">[managedAppConfiguration](../resources/intune_mam_managedappconfiguration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="bdadb-110">[managedAppConfiguration](../resources/intune_mam_managedappconfiguration.md) collection</span></span>|<span data-ttu-id="bdadb-111">列出 [managedAppConfiguration](../resources/intune_mam_managedappconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="bdadb-111">List properties and relationships of the [managedAppConfiguration](../resources/intune_mam_managedappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="bdadb-112">Get managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="bdadb-112">Get managedAppConfiguration</span></span>](../api/intune_mam_managedappconfiguration_get.md)|[<span data-ttu-id="bdadb-113">managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="bdadb-113">managedAppConfiguration</span></span>](../resources/intune_mam_managedappconfiguration.md)|<span data-ttu-id="bdadb-114">读取 [managedAppConfiguration](../resources/intune_mam_managedappconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="bdadb-114">Read properties and relationships of [plannerTaskDetails](../resources/intune_mam_managedappconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="bdadb-115">属性</span><span class="sxs-lookup"><span data-stu-id="bdadb-115">Properties</span></span>
|<span data-ttu-id="bdadb-116">属性</span><span class="sxs-lookup"><span data-stu-id="bdadb-116">Property</span></span>|<span data-ttu-id="bdadb-117">类型</span><span class="sxs-lookup"><span data-stu-id="bdadb-117">Type</span></span>|<span data-ttu-id="bdadb-118">说明</span><span class="sxs-lookup"><span data-stu-id="bdadb-118">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bdadb-119">displayName</span><span class="sxs-lookup"><span data-stu-id="bdadb-119">displayName</span></span>|<span data-ttu-id="bdadb-120">String</span><span class="sxs-lookup"><span data-stu-id="bdadb-120">String</span></span>|<span data-ttu-id="bdadb-121">策略显示名称。</span><span class="sxs-lookup"><span data-stu-id="bdadb-121">Policy display name.</span></span> <span data-ttu-id="bdadb-122">继承自 [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="bdadb-122">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="bdadb-123">description</span><span class="sxs-lookup"><span data-stu-id="bdadb-123">description</span></span>|<span data-ttu-id="bdadb-124">String</span><span class="sxs-lookup"><span data-stu-id="bdadb-124">String</span></span>|<span data-ttu-id="bdadb-125">策略的说明。</span><span class="sxs-lookup"><span data-stu-id="bdadb-125">The policy's description.</span></span> <span data-ttu-id="bdadb-126">继承自 [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="bdadb-126">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="bdadb-127">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bdadb-127">createdDateTime</span></span>|<span data-ttu-id="bdadb-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bdadb-128">DateTimeOffset</span></span>|<span data-ttu-id="bdadb-129">创建策略的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="bdadb-129">The date and time when the page was created.</span></span> <span data-ttu-id="bdadb-130">继承自 [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="bdadb-130">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="bdadb-131">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bdadb-131">lastModifiedDateTime</span></span>|<span data-ttu-id="bdadb-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bdadb-132">DateTimeOffset</span></span>|<span data-ttu-id="bdadb-133">上次修改策略的时间。</span><span class="sxs-lookup"><span data-stu-id="bdadb-133">Last time the policy was modified.</span></span> <span data-ttu-id="bdadb-134">继承自 [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="bdadb-134">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="bdadb-135">id</span><span class="sxs-lookup"><span data-stu-id="bdadb-135">id</span></span>|<span data-ttu-id="bdadb-136">String</span><span class="sxs-lookup"><span data-stu-id="bdadb-136">String</span></span>|<span data-ttu-id="bdadb-137">实体的键。</span><span class="sxs-lookup"><span data-stu-id="bdadb-137">Key of the setting.</span></span> <span data-ttu-id="bdadb-138">继承自 [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="bdadb-138">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="bdadb-139">version</span><span class="sxs-lookup"><span data-stu-id="bdadb-139">version</span></span>|<span data-ttu-id="bdadb-140">String</span><span class="sxs-lookup"><span data-stu-id="bdadb-140">String</span></span>|<span data-ttu-id="bdadb-141">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="bdadb-141">Version of the entity.</span></span> <span data-ttu-id="bdadb-142">继承自 [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="bdadb-142">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="bdadb-143">customSettings</span><span class="sxs-lookup"><span data-stu-id="bdadb-143">customSettings</span></span>|<span data-ttu-id="bdadb-144">[keyValuePair](../resources/intune_mam_keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="bdadb-144">[keyValuePair](../resources/intune_mam_keyvaluepair.md) collection</span></span>|<span data-ttu-id="bdadb-145">一组字符串键和字符串值对，要发送到配置范围确定的用户应用，且不被此服务改变</span><span class="sxs-lookup"><span data-stu-id="bdadb-145">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service</span></span>|

## <a name="relationships"></a><span data-ttu-id="bdadb-146">关系</span><span class="sxs-lookup"><span data-stu-id="bdadb-146">Relationships</span></span>
<span data-ttu-id="bdadb-147">无</span><span class="sxs-lookup"><span data-stu-id="bdadb-147">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="bdadb-148">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bdadb-148">JSON Representation</span></span>
<span data-ttu-id="bdadb-149">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bdadb-149">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppConfiguration",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "version": "String",
  "customSettings": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "String",
      "value": "String"
    }
  ]
}
```




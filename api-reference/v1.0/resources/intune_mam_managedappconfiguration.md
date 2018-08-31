# <a name="managedappconfiguration-resource-type"></a><span data-ttu-id="83838-101">managedAppConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="83838-101">managedAppConfiguration resource type</span></span>

> <span data-ttu-id="83838-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="83838-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="83838-103">用于将一组自定义设置按原样提供给配置范围确定的用户应用的配置。</span><span class="sxs-lookup"><span data-stu-id="83838-103">Configuration used to deliver a set of custom settings as-is to apps for users to whom the configuration is scoped</span></span>

<span data-ttu-id="83838-104">继承自 [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="83838-104">Inherits from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>

## <a name="methods"></a><span data-ttu-id="83838-105">方法</span><span class="sxs-lookup"><span data-stu-id="83838-105">Methods</span></span>
|<span data-ttu-id="83838-106">方法</span><span class="sxs-lookup"><span data-stu-id="83838-106">Method</span></span>|<span data-ttu-id="83838-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="83838-107">Return Type</span></span>|<span data-ttu-id="83838-108">说明</span><span class="sxs-lookup"><span data-stu-id="83838-108">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="83838-109">List managedAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="83838-109">List managedAppConfigurations</span></span>](../api/intune_mam_managedappconfiguration_list.md)|<span data-ttu-id="83838-110">[managedAppConfiguration](../resources/intune_mam_managedappconfiguration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="83838-110">[managedAppConfiguration](../resources/intune_mam_managedappconfiguration.md) collection</span></span>|<span data-ttu-id="83838-111">列出 [managedAppConfiguration](../resources/intune_mam_managedappconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="83838-111">List properties and relationships of the [managedAppConfiguration](../resources/intune_mam_managedappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="83838-112">Get managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="83838-112">Get managedAppConfiguration</span></span>](../api/intune_mam_managedappconfiguration_get.md)|[<span data-ttu-id="83838-113">managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="83838-113">managedAppConfiguration</span></span>](../resources/intune_mam_managedappconfiguration.md)|<span data-ttu-id="83838-114">读取 [managedAppConfiguration](../resources/intune_mam_managedappconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="83838-114">Read properties and relationships of the [managedAppConfiguration](../resources/intune_mam_managedappconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="83838-115">属性</span><span class="sxs-lookup"><span data-stu-id="83838-115">Properties</span></span>
|<span data-ttu-id="83838-116">属性</span><span class="sxs-lookup"><span data-stu-id="83838-116">Property</span></span>|<span data-ttu-id="83838-117">类型</span><span class="sxs-lookup"><span data-stu-id="83838-117">Type</span></span>|<span data-ttu-id="83838-118">说明</span><span class="sxs-lookup"><span data-stu-id="83838-118">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="83838-119">displayName</span><span class="sxs-lookup"><span data-stu-id="83838-119">displayName</span></span>|<span data-ttu-id="83838-120">String</span><span class="sxs-lookup"><span data-stu-id="83838-120">String</span></span>|<span data-ttu-id="83838-121">策略显示名称。</span><span class="sxs-lookup"><span data-stu-id="83838-121">Policy display name.</span></span> <span data-ttu-id="83838-122">继承自 [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="83838-122">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="83838-123">description</span><span class="sxs-lookup"><span data-stu-id="83838-123">description</span></span>|<span data-ttu-id="83838-124">String</span><span class="sxs-lookup"><span data-stu-id="83838-124">String</span></span>|<span data-ttu-id="83838-125">策略的说明。</span><span class="sxs-lookup"><span data-stu-id="83838-125">The policy's description.</span></span> <span data-ttu-id="83838-126">继承自 [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="83838-126">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="83838-127">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="83838-127">createdDateTime</span></span>|<span data-ttu-id="83838-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="83838-128">DateTimeOffset</span></span>|<span data-ttu-id="83838-129">创建策略的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="83838-129">The date and time the policy was created.</span></span> <span data-ttu-id="83838-130">继承自 [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="83838-130">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="83838-131">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="83838-131">lastModifiedDateTime</span></span>|<span data-ttu-id="83838-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="83838-132">DateTimeOffset</span></span>|<span data-ttu-id="83838-133">上次修改策略的时间。</span><span class="sxs-lookup"><span data-stu-id="83838-133">Last time the policy was modified.</span></span> <span data-ttu-id="83838-134">继承自 [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="83838-134">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="83838-135">id</span><span class="sxs-lookup"><span data-stu-id="83838-135">id</span></span>|<span data-ttu-id="83838-136">字符串</span><span class="sxs-lookup"><span data-stu-id="83838-136">String</span></span>|<span data-ttu-id="83838-137">实体的键。</span><span class="sxs-lookup"><span data-stu-id="83838-137">Key of the entity.</span></span> <span data-ttu-id="83838-138">继承自 [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="83838-138">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="83838-139">version</span><span class="sxs-lookup"><span data-stu-id="83838-139">version</span></span>|<span data-ttu-id="83838-140">String</span><span class="sxs-lookup"><span data-stu-id="83838-140">String</span></span>|<span data-ttu-id="83838-141">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="83838-141">Version of the entity.</span></span> <span data-ttu-id="83838-142">继承自 [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="83838-142">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="83838-143">customSettings</span><span class="sxs-lookup"><span data-stu-id="83838-143">customSettings</span></span>|<span data-ttu-id="83838-144">[keyValuePair](../resources/intune_mam_keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="83838-144">[keyValuePair](../resources/intune_mam_keyvaluepair.md) collection</span></span>|<span data-ttu-id="83838-145">一组字符串键和字符串值对，要发送到配置范围确定的用户应用，且不被此服务改变</span><span class="sxs-lookup"><span data-stu-id="83838-145">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service</span></span>|

## <a name="relationships"></a><span data-ttu-id="83838-146">关系</span><span class="sxs-lookup"><span data-stu-id="83838-146">Relationships</span></span>
<span data-ttu-id="83838-147">无</span><span class="sxs-lookup"><span data-stu-id="83838-147">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="83838-148">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="83838-148">JSON Representation</span></span>
<span data-ttu-id="83838-149">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="83838-149">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "abstract": true,
  "keyProperty": "id",
  "baseType": "microsoft.graph.managedAppPolicy",
  "@odata.type": "microsoft.graph.managedAppConfiguration"
}-->
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




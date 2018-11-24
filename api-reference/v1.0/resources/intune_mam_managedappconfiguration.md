# <a name="managedappconfiguration-resource-type"></a><span data-ttu-id="177db-101">managedAppConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="177db-101">managedAppConfiguration resource type</span></span>

> <span data-ttu-id="177db-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="177db-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="177db-103">用于将一组自定义设置按原样提供给配置范围确定的用户应用的配置。</span><span class="sxs-lookup"><span data-stu-id="177db-103">Configuration used to deliver a set of custom settings as-is to apps for users to whom the configuration is scoped</span></span>

<span data-ttu-id="177db-104">继承自 [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="177db-104">Inherits from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>

## <a name="methods"></a><span data-ttu-id="177db-105">方法</span><span class="sxs-lookup"><span data-stu-id="177db-105">Methods</span></span>
|<span data-ttu-id="177db-106">方法</span><span class="sxs-lookup"><span data-stu-id="177db-106">Method</span></span>|<span data-ttu-id="177db-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="177db-107">Return Type</span></span>|<span data-ttu-id="177db-108">说明</span><span class="sxs-lookup"><span data-stu-id="177db-108">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="177db-109">List managedAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="177db-109">List managedAppConfigurations</span></span>](../api/intune_mam_managedappconfiguration_list.md)|<span data-ttu-id="177db-110">[managedAppConfiguration](../resources/intune_mam_managedappconfiguration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="177db-110">[managedAppConfiguration](../resources/intune_mam_managedappconfiguration.md) collection</span></span>|<span data-ttu-id="177db-111">列出 [managedAppConfiguration](../resources/intune_mam_managedappconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="177db-111">List properties and relationships of the [managedAppConfiguration](../resources/intune_mam_managedappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="177db-112">Get managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="177db-112">Get managedAppConfiguration</span></span>](../api/intune_mam_managedappconfiguration_get.md)|[<span data-ttu-id="177db-113">managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="177db-113">managedAppConfiguration</span></span>](../resources/intune_mam_managedappconfiguration.md)|<span data-ttu-id="177db-114">读取 [managedAppConfiguration](../resources/intune_mam_managedappconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="177db-114">Read properties and relationships of the [managedAppConfiguration](../resources/intune_mam_managedappconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="177db-115">属性</span><span class="sxs-lookup"><span data-stu-id="177db-115">Properties</span></span>
|<span data-ttu-id="177db-116">属性</span><span class="sxs-lookup"><span data-stu-id="177db-116">Property</span></span>|<span data-ttu-id="177db-117">类型</span><span class="sxs-lookup"><span data-stu-id="177db-117">Type</span></span>|<span data-ttu-id="177db-118">说明</span><span class="sxs-lookup"><span data-stu-id="177db-118">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="177db-119">displayName</span><span class="sxs-lookup"><span data-stu-id="177db-119">displayName</span></span>|<span data-ttu-id="177db-120">String</span><span class="sxs-lookup"><span data-stu-id="177db-120">String</span></span>|<span data-ttu-id="177db-121">策略显示名称。</span><span class="sxs-lookup"><span data-stu-id="177db-121">Policy display name.</span></span> <span data-ttu-id="177db-122">继承自 [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="177db-122">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="177db-123">description</span><span class="sxs-lookup"><span data-stu-id="177db-123">description</span></span>|<span data-ttu-id="177db-124">String</span><span class="sxs-lookup"><span data-stu-id="177db-124">String</span></span>|<span data-ttu-id="177db-125">策略的说明。</span><span class="sxs-lookup"><span data-stu-id="177db-125">The policy's description.</span></span> <span data-ttu-id="177db-126">继承自 [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="177db-126">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="177db-127">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="177db-127">createdDateTime</span></span>|<span data-ttu-id="177db-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="177db-128">DateTimeOffset</span></span>|<span data-ttu-id="177db-129">创建策略的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="177db-129">The date and time the policy was created.</span></span> <span data-ttu-id="177db-130">继承自 [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="177db-130">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="177db-131">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="177db-131">lastModifiedDateTime</span></span>|<span data-ttu-id="177db-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="177db-132">DateTimeOffset</span></span>|<span data-ttu-id="177db-133">上次修改策略的时间。</span><span class="sxs-lookup"><span data-stu-id="177db-133">Last time the policy was modified.</span></span> <span data-ttu-id="177db-134">继承自 [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="177db-134">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="177db-135">id</span><span class="sxs-lookup"><span data-stu-id="177db-135">id</span></span>|<span data-ttu-id="177db-136">String</span><span class="sxs-lookup"><span data-stu-id="177db-136">String</span></span>|<span data-ttu-id="177db-137">实体的键。</span><span class="sxs-lookup"><span data-stu-id="177db-137">Key of the entity.</span></span> <span data-ttu-id="177db-138">继承自 [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="177db-138">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="177db-139">version</span><span class="sxs-lookup"><span data-stu-id="177db-139">version</span></span>|<span data-ttu-id="177db-140">String</span><span class="sxs-lookup"><span data-stu-id="177db-140">String</span></span>|<span data-ttu-id="177db-141">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="177db-141">Version of the entity.</span></span> <span data-ttu-id="177db-142">继承自 [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="177db-142">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="177db-143">customSettings</span><span class="sxs-lookup"><span data-stu-id="177db-143">customSettings</span></span>|<span data-ttu-id="177db-144">[keyValuePair](../resources/intune_mam_keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="177db-144">[keyValuePair](../resources/intune_mam_keyvaluepair.md) collection</span></span>|<span data-ttu-id="177db-145">一组字符串键和字符串值对，要发送到配置范围确定的用户应用，且不被此服务改变</span><span class="sxs-lookup"><span data-stu-id="177db-145">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service</span></span>|

## <a name="relationships"></a><span data-ttu-id="177db-146">关系</span><span class="sxs-lookup"><span data-stu-id="177db-146">Relationships</span></span>
<span data-ttu-id="177db-147">无</span><span class="sxs-lookup"><span data-stu-id="177db-147">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="177db-148">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="177db-148">JSON Representation</span></span>
<span data-ttu-id="177db-149">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="177db-149">Here is a JSON representation of the resource.</span></span>
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




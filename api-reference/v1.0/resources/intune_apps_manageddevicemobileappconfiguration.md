# <a name="manageddevicemobileappconfiguration-resource-type"></a><span data-ttu-id="1fec9-101">managedDeviceMobileAppConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="1fec9-101">managedDeviceMobileAppConfiguration resource type</span></span>

> <span data-ttu-id="1fec9-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="1fec9-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1fec9-103">已注册设备移动应用配置的抽象类</span><span class="sxs-lookup"><span data-stu-id="1fec9-103">An abstract class for Mobile app configuration for enrolled devices.</span></span>
## <a name="methods"></a><span data-ttu-id="1fec9-104">方法</span><span class="sxs-lookup"><span data-stu-id="1fec9-104">Methods</span></span>
|<span data-ttu-id="1fec9-105">方法</span><span class="sxs-lookup"><span data-stu-id="1fec9-105">Method</span></span>|<span data-ttu-id="1fec9-106">返回类型</span><span class="sxs-lookup"><span data-stu-id="1fec9-106">Return Type</span></span>|<span data-ttu-id="1fec9-107">说明</span><span class="sxs-lookup"><span data-stu-id="1fec9-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="1fec9-108">列举 managedDeviceMobileAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="1fec9-108">List managedDeviceMobileAppConfigurations</span></span>](../api/intune_apps_manageddevicemobileappconfiguration_list.md)|<span data-ttu-id="1fec9-109">[managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1fec9-109">[managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md) collection</span></span>|<span data-ttu-id="1fec9-110">列出 [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="1fec9-110">List properties and relationships of the [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="1fec9-111">获取 managedDeviceMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="1fec9-111">Get managedDeviceMobileAppConfiguration</span></span>](../api/intune_apps_manageddevicemobileappconfiguration_get.md)|[<span data-ttu-id="1fec9-112">managedDeviceMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="1fec9-112">managedDeviceMobileAppConfiguration</span></span>](../resources/intune_apps_manageddevicemobileappconfiguration.md)|<span data-ttu-id="1fec9-113">读取 [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="1fec9-113">Read properties and relationships of the [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="1fec9-114">属性</span><span class="sxs-lookup"><span data-stu-id="1fec9-114">Properties</span></span>
|<span data-ttu-id="1fec9-115">属性</span><span class="sxs-lookup"><span data-stu-id="1fec9-115">Property</span></span>|<span data-ttu-id="1fec9-116">类型</span><span class="sxs-lookup"><span data-stu-id="1fec9-116">Type</span></span>|<span data-ttu-id="1fec9-117">说明</span><span class="sxs-lookup"><span data-stu-id="1fec9-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1fec9-118">ID</span><span class="sxs-lookup"><span data-stu-id="1fec9-118">id</span></span>|<span data-ttu-id="1fec9-119">字符串</span><span class="sxs-lookup"><span data-stu-id="1fec9-119">String</span></span>|<span data-ttu-id="1fec9-120">实体的键。</span><span class="sxs-lookup"><span data-stu-id="1fec9-120">Key of the entity.</span></span>|
|<span data-ttu-id="1fec9-121">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="1fec9-121">targetedMobileApps</span></span>|<span data-ttu-id="1fec9-122">String 集合</span><span class="sxs-lookup"><span data-stu-id="1fec9-122">String collection</span></span>|<span data-ttu-id="1fec9-123">关联的应用。</span><span class="sxs-lookup"><span data-stu-id="1fec9-123">the associated app.</span></span>|
|<span data-ttu-id="1fec9-124">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1fec9-124">createdDateTime</span></span>|<span data-ttu-id="1fec9-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1fec9-125">DateTimeOffset</span></span>|<span data-ttu-id="1fec9-126">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="1fec9-126">DateTime the object was created.</span></span>|
|<span data-ttu-id="1fec9-127">说明</span><span class="sxs-lookup"><span data-stu-id="1fec9-127">description</span></span>|<span data-ttu-id="1fec9-128">字符串</span><span class="sxs-lookup"><span data-stu-id="1fec9-128">String</span></span>|<span data-ttu-id="1fec9-129">管理员提供的设备配置说明。</span><span class="sxs-lookup"><span data-stu-id="1fec9-129">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="1fec9-130">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1fec9-130">lastModifiedDateTime</span></span>|<span data-ttu-id="1fec9-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1fec9-131">DateTimeOffset</span></span>|<span data-ttu-id="1fec9-132">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="1fec9-132">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="1fec9-133">displayName</span><span class="sxs-lookup"><span data-stu-id="1fec9-133">displayName</span></span>|<span data-ttu-id="1fec9-134">字符串</span><span class="sxs-lookup"><span data-stu-id="1fec9-134">String</span></span>|<span data-ttu-id="1fec9-135">管理员提供的设备配置名称。</span><span class="sxs-lookup"><span data-stu-id="1fec9-135">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="1fec9-136">版本</span><span class="sxs-lookup"><span data-stu-id="1fec9-136">version</span></span>|<span data-ttu-id="1fec9-137">Int32</span><span class="sxs-lookup"><span data-stu-id="1fec9-137">Int32</span></span>|<span data-ttu-id="1fec9-138">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="1fec9-138">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1fec9-139">关系</span><span class="sxs-lookup"><span data-stu-id="1fec9-139">Relationships</span></span>
|<span data-ttu-id="1fec9-140">关系</span><span class="sxs-lookup"><span data-stu-id="1fec9-140">Relationship</span></span>|<span data-ttu-id="1fec9-141">类型</span><span class="sxs-lookup"><span data-stu-id="1fec9-141">Type</span></span>|<span data-ttu-id="1fec9-142">说明</span><span class="sxs-lookup"><span data-stu-id="1fec9-142">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1fec9-143">赋值</span><span class="sxs-lookup"><span data-stu-id="1fec9-143">assignments</span></span>|<span data-ttu-id="1fec9-144">[managedDeviceMobileAppConfigurationAssignment](../resources/intune_apps_manageddevicemobileappconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1fec9-144">[managedDeviceMobileAppConfigurationAssignment](../resources/intune_apps_manageddevicemobileappconfigurationassignment.md) collection</span></span>|<span data-ttu-id="1fec9-145">应用配置的组分配列表。</span><span class="sxs-lookup"><span data-stu-id="1fec9-145">The list of group assignemenets for app configration.</span></span>|
|<span data-ttu-id="1fec9-146">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="1fec9-146">deviceStatuses</span></span>|<span data-ttu-id="1fec9-147">[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune_apps_manageddevicemobileappconfigurationdevicestatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1fec9-147">[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune_apps_manageddevicemobileappconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="1fec9-148">ManagedDeviceMobileAppConfigurationDeviceStatus 的列表。</span><span class="sxs-lookup"><span data-stu-id="1fec9-148">List of ManagedDeviceMobileAppConfigurationDeviceStatus.</span></span>|
|<span data-ttu-id="1fec9-149">userStatuses</span><span class="sxs-lookup"><span data-stu-id="1fec9-149">userStatuses</span></span>|<span data-ttu-id="1fec9-150">[managedDeviceMobileAppConfigurationUserStatus](../resources/intune_apps_manageddevicemobileappconfigurationuserstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1fec9-150">[managedDeviceMobileAppConfigurationUserStatus](../resources/intune_apps_manageddevicemobileappconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="1fec9-151">ManagedDeviceMobileAppConfigurationUserStatus 列表</span><span class="sxs-lookup"><span data-stu-id="1fec9-151">List of ManagedDeviceMobileAppConfigurationUserStatus.</span></span>|
|<span data-ttu-id="1fec9-152">deviceStatusSummary</span><span class="sxs-lookup"><span data-stu-id="1fec9-152">deviceStatusSummary</span></span>|[<span data-ttu-id="1fec9-153">managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="1fec9-153">managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../resources/intune_apps_manageddevicemobileappconfigurationdevicesummary.md)|<span data-ttu-id="1fec9-154">应用配置设备状态摘要。</span><span class="sxs-lookup"><span data-stu-id="1fec9-154">App configuration device status summary.</span></span>|
|<span data-ttu-id="1fec9-155">userStatusSummary</span><span class="sxs-lookup"><span data-stu-id="1fec9-155">userStatusSummary</span></span>|[<span data-ttu-id="1fec9-156">managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="1fec9-156">managedDeviceMobileAppConfigurationUserSummary</span></span>](../resources/intune_apps_manageddevicemobileappconfigurationusersummary.md)|<span data-ttu-id="1fec9-157">应用配置用户状态摘要。</span><span class="sxs-lookup"><span data-stu-id="1fec9-157">App configuration user status summary.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1fec9-158">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1fec9-158">JSON Representation</span></span>
<span data-ttu-id="1fec9-159">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1fec9-159">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "abstract": true,
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.managedDeviceMobileAppConfiguration"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfiguration",
  "id": "String (identifier)",
  "targetedMobileApps": [
    "String"
  ],
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "version": 1024
}
```




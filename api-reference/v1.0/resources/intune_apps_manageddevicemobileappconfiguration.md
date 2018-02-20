# <a name="manageddevicemobileappconfiguration-resource-type"></a><span data-ttu-id="0fb25-101">managedDeviceMobileAppConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="0fb25-101">managedDeviceMobileAppConfiguration resource type</span></span>

> <span data-ttu-id="0fb25-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="0fb25-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0fb25-103">已注册设备移动应用配置的抽象类</span><span class="sxs-lookup"><span data-stu-id="0fb25-103">An abstract class for Mobile app configuration for enrolled devices.</span></span>
## <a name="methods"></a><span data-ttu-id="0fb25-104">方法</span><span class="sxs-lookup"><span data-stu-id="0fb25-104">Methods</span></span>
|<span data-ttu-id="0fb25-105">方法</span><span class="sxs-lookup"><span data-stu-id="0fb25-105">Method</span></span>|<span data-ttu-id="0fb25-106">返回类型</span><span class="sxs-lookup"><span data-stu-id="0fb25-106">Return Type</span></span>|<span data-ttu-id="0fb25-107">说明</span><span class="sxs-lookup"><span data-stu-id="0fb25-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="0fb25-108">List managedDeviceMobileAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="0fb25-108">List managedDeviceMobileAppConfigurations</span></span>](../api/intune_apps_manageddevicemobileappconfiguration_list.md)|<span data-ttu-id="0fb25-109">[managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0fb25-109">[managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md) collection</span></span>|<span data-ttu-id="0fb25-110">列出 [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0fb25-110">List properties and relationships of the [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="0fb25-111">Get managedDeviceMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="0fb25-111">Get managedDeviceMobileAppConfiguration</span></span>](../api/intune_apps_manageddevicemobileappconfiguration_get.md)|[<span data-ttu-id="0fb25-112">managedDeviceMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="0fb25-112">managedDeviceMobileAppConfiguration</span></span>](../resources/intune_apps_manageddevicemobileappconfiguration.md)|<span data-ttu-id="0fb25-113">读取 [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0fb25-113">Read properties and relationships of [plannerProgressTaskBoardTaskFormat](../resources/intune_apps_manageddevicemobileappconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="0fb25-114">属性</span><span class="sxs-lookup"><span data-stu-id="0fb25-114">Properties</span></span>
|<span data-ttu-id="0fb25-115">属性</span><span class="sxs-lookup"><span data-stu-id="0fb25-115">Property</span></span>|<span data-ttu-id="0fb25-116">类型</span><span class="sxs-lookup"><span data-stu-id="0fb25-116">Type</span></span>|<span data-ttu-id="0fb25-117">说明</span><span class="sxs-lookup"><span data-stu-id="0fb25-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0fb25-118">id</span><span class="sxs-lookup"><span data-stu-id="0fb25-118">id</span></span>|<span data-ttu-id="0fb25-119">String</span><span class="sxs-lookup"><span data-stu-id="0fb25-119">String</span></span>|<span data-ttu-id="0fb25-120">实体的键。</span><span class="sxs-lookup"><span data-stu-id="0fb25-120">Key of the setting.</span></span>|
|<span data-ttu-id="0fb25-121">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="0fb25-121">targetedMobileApps</span></span>|<span data-ttu-id="0fb25-122">String 集合</span><span class="sxs-lookup"><span data-stu-id="0fb25-122">String collection</span></span>|<span data-ttu-id="0fb25-123">关联的应用。</span><span class="sxs-lookup"><span data-stu-id="0fb25-123">the associated app.</span></span>|
|<span data-ttu-id="0fb25-124">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0fb25-124">createdDateTime</span></span>|<span data-ttu-id="0fb25-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0fb25-125">DateTimeOffset</span></span>|<span data-ttu-id="0fb25-126">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="0fb25-126">DateTime the object was created.</span></span>|
|<span data-ttu-id="0fb25-127">description</span><span class="sxs-lookup"><span data-stu-id="0fb25-127">description</span></span>|<span data-ttu-id="0fb25-128">String</span><span class="sxs-lookup"><span data-stu-id="0fb25-128">String</span></span>|<span data-ttu-id="0fb25-129">管理员提供的设备配置说明。</span><span class="sxs-lookup"><span data-stu-id="0fb25-129">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="0fb25-130">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0fb25-130">lastModifiedDateTime</span></span>|<span data-ttu-id="0fb25-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0fb25-131">DateTimeOffset</span></span>|<span data-ttu-id="0fb25-132">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="0fb25-132">Indicates the date the object was last modified.</span></span>|
|<span data-ttu-id="0fb25-133">displayName</span><span class="sxs-lookup"><span data-stu-id="0fb25-133">displayName</span></span>|<span data-ttu-id="0fb25-134">String</span><span class="sxs-lookup"><span data-stu-id="0fb25-134">String</span></span>|<span data-ttu-id="0fb25-135">管理员提供的设备配置名称。</span><span class="sxs-lookup"><span data-stu-id="0fb25-135">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="0fb25-136">version</span><span class="sxs-lookup"><span data-stu-id="0fb25-136">version</span></span>|<span data-ttu-id="0fb25-137">Int32</span><span class="sxs-lookup"><span data-stu-id="0fb25-137">Int32</span></span>|<span data-ttu-id="0fb25-138">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="0fb25-138">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0fb25-139">关系</span><span class="sxs-lookup"><span data-stu-id="0fb25-139">Relationships</span></span>
|<span data-ttu-id="0fb25-140">关系</span><span class="sxs-lookup"><span data-stu-id="0fb25-140">Relationship</span></span>|<span data-ttu-id="0fb25-141">类型</span><span class="sxs-lookup"><span data-stu-id="0fb25-141">Type</span></span>|<span data-ttu-id="0fb25-142">说明</span><span class="sxs-lookup"><span data-stu-id="0fb25-142">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0fb25-143">assignments</span><span class="sxs-lookup"><span data-stu-id="0fb25-143">assignments</span></span>|<span data-ttu-id="0fb25-144">[managedDeviceMobileAppConfigurationAssignment](../resources/intune_apps_manageddevicemobileappconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0fb25-144">[managedDeviceMobileAppConfigurationAssignment](../resources/intune_apps_manageddevicemobileappconfigurationassignment.md) collection</span></span>|<span data-ttu-id="0fb25-145">应用配置的组分配列表。</span><span class="sxs-lookup"><span data-stu-id="0fb25-145">The list of group assignemenets for app configration.</span></span>|
|<span data-ttu-id="0fb25-146">userStatuses</span><span class="sxs-lookup"><span data-stu-id="0fb25-146">userStatuses</span></span>|<span data-ttu-id="0fb25-147">[managedDeviceMobileAppConfigurationUserStatus](../resources/intune_apps_manageddevicemobileappconfigurationuserstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0fb25-147">[managedDeviceMobileAppConfigurationUserStatus](../resources/intune_apps_manageddevicemobileappconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="0fb25-148">ManagedDeviceMobileAppConfigurationUserStatus 列表</span><span class="sxs-lookup"><span data-stu-id="0fb25-148">List of ManagedDeviceMobileAppConfigurationUserStatus.</span></span>|
|<span data-ttu-id="0fb25-149">deviceStatusSummary</span><span class="sxs-lookup"><span data-stu-id="0fb25-149">deviceStatusSummary</span></span>|[<span data-ttu-id="0fb25-150">managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="0fb25-150">managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../resources/intune_apps_manageddevicemobileappconfigurationdevicesummary.md)|<span data-ttu-id="0fb25-151">应用配置设备状态摘要。</span><span class="sxs-lookup"><span data-stu-id="0fb25-151">App configuration device status summary.</span></span>|
|<span data-ttu-id="0fb25-152">userStatusSummary</span><span class="sxs-lookup"><span data-stu-id="0fb25-152">userStatusSummary</span></span>|[<span data-ttu-id="0fb25-153">managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="0fb25-153">managedDeviceMobileAppConfigurationUserSummary</span></span>](../resources/intune_apps_manageddevicemobileappconfigurationusersummary.md)|<span data-ttu-id="0fb25-154">应用配置用户状态摘要。</span><span class="sxs-lookup"><span data-stu-id="0fb25-154">App configuration user status summary.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0fb25-155">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0fb25-155">JSON Representation</span></span>
<span data-ttu-id="0fb25-156">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0fb25-156">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDeviceMobileAppConfiguration"
}
-->
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




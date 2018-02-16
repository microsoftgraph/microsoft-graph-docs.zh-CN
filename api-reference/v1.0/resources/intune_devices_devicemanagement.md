# <a name="devicemanagement-resource-type"></a><span data-ttu-id="7e2eb-101">deviceManagement 资源类型</span><span class="sxs-lookup"><span data-stu-id="7e2eb-101">deviceManagement resource type</span></span>

> <span data-ttu-id="7e2eb-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="7e2eb-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7e2eb-103">充当所有设备管理功能的容器的单例实体。</span><span class="sxs-lookup"><span data-stu-id="7e2eb-103">Singleton entity that acts as a container for all device management functionality.</span></span>
## <a name="methods"></a><span data-ttu-id="7e2eb-104">方法</span><span class="sxs-lookup"><span data-stu-id="7e2eb-104">Methods</span></span>
|<span data-ttu-id="7e2eb-105">方法</span><span class="sxs-lookup"><span data-stu-id="7e2eb-105">Method</span></span>|<span data-ttu-id="7e2eb-106">返回类型</span><span class="sxs-lookup"><span data-stu-id="7e2eb-106">Return Type</span></span>|<span data-ttu-id="7e2eb-107">说明</span><span class="sxs-lookup"><span data-stu-id="7e2eb-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="7e2eb-108">获取 deviceManagement</span><span class="sxs-lookup"><span data-stu-id="7e2eb-108">Get deviceManagement</span></span>](../api/intune_devices_devicemanagement_get.md)|[<span data-ttu-id="7e2eb-109">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="7e2eb-109">deviceManagement</span></span>](../resources/intune_devices_devicemanagement.md)|<span data-ttu-id="7e2eb-110">读取 [deviceManagement](../resources/intune_devices_devicemanagement.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="7e2eb-110">Read properties and relationships of [plannerTaskDetails](../resources/intune_devices_devicemanagement.md) object.</span></span>|
|[<span data-ttu-id="7e2eb-111">更新 deviceManagement</span><span class="sxs-lookup"><span data-stu-id="7e2eb-111">Update deviceManagement</span></span>](../api/intune_devices_devicemanagement_update.md)|[<span data-ttu-id="7e2eb-112">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="7e2eb-112">deviceManagement</span></span>](../resources/intune_devices_devicemanagement.md)|<span data-ttu-id="7e2eb-113">更新 [deviceManagement](../resources/intune_devices_devicemanagement.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="7e2eb-113">Update the properties of a [calendar](../resources/intune_devices_devicemanagement.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="7e2eb-114">属性</span><span class="sxs-lookup"><span data-stu-id="7e2eb-114">Properties</span></span>
|<span data-ttu-id="7e2eb-115">属性</span><span class="sxs-lookup"><span data-stu-id="7e2eb-115">Property</span></span>|<span data-ttu-id="7e2eb-116">类型</span><span class="sxs-lookup"><span data-stu-id="7e2eb-116">Type</span></span>|<span data-ttu-id="7e2eb-117">说明</span><span class="sxs-lookup"><span data-stu-id="7e2eb-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7e2eb-118">id</span><span class="sxs-lookup"><span data-stu-id="7e2eb-118">id</span></span>|<span data-ttu-id="7e2eb-119">String</span><span class="sxs-lookup"><span data-stu-id="7e2eb-119">String</span></span>|<span data-ttu-id="7e2eb-120">设备唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="7e2eb-120">Unique Identifier for the device</span></span>|
|<span data-ttu-id="7e2eb-121">subscriptionState</span><span class="sxs-lookup"><span data-stu-id="7e2eb-121">subscriptionState</span></span>|<span data-ttu-id="7e2eb-122">String</span><span class="sxs-lookup"><span data-stu-id="7e2eb-122">String</span></span>|<span data-ttu-id="7e2eb-123">租户移动设备管理订阅状态。</span><span class="sxs-lookup"><span data-stu-id="7e2eb-123">Tenant mobile device management subscription state.</span></span> <span data-ttu-id="7e2eb-124">可取值为：`pending`、`active`、`warning`、`disabled`、`deleted`、`blocked`、`lockedOut`。</span><span class="sxs-lookup"><span data-stu-id="7e2eb-124">Possible values are: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7e2eb-125">关系</span><span class="sxs-lookup"><span data-stu-id="7e2eb-125">Relationships</span></span>
|<span data-ttu-id="7e2eb-126">关系</span><span class="sxs-lookup"><span data-stu-id="7e2eb-126">Relationship</span></span>|<span data-ttu-id="7e2eb-127">类型</span><span class="sxs-lookup"><span data-stu-id="7e2eb-127">Type</span></span>|<span data-ttu-id="7e2eb-128">说明</span><span class="sxs-lookup"><span data-stu-id="7e2eb-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7e2eb-129">applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="7e2eb-129">applePushNotificationCertificate</span></span>|[<span data-ttu-id="7e2eb-130">applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="7e2eb-130">applePushNotificationCertificate</span></span>](../resources/intune_devices_applepushnotificationcertificate.md)|<span data-ttu-id="7e2eb-131">Apple 推送通知证书。</span><span class="sxs-lookup"><span data-stu-id="7e2eb-131">Apple push notification certificate.</span></span>|
|<span data-ttu-id="7e2eb-132">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="7e2eb-132">managedDeviceOverview</span></span>|[<span data-ttu-id="7e2eb-133">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="7e2eb-133">managedDeviceOverview</span></span>](../resources/intune_devices_manageddeviceoverview.md)|<span data-ttu-id="7e2eb-134">设备概述</span><span class="sxs-lookup"><span data-stu-id="7e2eb-134">Device overview</span></span>|
|<span data-ttu-id="7e2eb-135">detectedApps</span><span class="sxs-lookup"><span data-stu-id="7e2eb-135">detectedApps</span></span>|<span data-ttu-id="7e2eb-136">[detectedApp](../resources/intune_devices_detectedapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7e2eb-136">[detectedApp](../resources/intune_devices_detectedapp.md) collection</span></span>|<span data-ttu-id="7e2eb-137">检测到与设备关联的应用的列表。</span><span class="sxs-lookup"><span data-stu-id="7e2eb-137">The list of detected apps associated with a device.</span></span>|
|<span data-ttu-id="7e2eb-138">managedDevices</span><span class="sxs-lookup"><span data-stu-id="7e2eb-138">managedDevices</span></span>|<span data-ttu-id="7e2eb-139">[managedDevice](../resources/intune_devices_manageddevice.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7e2eb-139">[managedDevice](../resources/intune_devices_manageddevice.md) collection</span></span>|<span data-ttu-id="7e2eb-140">托管设备列表。</span><span class="sxs-lookup"><span data-stu-id="7e2eb-140">The list of managed devices.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7e2eb-141">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7e2eb-141">JSON Representation</span></span>
<span data-ttu-id="7e2eb-142">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7e2eb-142">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagement",
  "id": "String (identifier)",
  "subscriptionState": "String"
}
```




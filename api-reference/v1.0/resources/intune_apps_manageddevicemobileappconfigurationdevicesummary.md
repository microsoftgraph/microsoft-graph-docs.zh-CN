# <a name="manageddevicemobileappconfigurationdevicesummary-resource-type"></a><span data-ttu-id="a852e-101">managedDeviceMobileAppConfigurationDeviceSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="a852e-101">managedDeviceMobileAppConfigurationDeviceSummary resource type</span></span>

> <span data-ttu-id="a852e-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="a852e-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a852e-103">包含 MDM 移动应用配置设备状态摘要的属性、继承属性和操作。</span><span class="sxs-lookup"><span data-stu-id="a852e-103">Contains properties, inherited properties and actions for an MDM mobile app configuration device status summary.</span></span>
## <a name="methods"></a><span data-ttu-id="a852e-104">方法</span><span class="sxs-lookup"><span data-stu-id="a852e-104">Methods</span></span>
|<span data-ttu-id="a852e-105">方法</span><span class="sxs-lookup"><span data-stu-id="a852e-105">Method</span></span>|<span data-ttu-id="a852e-106">返回类型</span><span class="sxs-lookup"><span data-stu-id="a852e-106">Return Type</span></span>|<span data-ttu-id="a852e-107">说明</span><span class="sxs-lookup"><span data-stu-id="a852e-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a852e-108">获取 managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="a852e-108">Get managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../api/intune_apps_manageddevicemobileappconfigurationdevicesummary_get.md)|[<span data-ttu-id="a852e-109">managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="a852e-109">managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../resources/intune_apps_manageddevicemobileappconfigurationdevicesummary.md)|<span data-ttu-id="a852e-110">读取 [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune_apps_manageddevicemobileappconfigurationdevicesummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a852e-110">Read properties and relationships of [plannerTaskDetails](../resources/intune_apps_manageddevicemobileappconfigurationdevicesummary.md) object.</span></span>|
|[<span data-ttu-id="a852e-111">更新 managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="a852e-111">Update managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../api/intune_apps_manageddevicemobileappconfigurationdevicesummary_update.md)|[<span data-ttu-id="a852e-112">managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="a852e-112">managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../resources/intune_apps_manageddevicemobileappconfigurationdevicesummary.md)|<span data-ttu-id="a852e-113">更新 [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune_apps_manageddevicemobileappconfigurationdevicesummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="a852e-113">Update the properties of a [calendar](../resources/intune_apps_manageddevicemobileappconfigurationdevicesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="a852e-114">属性</span><span class="sxs-lookup"><span data-stu-id="a852e-114">Properties</span></span>
|<span data-ttu-id="a852e-115">属性</span><span class="sxs-lookup"><span data-stu-id="a852e-115">Property</span></span>|<span data-ttu-id="a852e-116">类型</span><span class="sxs-lookup"><span data-stu-id="a852e-116">Type</span></span>|<span data-ttu-id="a852e-117">说明</span><span class="sxs-lookup"><span data-stu-id="a852e-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a852e-118">id</span><span class="sxs-lookup"><span data-stu-id="a852e-118">id</span></span>|<span data-ttu-id="a852e-119">String</span><span class="sxs-lookup"><span data-stu-id="a852e-119">String</span></span>|<span data-ttu-id="a852e-120">实体的键。</span><span class="sxs-lookup"><span data-stu-id="a852e-120">Key of the setting.</span></span>|
|<span data-ttu-id="a852e-121">pendingCount</span><span class="sxs-lookup"><span data-stu-id="a852e-121">pendingCount</span></span>|<span data-ttu-id="a852e-122">Int32</span><span class="sxs-lookup"><span data-stu-id="a852e-122">Int32</span></span>|<span data-ttu-id="a852e-123">待定设备的数量</span><span class="sxs-lookup"><span data-stu-id="a852e-123">Number of pending devices</span></span>|
|<span data-ttu-id="a852e-124">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="a852e-124">notApplicableCount</span></span>|<span data-ttu-id="a852e-125">Int32</span><span class="sxs-lookup"><span data-stu-id="a852e-125">Int32</span></span>|<span data-ttu-id="a852e-126">不适用设备的数量</span><span class="sxs-lookup"><span data-stu-id="a852e-126">Number of not applicable devices</span></span>|
|<span data-ttu-id="a852e-127">successCount</span><span class="sxs-lookup"><span data-stu-id="a852e-127">successCount</span></span>|<span data-ttu-id="a852e-128">Int32</span><span class="sxs-lookup"><span data-stu-id="a852e-128">Int32</span></span>|<span data-ttu-id="a852e-129">成功的设备数量</span><span class="sxs-lookup"><span data-stu-id="a852e-129">Number of succeeded devices</span></span>|
|<span data-ttu-id="a852e-130">errorCount</span><span class="sxs-lookup"><span data-stu-id="a852e-130">errorCount</span></span>|<span data-ttu-id="a852e-131">Int32</span><span class="sxs-lookup"><span data-stu-id="a852e-131">Int32</span></span>|<span data-ttu-id="a852e-132">错误设备的数量</span><span class="sxs-lookup"><span data-stu-id="a852e-132">Number of error devices</span></span>|
|<span data-ttu-id="a852e-133">failedCount</span><span class="sxs-lookup"><span data-stu-id="a852e-133">failedCount</span></span>|<span data-ttu-id="a852e-134">Int32</span><span class="sxs-lookup"><span data-stu-id="a852e-134">Int32</span></span>|<span data-ttu-id="a852e-135">失败的设备数量</span><span class="sxs-lookup"><span data-stu-id="a852e-135">Number of failed devices</span></span>|
|<span data-ttu-id="a852e-136">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="a852e-136">lastUpdateDateTime</span></span>|<span data-ttu-id="a852e-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a852e-137">DateTimeOffset</span></span>|<span data-ttu-id="a852e-138">上次更新时间</span><span class="sxs-lookup"><span data-stu-id="a852e-138">Last update time</span></span>|
|<span data-ttu-id="a852e-139">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="a852e-139">configurationVersion</span></span>|<span data-ttu-id="a852e-140">Int32</span><span class="sxs-lookup"><span data-stu-id="a852e-140">Int32</span></span>|<span data-ttu-id="a852e-141">用于此概述的策略版本</span><span class="sxs-lookup"><span data-stu-id="a852e-141">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="a852e-142">关系</span><span class="sxs-lookup"><span data-stu-id="a852e-142">Relationships</span></span>
<span data-ttu-id="a852e-143">无</span><span class="sxs-lookup"><span data-stu-id="a852e-143">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a852e-144">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a852e-144">JSON Representation</span></span>
<span data-ttu-id="a852e-145">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a852e-145">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDeviceMobileAppConfigurationDeviceSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationDeviceSummary",
  "id": "String (identifier)",
  "pendingCount": 1024,
  "notApplicableCount": 1024,
  "successCount": 1024,
  "errorCount": 1024,
  "failedCount": 1024,
  "lastUpdateDateTime": "String (timestamp)",
  "configurationVersion": 1024
}
```




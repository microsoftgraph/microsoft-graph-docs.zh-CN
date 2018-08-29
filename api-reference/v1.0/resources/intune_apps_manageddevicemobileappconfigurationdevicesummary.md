# <a name="manageddevicemobileappconfigurationdevicesummary-resource-type"></a><span data-ttu-id="0e9cf-101">managedDeviceMobileAppConfigurationDeviceSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="0e9cf-101">managedDeviceMobileAppConfigurationDeviceSummary resource type</span></span>

> <span data-ttu-id="0e9cf-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="0e9cf-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0e9cf-103">包含 MDM 移动应用配置设备状态摘要的属性、继承属性和操作。</span><span class="sxs-lookup"><span data-stu-id="0e9cf-103">Contains properties, inherited properties and actions for an MDM mobile app configuration device status summary.</span></span>
## <a name="methods"></a><span data-ttu-id="0e9cf-104">方法</span><span class="sxs-lookup"><span data-stu-id="0e9cf-104">Methods</span></span>
|<span data-ttu-id="0e9cf-105">方法</span><span class="sxs-lookup"><span data-stu-id="0e9cf-105">Method</span></span>|<span data-ttu-id="0e9cf-106">返回类型</span><span class="sxs-lookup"><span data-stu-id="0e9cf-106">Return Type</span></span>|<span data-ttu-id="0e9cf-107">说明</span><span class="sxs-lookup"><span data-stu-id="0e9cf-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="0e9cf-108">获取 managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="0e9cf-108">Get managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../api/intune_apps_manageddevicemobileappconfigurationdevicesummary_get.md)|[<span data-ttu-id="0e9cf-109">managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="0e9cf-109">managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../resources/intune_apps_manageddevicemobileappconfigurationdevicesummary.md)|<span data-ttu-id="0e9cf-110">读取 [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune_apps_manageddevicemobileappconfigurationdevicesummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0e9cf-110">Read properties and relationships of the [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune_apps_manageddevicemobileappconfigurationdevicesummary.md) object.</span></span>|
|[<span data-ttu-id="0e9cf-111">更新 managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="0e9cf-111">Update managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../api/intune_apps_manageddevicemobileappconfigurationdevicesummary_update.md)|[<span data-ttu-id="0e9cf-112">managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="0e9cf-112">managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../resources/intune_apps_manageddevicemobileappconfigurationdevicesummary.md)|<span data-ttu-id="0e9cf-113">更新 [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune_apps_manageddevicemobileappconfigurationdevicesummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="0e9cf-113">Update the properties of a [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune_apps_manageddevicemobileappconfigurationdevicesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="0e9cf-114">属性</span><span class="sxs-lookup"><span data-stu-id="0e9cf-114">Properties</span></span>
|<span data-ttu-id="0e9cf-115">属性</span><span class="sxs-lookup"><span data-stu-id="0e9cf-115">Property</span></span>|<span data-ttu-id="0e9cf-116">类型</span><span class="sxs-lookup"><span data-stu-id="0e9cf-116">Type</span></span>|<span data-ttu-id="0e9cf-117">说明</span><span class="sxs-lookup"><span data-stu-id="0e9cf-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0e9cf-118">id</span><span class="sxs-lookup"><span data-stu-id="0e9cf-118">id</span></span>|<span data-ttu-id="0e9cf-119">字符串</span><span class="sxs-lookup"><span data-stu-id="0e9cf-119">String</span></span>|<span data-ttu-id="0e9cf-120">实体的键。</span><span class="sxs-lookup"><span data-stu-id="0e9cf-120">Key of the entity.</span></span>|
|<span data-ttu-id="0e9cf-121">pendingCount</span><span class="sxs-lookup"><span data-stu-id="0e9cf-121">pendingCount</span></span>|<span data-ttu-id="0e9cf-122">Int32</span><span class="sxs-lookup"><span data-stu-id="0e9cf-122">Int32</span></span>|<span data-ttu-id="0e9cf-123">挂起设备的数量</span><span class="sxs-lookup"><span data-stu-id="0e9cf-123">Number of pending devices</span></span>|
|<span data-ttu-id="0e9cf-124">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="0e9cf-124">notApplicableCount</span></span>|<span data-ttu-id="0e9cf-125">Int32</span><span class="sxs-lookup"><span data-stu-id="0e9cf-125">Int32</span></span>|<span data-ttu-id="0e9cf-126">不适用设备的数量</span><span class="sxs-lookup"><span data-stu-id="0e9cf-126">Number of not applicable devices</span></span>|
|<span data-ttu-id="0e9cf-127">successCount</span><span class="sxs-lookup"><span data-stu-id="0e9cf-127">successCount</span></span>|<span data-ttu-id="0e9cf-128">Int32</span><span class="sxs-lookup"><span data-stu-id="0e9cf-128">Int32</span></span>|<span data-ttu-id="0e9cf-129">成功设备的数量</span><span class="sxs-lookup"><span data-stu-id="0e9cf-129">Number of succeeded devices</span></span>|
|<span data-ttu-id="0e9cf-130">errorCount</span><span class="sxs-lookup"><span data-stu-id="0e9cf-130">errorCount</span></span>|<span data-ttu-id="0e9cf-131">Int32</span><span class="sxs-lookup"><span data-stu-id="0e9cf-131">Int32</span></span>|<span data-ttu-id="0e9cf-132">错误设备的数量</span><span class="sxs-lookup"><span data-stu-id="0e9cf-132">Number of error devices</span></span>|
|<span data-ttu-id="0e9cf-133">failedCount</span><span class="sxs-lookup"><span data-stu-id="0e9cf-133">failedCount</span></span>|<span data-ttu-id="0e9cf-134">Int32</span><span class="sxs-lookup"><span data-stu-id="0e9cf-134">Int32</span></span>|<span data-ttu-id="0e9cf-135">失败设备的数量</span><span class="sxs-lookup"><span data-stu-id="0e9cf-135">Number of failed devices</span></span>|
|<span data-ttu-id="0e9cf-136">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="0e9cf-136">lastUpdateDateTime</span></span>|<span data-ttu-id="0e9cf-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0e9cf-137">DateTimeOffset</span></span>|<span data-ttu-id="0e9cf-138">上次更新时间</span><span class="sxs-lookup"><span data-stu-id="0e9cf-138">Last update time</span></span>|
|<span data-ttu-id="0e9cf-139">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="0e9cf-139">configurationVersion</span></span>|<span data-ttu-id="0e9cf-140">Int32</span><span class="sxs-lookup"><span data-stu-id="0e9cf-140">Int32</span></span>|<span data-ttu-id="0e9cf-141">用于此概述的策略版本</span><span class="sxs-lookup"><span data-stu-id="0e9cf-141">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="0e9cf-142">关系</span><span class="sxs-lookup"><span data-stu-id="0e9cf-142">Relationships</span></span>
<span data-ttu-id="0e9cf-143">无</span><span class="sxs-lookup"><span data-stu-id="0e9cf-143">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="0e9cf-144">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0e9cf-144">JSON Representation</span></span>
<span data-ttu-id="0e9cf-145">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0e9cf-145">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.managedDeviceMobileAppConfigurationDeviceSummary"
}-->
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




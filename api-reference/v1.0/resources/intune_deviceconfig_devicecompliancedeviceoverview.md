# <a name="devicecompliancedeviceoverview-resource-type"></a><span data-ttu-id="476d7-101">deviceComplianceDeviceOverview 资源类型</span><span class="sxs-lookup"><span data-stu-id="476d7-101">deviceComplianceDeviceOverview resource type</span></span>

> <span data-ttu-id="476d7-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="476d7-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="476d7-103">尚未记录</span><span class="sxs-lookup"><span data-stu-id="476d7-103">Not yet documented</span></span>
## <a name="methods"></a><span data-ttu-id="476d7-104">方法</span><span class="sxs-lookup"><span data-stu-id="476d7-104">Methods</span></span>
|<span data-ttu-id="476d7-105">方法</span><span class="sxs-lookup"><span data-stu-id="476d7-105">Method</span></span>|<span data-ttu-id="476d7-106">返回类型</span><span class="sxs-lookup"><span data-stu-id="476d7-106">Return Type</span></span>|<span data-ttu-id="476d7-107">说明</span><span class="sxs-lookup"><span data-stu-id="476d7-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="476d7-108">获取 deviceComplianceDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="476d7-108">Get deviceComplianceDeviceOverview</span></span>](../api/intune_deviceconfig_devicecompliancedeviceoverview_get.md)|[<span data-ttu-id="476d7-109">deviceComplianceDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="476d7-109">deviceComplianceDeviceOverview</span></span>](../resources/intune_deviceconfig_devicecompliancedeviceoverview.md)|<span data-ttu-id="476d7-110">读取 [deviceComplianceDeviceOverview](../resources/intune_deviceconfig_devicecompliancedeviceoverview.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="476d7-110">Read properties and relationships of the [deviceComplianceDeviceOverview](../resources/intune_deviceconfig_devicecompliancedeviceoverview.md) object.</span></span>|
|[<span data-ttu-id="476d7-111">更新 deviceComplianceDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="476d7-111">Update deviceComplianceDeviceOverview</span></span>](../api/intune_deviceconfig_devicecompliancedeviceoverview_update.md)|[<span data-ttu-id="476d7-112">deviceComplianceDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="476d7-112">deviceComplianceDeviceOverview</span></span>](../resources/intune_deviceconfig_devicecompliancedeviceoverview.md)|<span data-ttu-id="476d7-113">更新 [deviceComplianceDeviceOverview](../resources/intune_deviceconfig_devicecompliancedeviceoverview.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="476d7-113">Update the properties of a [deviceComplianceDeviceOverview](../resources/intune_deviceconfig_devicecompliancedeviceoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="476d7-114">属性</span><span class="sxs-lookup"><span data-stu-id="476d7-114">Properties</span></span>
|<span data-ttu-id="476d7-115">属性</span><span class="sxs-lookup"><span data-stu-id="476d7-115">Property</span></span>|<span data-ttu-id="476d7-116">类型</span><span class="sxs-lookup"><span data-stu-id="476d7-116">Type</span></span>|<span data-ttu-id="476d7-117">说明</span><span class="sxs-lookup"><span data-stu-id="476d7-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="476d7-118">ID</span><span class="sxs-lookup"><span data-stu-id="476d7-118">id</span></span>|<span data-ttu-id="476d7-119">字符串</span><span class="sxs-lookup"><span data-stu-id="476d7-119">String</span></span>|<span data-ttu-id="476d7-120">实体的键。</span><span class="sxs-lookup"><span data-stu-id="476d7-120">Key of the entity.</span></span>|
|<span data-ttu-id="476d7-121">pendingCount</span><span class="sxs-lookup"><span data-stu-id="476d7-121">pendingCount</span></span>|<span data-ttu-id="476d7-122">Int32</span><span class="sxs-lookup"><span data-stu-id="476d7-122">Int32</span></span>|<span data-ttu-id="476d7-123">挂起设备的数量</span><span class="sxs-lookup"><span data-stu-id="476d7-123">Number of pending devices</span></span>|
|<span data-ttu-id="476d7-124">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="476d7-124">notApplicableCount</span></span>|<span data-ttu-id="476d7-125">Int32</span><span class="sxs-lookup"><span data-stu-id="476d7-125">Int32</span></span>|<span data-ttu-id="476d7-126">不适用设备的数量</span><span class="sxs-lookup"><span data-stu-id="476d7-126">Number of not applicable devices</span></span>|
|<span data-ttu-id="476d7-127">successCount</span><span class="sxs-lookup"><span data-stu-id="476d7-127">successCount</span></span>|<span data-ttu-id="476d7-128">Int32</span><span class="sxs-lookup"><span data-stu-id="476d7-128">Int32</span></span>|<span data-ttu-id="476d7-129">成功设备的数量</span><span class="sxs-lookup"><span data-stu-id="476d7-129">Number of succeeded devices</span></span>|
|<span data-ttu-id="476d7-130">errorCount</span><span class="sxs-lookup"><span data-stu-id="476d7-130">errorCount</span></span>|<span data-ttu-id="476d7-131">Int32</span><span class="sxs-lookup"><span data-stu-id="476d7-131">Int32</span></span>|<span data-ttu-id="476d7-132">错误设备的数量</span><span class="sxs-lookup"><span data-stu-id="476d7-132">Number of error devices</span></span>|
|<span data-ttu-id="476d7-133">failedCount</span><span class="sxs-lookup"><span data-stu-id="476d7-133">failedCount</span></span>|<span data-ttu-id="476d7-134">Int32</span><span class="sxs-lookup"><span data-stu-id="476d7-134">Int32</span></span>|<span data-ttu-id="476d7-135">失败设备的数量</span><span class="sxs-lookup"><span data-stu-id="476d7-135">Number of failed devices</span></span>|
|<span data-ttu-id="476d7-136">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="476d7-136">lastUpdateDateTime</span></span>|<span data-ttu-id="476d7-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="476d7-137">DateTimeOffset</span></span>|<span data-ttu-id="476d7-138">上次更新时间</span><span class="sxs-lookup"><span data-stu-id="476d7-138">Last update time</span></span>|
|<span data-ttu-id="476d7-139">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="476d7-139">configurationVersion</span></span>|<span data-ttu-id="476d7-140">Int32</span><span class="sxs-lookup"><span data-stu-id="476d7-140">Int32</span></span>|<span data-ttu-id="476d7-141">用于此概述的策略版本</span><span class="sxs-lookup"><span data-stu-id="476d7-141">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="476d7-142">关系</span><span class="sxs-lookup"><span data-stu-id="476d7-142">Relationships</span></span>
<span data-ttu-id="476d7-143">无</span><span class="sxs-lookup"><span data-stu-id="476d7-143">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="476d7-144">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="476d7-144">JSON Representation</span></span>
<span data-ttu-id="476d7-145">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="476d7-145">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.deviceComplianceDeviceOverview"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComplianceDeviceOverview",
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




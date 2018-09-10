# <a name="devicecompliancedeviceoverview-resource-type"></a><span data-ttu-id="0af0b-101">deviceComplianceDeviceOverview 资源类型</span><span class="sxs-lookup"><span data-stu-id="0af0b-101">deviceComplianceDeviceOverview resource type</span></span>

> <span data-ttu-id="0af0b-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="0af0b-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0af0b-103">尚未记录</span><span class="sxs-lookup"><span data-stu-id="0af0b-103">Not yet documented</span></span>
## <a name="methods"></a><span data-ttu-id="0af0b-104">方法</span><span class="sxs-lookup"><span data-stu-id="0af0b-104">Methods</span></span>
|<span data-ttu-id="0af0b-105">方法</span><span class="sxs-lookup"><span data-stu-id="0af0b-105">Method</span></span>|<span data-ttu-id="0af0b-106">返回类型</span><span class="sxs-lookup"><span data-stu-id="0af0b-106">Return Type</span></span>|<span data-ttu-id="0af0b-107">说明</span><span class="sxs-lookup"><span data-stu-id="0af0b-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="0af0b-108">获取 deviceComplianceDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="0af0b-108">Get deviceComplianceDeviceOverview</span></span>](../api/intune_deviceconfig_devicecompliancedeviceoverview_get.md)|[<span data-ttu-id="0af0b-109">deviceComplianceDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="0af0b-109">deviceComplianceDeviceOverview</span></span>](../resources/intune_deviceconfig_devicecompliancedeviceoverview.md)|<span data-ttu-id="0af0b-110">读取 [deviceComplianceDeviceOverview](../resources/intune_deviceconfig_devicecompliancedeviceoverview.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0af0b-110">Read properties and relationships of the [deviceComplianceDeviceOverview](../resources/intune_deviceconfig_devicecompliancedeviceoverview.md) object.</span></span>|
|[<span data-ttu-id="0af0b-111">更新 deviceComplianceDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="0af0b-111">Update deviceComplianceDeviceOverview</span></span>](../api/intune_deviceconfig_devicecompliancedeviceoverview_update.md)|[<span data-ttu-id="0af0b-112">deviceComplianceDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="0af0b-112">deviceComplianceDeviceOverview</span></span>](../resources/intune_deviceconfig_devicecompliancedeviceoverview.md)|<span data-ttu-id="0af0b-113">更新 [deviceComplianceDeviceOverview](../resources/intune_deviceconfig_devicecompliancedeviceoverview.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="0af0b-113">Update the properties of a [deviceComplianceDeviceOverview](../resources/intune_deviceconfig_devicecompliancedeviceoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="0af0b-114">属性</span><span class="sxs-lookup"><span data-stu-id="0af0b-114">Properties</span></span>
|<span data-ttu-id="0af0b-115">属性</span><span class="sxs-lookup"><span data-stu-id="0af0b-115">Property</span></span>|<span data-ttu-id="0af0b-116">类型</span><span class="sxs-lookup"><span data-stu-id="0af0b-116">Type</span></span>|<span data-ttu-id="0af0b-117">说明</span><span class="sxs-lookup"><span data-stu-id="0af0b-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0af0b-118">ID</span><span class="sxs-lookup"><span data-stu-id="0af0b-118">id</span></span>|<span data-ttu-id="0af0b-119">字符串</span><span class="sxs-lookup"><span data-stu-id="0af0b-119">String</span></span>|<span data-ttu-id="0af0b-120">实体的键。</span><span class="sxs-lookup"><span data-stu-id="0af0b-120">Key of the entity.</span></span>|
|<span data-ttu-id="0af0b-121">pendingCount</span><span class="sxs-lookup"><span data-stu-id="0af0b-121">pendingCount</span></span>|<span data-ttu-id="0af0b-122">Int32</span><span class="sxs-lookup"><span data-stu-id="0af0b-122">Int32</span></span>|<span data-ttu-id="0af0b-123">挂起设备的数量</span><span class="sxs-lookup"><span data-stu-id="0af0b-123">Number of pending devices</span></span>|
|<span data-ttu-id="0af0b-124">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="0af0b-124">notApplicableCount</span></span>|<span data-ttu-id="0af0b-125">Int32</span><span class="sxs-lookup"><span data-stu-id="0af0b-125">Int32</span></span>|<span data-ttu-id="0af0b-126">不适用设备的数量</span><span class="sxs-lookup"><span data-stu-id="0af0b-126">Number of not applicable devices</span></span>|
|<span data-ttu-id="0af0b-127">successCount</span><span class="sxs-lookup"><span data-stu-id="0af0b-127">successCount</span></span>|<span data-ttu-id="0af0b-128">Int32</span><span class="sxs-lookup"><span data-stu-id="0af0b-128">Int32</span></span>|<span data-ttu-id="0af0b-129">成功设备的数量</span><span class="sxs-lookup"><span data-stu-id="0af0b-129">Number of succeeded devices</span></span>|
|<span data-ttu-id="0af0b-130">errorCount</span><span class="sxs-lookup"><span data-stu-id="0af0b-130">errorCount</span></span>|<span data-ttu-id="0af0b-131">Int32</span><span class="sxs-lookup"><span data-stu-id="0af0b-131">Int32</span></span>|<span data-ttu-id="0af0b-132">错误设备的数量</span><span class="sxs-lookup"><span data-stu-id="0af0b-132">Number of error devices</span></span>|
|<span data-ttu-id="0af0b-133">failedCount</span><span class="sxs-lookup"><span data-stu-id="0af0b-133">failedCount</span></span>|<span data-ttu-id="0af0b-134">Int32</span><span class="sxs-lookup"><span data-stu-id="0af0b-134">Int32</span></span>|<span data-ttu-id="0af0b-135">失败设备的数量</span><span class="sxs-lookup"><span data-stu-id="0af0b-135">Number of failed devices</span></span>|
|<span data-ttu-id="0af0b-136">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="0af0b-136">lastUpdateDateTime</span></span>|<span data-ttu-id="0af0b-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0af0b-137">DateTimeOffset</span></span>|<span data-ttu-id="0af0b-138">上次更新时间</span><span class="sxs-lookup"><span data-stu-id="0af0b-138">Last update time</span></span>|
|<span data-ttu-id="0af0b-139">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="0af0b-139">configurationVersion</span></span>|<span data-ttu-id="0af0b-140">Int32</span><span class="sxs-lookup"><span data-stu-id="0af0b-140">Int32</span></span>|<span data-ttu-id="0af0b-141">用于此概述的策略版本</span><span class="sxs-lookup"><span data-stu-id="0af0b-141">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="0af0b-142">关系</span><span class="sxs-lookup"><span data-stu-id="0af0b-142">Relationships</span></span>
<span data-ttu-id="0af0b-143">无</span><span class="sxs-lookup"><span data-stu-id="0af0b-143">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="0af0b-144">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0af0b-144">JSON Representation</span></span>
<span data-ttu-id="0af0b-145">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0af0b-145">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id",
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









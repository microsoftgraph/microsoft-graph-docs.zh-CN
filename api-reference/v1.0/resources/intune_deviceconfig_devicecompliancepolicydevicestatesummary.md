# <a name="devicecompliancepolicydevicestatesummary-resource-type"></a><span data-ttu-id="f5737-101">deviceCompliancePolicyDeviceStateSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="f5737-101">deviceCompliancePolicyDeviceStateSummary resource type</span></span>

> <span data-ttu-id="f5737-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="f5737-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f5737-103">尚未记录</span><span class="sxs-lookup"><span data-stu-id="f5737-103">Not yet documented</span></span>
## <a name="methods"></a><span data-ttu-id="f5737-104">方法</span><span class="sxs-lookup"><span data-stu-id="f5737-104">Methods</span></span>
|<span data-ttu-id="f5737-105">方法</span><span class="sxs-lookup"><span data-stu-id="f5737-105">Method</span></span>|<span data-ttu-id="f5737-106">返回类型</span><span class="sxs-lookup"><span data-stu-id="f5737-106">Return Type</span></span>|<span data-ttu-id="f5737-107">说明</span><span class="sxs-lookup"><span data-stu-id="f5737-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f5737-108">获取 deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="f5737-108">Get deviceCompliancePolicyDeviceStateSummary</span></span>](../api/intune_deviceconfig_devicecompliancepolicydevicestatesummary_get.md)|[<span data-ttu-id="f5737-109">deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="f5737-109">deviceCompliancePolicyDeviceStateSummary</span></span>](../resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary.md)|<span data-ttu-id="f5737-110">读取 [deviceCompliancePolicyDeviceStateSummary](../resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f5737-110">Read properties and relationships of [plannerTaskDetails](../resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary.md) object.</span></span>|
|[<span data-ttu-id="f5737-111">更新 deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="f5737-111">Update deviceCompliancePolicyDeviceStateSummary</span></span>](../api/intune_deviceconfig_devicecompliancepolicydevicestatesummary_update.md)|[<span data-ttu-id="f5737-112">deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="f5737-112">deviceCompliancePolicyDeviceStateSummary</span></span>](../resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary.md)|<span data-ttu-id="f5737-113">更新 [deviceCompliancePolicyDeviceStateSummary](../resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="f5737-113">Update the properties of a [calendar](../resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="f5737-114">属性</span><span class="sxs-lookup"><span data-stu-id="f5737-114">Properties</span></span>
|<span data-ttu-id="f5737-115">属性</span><span class="sxs-lookup"><span data-stu-id="f5737-115">Property</span></span>|<span data-ttu-id="f5737-116">类型</span><span class="sxs-lookup"><span data-stu-id="f5737-116">Type</span></span>|<span data-ttu-id="f5737-117">说明</span><span class="sxs-lookup"><span data-stu-id="f5737-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f5737-118">inGracePeriodCount</span><span class="sxs-lookup"><span data-stu-id="f5737-118">inGracePeriodCount</span></span>|<span data-ttu-id="f5737-119">Int32</span><span class="sxs-lookup"><span data-stu-id="f5737-119">Int32</span></span>|<span data-ttu-id="f5737-120">宽限期内的设备数</span><span class="sxs-lookup"><span data-stu-id="f5737-120">Number of devices that are in grace period</span></span>|
|<span data-ttu-id="f5737-121">configManagerCount</span><span class="sxs-lookup"><span data-stu-id="f5737-121">configManagerCount</span></span>|<span data-ttu-id="f5737-122">Int32</span><span class="sxs-lookup"><span data-stu-id="f5737-122">Int32</span></span>|<span data-ttu-id="f5737-123">由 System Center Configuration Manager 管理合规性的设备数</span><span class="sxs-lookup"><span data-stu-id="f5737-123">Number of devices that have compliance managed by System Center Configuration Manager</span></span>|
|<span data-ttu-id="f5737-124">id</span><span class="sxs-lookup"><span data-stu-id="f5737-124">id</span></span>|<span data-ttu-id="f5737-125">String</span><span class="sxs-lookup"><span data-stu-id="f5737-125">String</span></span>|<span data-ttu-id="f5737-126">实体的键。</span><span class="sxs-lookup"><span data-stu-id="f5737-126">Key of the setting.</span></span>|
|<span data-ttu-id="f5737-127">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f5737-127">unknownDeviceCount</span></span>|<span data-ttu-id="f5737-128">Int32</span><span class="sxs-lookup"><span data-stu-id="f5737-128">Int32</span></span>|<span data-ttu-id="f5737-129">未知设备的数量</span><span class="sxs-lookup"><span data-stu-id="f5737-129">Number of unknown devices</span></span>|
|<span data-ttu-id="f5737-130">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f5737-130">notApplicableDeviceCount</span></span>|<span data-ttu-id="f5737-131">Int32</span><span class="sxs-lookup"><span data-stu-id="f5737-131">Int32</span></span>|<span data-ttu-id="f5737-132">不适用设备的数量</span><span class="sxs-lookup"><span data-stu-id="f5737-132">Number of not applicable devices</span></span>|
|<span data-ttu-id="f5737-133">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f5737-133">compliantDeviceCount</span></span>|<span data-ttu-id="f5737-134">Int32</span><span class="sxs-lookup"><span data-stu-id="f5737-134">Int32</span></span>|<span data-ttu-id="f5737-135">兼容设备的数量</span><span class="sxs-lookup"><span data-stu-id="f5737-135">Number of compliant devices</span></span>|
|<span data-ttu-id="f5737-136">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f5737-136">remediatedDeviceCount</span></span>|<span data-ttu-id="f5737-137">Int32</span><span class="sxs-lookup"><span data-stu-id="f5737-137">Int32</span></span>|<span data-ttu-id="f5737-138">已修复设备数</span><span class="sxs-lookup"><span data-stu-id="f5737-138">Number of remediated devices</span></span>|
|<span data-ttu-id="f5737-139">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f5737-139">nonCompliantDeviceCount</span></span>|<span data-ttu-id="f5737-140">Int32</span><span class="sxs-lookup"><span data-stu-id="f5737-140">Int32</span></span>|<span data-ttu-id="f5737-141">不兼容设备的数量</span><span class="sxs-lookup"><span data-stu-id="f5737-141">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="f5737-142">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f5737-142">errorDeviceCount</span></span>|<span data-ttu-id="f5737-143">Int32</span><span class="sxs-lookup"><span data-stu-id="f5737-143">Int32</span></span>|<span data-ttu-id="f5737-144">错误设备的数量</span><span class="sxs-lookup"><span data-stu-id="f5737-144">Number of error devices</span></span>|
|<span data-ttu-id="f5737-145">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f5737-145">conflictDeviceCount</span></span>|<span data-ttu-id="f5737-146">Int32</span><span class="sxs-lookup"><span data-stu-id="f5737-146">Int32</span></span>|<span data-ttu-id="f5737-147">冲突设备的数量</span><span class="sxs-lookup"><span data-stu-id="f5737-147">Number of conflict devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="f5737-148">关系</span><span class="sxs-lookup"><span data-stu-id="f5737-148">Relationships</span></span>
<span data-ttu-id="f5737-149">无</span><span class="sxs-lookup"><span data-stu-id="f5737-149">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f5737-150">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f5737-150">JSON Representation</span></span>
<span data-ttu-id="f5737-151">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f5737-151">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceCompliancePolicyDeviceStateSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyDeviceStateSummary",
  "inGracePeriodCount": 1024,
  "configManagerCount": 1024,
  "id": "String (identifier)",
  "unknownDeviceCount": 1024,
  "notApplicableDeviceCount": 1024,
  "compliantDeviceCount": 1024,
  "remediatedDeviceCount": 1024,
  "nonCompliantDeviceCount": 1024,
  "errorDeviceCount": 1024,
  "conflictDeviceCount": 1024
}
```




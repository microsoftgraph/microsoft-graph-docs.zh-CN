# <a name="devicecompliancepolicydevicestatesummary-resource-type"></a><span data-ttu-id="1786c-101">deviceCompliancePolicyDeviceStateSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="1786c-101">deviceCompliancePolicyDeviceStateSummary resource type</span></span>

> <span data-ttu-id="1786c-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="1786c-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1786c-103">尚未记录</span><span class="sxs-lookup"><span data-stu-id="1786c-103">Not yet documented</span></span>
## <a name="methods"></a><span data-ttu-id="1786c-104">方法</span><span class="sxs-lookup"><span data-stu-id="1786c-104">Methods</span></span>
|<span data-ttu-id="1786c-105">方法</span><span class="sxs-lookup"><span data-stu-id="1786c-105">Method</span></span>|<span data-ttu-id="1786c-106">返回类型</span><span class="sxs-lookup"><span data-stu-id="1786c-106">Return Type</span></span>|<span data-ttu-id="1786c-107">说明</span><span class="sxs-lookup"><span data-stu-id="1786c-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="1786c-108">获取 deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="1786c-108">Get deviceCompliancePolicyDeviceStateSummary</span></span>](../api/intune_deviceconfig_devicecompliancepolicydevicestatesummary_get.md)|[<span data-ttu-id="1786c-109">deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="1786c-109">deviceCompliancePolicyDeviceStateSummary</span></span>](../resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary.md)|<span data-ttu-id="1786c-110">读取 [deviceCompliancePolicyDeviceStateSummary](../resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="1786c-110">Read properties and relationships of the [deviceCompliancePolicyDeviceStateSummary](../resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary.md) object.</span></span>|
|[<span data-ttu-id="1786c-111">更新 deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="1786c-111">Update deviceCompliancePolicyDeviceStateSummary</span></span>](../api/intune_deviceconfig_devicecompliancepolicydevicestatesummary_update.md)|[<span data-ttu-id="1786c-112">deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="1786c-112">deviceCompliancePolicyDeviceStateSummary</span></span>](../resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary.md)|<span data-ttu-id="1786c-113">更新 [deviceCompliancePolicyDeviceStateSummary](../resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="1786c-113">Update the properties of a [deviceCompliancePolicyDeviceStateSummary](../resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="1786c-114">属性</span><span class="sxs-lookup"><span data-stu-id="1786c-114">Properties</span></span>
|<span data-ttu-id="1786c-115">属性</span><span class="sxs-lookup"><span data-stu-id="1786c-115">Property</span></span>|<span data-ttu-id="1786c-116">类型</span><span class="sxs-lookup"><span data-stu-id="1786c-116">Type</span></span>|<span data-ttu-id="1786c-117">说明</span><span class="sxs-lookup"><span data-stu-id="1786c-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1786c-118">inGracePeriodCount</span><span class="sxs-lookup"><span data-stu-id="1786c-118">inGracePeriodCount</span></span>|<span data-ttu-id="1786c-119">Int32</span><span class="sxs-lookup"><span data-stu-id="1786c-119">Int32</span></span>|<span data-ttu-id="1786c-120">宽限期内的设备数</span><span class="sxs-lookup"><span data-stu-id="1786c-120">Number of devices that are in grace period</span></span>|
|<span data-ttu-id="1786c-121">configManagerCount</span><span class="sxs-lookup"><span data-stu-id="1786c-121">configManagerCount</span></span>|<span data-ttu-id="1786c-122">Int32</span><span class="sxs-lookup"><span data-stu-id="1786c-122">Int32</span></span>|<span data-ttu-id="1786c-123">由 System Center Configuration Manager 管理符合性的设备数</span><span class="sxs-lookup"><span data-stu-id="1786c-123">Number of devices that have compliance managed by System Center Configuration Manager</span></span>|
|<span data-ttu-id="1786c-124">id</span><span class="sxs-lookup"><span data-stu-id="1786c-124">id</span></span>|<span data-ttu-id="1786c-125">字符串</span><span class="sxs-lookup"><span data-stu-id="1786c-125">String</span></span>|<span data-ttu-id="1786c-126">实体的键。</span><span class="sxs-lookup"><span data-stu-id="1786c-126">Key of the entity.</span></span>|
|<span data-ttu-id="1786c-127">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1786c-127">unknownDeviceCount</span></span>|<span data-ttu-id="1786c-128">Int32</span><span class="sxs-lookup"><span data-stu-id="1786c-128">Int32</span></span>|<span data-ttu-id="1786c-129">未知设备的数量</span><span class="sxs-lookup"><span data-stu-id="1786c-129">Number of unknown devices</span></span>|
|<span data-ttu-id="1786c-130">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1786c-130">notApplicableDeviceCount</span></span>|<span data-ttu-id="1786c-131">Int32</span><span class="sxs-lookup"><span data-stu-id="1786c-131">Int32</span></span>|<span data-ttu-id="1786c-132">不适用设备的数量</span><span class="sxs-lookup"><span data-stu-id="1786c-132">Number of not applicable devices</span></span>|
|<span data-ttu-id="1786c-133">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1786c-133">compliantDeviceCount</span></span>|<span data-ttu-id="1786c-134">Int32</span><span class="sxs-lookup"><span data-stu-id="1786c-134">Int32</span></span>|<span data-ttu-id="1786c-135">兼容设备的数量</span><span class="sxs-lookup"><span data-stu-id="1786c-135">Number of compliant devices</span></span>|
|<span data-ttu-id="1786c-136">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1786c-136">remediatedDeviceCount</span></span>|<span data-ttu-id="1786c-137">Int32</span><span class="sxs-lookup"><span data-stu-id="1786c-137">Int32</span></span>|<span data-ttu-id="1786c-138">已修复设备的数量</span><span class="sxs-lookup"><span data-stu-id="1786c-138">Number of remediated devices</span></span>|
|<span data-ttu-id="1786c-139">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1786c-139">nonCompliantDeviceCount</span></span>|<span data-ttu-id="1786c-140">Int32</span><span class="sxs-lookup"><span data-stu-id="1786c-140">Int32</span></span>|<span data-ttu-id="1786c-141">不兼容设备的数量</span><span class="sxs-lookup"><span data-stu-id="1786c-141">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="1786c-142">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1786c-142">errorDeviceCount</span></span>|<span data-ttu-id="1786c-143">Int32</span><span class="sxs-lookup"><span data-stu-id="1786c-143">Int32</span></span>|<span data-ttu-id="1786c-144">错误设备的数量</span><span class="sxs-lookup"><span data-stu-id="1786c-144">Number of error devices</span></span>|
|<span data-ttu-id="1786c-145">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1786c-145">conflictDeviceCount</span></span>|<span data-ttu-id="1786c-146">Int32</span><span class="sxs-lookup"><span data-stu-id="1786c-146">Int32</span></span>|<span data-ttu-id="1786c-147">冲突设备的数量</span><span class="sxs-lookup"><span data-stu-id="1786c-147">Number of conflict devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="1786c-148">关系</span><span class="sxs-lookup"><span data-stu-id="1786c-148">Relationships</span></span>
<span data-ttu-id="1786c-149">无</span><span class="sxs-lookup"><span data-stu-id="1786c-149">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="1786c-150">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1786c-150">JSON Representation</span></span>
<span data-ttu-id="1786c-151">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1786c-151">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.deviceCompliancePolicyDeviceStateSummary"
}-->
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




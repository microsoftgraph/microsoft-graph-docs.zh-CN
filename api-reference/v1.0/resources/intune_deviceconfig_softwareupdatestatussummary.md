# <a name="softwareupdatestatussummary-resource-type"></a><span data-ttu-id="b0cdc-101">softwareUpdateStatusSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="b0cdc-101">softwareUpdateStatusSummary resource type</span></span>

> <span data-ttu-id="b0cdc-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="b0cdc-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b0cdc-103">尚未记录</span><span class="sxs-lookup"><span data-stu-id="b0cdc-103">Not yet documented</span></span>
## <a name="methods"></a><span data-ttu-id="b0cdc-104">方法</span><span class="sxs-lookup"><span data-stu-id="b0cdc-104">Methods</span></span>
|<span data-ttu-id="b0cdc-105">方法</span><span class="sxs-lookup"><span data-stu-id="b0cdc-105">Method</span></span>|<span data-ttu-id="b0cdc-106">返回类型</span><span class="sxs-lookup"><span data-stu-id="b0cdc-106">Return Type</span></span>|<span data-ttu-id="b0cdc-107">说明</span><span class="sxs-lookup"><span data-stu-id="b0cdc-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b0cdc-108">获取 softwareUpdateStatusSummary</span><span class="sxs-lookup"><span data-stu-id="b0cdc-108">Get softwareUpdateStatusSummary</span></span>](../api/intune_deviceconfig_softwareupdatestatussummary_get.md)|[<span data-ttu-id="b0cdc-109">softwareUpdateStatusSummary</span><span class="sxs-lookup"><span data-stu-id="b0cdc-109">softwareUpdateStatusSummary</span></span>](../resources/intune_deviceconfig_softwareupdatestatussummary.md)|<span data-ttu-id="b0cdc-110">读取 [softwareUpdateStatusSummary](../resources/intune_deviceconfig_softwareupdatestatussummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b0cdc-110">Read properties and relationships of the [softwareUpdateStatusSummary](../resources/intune_deviceconfig_softwareupdatestatussummary.md) object.</span></span>|
|[<span data-ttu-id="b0cdc-111">更新 softwareUpdateStatusSummary</span><span class="sxs-lookup"><span data-stu-id="b0cdc-111">Update softwareUpdateStatusSummary</span></span>](../api/intune_deviceconfig_softwareupdatestatussummary_update.md)|[<span data-ttu-id="b0cdc-112">softwareUpdateStatusSummary</span><span class="sxs-lookup"><span data-stu-id="b0cdc-112">softwareUpdateStatusSummary</span></span>](../resources/intune_deviceconfig_softwareupdatestatussummary.md)|<span data-ttu-id="b0cdc-113">更新 [softwareUpdateStatusSummary](../resources/intune_deviceconfig_softwareupdatestatussummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b0cdc-113">Update the properties of a [softwareUpdateStatusSummary](../resources/intune_deviceconfig_softwareupdatestatussummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b0cdc-114">属性</span><span class="sxs-lookup"><span data-stu-id="b0cdc-114">Properties</span></span>
|<span data-ttu-id="b0cdc-115">属性</span><span class="sxs-lookup"><span data-stu-id="b0cdc-115">Property</span></span>|<span data-ttu-id="b0cdc-116">类型</span><span class="sxs-lookup"><span data-stu-id="b0cdc-116">Type</span></span>|<span data-ttu-id="b0cdc-117">说明</span><span class="sxs-lookup"><span data-stu-id="b0cdc-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b0cdc-118">ID</span><span class="sxs-lookup"><span data-stu-id="b0cdc-118">id</span></span>|<span data-ttu-id="b0cdc-119">字符串</span><span class="sxs-lookup"><span data-stu-id="b0cdc-119">String</span></span>|<span data-ttu-id="b0cdc-120">实体的键。</span><span class="sxs-lookup"><span data-stu-id="b0cdc-120">Key of the entity.</span></span>|
|<span data-ttu-id="b0cdc-121">displayName</span><span class="sxs-lookup"><span data-stu-id="b0cdc-121">displayName</span></span>|<span data-ttu-id="b0cdc-122">字符串</span><span class="sxs-lookup"><span data-stu-id="b0cdc-122">String</span></span>|<span data-ttu-id="b0cdc-123">策略的名称。</span><span class="sxs-lookup"><span data-stu-id="b0cdc-123">The name of the policy.</span></span>|
|<span data-ttu-id="b0cdc-124">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b0cdc-124">compliantDeviceCount</span></span>|<span data-ttu-id="b0cdc-125">Int32</span><span class="sxs-lookup"><span data-stu-id="b0cdc-125">Int32</span></span>|<span data-ttu-id="b0cdc-126">兼容设备的数量。</span><span class="sxs-lookup"><span data-stu-id="b0cdc-126">Number of compliant devices.</span></span>|
|<span data-ttu-id="b0cdc-127">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b0cdc-127">nonCompliantDeviceCount</span></span>|<span data-ttu-id="b0cdc-128">Int32</span><span class="sxs-lookup"><span data-stu-id="b0cdc-128">Int32</span></span>|<span data-ttu-id="b0cdc-129">不兼容设备的数量。</span><span class="sxs-lookup"><span data-stu-id="b0cdc-129">Number of non compliant devices.</span></span>|
|<span data-ttu-id="b0cdc-130">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b0cdc-130">remediatedDeviceCount</span></span>|<span data-ttu-id="b0cdc-131">Int32</span><span class="sxs-lookup"><span data-stu-id="b0cdc-131">Int32</span></span>|<span data-ttu-id="b0cdc-132">已修复设备的数量。</span><span class="sxs-lookup"><span data-stu-id="b0cdc-132">Number of remediated devices.</span></span>|
|<span data-ttu-id="b0cdc-133">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b0cdc-133">errorDeviceCount</span></span>|<span data-ttu-id="b0cdc-134">Int32</span><span class="sxs-lookup"><span data-stu-id="b0cdc-134">Int32</span></span>|<span data-ttu-id="b0cdc-135">出现错误的设备数量。</span><span class="sxs-lookup"><span data-stu-id="b0cdc-135">Number of devices had error.</span></span>|
|<span data-ttu-id="b0cdc-136">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b0cdc-136">unknownDeviceCount</span></span>|<span data-ttu-id="b0cdc-137">Int32</span><span class="sxs-lookup"><span data-stu-id="b0cdc-137">Int32</span></span>|<span data-ttu-id="b0cdc-138">未知设备的数量。</span><span class="sxs-lookup"><span data-stu-id="b0cdc-138">Number of unknown devices.</span></span>|
|<span data-ttu-id="b0cdc-139">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b0cdc-139">conflictDeviceCount</span></span>|<span data-ttu-id="b0cdc-140">Int32</span><span class="sxs-lookup"><span data-stu-id="b0cdc-140">Int32</span></span>|<span data-ttu-id="b0cdc-141">冲突设备的数量。</span><span class="sxs-lookup"><span data-stu-id="b0cdc-141">Number of conflict devices.</span></span>|
|<span data-ttu-id="b0cdc-142">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b0cdc-142">notApplicableDeviceCount</span></span>|<span data-ttu-id="b0cdc-143">Int32</span><span class="sxs-lookup"><span data-stu-id="b0cdc-143">Int32</span></span>|<span data-ttu-id="b0cdc-144">不适用设备的数量。</span><span class="sxs-lookup"><span data-stu-id="b0cdc-144">Number of not applicable devices.</span></span>|
|<span data-ttu-id="b0cdc-145">compliantUserCount</span><span class="sxs-lookup"><span data-stu-id="b0cdc-145">compliantUserCount</span></span>|<span data-ttu-id="b0cdc-146">Int32</span><span class="sxs-lookup"><span data-stu-id="b0cdc-146">Int32</span></span>|<span data-ttu-id="b0cdc-147">兼容用户的数量。</span><span class="sxs-lookup"><span data-stu-id="b0cdc-147">Number of compliant users.</span></span>|
|<span data-ttu-id="b0cdc-148">nonCompliantUserCount</span><span class="sxs-lookup"><span data-stu-id="b0cdc-148">nonCompliantUserCount</span></span>|<span data-ttu-id="b0cdc-149">Int32</span><span class="sxs-lookup"><span data-stu-id="b0cdc-149">Int32</span></span>|<span data-ttu-id="b0cdc-150">不兼容用户的数量。</span><span class="sxs-lookup"><span data-stu-id="b0cdc-150">Number of non compliant users.</span></span>|
|<span data-ttu-id="b0cdc-151">remediatedUserCount</span><span class="sxs-lookup"><span data-stu-id="b0cdc-151">remediatedUserCount</span></span>|<span data-ttu-id="b0cdc-152">Int32</span><span class="sxs-lookup"><span data-stu-id="b0cdc-152">Int32</span></span>|<span data-ttu-id="b0cdc-153">已修复用户的数量。</span><span class="sxs-lookup"><span data-stu-id="b0cdc-153">Number of remediated users.</span></span>|
|<span data-ttu-id="b0cdc-154">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="b0cdc-154">errorUserCount</span></span>|<span data-ttu-id="b0cdc-155">Int32</span><span class="sxs-lookup"><span data-stu-id="b0cdc-155">Int32</span></span>|<span data-ttu-id="b0cdc-156">出现错误的用户数量。</span><span class="sxs-lookup"><span data-stu-id="b0cdc-156">Number of users had error.</span></span>|
|<span data-ttu-id="b0cdc-157">unknownUserCount</span><span class="sxs-lookup"><span data-stu-id="b0cdc-157">unknownUserCount</span></span>|<span data-ttu-id="b0cdc-158">Int32</span><span class="sxs-lookup"><span data-stu-id="b0cdc-158">Int32</span></span>|<span data-ttu-id="b0cdc-159">未知用户的数量。</span><span class="sxs-lookup"><span data-stu-id="b0cdc-159">Number of unknown users.</span></span>|
|<span data-ttu-id="b0cdc-160">conflictUserCount</span><span class="sxs-lookup"><span data-stu-id="b0cdc-160">conflictUserCount</span></span>|<span data-ttu-id="b0cdc-161">Int32</span><span class="sxs-lookup"><span data-stu-id="b0cdc-161">Int32</span></span>|<span data-ttu-id="b0cdc-162">冲突用户的数量。</span><span class="sxs-lookup"><span data-stu-id="b0cdc-162">Number of conflict users.</span></span>|
|<span data-ttu-id="b0cdc-163">notApplicableUserCount</span><span class="sxs-lookup"><span data-stu-id="b0cdc-163">notApplicableUserCount</span></span>|<span data-ttu-id="b0cdc-164">Int32</span><span class="sxs-lookup"><span data-stu-id="b0cdc-164">Int32</span></span>|<span data-ttu-id="b0cdc-165">不适用用户的数量。</span><span class="sxs-lookup"><span data-stu-id="b0cdc-165">Number of not applicable users.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b0cdc-166">关系</span><span class="sxs-lookup"><span data-stu-id="b0cdc-166">Relationships</span></span>
<span data-ttu-id="b0cdc-167">无</span><span class="sxs-lookup"><span data-stu-id="b0cdc-167">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b0cdc-168">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b0cdc-168">JSON Representation</span></span>
<span data-ttu-id="b0cdc-169">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b0cdc-169">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.softwareUpdateStatusSummary"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.softwareUpdateStatusSummary",
  "id": "String (identifier)",
  "displayName": "String",
  "compliantDeviceCount": 1024,
  "nonCompliantDeviceCount": 1024,
  "remediatedDeviceCount": 1024,
  "errorDeviceCount": 1024,
  "unknownDeviceCount": 1024,
  "conflictDeviceCount": 1024,
  "notApplicableDeviceCount": 1024,
  "compliantUserCount": 1024,
  "nonCompliantUserCount": 1024,
  "remediatedUserCount": 1024,
  "errorUserCount": 1024,
  "unknownUserCount": 1024,
  "conflictUserCount": 1024,
  "notApplicableUserCount": 1024
}
```









# <a name="softwareupdatestatussummary-resource-type"></a><span data-ttu-id="cf00b-101">softwareUpdateStatusSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="cf00b-101">softwareUpdateStatusSummary resource type</span></span>

> <span data-ttu-id="cf00b-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="cf00b-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cf00b-103">尚未记录</span><span class="sxs-lookup"><span data-stu-id="cf00b-103">Not yet documented</span></span>
## <a name="methods"></a><span data-ttu-id="cf00b-104">方法</span><span class="sxs-lookup"><span data-stu-id="cf00b-104">Methods</span></span>
|<span data-ttu-id="cf00b-105">方法</span><span class="sxs-lookup"><span data-stu-id="cf00b-105">Method</span></span>|<span data-ttu-id="cf00b-106">返回类型</span><span class="sxs-lookup"><span data-stu-id="cf00b-106">Return Type</span></span>|<span data-ttu-id="cf00b-107">说明</span><span class="sxs-lookup"><span data-stu-id="cf00b-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="cf00b-108">获取 softwareUpdateStatusSummary</span><span class="sxs-lookup"><span data-stu-id="cf00b-108">Get softwareUpdateStatusSummary</span></span>](../api/intune_deviceconfig_softwareupdatestatussummary_get.md)|[<span data-ttu-id="cf00b-109">softwareUpdateStatusSummary</span><span class="sxs-lookup"><span data-stu-id="cf00b-109">softwareUpdateStatusSummary</span></span>](../resources/intune_deviceconfig_softwareupdatestatussummary.md)|<span data-ttu-id="cf00b-110">读取 [softwareUpdateStatusSummary](../resources/intune_deviceconfig_softwareupdatestatussummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="cf00b-110">Read properties and relationships of [plannerProgressTaskBoardTaskFormat](../resources/intune_deviceconfig_softwareupdatestatussummary.md) object.</span></span>|
|[<span data-ttu-id="cf00b-111">更新 softwareUpdateStatusSummary</span><span class="sxs-lookup"><span data-stu-id="cf00b-111">Update softwareUpdateStatusSummary</span></span>](../api/intune_deviceconfig_softwareupdatestatussummary_update.md)|[<span data-ttu-id="cf00b-112">softwareUpdateStatusSummary</span><span class="sxs-lookup"><span data-stu-id="cf00b-112">softwareUpdateStatusSummary</span></span>](../resources/intune_deviceconfig_softwareupdatestatussummary.md)|<span data-ttu-id="cf00b-113">更新 [softwareUpdateStatusSummary](../resources/intune_deviceconfig_softwareupdatestatussummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="cf00b-113">Update the properties of a [calendar](../resources/intune_deviceconfig_softwareupdatestatussummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="cf00b-114">属性</span><span class="sxs-lookup"><span data-stu-id="cf00b-114">Properties</span></span>
|<span data-ttu-id="cf00b-115">属性</span><span class="sxs-lookup"><span data-stu-id="cf00b-115">Property</span></span>|<span data-ttu-id="cf00b-116">类型</span><span class="sxs-lookup"><span data-stu-id="cf00b-116">Type</span></span>|<span data-ttu-id="cf00b-117">说明</span><span class="sxs-lookup"><span data-stu-id="cf00b-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cf00b-118">id</span><span class="sxs-lookup"><span data-stu-id="cf00b-118">id</span></span>|<span data-ttu-id="cf00b-119">String</span><span class="sxs-lookup"><span data-stu-id="cf00b-119">String</span></span>|<span data-ttu-id="cf00b-120">实体的键。</span><span class="sxs-lookup"><span data-stu-id="cf00b-120">Key of the setting.</span></span>|
|<span data-ttu-id="cf00b-121">displayName</span><span class="sxs-lookup"><span data-stu-id="cf00b-121">displayName</span></span>|<span data-ttu-id="cf00b-122">String</span><span class="sxs-lookup"><span data-stu-id="cf00b-122">String</span></span>|<span data-ttu-id="cf00b-123">策略的名称。</span><span class="sxs-lookup"><span data-stu-id="cf00b-123">The name of the site policy to apply</span></span>|
|<span data-ttu-id="cf00b-124">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="cf00b-124">compliantDeviceCount</span></span>|<span data-ttu-id="cf00b-125">Int32</span><span class="sxs-lookup"><span data-stu-id="cf00b-125">Int32</span></span>|<span data-ttu-id="cf00b-126">兼容设备的数量。</span><span class="sxs-lookup"><span data-stu-id="cf00b-126">Number of compliant devices.</span></span>|
|<span data-ttu-id="cf00b-127">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="cf00b-127">nonCompliantDeviceCount</span></span>|<span data-ttu-id="cf00b-128">Int32</span><span class="sxs-lookup"><span data-stu-id="cf00b-128">Int32</span></span>|<span data-ttu-id="cf00b-129">不兼容设备的数量。</span><span class="sxs-lookup"><span data-stu-id="cf00b-129">Number of non compliant devices.</span></span>|
|<span data-ttu-id="cf00b-130">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="cf00b-130">remediatedDeviceCount</span></span>|<span data-ttu-id="cf00b-131">Int32</span><span class="sxs-lookup"><span data-stu-id="cf00b-131">Int32</span></span>|<span data-ttu-id="cf00b-132">已修复设备的数量。</span><span class="sxs-lookup"><span data-stu-id="cf00b-132">Number of remediated devices.</span></span>|
|<span data-ttu-id="cf00b-133">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="cf00b-133">errorDeviceCount</span></span>|<span data-ttu-id="cf00b-134">Int32</span><span class="sxs-lookup"><span data-stu-id="cf00b-134">Int32</span></span>|<span data-ttu-id="cf00b-135">出现错误的设备数量。</span><span class="sxs-lookup"><span data-stu-id="cf00b-135">Number of devices had error.</span></span>|
|<span data-ttu-id="cf00b-136">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="cf00b-136">unknownDeviceCount</span></span>|<span data-ttu-id="cf00b-137">Int32</span><span class="sxs-lookup"><span data-stu-id="cf00b-137">Int32</span></span>|<span data-ttu-id="cf00b-138">未知设备的数量。</span><span class="sxs-lookup"><span data-stu-id="cf00b-138">Number of unknown devices.</span></span>|
|<span data-ttu-id="cf00b-139">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="cf00b-139">conflictDeviceCount</span></span>|<span data-ttu-id="cf00b-140">Int32</span><span class="sxs-lookup"><span data-stu-id="cf00b-140">Int32</span></span>|<span data-ttu-id="cf00b-141">冲突设备的数量。</span><span class="sxs-lookup"><span data-stu-id="cf00b-141">Number of conflict devices.</span></span>|
|<span data-ttu-id="cf00b-142">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="cf00b-142">notApplicableDeviceCount</span></span>|<span data-ttu-id="cf00b-143">Int32</span><span class="sxs-lookup"><span data-stu-id="cf00b-143">Int32</span></span>|<span data-ttu-id="cf00b-144">不适用设备的数量。</span><span class="sxs-lookup"><span data-stu-id="cf00b-144">Number of not applicable devices.</span></span>|
|<span data-ttu-id="cf00b-145">compliantUserCount</span><span class="sxs-lookup"><span data-stu-id="cf00b-145">compliantUserCount</span></span>|<span data-ttu-id="cf00b-146">Int32</span><span class="sxs-lookup"><span data-stu-id="cf00b-146">Int32</span></span>|<span data-ttu-id="cf00b-147">兼容用户的数量。</span><span class="sxs-lookup"><span data-stu-id="cf00b-147">Number of users: 542</span></span>|
|<span data-ttu-id="cf00b-148">nonCompliantUserCount</span><span class="sxs-lookup"><span data-stu-id="cf00b-148">nonCompliantUserCount</span></span>|<span data-ttu-id="cf00b-149">Int32</span><span class="sxs-lookup"><span data-stu-id="cf00b-149">Int32</span></span>|<span data-ttu-id="cf00b-150">不兼容用户的数量。</span><span class="sxs-lookup"><span data-stu-id="cf00b-150">Number of non compliant users.</span></span>|
|<span data-ttu-id="cf00b-151">remediatedUserCount</span><span class="sxs-lookup"><span data-stu-id="cf00b-151">remediatedUserCount</span></span>|<span data-ttu-id="cf00b-152">Int32</span><span class="sxs-lookup"><span data-stu-id="cf00b-152">Int32</span></span>|<span data-ttu-id="cf00b-153">已修复用户的数量。</span><span class="sxs-lookup"><span data-stu-id="cf00b-153">Number of users: 542</span></span>|
|<span data-ttu-id="cf00b-154">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="cf00b-154">errorUserCount</span></span>|<span data-ttu-id="cf00b-155">Int32</span><span class="sxs-lookup"><span data-stu-id="cf00b-155">Int32</span></span>|<span data-ttu-id="cf00b-156">出现错误的用户数量。</span><span class="sxs-lookup"><span data-stu-id="cf00b-156">Number of users had error.</span></span>|
|<span data-ttu-id="cf00b-157">unknownUserCount</span><span class="sxs-lookup"><span data-stu-id="cf00b-157">unknownUserCount</span></span>|<span data-ttu-id="cf00b-158">Int32</span><span class="sxs-lookup"><span data-stu-id="cf00b-158">Int32</span></span>|<span data-ttu-id="cf00b-159">未知用户的数量。</span><span class="sxs-lookup"><span data-stu-id="cf00b-159">Number of users: 542</span></span>|
|<span data-ttu-id="cf00b-160">conflictUserCount</span><span class="sxs-lookup"><span data-stu-id="cf00b-160">conflictUserCount</span></span>|<span data-ttu-id="cf00b-161">Int32</span><span class="sxs-lookup"><span data-stu-id="cf00b-161">Int32</span></span>|<span data-ttu-id="cf00b-162">冲突用户的数量。</span><span class="sxs-lookup"><span data-stu-id="cf00b-162">Number of users: 542</span></span>|
|<span data-ttu-id="cf00b-163">notApplicableUserCount</span><span class="sxs-lookup"><span data-stu-id="cf00b-163">notApplicableUserCount</span></span>|<span data-ttu-id="cf00b-164">Int32</span><span class="sxs-lookup"><span data-stu-id="cf00b-164">Int32</span></span>|<span data-ttu-id="cf00b-165">不适用用户的数量。</span><span class="sxs-lookup"><span data-stu-id="cf00b-165">Number of not applicable users.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cf00b-166">关系</span><span class="sxs-lookup"><span data-stu-id="cf00b-166">Relationships</span></span>
<span data-ttu-id="cf00b-167">无</span><span class="sxs-lookup"><span data-stu-id="cf00b-167">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="cf00b-168">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cf00b-168">JSON Representation</span></span>
<span data-ttu-id="cf00b-169">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cf00b-169">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.softwareUpdateStatusSummary"
}
-->
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




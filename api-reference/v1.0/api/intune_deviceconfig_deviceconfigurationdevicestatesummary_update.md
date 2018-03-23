# <a name="update-deviceconfigurationdevicestatesummary"></a><span data-ttu-id="1d8b6-101">更新 deviceConfigurationDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="1d8b6-101">Update deviceConfigurationDeviceStateSummary</span></span>

> <span data-ttu-id="1d8b6-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="1d8b6-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1d8b6-103">更新 [deviceConfigurationDeviceStateSummary](../resources/intune_deviceconfig_deviceconfigurationdevicestatesummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="1d8b6-103">Update the properties of a [calendar](../resources/intune_deviceconfig_deviceconfigurationdevicestatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1d8b6-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="1d8b6-104">Prerequisites</span></span>
<span data-ttu-id="1d8b6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="1d8b6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="1d8b6-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="1d8b6-107">Permission type</span></span>|<span data-ttu-id="1d8b6-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="1d8b6-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1d8b6-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1d8b6-109">Delegated (work or school account)</span></span>|<span data-ttu-id="1d8b6-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1d8b6-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1d8b6-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1d8b6-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1d8b6-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="1d8b6-112">Not supported.</span></span>|
|<span data-ttu-id="1d8b6-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="1d8b6-113">Application</span></span>|<span data-ttu-id="1d8b6-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="1d8b6-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1d8b6-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1d8b6-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurationDeviceStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="1d8b6-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="1d8b6-116">Request headers</span></span>
|<span data-ttu-id="1d8b6-117">标头</span><span class="sxs-lookup"><span data-stu-id="1d8b6-117">Header</span></span>|<span data-ttu-id="1d8b6-118">值</span><span class="sxs-lookup"><span data-stu-id="1d8b6-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1d8b6-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="1d8b6-119">Authorization</span></span>|<span data-ttu-id="1d8b6-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="1d8b6-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="1d8b6-121">Accept</span><span class="sxs-lookup"><span data-stu-id="1d8b6-121">Accept</span></span>|<span data-ttu-id="1d8b6-122">application/json</span><span class="sxs-lookup"><span data-stu-id="1d8b6-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1d8b6-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="1d8b6-123">Request body</span></span>
<span data-ttu-id="1d8b6-124">在请求正文中，提供 [deviceConfigurationDeviceStateSummary](../resources/intune_deviceconfig_deviceconfigurationdevicestatesummary.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1d8b6-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_deviceconfig_deviceconfigurationdevicestatesummary.md) object.</span></span>

<span data-ttu-id="1d8b6-125">下表显示创建 [deviceConfigurationDeviceStateSummary](../resources/intune_deviceconfig_deviceconfigurationdevicestatesummary.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="1d8b6-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="1d8b6-126">属性</span><span class="sxs-lookup"><span data-stu-id="1d8b6-126">Property</span></span>|<span data-ttu-id="1d8b6-127">类型</span><span class="sxs-lookup"><span data-stu-id="1d8b6-127">Type</span></span>|<span data-ttu-id="1d8b6-128">说明</span><span class="sxs-lookup"><span data-stu-id="1d8b6-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1d8b6-129">id</span><span class="sxs-lookup"><span data-stu-id="1d8b6-129">id</span></span>|<span data-ttu-id="1d8b6-130">String</span><span class="sxs-lookup"><span data-stu-id="1d8b6-130">String</span></span>|<span data-ttu-id="1d8b6-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="1d8b6-131">Key of the setting.</span></span>|
|<span data-ttu-id="1d8b6-132">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1d8b6-132">unknownDeviceCount</span></span>|<span data-ttu-id="1d8b6-133">Int32</span><span class="sxs-lookup"><span data-stu-id="1d8b6-133">Int32</span></span>|<span data-ttu-id="1d8b6-134">未知设备的数量</span><span class="sxs-lookup"><span data-stu-id="1d8b6-134">Number of unknown devices</span></span>|
|<span data-ttu-id="1d8b6-135">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1d8b6-135">notApplicableDeviceCount</span></span>|<span data-ttu-id="1d8b6-136">Int32</span><span class="sxs-lookup"><span data-stu-id="1d8b6-136">Int32</span></span>|<span data-ttu-id="1d8b6-137">不适用设备的数量</span><span class="sxs-lookup"><span data-stu-id="1d8b6-137">Number of not applicable devices</span></span>|
|<span data-ttu-id="1d8b6-138">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1d8b6-138">compliantDeviceCount</span></span>|<span data-ttu-id="1d8b6-139">Int32</span><span class="sxs-lookup"><span data-stu-id="1d8b6-139">Int32</span></span>|<span data-ttu-id="1d8b6-140">兼容设备的数量</span><span class="sxs-lookup"><span data-stu-id="1d8b6-140">Number of compliant devices</span></span>|
|<span data-ttu-id="1d8b6-141">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1d8b6-141">remediatedDeviceCount</span></span>|<span data-ttu-id="1d8b6-142">Int32</span><span class="sxs-lookup"><span data-stu-id="1d8b6-142">Int32</span></span>|<span data-ttu-id="1d8b6-143">已修复设备的数量</span><span class="sxs-lookup"><span data-stu-id="1d8b6-143">Number of remediated devices</span></span>|
|<span data-ttu-id="1d8b6-144">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1d8b6-144">nonCompliantDeviceCount</span></span>|<span data-ttu-id="1d8b6-145">Int32</span><span class="sxs-lookup"><span data-stu-id="1d8b6-145">Int32</span></span>|<span data-ttu-id="1d8b6-146">不兼容设备的数量</span><span class="sxs-lookup"><span data-stu-id="1d8b6-146">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="1d8b6-147">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1d8b6-147">errorDeviceCount</span></span>|<span data-ttu-id="1d8b6-148">Int32</span><span class="sxs-lookup"><span data-stu-id="1d8b6-148">Int32</span></span>|<span data-ttu-id="1d8b6-149">错误设备的数量</span><span class="sxs-lookup"><span data-stu-id="1d8b6-149">Number of error devices</span></span>|
|<span data-ttu-id="1d8b6-150">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1d8b6-150">conflictDeviceCount</span></span>|<span data-ttu-id="1d8b6-151">Int32</span><span class="sxs-lookup"><span data-stu-id="1d8b6-151">Int32</span></span>|<span data-ttu-id="1d8b6-152">冲突设备的数量</span><span class="sxs-lookup"><span data-stu-id="1d8b6-152">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="1d8b6-153">响应</span><span class="sxs-lookup"><span data-stu-id="1d8b6-153">Response</span></span>
<span data-ttu-id="1d8b6-154">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [deviceConfigurationDeviceStateSummary](../resources/intune_deviceconfig_deviceconfigurationdevicestatesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1d8b6-154">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_deviceconfig_deviceconfigurationdevicestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1d8b6-155">示例</span><span class="sxs-lookup"><span data-stu-id="1d8b6-155">Example</span></span>
### <a name="request"></a><span data-ttu-id="1d8b6-156">请求</span><span class="sxs-lookup"><span data-stu-id="1d8b6-156">Request</span></span>
<span data-ttu-id="1d8b6-157">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1d8b6-157">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurationDeviceStateSummaries
Content-type: application/json
Content-length: 214

{
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```

### <a name="response"></a><span data-ttu-id="1d8b6-158">响应</span><span class="sxs-lookup"><span data-stu-id="1d8b6-158">Response</span></span>
<span data-ttu-id="1d8b6-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1d8b6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 339

{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceStateSummary",
  "id": "5db26f5a-6f5a-5db2-5a6f-b25d5a6fb25d",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```




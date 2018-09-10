# <a name="update-manageddeviceoverview"></a><span data-ttu-id="8798b-101">更新 managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="8798b-101">Update managedDeviceOverview</span></span>

> <span data-ttu-id="8798b-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="8798b-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8798b-103">更新 [managedDeviceOverview](../resources/intune_devices_manageddeviceoverview.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="8798b-103">Update the properties of a [managedDeviceOverview](../resources/intune_devices_manageddeviceoverview.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8798b-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="8798b-104">Prerequisites</span></span>
<span data-ttu-id="8798b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="8798b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="8798b-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="8798b-107">Permission type</span></span>|<span data-ttu-id="8798b-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="8798b-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8798b-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8798b-109">Delegated (work or school account)</span></span>|<span data-ttu-id="8798b-110">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8798b-110">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="8798b-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8798b-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8798b-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="8798b-112">Not supported.</span></span>|
|<span data-ttu-id="8798b-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="8798b-113">Application</span></span>|<span data-ttu-id="8798b-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="8798b-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8798b-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8798b-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managedDeviceOverview
```

## <a name="request-headers"></a><span data-ttu-id="8798b-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="8798b-116">Request headers</span></span>
|<span data-ttu-id="8798b-117">标头</span><span class="sxs-lookup"><span data-stu-id="8798b-117">Header</span></span>|<span data-ttu-id="8798b-118">值</span><span class="sxs-lookup"><span data-stu-id="8798b-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8798b-119">授权</span><span class="sxs-lookup"><span data-stu-id="8798b-119">Authorization</span></span>|<span data-ttu-id="8798b-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="8798b-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8798b-121">Accept</span><span class="sxs-lookup"><span data-stu-id="8798b-121">Accept</span></span>|<span data-ttu-id="8798b-122">application/json</span><span class="sxs-lookup"><span data-stu-id="8798b-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8798b-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="8798b-123">Request body</span></span>
<span data-ttu-id="8798b-124">在请求正文中，提供 [managedDeviceOverview](../resources/intune_devices_manageddeviceoverview.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8798b-124">In the request body, supply a JSON representation for the [managedDeviceOverview](../resources/intune_devices_manageddeviceoverview.md) object.</span></span>

<span data-ttu-id="8798b-125">下表显示创建 [managedDeviceOverview](../resources/intune_devices_manageddeviceoverview.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="8798b-125">The following table shows the properties that are required when you create the [managedDeviceOverview](../resources/intune_devices_manageddeviceoverview.md).</span></span>

|<span data-ttu-id="8798b-126">属性</span><span class="sxs-lookup"><span data-stu-id="8798b-126">Property</span></span>|<span data-ttu-id="8798b-127">类型</span><span class="sxs-lookup"><span data-stu-id="8798b-127">Type</span></span>|<span data-ttu-id="8798b-128">说明</span><span class="sxs-lookup"><span data-stu-id="8798b-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8798b-129">ID</span><span class="sxs-lookup"><span data-stu-id="8798b-129">id</span></span>|<span data-ttu-id="8798b-130">String</span><span class="sxs-lookup"><span data-stu-id="8798b-130">String</span></span>|<span data-ttu-id="8798b-131">摘要的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="8798b-131">Unique Identifier for the summary</span></span>|
|<span data-ttu-id="8798b-132">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8798b-132">enrolledDeviceCount</span></span>|<span data-ttu-id="8798b-133">Int32</span><span class="sxs-lookup"><span data-stu-id="8798b-133">Int32</span></span>|<span data-ttu-id="8798b-134">总注册设备计数。</span><span class="sxs-lookup"><span data-stu-id="8798b-134">Total enrolled device count.</span></span> <span data-ttu-id="8798b-135">不包括通过 Intune PC 代理管理的 PC 设备。</span><span class="sxs-lookup"><span data-stu-id="8798b-135">Does not include PC devices managed via Intune PC Agent</span></span>|
|<span data-ttu-id="8798b-136">mdmEnrolledCount</span><span class="sxs-lookup"><span data-stu-id="8798b-136">mdmEnrolledCount</span></span>|<span data-ttu-id="8798b-137">Int32</span><span class="sxs-lookup"><span data-stu-id="8798b-137">Int32</span></span>|<span data-ttu-id="8798b-138">MDM 中注册的设备数</span><span class="sxs-lookup"><span data-stu-id="8798b-138">The number of devices enrolled in MDM</span></span>|
|<span data-ttu-id="8798b-139">dualEnrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8798b-139">dualEnrolledDeviceCount</span></span>|<span data-ttu-id="8798b-140">Int32</span><span class="sxs-lookup"><span data-stu-id="8798b-140">Int32</span></span>|<span data-ttu-id="8798b-141">MDM 和 EAS 中注册的设备数</span><span class="sxs-lookup"><span data-stu-id="8798b-141">The number of devices enrolled in both MDM and EAS</span></span>|
|<span data-ttu-id="8798b-142">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="8798b-142">deviceOperatingSystemSummary</span></span>|[<span data-ttu-id="8798b-143">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="8798b-143">deviceOperatingSystemSummary</span></span>](../resources/intune_devices_deviceoperatingsystemsummary.md)|<span data-ttu-id="8798b-144">设备操作系统摘要。</span><span class="sxs-lookup"><span data-stu-id="8798b-144">Device operating system summary.</span></span>|
|<span data-ttu-id="8798b-145">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="8798b-145">deviceExchangeAccessStateSummary</span></span>|[<span data-ttu-id="8798b-146">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="8798b-146">deviceExchangeAccessStateSummary</span></span>](../resources/intune_devices_deviceexchangeaccessstatesummary.md)|<span data-ttu-id="8798b-147">Intune 中的 Exchange 访问状态的分配</span><span class="sxs-lookup"><span data-stu-id="8798b-147">Distribution of Exchange Access State in Intune</span></span>|



## <a name="response"></a><span data-ttu-id="8798b-148">响应</span><span class="sxs-lookup"><span data-stu-id="8798b-148">Response</span></span>
<span data-ttu-id="8798b-149">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [managedDeviceOverview](../resources/intune_devices_manageddeviceoverview.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8798b-149">If successful, this method returns a `200 OK` response code and an updated [managedDeviceOverview](../resources/intune_devices_manageddeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8798b-150">示例</span><span class="sxs-lookup"><span data-stu-id="8798b-150">Example</span></span>
### <a name="request"></a><span data-ttu-id="8798b-151">请求</span><span class="sxs-lookup"><span data-stu-id="8798b-151">Request</span></span>
<span data-ttu-id="8798b-152">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8798b-152">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/managedDeviceOverview
Content-type: application/json
Content-length: 625

{
  "enrolledDeviceCount": 3,
  "mdmEnrolledCount": 0,
  "dualEnrolledDeviceCount": 7,
  "deviceOperatingSystemSummary": {
    "@odata.type": "microsoft.graph.deviceOperatingSystemSummary",
    "androidCount": 12,
    "iosCount": 8,
    "macOSCount": 10,
    "windowsMobileCount": 2,
    "windowsCount": 12,
    "unknownCount": 12
  },
  "deviceExchangeAccessStateSummary": {
    "@odata.type": "microsoft.graph.deviceExchangeAccessStateSummary",
    "allowedDeviceCount": 2,
    "blockedDeviceCount": 2,
    "quarantinedDeviceCount": 6,
    "unknownDeviceCount": 2,
    "unavailableDeviceCount": 6
  }
}
```

### <a name="response"></a><span data-ttu-id="8798b-153">响应</span><span class="sxs-lookup"><span data-stu-id="8798b-153">Response</span></span>
<span data-ttu-id="8798b-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8798b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 734

{
  "@odata.type": "#microsoft.graph.managedDeviceOverview",
  "id": "42a91653-1653-42a9-5316-a9425316a942",
  "enrolledDeviceCount": 3,
  "mdmEnrolledCount": 0,
  "dualEnrolledDeviceCount": 7,
  "deviceOperatingSystemSummary": {
    "@odata.type": "microsoft.graph.deviceOperatingSystemSummary",
    "androidCount": 12,
    "iosCount": 8,
    "macOSCount": 10,
    "windowsMobileCount": 2,
    "windowsCount": 12,
    "unknownCount": 12
  },
  "deviceExchangeAccessStateSummary": {
    "@odata.type": "microsoft.graph.deviceExchangeAccessStateSummary",
    "allowedDeviceCount": 2,
    "blockedDeviceCount": 2,
    "quarantinedDeviceCount": 6,
    "unknownDeviceCount": 2,
    "unavailableDeviceCount": 6
  }
}
```









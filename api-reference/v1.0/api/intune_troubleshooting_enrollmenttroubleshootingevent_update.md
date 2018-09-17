# <a name="update-enrollmenttroubleshootingevent"></a><span data-ttu-id="c41c1-101">更新 enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="c41c1-101">Update enrollmentTroubleshootingEvent</span></span>

> <span data-ttu-id="c41c1-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="c41c1-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c41c1-103">更新 [enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="c41c1-103">Update the properties of a [enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c41c1-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="c41c1-104">Prerequisites</span></span>
<span data-ttu-id="c41c1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="c41c1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="c41c1-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="c41c1-107">Permission type</span></span>|<span data-ttu-id="c41c1-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c41c1-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c41c1-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c41c1-109">Delegated (work or school account)</span></span>|<span data-ttu-id="c41c1-110">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c41c1-110">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="c41c1-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c41c1-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c41c1-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="c41c1-112">Not supported.</span></span>|
|<span data-ttu-id="c41c1-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="c41c1-113">Application</span></span>|<span data-ttu-id="c41c1-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="c41c1-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c41c1-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c41c1-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="c41c1-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="c41c1-116">Request headers</span></span>
|<span data-ttu-id="c41c1-117">标头</span><span class="sxs-lookup"><span data-stu-id="c41c1-117">Header</span></span>|<span data-ttu-id="c41c1-118">值</span><span class="sxs-lookup"><span data-stu-id="c41c1-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c41c1-119">授权</span><span class="sxs-lookup"><span data-stu-id="c41c1-119">Authorization</span></span>|<span data-ttu-id="c41c1-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c41c1-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c41c1-121">接受</span><span class="sxs-lookup"><span data-stu-id="c41c1-121">Accept</span></span>|<span data-ttu-id="c41c1-122">application/json</span><span class="sxs-lookup"><span data-stu-id="c41c1-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c41c1-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="c41c1-123">Request body</span></span>
<span data-ttu-id="c41c1-124">在请求正文中，提供 [enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c41c1-124">In the request body, supply a JSON representation for the [enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md) object.</span></span>

<span data-ttu-id="c41c1-125">下表显示创建 [enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="c41c1-125">The following table shows the properties that are required when you create the [enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md).</span></span>

|<span data-ttu-id="c41c1-126">属性</span><span class="sxs-lookup"><span data-stu-id="c41c1-126">Property</span></span>|<span data-ttu-id="c41c1-127">类型</span><span class="sxs-lookup"><span data-stu-id="c41c1-127">Type</span></span>|<span data-ttu-id="c41c1-128">说明</span><span class="sxs-lookup"><span data-stu-id="c41c1-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c41c1-129">ID</span><span class="sxs-lookup"><span data-stu-id="c41c1-129">id</span></span>|<span data-ttu-id="c41c1-130">字符串</span><span class="sxs-lookup"><span data-stu-id="c41c1-130">String</span></span>|<span data-ttu-id="c41c1-131">对象的 UUID。继承自 [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="c41c1-131">UUID for the object Inherited from [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="c41c1-132">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="c41c1-132">eventDateTime</span></span>|<span data-ttu-id="c41c1-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c41c1-133">DateTimeOffset</span></span>|<span data-ttu-id="c41c1-134">事件发生的时间。</span><span class="sxs-lookup"><span data-stu-id="c41c1-134">Time when the event occurred .</span></span> <span data-ttu-id="c41c1-135">继承自 [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="c41c1-135">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="c41c1-136">correlationId</span><span class="sxs-lookup"><span data-stu-id="c41c1-136">correlationId</span></span>|<span data-ttu-id="c41c1-137">字符串</span><span class="sxs-lookup"><span data-stu-id="c41c1-137">String</span></span>|<span data-ttu-id="c41c1-138">用于跟踪服务中的故障的 ID。</span><span class="sxs-lookup"><span data-stu-id="c41c1-138">Id used for tracing the failure in the service.</span></span> <span data-ttu-id="c41c1-139">继承自 [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="c41c1-139">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="c41c1-140">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="c41c1-140">managedDeviceIdentifier</span></span>|<span data-ttu-id="c41c1-141">字符串</span><span class="sxs-lookup"><span data-stu-id="c41c1-141">String</span></span>|<span data-ttu-id="c41c1-142">Intune 创建或收集的设备标识符。</span><span class="sxs-lookup"><span data-stu-id="c41c1-142">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="c41c1-143">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="c41c1-143">operatingSystem</span></span>|<span data-ttu-id="c41c1-144">字符串</span><span class="sxs-lookup"><span data-stu-id="c41c1-144">String</span></span>|<span data-ttu-id="c41c1-145">操作系统。</span><span class="sxs-lookup"><span data-stu-id="c41c1-145">Operating System.</span></span>|
|<span data-ttu-id="c41c1-146">osVersion</span><span class="sxs-lookup"><span data-stu-id="c41c1-146">osVersion</span></span>|<span data-ttu-id="c41c1-147">字符串</span><span class="sxs-lookup"><span data-stu-id="c41c1-147">String</span></span>|<span data-ttu-id="c41c1-148">操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="c41c1-148">OS Version.</span></span>|
|<span data-ttu-id="c41c1-149">userId</span><span class="sxs-lookup"><span data-stu-id="c41c1-149">userId</span></span>|<span data-ttu-id="c41c1-150">字符串</span><span class="sxs-lookup"><span data-stu-id="c41c1-150">String</span></span>|<span data-ttu-id="c41c1-151">尝试注册设备的用户的标识符。</span><span class="sxs-lookup"><span data-stu-id="c41c1-151">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="c41c1-152">deviceId</span><span class="sxs-lookup"><span data-stu-id="c41c1-152">deviceId</span></span>|<span data-ttu-id="c41c1-153">字符串</span><span class="sxs-lookup"><span data-stu-id="c41c1-153">String</span></span>|<span data-ttu-id="c41c1-154">Azure AD 设备标识符。</span><span class="sxs-lookup"><span data-stu-id="c41c1-154">Azure AD device identifier.</span></span>|
|<span data-ttu-id="c41c1-155">enrollmentType</span><span class="sxs-lookup"><span data-stu-id="c41c1-155">enrollmentType</span></span>|[<span data-ttu-id="c41c1-156">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="c41c1-156">deviceEnrollmentType</span></span>](../resources/intune_shared_deviceenrollmenttype.md)|<span data-ttu-id="c41c1-157">注册类型。</span><span class="sxs-lookup"><span data-stu-id="c41c1-157">Type of the enrollment.</span></span> <span data-ttu-id="c41c1-158">可取值为：`unknown`、`userEnrollment`、`deviceEnrollmentManager`、`appleBulkWithUser`、`appleBulkWithoutUser`、`windowsAzureADJoin`、`windowsBulkUserless`、`windowsAutoEnrollment`、`windowsBulkAzureDomainJoin`、`windowsCoManagement`。</span><span class="sxs-lookup"><span data-stu-id="c41c1-158">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="c41c1-159">failureCategory</span><span class="sxs-lookup"><span data-stu-id="c41c1-159">failureCategory</span></span>|[<span data-ttu-id="c41c1-160">deviceEnrollmentFailureReason</span><span class="sxs-lookup"><span data-stu-id="c41c1-160">deviceEnrollmentFailureReason values</span></span>](../resources/intune_troubleshooting_deviceenrollmentfailurereason.md)|<span data-ttu-id="c41c1-161">Highlevel 失败类别。</span><span class="sxs-lookup"><span data-stu-id="c41c1-161">Highlevel failure category.</span></span> <span data-ttu-id="c41c1-162">可取值为：`unknown`、`authentication`、`authorization`、`accountValidation`、`userValidation`、`deviceNotSupported`、`inMaintenance`、`badRequest`、`featureNotSupported`、`enrollmentRestrictionsEnforced`、`clientDisconnected`、`userAbandonment`。</span><span class="sxs-lookup"><span data-stu-id="c41c1-162">Possible values are: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`, `userAbandonment`.</span></span>|
|<span data-ttu-id="c41c1-163">failureReason</span><span class="sxs-lookup"><span data-stu-id="c41c1-163">failureReason</span></span>|<span data-ttu-id="c41c1-164">字符串</span><span class="sxs-lookup"><span data-stu-id="c41c1-164">String</span></span>|<span data-ttu-id="c41c1-165">详细失败原因。</span><span class="sxs-lookup"><span data-stu-id="c41c1-165">Detailed failure reason.</span></span>|



## <a name="response"></a><span data-ttu-id="c41c1-166">响应</span><span class="sxs-lookup"><span data-stu-id="c41c1-166">Response</span></span>
<span data-ttu-id="c41c1-167">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c41c1-167">If successful, this method returns a `200 OK` response code and an updated [enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c41c1-168">示例</span><span class="sxs-lookup"><span data-stu-id="c41c1-168">Example</span></span>
### <a name="request"></a><span data-ttu-id="c41c1-169">请求</span><span class="sxs-lookup"><span data-stu-id="c41c1-169">Request</span></span>
<span data-ttu-id="c41c1-170">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c41c1-170">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1/deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
Content-type: application/json
Content-length: 440

{
  "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
  "correlationId": "Correlation Id value",
  "managedDeviceIdentifier": "Managed Device Identifier value",
  "operatingSystem": "Operating System value",
  "osVersion": "Os Version value",
  "userId": "User Id value",
  "deviceId": "Device Id value",
  "enrollmentType": "userEnrollment",
  "failureCategory": "authentication",
  "failureReason": "Failure Reason value"
}
```

### <a name="response"></a><span data-ttu-id="c41c1-171">响应</span><span class="sxs-lookup"><span data-stu-id="c41c1-171">Response</span></span>
<span data-ttu-id="c41c1-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c41c1-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 558

{
  "@odata.type": "#microsoft.graph.enrollmentTroubleshootingEvent",
  "id": "c4a623f5-23f5-c4a6-f523-a6c4f523a6c4",
  "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
  "correlationId": "Correlation Id value",
  "managedDeviceIdentifier": "Managed Device Identifier value",
  "operatingSystem": "Operating System value",
  "osVersion": "Os Version value",
  "userId": "User Id value",
  "deviceId": "Device Id value",
  "enrollmentType": "userEnrollment",
  "failureCategory": "authentication",
  "failureReason": "Failure Reason value"
}
```





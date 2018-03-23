# <a name="create-enrollmenttroubleshootingevent"></a><span data-ttu-id="aad61-101">创建 enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="aad61-101">Create enrollmentTroubleshootingEvent</span></span>

> <span data-ttu-id="aad61-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="aad61-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="aad61-103">创建新的 [enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="aad61-103">Create a new [plannerBucket](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="aad61-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="aad61-104">Prerequisites</span></span>
<span data-ttu-id="aad61-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="aad61-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="aad61-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="aad61-107">Permission type</span></span>|<span data-ttu-id="aad61-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="aad61-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aad61-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="aad61-109">Delegated (work or school account)</span></span>|<span data-ttu-id="aad61-110">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aad61-110">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="aad61-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="aad61-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aad61-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="aad61-112">Not supported.</span></span>|
|<span data-ttu-id="aad61-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="aad61-113">Application</span></span>|<span data-ttu-id="aad61-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="aad61-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="aad61-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="aad61-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/troubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="aad61-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="aad61-116">Request headers</span></span>
|<span data-ttu-id="aad61-117">标头</span><span class="sxs-lookup"><span data-stu-id="aad61-117">Header</span></span>|<span data-ttu-id="aad61-118">值</span><span class="sxs-lookup"><span data-stu-id="aad61-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aad61-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="aad61-119">Authorization</span></span>|<span data-ttu-id="aad61-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="aad61-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="aad61-121">Accept</span><span class="sxs-lookup"><span data-stu-id="aad61-121">Accept</span></span>|<span data-ttu-id="aad61-122">application/json</span><span class="sxs-lookup"><span data-stu-id="aad61-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aad61-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="aad61-123">Request body</span></span>
<span data-ttu-id="aad61-124">在请求正文中，提供 enrollmentTroubleshootingEvent 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="aad61-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="aad61-125">下表显示创建 enrollmentTroubleshootingEvent 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="aad61-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="aad61-126">属性</span><span class="sxs-lookup"><span data-stu-id="aad61-126">Property</span></span>|<span data-ttu-id="aad61-127">类型</span><span class="sxs-lookup"><span data-stu-id="aad61-127">Type</span></span>|<span data-ttu-id="aad61-128">说明</span><span class="sxs-lookup"><span data-stu-id="aad61-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aad61-129">id</span><span class="sxs-lookup"><span data-stu-id="aad61-129">id</span></span>|<span data-ttu-id="aad61-130">String</span><span class="sxs-lookup"><span data-stu-id="aad61-130">String</span></span>|<span data-ttu-id="aad61-131">对象的 UUID。继承自 [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="aad61-131">UUID for the object Inherited from [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="aad61-132">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="aad61-132">eventDateTime</span></span>|<span data-ttu-id="aad61-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aad61-133">DateTimeOffset</span></span>|<span data-ttu-id="aad61-134">事件发生的时间。</span><span class="sxs-lookup"><span data-stu-id="aad61-134">Time when the event occurred .</span></span> <span data-ttu-id="aad61-135">继承自 [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="aad61-135">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="aad61-136">correlationId</span><span class="sxs-lookup"><span data-stu-id="aad61-136">correlationId</span></span>|<span data-ttu-id="aad61-137">String</span><span class="sxs-lookup"><span data-stu-id="aad61-137">String</span></span>|<span data-ttu-id="aad61-138">用于跟踪服务中的故障的 ID。</span><span class="sxs-lookup"><span data-stu-id="aad61-138">Id used for tracing the failure in the service.</span></span> <span data-ttu-id="aad61-139">继承自 [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="aad61-139">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="aad61-140">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="aad61-140">managedDeviceIdentifier</span></span>|<span data-ttu-id="aad61-141">String</span><span class="sxs-lookup"><span data-stu-id="aad61-141">String</span></span>|<span data-ttu-id="aad61-142">Intune 创建或收集的设备标识符。</span><span class="sxs-lookup"><span data-stu-id="aad61-142">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="aad61-143">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="aad61-143">operatingSystem</span></span>|<span data-ttu-id="aad61-144">String</span><span class="sxs-lookup"><span data-stu-id="aad61-144">String</span></span>|<span data-ttu-id="aad61-145">操作系统。</span><span class="sxs-lookup"><span data-stu-id="aad61-145">Operating system</span></span>|
|<span data-ttu-id="aad61-146">osVersion</span><span class="sxs-lookup"><span data-stu-id="aad61-146">osVersion</span></span>|<span data-ttu-id="aad61-147">String</span><span class="sxs-lookup"><span data-stu-id="aad61-147">String</span></span>|<span data-ttu-id="aad61-148">操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="aad61-148">OS Version.</span></span>|
|<span data-ttu-id="aad61-149">userId</span><span class="sxs-lookup"><span data-stu-id="aad61-149">userID</span></span>|<span data-ttu-id="aad61-150">String</span><span class="sxs-lookup"><span data-stu-id="aad61-150">String</span></span>|<span data-ttu-id="aad61-151">尝试注册设备的用户的标识符。</span><span class="sxs-lookup"><span data-stu-id="aad61-151">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="aad61-152">deviceId</span><span class="sxs-lookup"><span data-stu-id="aad61-152">deviceId</span></span>|<span data-ttu-id="aad61-153">String</span><span class="sxs-lookup"><span data-stu-id="aad61-153">String</span></span>|<span data-ttu-id="aad61-154">Azure AD 设备标识符。</span><span class="sxs-lookup"><span data-stu-id="aad61-154">Azure AD device identifier.</span></span>|
|<span data-ttu-id="aad61-155">enrollmentType</span><span class="sxs-lookup"><span data-stu-id="aad61-155">enrollmentType</span></span>|<span data-ttu-id="aad61-156">String</span><span class="sxs-lookup"><span data-stu-id="aad61-156">String</span></span>|<span data-ttu-id="aad61-157">注册类型。</span><span class="sxs-lookup"><span data-stu-id="aad61-157">Type of the enrollment.</span></span> <span data-ttu-id="aad61-158">可取值为：`unknown`、`userEnrollment`、`deviceEnrollmentManager`、`appleBulkWithUser`、`appleBulkWithoutUser`、`windowsAzureADJoin`、`windowsBulkUserless`、`windowsAutoEnrollment`、`windowsBulkAzureDomainJoin`、`windowsCoManagement`。</span><span class="sxs-lookup"><span data-stu-id="aad61-158">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="aad61-159">failureCategory</span><span class="sxs-lookup"><span data-stu-id="aad61-159">failureCategory</span></span>|<span data-ttu-id="aad61-160">String</span><span class="sxs-lookup"><span data-stu-id="aad61-160">String</span></span>|<span data-ttu-id="aad61-161">Highlevel 失败类别。</span><span class="sxs-lookup"><span data-stu-id="aad61-161">Highlevel failure category.</span></span> <span data-ttu-id="aad61-162">可取值为：`unknown`、`authentication`、`authorization`、`accountValidation`、`userValidation`、`deviceNotSupported`、`inMaintenance`、`badRequest`、`featureNotSupported`、`enrollmentRestrictionsEnforced`、`clientDisconnected`。</span><span class="sxs-lookup"><span data-stu-id="aad61-162">Possible values are: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`.</span></span>|
|<span data-ttu-id="aad61-163">failureReason</span><span class="sxs-lookup"><span data-stu-id="aad61-163">failureReason</span></span>|<span data-ttu-id="aad61-164">String</span><span class="sxs-lookup"><span data-stu-id="aad61-164">String</span></span>|<span data-ttu-id="aad61-165">详细失败原因。</span><span class="sxs-lookup"><span data-stu-id="aad61-165">Detailed failure reason.</span></span>|



## <a name="response"></a><span data-ttu-id="aad61-166">响应</span><span class="sxs-lookup"><span data-stu-id="aad61-166">Response</span></span>
<span data-ttu-id="aad61-167">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="aad61-167">If successful, this method returns a `201 Created` response code and a [directoryObject](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aad61-168">示例</span><span class="sxs-lookup"><span data-stu-id="aad61-168">Example</span></span>
### <a name="request"></a><span data-ttu-id="aad61-169">请求</span><span class="sxs-lookup"><span data-stu-id="aad61-169">Request</span></span>
<span data-ttu-id="aad61-170">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="aad61-170">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/troubleshootingEvents
Content-type: application/json
Content-length: 509

{
  "@odata.type": "#microsoft.graph.enrollmentTroubleshootingEvent",
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

### <a name="response"></a><span data-ttu-id="aad61-171">响应</span><span class="sxs-lookup"><span data-stu-id="aad61-171">Response</span></span>
<span data-ttu-id="aad61-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="aad61-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




# <a name="update-importedwindowsautopilotdeviceidentityupload"></a><span data-ttu-id="5c865-101">Update importedWindowsAutopilotDeviceIdentityUpload</span><span class="sxs-lookup"><span data-stu-id="5c865-101">Update importedWindowsAutopilotDeviceIdentityUpload</span></span>

> <span data-ttu-id="5c865-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="5c865-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5c865-103">更新 [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityupload.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="5c865-103">Update the properties of a [managedDeviceMobileAppConfigurationAssignment](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityupload.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5c865-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="5c865-104">Prerequisites</span></span>
<span data-ttu-id="5c865-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="5c865-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="5c865-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="5c865-107">Permission type</span></span>|<span data-ttu-id="5c865-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="5c865-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5c865-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5c865-109">Delegated (work or school account)</span></span>|<span data-ttu-id="5c865-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c865-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="5c865-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5c865-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5c865-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="5c865-112">Not supported.</span></span>|
|<span data-ttu-id="5c865-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="5c865-113">Application</span></span>|<span data-ttu-id="5c865-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="5c865-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5c865-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5c865-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}
```

## <a name="request-headers"></a><span data-ttu-id="5c865-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="5c865-116">Request headers</span></span>
|<span data-ttu-id="5c865-117">标头</span><span class="sxs-lookup"><span data-stu-id="5c865-117">Header</span></span>|<span data-ttu-id="5c865-118">值</span><span class="sxs-lookup"><span data-stu-id="5c865-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5c865-119">授权</span><span class="sxs-lookup"><span data-stu-id="5c865-119">Authorization</span></span>|<span data-ttu-id="5c865-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="5c865-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5c865-121">Accept</span><span class="sxs-lookup"><span data-stu-id="5c865-121">Accept</span></span>|<span data-ttu-id="5c865-122">application/json</span><span class="sxs-lookup"><span data-stu-id="5c865-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5c865-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="5c865-123">Request body</span></span>
<span data-ttu-id="5c865-124">在请求正文中，提供 [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityupload.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5c865-124">In the request body, supply a JSON representation for the [targetedManagedAppPolicyAssignment](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityupload.md) object.</span></span>

<span data-ttu-id="5c865-125">下表显示创建 [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityupload.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="5c865-125">The following table shows the properties that are required when you create the [enrollmentConfigurationAssignment](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityupload.md).</span></span>

|<span data-ttu-id="5c865-126">属性</span><span class="sxs-lookup"><span data-stu-id="5c865-126">Property</span></span>|<span data-ttu-id="5c865-127">类型</span><span class="sxs-lookup"><span data-stu-id="5c865-127">Type</span></span>|<span data-ttu-id="5c865-128">说明</span><span class="sxs-lookup"><span data-stu-id="5c865-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5c865-129">ID</span><span class="sxs-lookup"><span data-stu-id="5c865-129">id</span></span>|<span data-ttu-id="5c865-130">字符串</span><span class="sxs-lookup"><span data-stu-id="5c865-130">String</span></span>|<span data-ttu-id="5c865-131">对象的 GUID</span><span class="sxs-lookup"><span data-stu-id="5c865-131">The GUID for the object</span></span>|
|<span data-ttu-id="5c865-132">createdDateTimeUtc</span><span class="sxs-lookup"><span data-stu-id="5c865-132">createdDateTimeUtc</span></span>|<span data-ttu-id="5c865-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5c865-133">DateTimeOffset</span></span>|<span data-ttu-id="5c865-134">创建实体时的日期时间。</span><span class="sxs-lookup"><span data-stu-id="5c865-134">DateTime when the entity is created.</span></span>|
|<span data-ttu-id="5c865-135">status</span><span class="sxs-lookup"><span data-stu-id="5c865-135">status</span></span>|[<span data-ttu-id="5c865-136">importedWindowsAutopilotDeviceIdentityUploadStatus</span><span class="sxs-lookup"><span data-stu-id="5c865-136">importedWindowsAutopilotDeviceIdentityUploadStatus</span></span>](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityuploadstatus.md)|<span data-ttu-id="5c865-137">上载状态。</span><span class="sxs-lookup"><span data-stu-id="5c865-137">Upload status.</span></span> <span data-ttu-id="5c865-138">可取值为：`noUpload`、`pending`、`complete`、`error`。</span><span class="sxs-lookup"><span data-stu-id="5c865-138">Possible values are: `noUpload`, `pending`, `complete`, `error`.</span></span>|



## <a name="response"></a><span data-ttu-id="5c865-139">响应</span><span class="sxs-lookup"><span data-stu-id="5c865-139">Response</span></span>
<span data-ttu-id="5c865-140">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityupload.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5c865-140">If successful, this method returns a `200 OK` response code and an updated [enrollmentConfigurationAssignment](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityupload.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5c865-141">示例</span><span class="sxs-lookup"><span data-stu-id="5c865-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="5c865-142">请求</span><span class="sxs-lookup"><span data-stu-id="5c865-142">Request</span></span>
<span data-ttu-id="5c865-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5c865-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}
Content-type: application/json
Content-length: 89

{
  "createdDateTimeUtc": "2016-12-31T23:59:45.8788427-08:00",
  "status": "pending"
}
```

### <a name="response"></a><span data-ttu-id="5c865-144">响应</span><span class="sxs-lookup"><span data-stu-id="5c865-144">Response</span></span>
<span data-ttu-id="5c865-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5c865-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 221

{
  "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentityUpload",
  "id": "8d639524-9524-8d63-2495-638d2495638d",
  "createdDateTimeUtc": "2016-12-31T23:59:45.8788427-08:00",
  "status": "pending"
}
```









# <a name="update-importedwindowsautopilotdeviceidentityupload"></a><span data-ttu-id="50694-101">更新 importedWindowsAutopilotDeviceIdentityUpload</span><span class="sxs-lookup"><span data-stu-id="50694-101">Update importedWindowsAutopilotDeviceIdentityUpload</span></span>

> <span data-ttu-id="50694-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="50694-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="50694-103">更新[importedWindowsAutopilotDeviceIdentityUpload](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityupload.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="50694-103">Update the properties of a [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityupload.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="50694-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="50694-104">Prerequisites</span></span>
<span data-ttu-id="50694-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](../../../concepts/permissions_reference.md)。
</span><span class="sxs-lookup"><span data-stu-id="50694-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="50694-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="50694-107">Permission type</span></span>|<span data-ttu-id="50694-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="50694-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="50694-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="50694-109">Delegated (work or school account)</span></span>|<span data-ttu-id="50694-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50694-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="50694-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="50694-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="50694-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="50694-112">Not supported.</span></span>|
|<span data-ttu-id="50694-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="50694-113">Application</span></span>|<span data-ttu-id="50694-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="50694-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="50694-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="50694-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}
```

## <a name="request-headers"></a><span data-ttu-id="50694-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="50694-116">Request headers</span></span>
|<span data-ttu-id="50694-117">标头</span><span class="sxs-lookup"><span data-stu-id="50694-117">Header</span></span>|<span data-ttu-id="50694-118">值</span><span class="sxs-lookup"><span data-stu-id="50694-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="50694-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="50694-119">Authorization</span></span>|<span data-ttu-id="50694-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="50694-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="50694-121">Accept</span><span class="sxs-lookup"><span data-stu-id="50694-121">Accept</span></span>|<span data-ttu-id="50694-122">application/json</span><span class="sxs-lookup"><span data-stu-id="50694-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="50694-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="50694-123">Request body</span></span>
<span data-ttu-id="50694-124">在请求正文中，提供[importedWindowsAutopilotDeviceIdentityUpload](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityupload.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="50694-124">In the request body, supply a JSON representation for the [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityupload.md) object.</span></span>

<span data-ttu-id="50694-125">下表显示时创建[importedWindowsAutopilotDeviceIdentityUpload](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityupload.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="50694-125">The following table shows the properties that are required when you create the [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityupload.md).</span></span>

|<span data-ttu-id="50694-126">属性</span><span class="sxs-lookup"><span data-stu-id="50694-126">Property</span></span>|<span data-ttu-id="50694-127">类型</span><span class="sxs-lookup"><span data-stu-id="50694-127">Type</span></span>|<span data-ttu-id="50694-128">说明</span><span class="sxs-lookup"><span data-stu-id="50694-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="50694-129">id</span><span class="sxs-lookup"><span data-stu-id="50694-129">id</span></span>|<span data-ttu-id="50694-130">字符串</span><span class="sxs-lookup"><span data-stu-id="50694-130">String</span></span>|<span data-ttu-id="50694-131">对象的 GUID</span><span class="sxs-lookup"><span data-stu-id="50694-131">The GUID for the object</span></span>|
|<span data-ttu-id="50694-132">createdDateTimeUtc</span><span class="sxs-lookup"><span data-stu-id="50694-132">createdDateTimeUtc</span></span>|<span data-ttu-id="50694-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="50694-133">DateTimeOffset</span></span>|<span data-ttu-id="50694-134">创建实体时的日期时间。</span><span class="sxs-lookup"><span data-stu-id="50694-134">DateTime when the entity is created.</span></span>|
|<span data-ttu-id="50694-135">状态</span><span class="sxs-lookup"><span data-stu-id="50694-135">status</span></span>|[<span data-ttu-id="50694-136">importedWindowsAutopilotDeviceIdentityUploadStatus</span><span class="sxs-lookup"><span data-stu-id="50694-136">importedWindowsAutopilotDeviceIdentityUploadStatus</span></span>](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityuploadstatus.md)|<span data-ttu-id="50694-137">上载状态。</span><span class="sxs-lookup"><span data-stu-id="50694-137">Upload status.</span></span> <span data-ttu-id="50694-138">可取值为：`noUpload`、`pending`、`complete`、`error`。</span><span class="sxs-lookup"><span data-stu-id="50694-138">Possible values are: `noUpload`, `pending`, `complete`, `error`.</span></span>|



## <a name="response"></a><span data-ttu-id="50694-139">响应</span><span class="sxs-lookup"><span data-stu-id="50694-139">Response</span></span>
<span data-ttu-id="50694-140">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[importedWindowsAutopilotDeviceIdentityUpload](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityupload.md)对象。</span><span class="sxs-lookup"><span data-stu-id="50694-140">If successful, this method returns a `200 OK` response code and an updated [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityupload.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="50694-141">示例</span><span class="sxs-lookup"><span data-stu-id="50694-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="50694-142">请求</span><span class="sxs-lookup"><span data-stu-id="50694-142">Request</span></span>
<span data-ttu-id="50694-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="50694-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}
Content-type: application/json
Content-length: 172

{
  "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentityUpload",
  "createdDateTimeUtc": "2016-12-31T23:59:45.8788427-08:00",
  "status": "pending"
}
```

### <a name="response"></a><span data-ttu-id="50694-144">响应</span><span class="sxs-lookup"><span data-stu-id="50694-144">Response</span></span>
<span data-ttu-id="50694-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="50694-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




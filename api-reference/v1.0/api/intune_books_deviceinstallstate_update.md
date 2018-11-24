# <a name="update-deviceinstallstate"></a><span data-ttu-id="c283b-101">更新 deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="c283b-101">Update deviceInstallState</span></span>

> <span data-ttu-id="c283b-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="c283b-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c283b-103">更新 [deviceInstallState](../resources/intune_books_deviceinstallstate.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="c283b-103">Update the properties of a [deviceInstallState](../resources/intune_books_deviceinstallstate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c283b-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="c283b-104">Prerequisites</span></span>
<span data-ttu-id="c283b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="c283b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="c283b-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="c283b-107">Permission type</span></span>|<span data-ttu-id="c283b-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c283b-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c283b-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c283b-109">Delegated (work or school account)</span></span>|<span data-ttu-id="c283b-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c283b-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c283b-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c283b-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c283b-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="c283b-112">Not supported.</span></span>|
|<span data-ttu-id="c283b-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="c283b-113">Application</span></span>|<span data-ttu-id="c283b-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="c283b-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c283b-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c283b-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates/{deviceInstallStateId}
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}/deviceStates/{deviceInstallStateId}
```

## <a name="request-headers"></a><span data-ttu-id="c283b-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="c283b-116">Request headers</span></span>
|<span data-ttu-id="c283b-117">标头</span><span class="sxs-lookup"><span data-stu-id="c283b-117">Header</span></span>|<span data-ttu-id="c283b-118">值</span><span class="sxs-lookup"><span data-stu-id="c283b-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c283b-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="c283b-119">Authorization</span></span>|<span data-ttu-id="c283b-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c283b-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c283b-121">Accept</span><span class="sxs-lookup"><span data-stu-id="c283b-121">Accept</span></span>|<span data-ttu-id="c283b-122">application/json</span><span class="sxs-lookup"><span data-stu-id="c283b-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c283b-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="c283b-123">Request body</span></span>
<span data-ttu-id="c283b-124">在请求正文中，提供 [deviceInstallState](../resources/intune_books_deviceinstallstate.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c283b-124">In the request body, supply a JSON representation for the [deviceInstallState](../resources/intune_books_deviceinstallstate.md) object.</span></span>

<span data-ttu-id="c283b-125">下表显示创建 [deviceInstallState](../resources/intune_books_deviceinstallstate.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="c283b-125">The following table shows the properties that are required when you create the [deviceInstallState](../resources/intune_books_deviceinstallstate.md).</span></span>

|<span data-ttu-id="c283b-126">属性</span><span class="sxs-lookup"><span data-stu-id="c283b-126">Property</span></span>|<span data-ttu-id="c283b-127">类型</span><span class="sxs-lookup"><span data-stu-id="c283b-127">Type</span></span>|<span data-ttu-id="c283b-128">说明</span><span class="sxs-lookup"><span data-stu-id="c283b-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c283b-129">id</span><span class="sxs-lookup"><span data-stu-id="c283b-129">id</span></span>|<span data-ttu-id="c283b-130">String</span><span class="sxs-lookup"><span data-stu-id="c283b-130">String</span></span>|<span data-ttu-id="c283b-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="c283b-131">Key of the entity.</span></span>|
|<span data-ttu-id="c283b-132">deviceName</span><span class="sxs-lookup"><span data-stu-id="c283b-132">deviceName</span></span>|<span data-ttu-id="c283b-133">String</span><span class="sxs-lookup"><span data-stu-id="c283b-133">String</span></span>|<span data-ttu-id="c283b-134">设备名称。</span><span class="sxs-lookup"><span data-stu-id="c283b-134">Device name.</span></span>|
|<span data-ttu-id="c283b-135">deviceId</span><span class="sxs-lookup"><span data-stu-id="c283b-135">deviceId</span></span>|<span data-ttu-id="c283b-136">String</span><span class="sxs-lookup"><span data-stu-id="c283b-136">String</span></span>|<span data-ttu-id="c283b-137">设备 ID。</span><span class="sxs-lookup"><span data-stu-id="c283b-137">Device Id.</span></span>|
|<span data-ttu-id="c283b-138">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="c283b-138">lastSyncDateTime</span></span>|<span data-ttu-id="c283b-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c283b-139">DateTimeOffset</span></span>|<span data-ttu-id="c283b-140">上次同步日期和时间。</span><span class="sxs-lookup"><span data-stu-id="c283b-140">Last sync date and time.</span></span>|
|<span data-ttu-id="c283b-141">installState</span><span class="sxs-lookup"><span data-stu-id="c283b-141">installState</span></span>|[<span data-ttu-id="c283b-142">installState</span><span class="sxs-lookup"><span data-stu-id="c283b-142">installState</span></span>](../resources/intune_books_installstate.md)|<span data-ttu-id="c283b-143">电子图书的安装状态。</span><span class="sxs-lookup"><span data-stu-id="c283b-143">The install state of the eBook.</span></span> <span data-ttu-id="c283b-144">可取值为：`notApplicable`、`installed`、`failed`、`notInstalled`、`uninstallFailed`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="c283b-144">Possible values are: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed`, `unknown`.</span></span>|
|<span data-ttu-id="c283b-145">errorCode</span><span class="sxs-lookup"><span data-stu-id="c283b-145">errorCode</span></span>|<span data-ttu-id="c283b-146">String</span><span class="sxs-lookup"><span data-stu-id="c283b-146">String</span></span>|<span data-ttu-id="c283b-147">安装失败的错误代码。</span><span class="sxs-lookup"><span data-stu-id="c283b-147">The error code for install failures.</span></span>|
|<span data-ttu-id="c283b-148">osVersion</span><span class="sxs-lookup"><span data-stu-id="c283b-148">osVersion</span></span>|<span data-ttu-id="c283b-149">String</span><span class="sxs-lookup"><span data-stu-id="c283b-149">String</span></span>|<span data-ttu-id="c283b-150">操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="c283b-150">OS Version.</span></span>|
|<span data-ttu-id="c283b-151">osDescription</span><span class="sxs-lookup"><span data-stu-id="c283b-151">osDescription</span></span>|<span data-ttu-id="c283b-152">String</span><span class="sxs-lookup"><span data-stu-id="c283b-152">String</span></span>|<span data-ttu-id="c283b-153">操作系统说明。</span><span class="sxs-lookup"><span data-stu-id="c283b-153">OS Description.</span></span>|
|<span data-ttu-id="c283b-154">userName</span><span class="sxs-lookup"><span data-stu-id="c283b-154">userName</span></span>|<span data-ttu-id="c283b-155">String</span><span class="sxs-lookup"><span data-stu-id="c283b-155">String</span></span>|<span data-ttu-id="c283b-156">设备用户名。</span><span class="sxs-lookup"><span data-stu-id="c283b-156">Device User Name.</span></span>|



## <a name="response"></a><span data-ttu-id="c283b-157">响应</span><span class="sxs-lookup"><span data-stu-id="c283b-157">Response</span></span>
<span data-ttu-id="c283b-158">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [deviceInstallState](../resources/intune_books_deviceinstallstate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c283b-158">If successful, this method returns a `200 OK` response code and an updated [deviceInstallState](../resources/intune_books_deviceinstallstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c283b-159">示例</span><span class="sxs-lookup"><span data-stu-id="c283b-159">Example</span></span>
### <a name="request"></a><span data-ttu-id="c283b-160">请求</span><span class="sxs-lookup"><span data-stu-id="c283b-160">Request</span></span>
<span data-ttu-id="c283b-161">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c283b-161">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates/{deviceInstallStateId}
Content-type: application/json
Content-length: 374

{
  "@odata.type": "#microsoft.graph.deviceInstallState",
  "deviceName": "Device Name value",
  "deviceId": "Device Id value",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "installState": "installed",
  "errorCode": "Error Code value",
  "osVersion": "Os Version value",
  "osDescription": "Os Description value",
  "userName": "User Name value"
}
```

### <a name="response"></a><span data-ttu-id="c283b-162">响应</span><span class="sxs-lookup"><span data-stu-id="c283b-162">Response</span></span>
<span data-ttu-id="c283b-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c283b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 423

{
  "@odata.type": "#microsoft.graph.deviceInstallState",
  "id": "b9feb68f-b68f-b9fe-8fb6-feb98fb6feb9",
  "deviceName": "Device Name value",
  "deviceId": "Device Id value",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "installState": "installed",
  "errorCode": "Error Code value",
  "osVersion": "Os Version value",
  "osDescription": "Os Description value",
  "userName": "User Name value"
}
```




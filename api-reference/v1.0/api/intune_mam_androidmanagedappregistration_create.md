# <a name="create-androidmanagedappregistration"></a><span data-ttu-id="8e692-101">创建 androidManagedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="8e692-101">Create androidManagedAppRegistration</span></span>

> <span data-ttu-id="8e692-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="8e692-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8e692-103">创建新的 [androidManagedAppRegistration](../resources/intune_mam_androidmanagedappregistration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8e692-103">Create a new [plannerBucket](../resources/intune_mam_androidmanagedappregistration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8e692-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="8e692-104">Prerequisites</span></span>
<span data-ttu-id="8e692-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="8e692-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="8e692-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="8e692-107">Permission type</span></span>|<span data-ttu-id="8e692-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="8e692-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8e692-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8e692-109">Delegated (work or school account)</span></span>|<span data-ttu-id="8e692-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e692-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="8e692-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8e692-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8e692-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="8e692-112">Not supported.</span></span>|
|<span data-ttu-id="8e692-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="8e692-113">Application</span></span>|<span data-ttu-id="8e692-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="8e692-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8e692-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8e692-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedAppRegistrations
```

## <a name="request-headers"></a><span data-ttu-id="8e692-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="8e692-116">Request headers</span></span>
|<span data-ttu-id="8e692-117">标头</span><span class="sxs-lookup"><span data-stu-id="8e692-117">Header</span></span>|<span data-ttu-id="8e692-118">值</span><span class="sxs-lookup"><span data-stu-id="8e692-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8e692-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="8e692-119">Authorization</span></span>|<span data-ttu-id="8e692-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="8e692-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="8e692-121">Accept</span><span class="sxs-lookup"><span data-stu-id="8e692-121">Accept</span></span>|<span data-ttu-id="8e692-122">application/json</span><span class="sxs-lookup"><span data-stu-id="8e692-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8e692-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="8e692-123">Request body</span></span>
<span data-ttu-id="8e692-124">在请求正文中，提供 androidManagedAppRegistration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8e692-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="8e692-125">下表显示了创建 androidManagedAppRegistration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="8e692-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="8e692-126">属性</span><span class="sxs-lookup"><span data-stu-id="8e692-126">Property</span></span>|<span data-ttu-id="8e692-127">类型</span><span class="sxs-lookup"><span data-stu-id="8e692-127">Type</span></span>|<span data-ttu-id="8e692-128">说明</span><span class="sxs-lookup"><span data-stu-id="8e692-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8e692-129">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8e692-129">createdDateTime</span></span>|<span data-ttu-id="8e692-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8e692-130">DateTimeOffset</span></span>|<span data-ttu-id="8e692-131">创建的日期和时间。继承自 [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="8e692-131">Date and time of creation Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="8e692-132">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="8e692-132">lastSyncDateTime</span></span>|<span data-ttu-id="8e692-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8e692-133">DateTimeOffset</span></span>|<span data-ttu-id="8e692-134">上次应用与管理服务同步的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="8e692-134">Date and time of last the app synced with management service.</span></span> <span data-ttu-id="8e692-135">继承自 [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="8e692-135">Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="8e692-136">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="8e692-136">applicationVersion</span></span>|<span data-ttu-id="8e692-137">String</span><span class="sxs-lookup"><span data-stu-id="8e692-137">String</span></span>|<span data-ttu-id="8e692-138">应用版本。继承自 [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="8e692-138">App version Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="8e692-139">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="8e692-139">managementSdkVersion</span></span>|<span data-ttu-id="8e692-140">String</span><span class="sxs-lookup"><span data-stu-id="8e692-140">String</span></span>|<span data-ttu-id="8e692-141">应用管理 SDK 版本。继承自 [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="8e692-141">App management SDK version Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="8e692-142">platformVersion</span><span class="sxs-lookup"><span data-stu-id="8e692-142">platformVersion</span></span>|<span data-ttu-id="8e692-143">String</span><span class="sxs-lookup"><span data-stu-id="8e692-143">String</span></span>|<span data-ttu-id="8e692-144">操作系统版本。继承自 [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="8e692-144">Operating System version Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="8e692-145">deviceType</span><span class="sxs-lookup"><span data-stu-id="8e692-145">deviceType</span></span>|<span data-ttu-id="8e692-146">String</span><span class="sxs-lookup"><span data-stu-id="8e692-146">String</span></span>|<span data-ttu-id="8e692-147">主机设备类型。继承自 [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="8e692-147">Host device type Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="8e692-148">deviceTag</span><span class="sxs-lookup"><span data-stu-id="8e692-148">deviceTag</span></span>|<span data-ttu-id="8e692-149">String</span><span class="sxs-lookup"><span data-stu-id="8e692-149">String</span></span>|<span data-ttu-id="8e692-150">应用管理 SDK 生成的标记，它可帮助关联托管在同一设备上的应用。</span><span class="sxs-lookup"><span data-stu-id="8e692-150">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="8e692-151">不保证在所有情况下与应用关联。</span><span class="sxs-lookup"><span data-stu-id="8e692-151">Not guaranteed to relate apps in all conditions.</span></span> <span data-ttu-id="8e692-152">继承自 [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="8e692-152">Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="8e692-153">deviceName</span><span class="sxs-lookup"><span data-stu-id="8e692-153">deviceName</span></span>|<span data-ttu-id="8e692-154">String</span><span class="sxs-lookup"><span data-stu-id="8e692-154">String</span></span>|<span data-ttu-id="8e692-155">主机设备名称。继承自 [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="8e692-155">Host device name Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="8e692-156">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="8e692-156">flaggedReasons</span></span>|<span data-ttu-id="8e692-157">String 集合</span><span class="sxs-lookup"><span data-stu-id="8e692-157">String collection</span></span>|<span data-ttu-id="8e692-158">标记应用注册的零个或多个原因。</span><span class="sxs-lookup"><span data-stu-id="8e692-158">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="8e692-159">例如，</span><span class="sxs-lookup"><span data-stu-id="8e692-159">E.g.</span></span> <span data-ttu-id="8e692-160">应用正在根设备上运行。继承自 [managedAppRegistration](../resources/intune_mam_managedappregistration.md)。可取值为：`none`、`rootedDevice`。</span><span class="sxs-lookup"><span data-stu-id="8e692-160">app running on rooted device Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md) Possible values are: `none`, `rootedDevice`.</span></span>|
|<span data-ttu-id="8e692-161">userId</span><span class="sxs-lookup"><span data-stu-id="8e692-161">userID</span></span>|<span data-ttu-id="8e692-162">String</span><span class="sxs-lookup"><span data-stu-id="8e692-162">String</span></span>|<span data-ttu-id="8e692-163">此应用注册所属的用户 ID。</span><span class="sxs-lookup"><span data-stu-id="8e692-163">The user Id to who this app registration belongs.</span></span> <span data-ttu-id="8e692-164">继承自 [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="8e692-164">Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="8e692-165">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="8e692-165">appIdentifier</span></span>|[<span data-ttu-id="8e692-166">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="8e692-166">mobileAppIdentifier</span></span>](../resources/intune_mam_mobileappidentifier.md)|<span data-ttu-id="8e692-167">应用包标识符。继承自 [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="8e692-167">The app package Identifier Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="8e692-168">id</span><span class="sxs-lookup"><span data-stu-id="8e692-168">id</span></span>|<span data-ttu-id="8e692-169">String</span><span class="sxs-lookup"><span data-stu-id="8e692-169">String</span></span>|<span data-ttu-id="8e692-170">实体的键。</span><span class="sxs-lookup"><span data-stu-id="8e692-170">Key of the setting.</span></span> <span data-ttu-id="8e692-171">继承自 [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="8e692-171">Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="8e692-172">version</span><span class="sxs-lookup"><span data-stu-id="8e692-172">version</span></span>|<span data-ttu-id="8e692-173">String</span><span class="sxs-lookup"><span data-stu-id="8e692-173">String</span></span>|<span data-ttu-id="8e692-174">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="8e692-174">Version of the entity.</span></span> <span data-ttu-id="8e692-175">继承自 [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="8e692-175">Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="8e692-176">响应</span><span class="sxs-lookup"><span data-stu-id="8e692-176">Response</span></span>
<span data-ttu-id="8e692-177">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [androidManagedAppRegistration](../resources/intune_mam_androidmanagedappregistration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8e692-177">If successful, this method returns a `201 Created` response code and a [directoryObject](../resources/intune_mam_androidmanagedappregistration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8e692-178">示例</span><span class="sxs-lookup"><span data-stu-id="8e692-178">Example</span></span>
### <a name="request"></a><span data-ttu-id="8e692-179">请求</span><span class="sxs-lookup"><span data-stu-id="8e692-179">Request</span></span>
<span data-ttu-id="8e692-180">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8e692-180">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppRegistrations
Content-type: application/json
Content-length: 645

{
  "@odata.type": "#microsoft.graph.androidManagedAppRegistration",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "applicationVersion": "Application Version value",
  "managementSdkVersion": "Management Sdk Version value",
  "platformVersion": "Platform Version value",
  "deviceType": "Device Type value",
  "deviceTag": "Device Tag value",
  "deviceName": "Device Name value",
  "flaggedReasons": [
    "rootedDevice"
  ],
  "userId": "User Id value",
  "appIdentifier": {
    "@odata.type": "microsoft.graph.androidMobileAppIdentifier",
    "packageId": "Package Id value"
  },
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="8e692-181">响应</span><span class="sxs-lookup"><span data-stu-id="8e692-181">Response</span></span>
<span data-ttu-id="8e692-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8e692-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 753

{
  "@odata.type": "#microsoft.graph.androidManagedAppRegistration",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "applicationVersion": "Application Version value",
  "managementSdkVersion": "Management Sdk Version value",
  "platformVersion": "Platform Version value",
  "deviceType": "Device Type value",
  "deviceTag": "Device Tag value",
  "deviceName": "Device Name value",
  "flaggedReasons": [
    "rootedDevice"
  ],
  "userId": "User Id value",
  "appIdentifier": {
    "@odata.type": "microsoft.graph.androidMobileAppIdentifier",
    "packageId": "Package Id value"
  },
  "id": "0e064997-4997-0e06-9749-060e9749060e",
  "version": "Version value"
}
```




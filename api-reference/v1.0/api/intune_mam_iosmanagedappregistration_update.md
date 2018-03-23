# <a name="update-iosmanagedappregistration"></a><span data-ttu-id="78fb9-101">更新 iosManagedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="78fb9-101">Update iosManagedAppRegistration</span></span>

> <span data-ttu-id="78fb9-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="78fb9-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="78fb9-103">更新 [iosManagedAppRegistration](../resources/intune_mam_iosmanagedappregistration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="78fb9-103">Update the properties of a [calendar](../resources/intune_mam_iosmanagedappregistration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="78fb9-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="78fb9-104">Prerequisites</span></span>
<span data-ttu-id="78fb9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="78fb9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="78fb9-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="78fb9-107">Permission type</span></span>|<span data-ttu-id="78fb9-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="78fb9-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="78fb9-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="78fb9-109">Delegated (work or school account)</span></span>|<span data-ttu-id="78fb9-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="78fb9-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="78fb9-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="78fb9-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="78fb9-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="78fb9-112">Not supported.</span></span>|
|<span data-ttu-id="78fb9-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="78fb9-113">Application</span></span>|<span data-ttu-id="78fb9-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="78fb9-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="78fb9-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="78fb9-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}
```

## <a name="request-headers"></a><span data-ttu-id="78fb9-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="78fb9-116">Request headers</span></span>
|<span data-ttu-id="78fb9-117">标头</span><span class="sxs-lookup"><span data-stu-id="78fb9-117">Header</span></span>|<span data-ttu-id="78fb9-118">值</span><span class="sxs-lookup"><span data-stu-id="78fb9-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="78fb9-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="78fb9-119">Authorization</span></span>|<span data-ttu-id="78fb9-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="78fb9-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="78fb9-121">Accept</span><span class="sxs-lookup"><span data-stu-id="78fb9-121">Accept</span></span>|<span data-ttu-id="78fb9-122">application/json</span><span class="sxs-lookup"><span data-stu-id="78fb9-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="78fb9-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="78fb9-123">Request body</span></span>
<span data-ttu-id="78fb9-124">在请求正文中，提供 [iosManagedAppRegistration](../resources/intune_mam_iosmanagedappregistration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="78fb9-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_mam_iosmanagedappregistration.md) object.</span></span>

<span data-ttu-id="78fb9-125">下表显示创建 [iosManagedAppRegistration](../resources/intune_mam_iosmanagedappregistration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="78fb9-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="78fb9-126">属性</span><span class="sxs-lookup"><span data-stu-id="78fb9-126">Property</span></span>|<span data-ttu-id="78fb9-127">类型</span><span class="sxs-lookup"><span data-stu-id="78fb9-127">Type</span></span>|<span data-ttu-id="78fb9-128">说明</span><span class="sxs-lookup"><span data-stu-id="78fb9-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="78fb9-129">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="78fb9-129">createdDateTime</span></span>|<span data-ttu-id="78fb9-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="78fb9-130">DateTimeOffset</span></span>|<span data-ttu-id="78fb9-131">创建的日期和时间。继承自 [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="78fb9-131">Date and time of creation Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="78fb9-132">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="78fb9-132">lastSyncDateTime</span></span>|<span data-ttu-id="78fb9-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="78fb9-133">DateTimeOffset</span></span>|<span data-ttu-id="78fb9-134">上次应用与管理服务同步的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="78fb9-134">Date and time of last the app synced with management service.</span></span> <span data-ttu-id="78fb9-135">继承自 [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="78fb9-135">Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="78fb9-136">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="78fb9-136">applicationVersion</span></span>|<span data-ttu-id="78fb9-137">String</span><span class="sxs-lookup"><span data-stu-id="78fb9-137">String</span></span>|<span data-ttu-id="78fb9-138">应用版本。继承自 [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="78fb9-138">App version Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="78fb9-139">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="78fb9-139">managementSdkVersion</span></span>|<span data-ttu-id="78fb9-140">String</span><span class="sxs-lookup"><span data-stu-id="78fb9-140">String</span></span>|<span data-ttu-id="78fb9-141">应用管理 SDK 版本。继承自 [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="78fb9-141">App management SDK version Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="78fb9-142">platformVersion</span><span class="sxs-lookup"><span data-stu-id="78fb9-142">platformVersion</span></span>|<span data-ttu-id="78fb9-143">String</span><span class="sxs-lookup"><span data-stu-id="78fb9-143">String</span></span>|<span data-ttu-id="78fb9-144">操作系统版本。继承自 [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="78fb9-144">Operating System version Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="78fb9-145">deviceType</span><span class="sxs-lookup"><span data-stu-id="78fb9-145">deviceType</span></span>|<span data-ttu-id="78fb9-146">String</span><span class="sxs-lookup"><span data-stu-id="78fb9-146">String</span></span>|<span data-ttu-id="78fb9-147">主机设备类型。继承自 [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="78fb9-147">Host device type Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="78fb9-148">deviceTag</span><span class="sxs-lookup"><span data-stu-id="78fb9-148">deviceTag</span></span>|<span data-ttu-id="78fb9-149">String</span><span class="sxs-lookup"><span data-stu-id="78fb9-149">String</span></span>|<span data-ttu-id="78fb9-150">应用管理 SDK 生成的标记，它可帮助关联托管在同一设备上的应用。</span><span class="sxs-lookup"><span data-stu-id="78fb9-150">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="78fb9-151">不保证在所有情况下与应用关联。</span><span class="sxs-lookup"><span data-stu-id="78fb9-151">Not guaranteed to relate apps in all conditions.</span></span> <span data-ttu-id="78fb9-152">继承自 [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="78fb9-152">Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="78fb9-153">deviceName</span><span class="sxs-lookup"><span data-stu-id="78fb9-153">deviceName</span></span>|<span data-ttu-id="78fb9-154">String</span><span class="sxs-lookup"><span data-stu-id="78fb9-154">String</span></span>|<span data-ttu-id="78fb9-155">主机设备名称。继承自 [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="78fb9-155">Host device name Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="78fb9-156">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="78fb9-156">flaggedReasons</span></span>|<span data-ttu-id="78fb9-157">String 集合</span><span class="sxs-lookup"><span data-stu-id="78fb9-157">String collection</span></span>|<span data-ttu-id="78fb9-158">标记应用注册的零个或多个原因。</span><span class="sxs-lookup"><span data-stu-id="78fb9-158">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="78fb9-159">例如，</span><span class="sxs-lookup"><span data-stu-id="78fb9-159">E.g.</span></span> <span data-ttu-id="78fb9-160">应用正在根设备上运行。继承自 [managedAppRegistration](../resources/intune_mam_managedappregistration.md)。可取值为：`none`、`rootedDevice`。</span><span class="sxs-lookup"><span data-stu-id="78fb9-160">app running on rooted device Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md) Possible values are: `none`, `rootedDevice`.</span></span>|
|<span data-ttu-id="78fb9-161">userId</span><span class="sxs-lookup"><span data-stu-id="78fb9-161">userID</span></span>|<span data-ttu-id="78fb9-162">String</span><span class="sxs-lookup"><span data-stu-id="78fb9-162">String</span></span>|<span data-ttu-id="78fb9-163">此应用注册所属的用户 ID。</span><span class="sxs-lookup"><span data-stu-id="78fb9-163">The user Id to who this app registration belongs.</span></span> <span data-ttu-id="78fb9-164">继承自 [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="78fb9-164">Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="78fb9-165">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="78fb9-165">appIdentifier</span></span>|[<span data-ttu-id="78fb9-166">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="78fb9-166">mobileAppIdentifier</span></span>](../resources/intune_mam_mobileappidentifier.md)|<span data-ttu-id="78fb9-167">应用包标识符。继承自 [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="78fb9-167">The app package Identifier Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="78fb9-168">id</span><span class="sxs-lookup"><span data-stu-id="78fb9-168">id</span></span>|<span data-ttu-id="78fb9-169">String</span><span class="sxs-lookup"><span data-stu-id="78fb9-169">String</span></span>|<span data-ttu-id="78fb9-170">实体的键。</span><span class="sxs-lookup"><span data-stu-id="78fb9-170">Key of the setting.</span></span> <span data-ttu-id="78fb9-171">继承自 [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="78fb9-171">Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="78fb9-172">version</span><span class="sxs-lookup"><span data-stu-id="78fb9-172">version</span></span>|<span data-ttu-id="78fb9-173">String</span><span class="sxs-lookup"><span data-stu-id="78fb9-173">String</span></span>|<span data-ttu-id="78fb9-174">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="78fb9-174">Version of the entity.</span></span> <span data-ttu-id="78fb9-175">继承自 [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="78fb9-175">Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="78fb9-176">响应</span><span class="sxs-lookup"><span data-stu-id="78fb9-176">Response</span></span>
<span data-ttu-id="78fb9-177">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [iosManagedAppRegistration](../resources/intune_mam_iosmanagedappregistration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="78fb9-177">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_mam_iosmanagedappregistration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="78fb9-178">示例</span><span class="sxs-lookup"><span data-stu-id="78fb9-178">Example</span></span>
### <a name="request"></a><span data-ttu-id="78fb9-179">请求</span><span class="sxs-lookup"><span data-stu-id="78fb9-179">Request</span></span>
<span data-ttu-id="78fb9-180">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="78fb9-180">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}
Content-type: application/json
Content-length: 571

{
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
    "@odata.type": "microsoft.graph.iosMobileAppIdentifier",
    "bundleId": "Bundle Id value"
  },
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="78fb9-181">响应</span><span class="sxs-lookup"><span data-stu-id="78fb9-181">Response</span></span>
<span data-ttu-id="78fb9-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="78fb9-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 743

{
  "@odata.type": "#microsoft.graph.iosManagedAppRegistration",
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
    "@odata.type": "microsoft.graph.iosMobileAppIdentifier",
    "bundleId": "Bundle Id value"
  },
  "id": "47632c19-2c19-4763-192c-6347192c6347",
  "version": "Version value"
}
```




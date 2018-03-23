# <a name="update-androidforworkenrollmentprofile"></a><span data-ttu-id="457f1-101">更新 androidForWorkEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="457f1-101">Update androidForWorkEnrollmentProfile</span></span>

> <span data-ttu-id="457f1-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="457f1-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="457f1-103">更新 [androidForWorkEnrollmentProfile](../resources/intune_androidforwork_androidforworkenrollmentprofile.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="457f1-103">Update the properties of a [calendar](../resources/intune_androidforwork_androidforworkenrollmentprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="457f1-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="457f1-104">Prerequisites</span></span>
<span data-ttu-id="457f1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="457f1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="457f1-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="457f1-107">Permission type</span></span>|<span data-ttu-id="457f1-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="457f1-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="457f1-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="457f1-109">Delegated (work or school account)</span></span>|<span data-ttu-id="457f1-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="457f1-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="457f1-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="457f1-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="457f1-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="457f1-112">Not supported.</span></span>|
|<span data-ttu-id="457f1-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="457f1-113">Application</span></span>|<span data-ttu-id="457f1-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="457f1-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="457f1-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="457f1-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/androidForWorkEnrollmentProfiles/{androidForWorkEnrollmentProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="457f1-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="457f1-116">Request headers</span></span>
|<span data-ttu-id="457f1-117">标头</span><span class="sxs-lookup"><span data-stu-id="457f1-117">Header</span></span>|<span data-ttu-id="457f1-118">值</span><span class="sxs-lookup"><span data-stu-id="457f1-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="457f1-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="457f1-119">Authorization</span></span>|<span data-ttu-id="457f1-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="457f1-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="457f1-121">Accept</span><span class="sxs-lookup"><span data-stu-id="457f1-121">Accept</span></span>|<span data-ttu-id="457f1-122">application/json</span><span class="sxs-lookup"><span data-stu-id="457f1-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="457f1-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="457f1-123">Request body</span></span>
<span data-ttu-id="457f1-124">在请求正文中，提供 [androidForWorkEnrollmentProfile](../resources/intune_androidforwork_androidforworkenrollmentprofile.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="457f1-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_androidforwork_androidforworkenrollmentprofile.md) object.</span></span>

<span data-ttu-id="457f1-125">下表显示创建 [androidForWorkEnrollmentProfile](../resources/intune_androidforwork_androidforworkenrollmentprofile.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="457f1-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="457f1-126">属性</span><span class="sxs-lookup"><span data-stu-id="457f1-126">Property</span></span>|<span data-ttu-id="457f1-127">类型</span><span class="sxs-lookup"><span data-stu-id="457f1-127">Type</span></span>|<span data-ttu-id="457f1-128">说明</span><span class="sxs-lookup"><span data-stu-id="457f1-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="457f1-129">accountId</span><span class="sxs-lookup"><span data-stu-id="457f1-129">accountId</span></span>|<span data-ttu-id="457f1-130">String</span><span class="sxs-lookup"><span data-stu-id="457f1-130">String</span></span>|<span data-ttu-id="457f1-131">注册配置文件隶属的租户 GUID。</span><span class="sxs-lookup"><span data-stu-id="457f1-131">Tenant GUID the enrollment profile belongs to.</span></span>|
|<span data-ttu-id="457f1-132">id</span><span class="sxs-lookup"><span data-stu-id="457f1-132">id</span></span>|<span data-ttu-id="457f1-133">String</span><span class="sxs-lookup"><span data-stu-id="457f1-133">String</span></span>|<span data-ttu-id="457f1-134">注册配置文件的唯一 GUID。</span><span class="sxs-lookup"><span data-stu-id="457f1-134">Unique GUID for the enrollment profile.</span></span>|
|<span data-ttu-id="457f1-135">name</span><span class="sxs-lookup"><span data-stu-id="457f1-135">name</span></span>|<span data-ttu-id="457f1-136">String</span><span class="sxs-lookup"><span data-stu-id="457f1-136">String</span></span>|<span data-ttu-id="457f1-137">（已弃用）注册配置文件的显示名称。</span><span class="sxs-lookup"><span data-stu-id="457f1-137">(Deprecated) Display name for the enrollment profile.</span></span>|
|<span data-ttu-id="457f1-138">displayName</span><span class="sxs-lookup"><span data-stu-id="457f1-138">displayName</span></span>|<span data-ttu-id="457f1-139">String</span><span class="sxs-lookup"><span data-stu-id="457f1-139">String</span></span>|<span data-ttu-id="457f1-140">注册配置文件的显示名称。</span><span class="sxs-lookup"><span data-stu-id="457f1-140">Display name for the enrollment profile.</span></span>|
|<span data-ttu-id="457f1-141">description</span><span class="sxs-lookup"><span data-stu-id="457f1-141">description</span></span>|<span data-ttu-id="457f1-142">String</span><span class="sxs-lookup"><span data-stu-id="457f1-142">String</span></span>|<span data-ttu-id="457f1-143">注册配置文件的说明。</span><span class="sxs-lookup"><span data-stu-id="457f1-143">Description for the enrollment profile.</span></span>|
|<span data-ttu-id="457f1-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="457f1-144">createdDateTime</span></span>|<span data-ttu-id="457f1-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="457f1-145">DateTimeOffset</span></span>|<span data-ttu-id="457f1-146">注册配置文件的创建日期/时间。</span><span class="sxs-lookup"><span data-stu-id="457f1-146">Date time the enrollment profile was created.</span></span>|
|<span data-ttu-id="457f1-147">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="457f1-147">modifiedDateTime</span></span>|<span data-ttu-id="457f1-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="457f1-148">DateTimeOffset</span></span>|<span data-ttu-id="457f1-149">（已弃用）上次修改注册配置文件的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="457f1-149">(Deprecated) Date time the enrollment profile was last modified.</span></span>|
|<span data-ttu-id="457f1-150">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="457f1-150">lastModifiedDateTime</span></span>|<span data-ttu-id="457f1-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="457f1-151">DateTimeOffset</span></span>|<span data-ttu-id="457f1-152">上次修改注册配置文件的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="457f1-152">Date time the enrollment profile was last modified.</span></span>|
|<span data-ttu-id="457f1-153">tokenValue</span><span class="sxs-lookup"><span data-stu-id="457f1-153">tokenValue</span></span>|<span data-ttu-id="457f1-154">String</span><span class="sxs-lookup"><span data-stu-id="457f1-154">String</span></span>|<span data-ttu-id="457f1-155">为此注册配置文件最新创建的令牌的值。</span><span class="sxs-lookup"><span data-stu-id="457f1-155">Value of the most recently created token for this enrollment profile.</span></span>|
|<span data-ttu-id="457f1-156">tokenExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="457f1-156">tokenExpirationDateTime</span></span>|<span data-ttu-id="457f1-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="457f1-157">DateTimeOffset</span></span>|<span data-ttu-id="457f1-158">最新创建的令牌的到期日期/时间。</span><span class="sxs-lookup"><span data-stu-id="457f1-158">Date time the most recently created token will expire.</span></span>|
|<span data-ttu-id="457f1-159">totalEnrollmentCount</span><span class="sxs-lookup"><span data-stu-id="457f1-159">totalEnrollmentCount</span></span>|<span data-ttu-id="457f1-160">Int32</span><span class="sxs-lookup"><span data-stu-id="457f1-160">Int32</span></span>|<span data-ttu-id="457f1-161">（已弃用）已使用此注册配置文件进行注册的 Android 设备总数。</span><span class="sxs-lookup"><span data-stu-id="457f1-161">(Deprecated) Total number of Android devices that have enrolled using this enrollment profile.</span></span>|
|<span data-ttu-id="457f1-162">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="457f1-162">enrolledDeviceCount</span></span>|<span data-ttu-id="457f1-163">Int32</span><span class="sxs-lookup"><span data-stu-id="457f1-163">Int32</span></span>|<span data-ttu-id="457f1-164">已使用此注册配置文件进行注册的 Android 设备总数。</span><span class="sxs-lookup"><span data-stu-id="457f1-164">Total number of Android devices that have enrolled using this enrollment profile.</span></span>|
|<span data-ttu-id="457f1-165">qrCode</span><span class="sxs-lookup"><span data-stu-id="457f1-165">qrCode</span></span>|<span data-ttu-id="457f1-166">String</span><span class="sxs-lookup"><span data-stu-id="457f1-166">String</span></span>|<span data-ttu-id="457f1-167">（已弃用）用于生成此令牌的 QR 码的字符串。</span><span class="sxs-lookup"><span data-stu-id="457f1-167">(Deprecated) String used to generate a QR code for the token.</span></span>|
|<span data-ttu-id="457f1-168">qrCodeContent</span><span class="sxs-lookup"><span data-stu-id="457f1-168">qrCodeContent</span></span>|<span data-ttu-id="457f1-169">String</span><span class="sxs-lookup"><span data-stu-id="457f1-169">String</span></span>|<span data-ttu-id="457f1-170">用于生成此令牌的 QR 码的字符串。</span><span class="sxs-lookup"><span data-stu-id="457f1-170">String used to generate a QR code for the token.</span></span>|
|<span data-ttu-id="457f1-171">qrCodeImage</span><span class="sxs-lookup"><span data-stu-id="457f1-171">qrCodeImage</span></span>|[<span data-ttu-id="457f1-172">mimeContent</span><span class="sxs-lookup"><span data-stu-id="457f1-172">mimeContent</span></span>](../resources/intune_androidforwork_mimecontent.md)|<span data-ttu-id="457f1-173">用于生成此令牌的 QR 码的字符串。</span><span class="sxs-lookup"><span data-stu-id="457f1-173">String used to generate a QR code for the token.</span></span>|



## <a name="response"></a><span data-ttu-id="457f1-174">响应</span><span class="sxs-lookup"><span data-stu-id="457f1-174">Response</span></span>
<span data-ttu-id="457f1-175">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [androidForWorkEnrollmentProfile](../resources/intune_androidforwork_androidforworkenrollmentprofile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="457f1-175">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_androidforwork_androidforworkenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="457f1-176">示例</span><span class="sxs-lookup"><span data-stu-id="457f1-176">Example</span></span>
### <a name="request"></a><span data-ttu-id="457f1-177">请求</span><span class="sxs-lookup"><span data-stu-id="457f1-177">Request</span></span>
<span data-ttu-id="457f1-178">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="457f1-178">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/androidForWorkEnrollmentProfiles/{androidForWorkEnrollmentProfileId}
Content-type: application/json
Content-length: 575

{
  "accountId": "Account Id value",
  "name": "Name value",
  "displayName": "Display Name value",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "tokenValue": "Token Value value",
  "tokenExpirationDateTime": "2016-12-31T23:59:54.0590989-08:00",
  "totalEnrollmentCount": 4,
  "enrolledDeviceCount": 3,
  "qrCode": "Qr Code value",
  "qrCodeContent": "Qr Code Content value",
  "qrCodeImage": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  }
}
```

### <a name="response"></a><span data-ttu-id="457f1-179">响应</span><span class="sxs-lookup"><span data-stu-id="457f1-179">Response</span></span>
<span data-ttu-id="457f1-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="457f1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 813

{
  "@odata.type": "#microsoft.graph.androidForWorkEnrollmentProfile",
  "accountId": "Account Id value",
  "id": "e6742553-2553-e674-5325-74e6532574e6",
  "name": "Name value",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "tokenValue": "Token Value value",
  "tokenExpirationDateTime": "2016-12-31T23:59:54.0590989-08:00",
  "totalEnrollmentCount": 4,
  "enrolledDeviceCount": 3,
  "qrCode": "Qr Code value",
  "qrCodeContent": "Qr Code Content value",
  "qrCodeImage": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  }
}
```




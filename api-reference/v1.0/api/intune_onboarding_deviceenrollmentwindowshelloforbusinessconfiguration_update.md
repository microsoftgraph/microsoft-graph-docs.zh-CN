# <a name="update-deviceenrollmentwindowshelloforbusinessconfiguration"></a><span data-ttu-id="6442e-101">更新 deviceEnrollmentWindowsHelloForBusinessConfiguration</span><span class="sxs-lookup"><span data-stu-id="6442e-101">Update deviceEnrollmentWindowsHelloForBusinessConfiguration</span></span>

> <span data-ttu-id="6442e-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="6442e-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6442e-103">更新 [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="6442e-103">Update the properties of a [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6442e-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="6442e-104">Prerequisites</span></span>
<span data-ttu-id="6442e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="6442e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="6442e-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="6442e-107">Permission type</span></span>|<span data-ttu-id="6442e-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="6442e-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6442e-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6442e-109">Delegated (work or school account)</span></span>|<span data-ttu-id="6442e-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6442e-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="6442e-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6442e-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6442e-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="6442e-112">Not supported.</span></span>|
|<span data-ttu-id="6442e-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="6442e-113">Application</span></span>|<span data-ttu-id="6442e-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="6442e-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6442e-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6442e-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="6442e-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="6442e-116">Request headers</span></span>
|<span data-ttu-id="6442e-117">标头</span><span class="sxs-lookup"><span data-stu-id="6442e-117">Header</span></span>|<span data-ttu-id="6442e-118">值</span><span class="sxs-lookup"><span data-stu-id="6442e-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6442e-119">授权</span><span class="sxs-lookup"><span data-stu-id="6442e-119">Authorization</span></span>|<span data-ttu-id="6442e-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6442e-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6442e-121">接受</span><span class="sxs-lookup"><span data-stu-id="6442e-121">Accept</span></span>|<span data-ttu-id="6442e-122">application/json</span><span class="sxs-lookup"><span data-stu-id="6442e-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6442e-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="6442e-123">Request body</span></span>
<span data-ttu-id="6442e-124">在请求正文中，提供 [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6442e-124">In the request body, supply a JSON representation for the [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration.md) object.</span></span>

<span data-ttu-id="6442e-125">下表显示创建 [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="6442e-125">The following table shows the properties that are required when you create the [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration.md).</span></span>

|<span data-ttu-id="6442e-126">属性</span><span class="sxs-lookup"><span data-stu-id="6442e-126">Property</span></span>|<span data-ttu-id="6442e-127">类型</span><span class="sxs-lookup"><span data-stu-id="6442e-127">Type</span></span>|<span data-ttu-id="6442e-128">说明</span><span class="sxs-lookup"><span data-stu-id="6442e-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6442e-129">ID</span><span class="sxs-lookup"><span data-stu-id="6442e-129">id</span></span>|<span data-ttu-id="6442e-130">字符串</span><span class="sxs-lookup"><span data-stu-id="6442e-130">String</span></span>|<span data-ttu-id="6442e-131">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6442e-131">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="6442e-132">displayName</span><span class="sxs-lookup"><span data-stu-id="6442e-132">displayName</span></span>|<span data-ttu-id="6442e-133">字符串</span><span class="sxs-lookup"><span data-stu-id="6442e-133">String</span></span>|<span data-ttu-id="6442e-134">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6442e-134">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="6442e-135">说明</span><span class="sxs-lookup"><span data-stu-id="6442e-135">description</span></span>|<span data-ttu-id="6442e-136">字符串</span><span class="sxs-lookup"><span data-stu-id="6442e-136">String</span></span>|<span data-ttu-id="6442e-137">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6442e-137">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="6442e-138">优先级</span><span class="sxs-lookup"><span data-stu-id="6442e-138">priority</span></span>|<span data-ttu-id="6442e-139">Int32</span><span class="sxs-lookup"><span data-stu-id="6442e-139">Int32</span></span>|<span data-ttu-id="6442e-140">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6442e-140">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="6442e-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6442e-141">createdDateTime</span></span>|<span data-ttu-id="6442e-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6442e-142">DateTimeOffset</span></span>|<span data-ttu-id="6442e-143">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6442e-143">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="6442e-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6442e-144">lastModifiedDateTime</span></span>|<span data-ttu-id="6442e-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6442e-145">DateTimeOffset</span></span>|<span data-ttu-id="6442e-146">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6442e-146">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="6442e-147">版本</span><span class="sxs-lookup"><span data-stu-id="6442e-147">version</span></span>|<span data-ttu-id="6442e-148">Int32</span><span class="sxs-lookup"><span data-stu-id="6442e-148">Int32</span></span>|<span data-ttu-id="6442e-149">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6442e-149">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="6442e-150">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="6442e-150">pinMinimumLength</span></span>|<span data-ttu-id="6442e-151">Int32</span><span class="sxs-lookup"><span data-stu-id="6442e-151">Int32</span></span>|<span data-ttu-id="6442e-152">尚未记录</span><span class="sxs-lookup"><span data-stu-id="6442e-152">Not yet documented</span></span>|
|<span data-ttu-id="6442e-153">pinMaximumLength</span><span class="sxs-lookup"><span data-stu-id="6442e-153">pinMaximumLength</span></span>|<span data-ttu-id="6442e-154">Int32</span><span class="sxs-lookup"><span data-stu-id="6442e-154">Int32</span></span>|<span data-ttu-id="6442e-155">尚未记录</span><span class="sxs-lookup"><span data-stu-id="6442e-155">Not yet documented</span></span>|
|<span data-ttu-id="6442e-156">pinUppercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="6442e-156">pinUppercaseCharactersUsage</span></span>|[<span data-ttu-id="6442e-157">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="6442e-157">windowsHelloForBusinessPinUsage</span></span>](../resources/intune_onboarding_windowshelloforbusinesspinusage.md)|<span data-ttu-id="6442e-158">尚未记录。</span><span class="sxs-lookup"><span data-stu-id="6442e-158">Not yet documented</span></span> <span data-ttu-id="6442e-159">可取值为：`allowed`、`required`、`disallowed`。</span><span class="sxs-lookup"><span data-stu-id="6442e-159">The possible values are `allowed`, `required`, `disallowed`, , , , , , , , , or .</span></span>|
|<span data-ttu-id="6442e-160">pinLowercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="6442e-160">pinLowercaseCharactersUsage</span></span>|[<span data-ttu-id="6442e-161">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="6442e-161">windowsHelloForBusinessPinUsage</span></span>](../resources/intune_onboarding_windowshelloforbusinesspinusage.md)|<span data-ttu-id="6442e-162">尚未记录。</span><span class="sxs-lookup"><span data-stu-id="6442e-162">Not yet documented</span></span> <span data-ttu-id="6442e-163">可取值为：`allowed`、`required`、`disallowed`。</span><span class="sxs-lookup"><span data-stu-id="6442e-163">The possible values are `allowed`, `required`, `disallowed`, , , , , , , , , or .</span></span>|
|<span data-ttu-id="6442e-164">pinSpecialCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="6442e-164">pinSpecialCharactersUsage</span></span>|[<span data-ttu-id="6442e-165">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="6442e-165">windowsHelloForBusinessPinUsage</span></span>](../resources/intune_onboarding_windowshelloforbusinesspinusage.md)|<span data-ttu-id="6442e-166">尚未记录。</span><span class="sxs-lookup"><span data-stu-id="6442e-166">Not yet documented</span></span> <span data-ttu-id="6442e-167">可取值为：`allowed`、`required`、`disallowed`。</span><span class="sxs-lookup"><span data-stu-id="6442e-167">The possible values are `allowed`, `required`, `disallowed`, , , , , , , , , or .</span></span>|
|<span data-ttu-id="6442e-168">状态</span><span class="sxs-lookup"><span data-stu-id="6442e-168">state</span></span>|[<span data-ttu-id="6442e-169">启用</span><span class="sxs-lookup"><span data-stu-id="6442e-169">Enablement</span></span>](../resources/intune_onboarding_enablement.md)|<span data-ttu-id="6442e-170">尚未记录。</span><span class="sxs-lookup"><span data-stu-id="6442e-170">Not yet documented</span></span> <span data-ttu-id="6442e-171">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="6442e-171">The possible values are `notConfigured`, `enabled`, `disabled`, , , , , , , , , or .</span></span>|
|<span data-ttu-id="6442e-172">securityDeviceRequired</span><span class="sxs-lookup"><span data-stu-id="6442e-172">securityDeviceRequired</span></span>|<span data-ttu-id="6442e-173">布尔值</span><span class="sxs-lookup"><span data-stu-id="6442e-173">Boolean</span></span>|<span data-ttu-id="6442e-174">尚未记录</span><span class="sxs-lookup"><span data-stu-id="6442e-174">Not yet documented</span></span>|
|<span data-ttu-id="6442e-175">unlockWithBiometricsEnabled</span><span class="sxs-lookup"><span data-stu-id="6442e-175">unlockWithBiometricsEnabled</span></span>|<span data-ttu-id="6442e-176">布尔值</span><span class="sxs-lookup"><span data-stu-id="6442e-176">Boolean</span></span>|<span data-ttu-id="6442e-177">尚未记录</span><span class="sxs-lookup"><span data-stu-id="6442e-177">Not yet documented</span></span>|
|<span data-ttu-id="6442e-178">remotePassportEnabled</span><span class="sxs-lookup"><span data-stu-id="6442e-178">remotePassportEnabled</span></span>|<span data-ttu-id="6442e-179">布尔值</span><span class="sxs-lookup"><span data-stu-id="6442e-179">Boolean</span></span>|<span data-ttu-id="6442e-180">尚未记录</span><span class="sxs-lookup"><span data-stu-id="6442e-180">Not yet documented</span></span>|
|<span data-ttu-id="6442e-181">pinPreviousBlockCount</span><span class="sxs-lookup"><span data-stu-id="6442e-181">pinPreviousBlockCount</span></span>|<span data-ttu-id="6442e-182">Int32</span><span class="sxs-lookup"><span data-stu-id="6442e-182">Int32</span></span>|<span data-ttu-id="6442e-183">尚未记录</span><span class="sxs-lookup"><span data-stu-id="6442e-183">Not yet documented</span></span>|
|<span data-ttu-id="6442e-184">pinExpirationInDays</span><span class="sxs-lookup"><span data-stu-id="6442e-184">pinExpirationInDays</span></span>|<span data-ttu-id="6442e-185">Int32</span><span class="sxs-lookup"><span data-stu-id="6442e-185">Int32</span></span>|<span data-ttu-id="6442e-186">尚未记录</span><span class="sxs-lookup"><span data-stu-id="6442e-186">Not yet documented</span></span>|
|<span data-ttu-id="6442e-187">enhancedBiometricsState</span><span class="sxs-lookup"><span data-stu-id="6442e-187">enhancedBiometricsState</span></span>|[<span data-ttu-id="6442e-188">启用</span><span class="sxs-lookup"><span data-stu-id="6442e-188">Enablement</span></span>](../resources/intune_onboarding_enablement.md)|<span data-ttu-id="6442e-189">尚未记录。</span><span class="sxs-lookup"><span data-stu-id="6442e-189">Not yet documented</span></span> <span data-ttu-id="6442e-190">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="6442e-190">The possible values are `notConfigured`, `enabled`, `disabled`, , , , , , , , , or .</span></span>|



## <a name="response"></a><span data-ttu-id="6442e-191">响应</span><span class="sxs-lookup"><span data-stu-id="6442e-191">Response</span></span>
<span data-ttu-id="6442e-192">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6442e-192">If successful, this method returns a `200 OK` response code and an updated [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6442e-193">示例</span><span class="sxs-lookup"><span data-stu-id="6442e-193">Example</span></span>
### <a name="request"></a><span data-ttu-id="6442e-194">请求</span><span class="sxs-lookup"><span data-stu-id="6442e-194">Request</span></span>
<span data-ttu-id="6442e-195">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6442e-195">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
Content-type: application/json
Content-length: 602

{
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "version": 7,
  "pinMinimumLength": 0,
  "pinMaximumLength": 0,
  "pinUppercaseCharactersUsage": "required",
  "pinLowercaseCharactersUsage": "required",
  "pinSpecialCharactersUsage": "required",
  "state": "enabled",
  "securityDeviceRequired": true,
  "unlockWithBiometricsEnabled": true,
  "remotePassportEnabled": true,
  "pinPreviousBlockCount": 5,
  "pinExpirationInDays": 3,
  "enhancedBiometricsState": "enabled"
}
```

### <a name="response"></a><span data-ttu-id="6442e-196">响应</span><span class="sxs-lookup"><span data-stu-id="6442e-196">Response</span></span>
<span data-ttu-id="6442e-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6442e-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 801

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentWindowsHelloForBusinessConfiguration",
  "id": "3068e0cd-e0cd-3068-cde0-6830cde06830",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "version": 7,
  "pinMinimumLength": 0,
  "pinMaximumLength": 0,
  "pinUppercaseCharactersUsage": "required",
  "pinLowercaseCharactersUsage": "required",
  "pinSpecialCharactersUsage": "required",
  "state": "enabled",
  "securityDeviceRequired": true,
  "unlockWithBiometricsEnabled": true,
  "remotePassportEnabled": true,
  "pinPreviousBlockCount": 5,
  "pinExpirationInDays": 3,
  "enhancedBiometricsState": "enabled"
}
```




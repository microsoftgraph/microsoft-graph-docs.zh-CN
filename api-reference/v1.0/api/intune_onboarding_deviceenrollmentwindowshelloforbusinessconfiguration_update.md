# <a name="update-deviceenrollmentwindowshelloforbusinessconfiguration"></a><span data-ttu-id="b3c5b-101">更新 deviceEnrollmentWindowsHelloForBusinessConfiguration</span><span class="sxs-lookup"><span data-stu-id="b3c5b-101">Update deviceEnrollmentWindowsHelloForBusinessConfiguration</span></span>

> <span data-ttu-id="b3c5b-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="b3c5b-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b3c5b-103">更新 [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b3c5b-103">Update the properties of a [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b3c5b-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="b3c5b-104">Prerequisites</span></span>
<span data-ttu-id="b3c5b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="b3c5b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b3c5b-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="b3c5b-107">Permission type</span></span>|<span data-ttu-id="b3c5b-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b3c5b-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b3c5b-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b3c5b-109">Delegated (work or school account)</span></span>|<span data-ttu-id="b3c5b-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3c5b-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="b3c5b-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b3c5b-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b3c5b-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="b3c5b-112">Not supported.</span></span>|
|<span data-ttu-id="b3c5b-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="b3c5b-113">Application</span></span>|<span data-ttu-id="b3c5b-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="b3c5b-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b3c5b-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b3c5b-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="b3c5b-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="b3c5b-116">Request headers</span></span>
|<span data-ttu-id="b3c5b-117">标头</span><span class="sxs-lookup"><span data-stu-id="b3c5b-117">Header</span></span>|<span data-ttu-id="b3c5b-118">值</span><span class="sxs-lookup"><span data-stu-id="b3c5b-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b3c5b-119">授权</span><span class="sxs-lookup"><span data-stu-id="b3c5b-119">Authorization</span></span>|<span data-ttu-id="b3c5b-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b3c5b-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b3c5b-121">接受</span><span class="sxs-lookup"><span data-stu-id="b3c5b-121">Accept</span></span>|<span data-ttu-id="b3c5b-122">application/json</span><span class="sxs-lookup"><span data-stu-id="b3c5b-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b3c5b-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="b3c5b-123">Request body</span></span>
<span data-ttu-id="b3c5b-124">在请求正文中，提供 [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b3c5b-124">In the request body, supply a JSON representation for the [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration.md) object.</span></span>

<span data-ttu-id="b3c5b-125">下表显示创建 [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="b3c5b-125">The following table shows the properties that are required when you create the [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration.md).</span></span>

|<span data-ttu-id="b3c5b-126">属性</span><span class="sxs-lookup"><span data-stu-id="b3c5b-126">Property</span></span>|<span data-ttu-id="b3c5b-127">类型</span><span class="sxs-lookup"><span data-stu-id="b3c5b-127">Type</span></span>|<span data-ttu-id="b3c5b-128">说明</span><span class="sxs-lookup"><span data-stu-id="b3c5b-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b3c5b-129">ID</span><span class="sxs-lookup"><span data-stu-id="b3c5b-129">id</span></span>|<span data-ttu-id="b3c5b-130">字符串</span><span class="sxs-lookup"><span data-stu-id="b3c5b-130">String</span></span>|<span data-ttu-id="b3c5b-131">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b3c5b-131">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="b3c5b-132">displayName</span><span class="sxs-lookup"><span data-stu-id="b3c5b-132">displayName</span></span>|<span data-ttu-id="b3c5b-133">字符串</span><span class="sxs-lookup"><span data-stu-id="b3c5b-133">String</span></span>|<span data-ttu-id="b3c5b-134">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b3c5b-134">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="b3c5b-135">说明</span><span class="sxs-lookup"><span data-stu-id="b3c5b-135">description</span></span>|<span data-ttu-id="b3c5b-136">字符串</span><span class="sxs-lookup"><span data-stu-id="b3c5b-136">String</span></span>|<span data-ttu-id="b3c5b-137">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b3c5b-137">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="b3c5b-138">优先级</span><span class="sxs-lookup"><span data-stu-id="b3c5b-138">priority</span></span>|<span data-ttu-id="b3c5b-139">Int32</span><span class="sxs-lookup"><span data-stu-id="b3c5b-139">Int32</span></span>|<span data-ttu-id="b3c5b-140">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b3c5b-140">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="b3c5b-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b3c5b-141">createdDateTime</span></span>|<span data-ttu-id="b3c5b-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b3c5b-142">DateTimeOffset</span></span>|<span data-ttu-id="b3c5b-143">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b3c5b-143">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="b3c5b-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b3c5b-144">lastModifiedDateTime</span></span>|<span data-ttu-id="b3c5b-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b3c5b-145">DateTimeOffset</span></span>|<span data-ttu-id="b3c5b-146">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b3c5b-146">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="b3c5b-147">版本</span><span class="sxs-lookup"><span data-stu-id="b3c5b-147">version</span></span>|<span data-ttu-id="b3c5b-148">Int32</span><span class="sxs-lookup"><span data-stu-id="b3c5b-148">Int32</span></span>|<span data-ttu-id="b3c5b-149">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b3c5b-149">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="b3c5b-150">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="b3c5b-150">pinMinimumLength</span></span>|<span data-ttu-id="b3c5b-151">Int32</span><span class="sxs-lookup"><span data-stu-id="b3c5b-151">Int32</span></span>|<span data-ttu-id="b3c5b-152">尚未记录</span><span class="sxs-lookup"><span data-stu-id="b3c5b-152">Not yet documented</span></span>|
|<span data-ttu-id="b3c5b-153">pinMaximumLength</span><span class="sxs-lookup"><span data-stu-id="b3c5b-153">pinMaximumLength</span></span>|<span data-ttu-id="b3c5b-154">Int32</span><span class="sxs-lookup"><span data-stu-id="b3c5b-154">Int32</span></span>|<span data-ttu-id="b3c5b-155">尚未记录</span><span class="sxs-lookup"><span data-stu-id="b3c5b-155">Not yet documented</span></span>|
|<span data-ttu-id="b3c5b-156">pinUppercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="b3c5b-156">pinUppercaseCharactersUsage</span></span>|[<span data-ttu-id="b3c5b-157">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="b3c5b-157">windowsHelloForBusinessPinUsage</span></span>](../resources/intune_onboarding_windowshelloforbusinesspinusage.md)|<span data-ttu-id="b3c5b-p102">尚未记录。可取值为：`allowed`、`required`、`disallowed`。</span><span class="sxs-lookup"><span data-stu-id="b3c5b-p102">Not yet documented Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="b3c5b-160">pinLowercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="b3c5b-160">pinLowercaseCharactersUsage</span></span>|[<span data-ttu-id="b3c5b-161">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="b3c5b-161">windowsHelloForBusinessPinUsage</span></span>](../resources/intune_onboarding_windowshelloforbusinesspinusage.md)|<span data-ttu-id="b3c5b-p103">尚未记录。可取值为：`allowed`、`required`、`disallowed`。</span><span class="sxs-lookup"><span data-stu-id="b3c5b-p103">Not yet documented Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="b3c5b-164">pinSpecialCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="b3c5b-164">pinSpecialCharactersUsage</span></span>|[<span data-ttu-id="b3c5b-165">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="b3c5b-165">windowsHelloForBusinessPinUsage</span></span>](../resources/intune_onboarding_windowshelloforbusinesspinusage.md)|<span data-ttu-id="b3c5b-p104">尚未记录。可取值为：`allowed`、`required`、`disallowed`。</span><span class="sxs-lookup"><span data-stu-id="b3c5b-p104">Not yet documented Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="b3c5b-168">state</span><span class="sxs-lookup"><span data-stu-id="b3c5b-168">state</span></span>|[<span data-ttu-id="b3c5b-169">enablement</span><span class="sxs-lookup"><span data-stu-id="b3c5b-169">Enablement</span></span>](../resources/intune_onboarding_enablement.md)|<span data-ttu-id="b3c5b-p105">尚未记录。可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="b3c5b-p105">Not yet documented Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="b3c5b-172">securityDeviceRequired</span><span class="sxs-lookup"><span data-stu-id="b3c5b-172">securityDeviceRequired</span></span>|<span data-ttu-id="b3c5b-173">布尔值</span><span class="sxs-lookup"><span data-stu-id="b3c5b-173">Boolean</span></span>|<span data-ttu-id="b3c5b-174">尚未记录</span><span class="sxs-lookup"><span data-stu-id="b3c5b-174">Not yet documented</span></span>|
|<span data-ttu-id="b3c5b-175">unlockWithBiometricsEnabled</span><span class="sxs-lookup"><span data-stu-id="b3c5b-175">unlockWithBiometricsEnabled</span></span>|<span data-ttu-id="b3c5b-176">布尔值</span><span class="sxs-lookup"><span data-stu-id="b3c5b-176">Boolean</span></span>|<span data-ttu-id="b3c5b-177">尚未记录</span><span class="sxs-lookup"><span data-stu-id="b3c5b-177">Not yet documented</span></span>|
|<span data-ttu-id="b3c5b-178">remotePassportEnabled</span><span class="sxs-lookup"><span data-stu-id="b3c5b-178">remotePassportEnabled</span></span>|<span data-ttu-id="b3c5b-179">布尔值</span><span class="sxs-lookup"><span data-stu-id="b3c5b-179">Boolean</span></span>|<span data-ttu-id="b3c5b-180">尚未记录</span><span class="sxs-lookup"><span data-stu-id="b3c5b-180">Not yet documented</span></span>|
|<span data-ttu-id="b3c5b-181">pinPreviousBlockCount</span><span class="sxs-lookup"><span data-stu-id="b3c5b-181">pinPreviousBlockCount</span></span>|<span data-ttu-id="b3c5b-182">Int32</span><span class="sxs-lookup"><span data-stu-id="b3c5b-182">Int32</span></span>|<span data-ttu-id="b3c5b-183">尚未记录</span><span class="sxs-lookup"><span data-stu-id="b3c5b-183">Not yet documented</span></span>|
|<span data-ttu-id="b3c5b-184">pinExpirationInDays</span><span class="sxs-lookup"><span data-stu-id="b3c5b-184">pinExpirationInDays</span></span>|<span data-ttu-id="b3c5b-185">Int32</span><span class="sxs-lookup"><span data-stu-id="b3c5b-185">Int32</span></span>|<span data-ttu-id="b3c5b-186">尚未记录</span><span class="sxs-lookup"><span data-stu-id="b3c5b-186">Not yet documented</span></span>|
|<span data-ttu-id="b3c5b-187">enhancedBiometricsState</span><span class="sxs-lookup"><span data-stu-id="b3c5b-187">enhancedBiometricsState</span></span>|[<span data-ttu-id="b3c5b-188">enablement</span><span class="sxs-lookup"><span data-stu-id="b3c5b-188">Enablement</span></span>](../resources/intune_onboarding_enablement.md)|<span data-ttu-id="b3c5b-p106">尚未记录。可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="b3c5b-p106">Not yet documented Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|



## <a name="response"></a><span data-ttu-id="b3c5b-191">响应</span><span class="sxs-lookup"><span data-stu-id="b3c5b-191">Response</span></span>
<span data-ttu-id="b3c5b-192">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b3c5b-192">If successful, this method returns a `200 OK` response code and an updated [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b3c5b-193">示例</span><span class="sxs-lookup"><span data-stu-id="b3c5b-193">Example</span></span>
### <a name="request"></a><span data-ttu-id="b3c5b-194">请求</span><span class="sxs-lookup"><span data-stu-id="b3c5b-194">Request</span></span>
<span data-ttu-id="b3c5b-195">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b3c5b-195">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b3c5b-196">响应</span><span class="sxs-lookup"><span data-stu-id="b3c5b-196">Response</span></span>
<span data-ttu-id="b3c5b-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b3c5b-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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









# <a name="update-deviceenrollmentplatformrestrictionsconfiguration"></a><span data-ttu-id="3c0ae-101">更新 deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="3c0ae-101">Update deviceEnrollmentPlatformRestrictionsConfiguration</span></span>

> <span data-ttu-id="3c0ae-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="3c0ae-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3c0ae-103">更新 [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune_onboarding_deviceenrollmentplatformrestrictionsconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="3c0ae-103">Update the properties of a [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune_onboarding_deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3c0ae-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="3c0ae-104">Prerequisites</span></span>
<span data-ttu-id="3c0ae-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="3c0ae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="3c0ae-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="3c0ae-107">Permission type</span></span>|<span data-ttu-id="3c0ae-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="3c0ae-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3c0ae-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3c0ae-109">Delegated (work or school account)</span></span>|<span data-ttu-id="3c0ae-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c0ae-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="3c0ae-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3c0ae-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3c0ae-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="3c0ae-112">Not supported.</span></span>|
|<span data-ttu-id="3c0ae-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="3c0ae-113">Application</span></span>|<span data-ttu-id="3c0ae-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="3c0ae-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3c0ae-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3c0ae-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="3c0ae-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="3c0ae-116">Request headers</span></span>
|<span data-ttu-id="3c0ae-117">标头</span><span class="sxs-lookup"><span data-stu-id="3c0ae-117">Header</span></span>|<span data-ttu-id="3c0ae-118">值</span><span class="sxs-lookup"><span data-stu-id="3c0ae-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3c0ae-119">授权</span><span class="sxs-lookup"><span data-stu-id="3c0ae-119">Authorization</span></span>|<span data-ttu-id="3c0ae-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="3c0ae-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3c0ae-121">Accept</span><span class="sxs-lookup"><span data-stu-id="3c0ae-121">Accept</span></span>|<span data-ttu-id="3c0ae-122">application/json</span><span class="sxs-lookup"><span data-stu-id="3c0ae-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3c0ae-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="3c0ae-123">Request body</span></span>
<span data-ttu-id="3c0ae-124">在请求正文中，提供 [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune_onboarding_deviceenrollmentplatformrestrictionsconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3c0ae-124">In the request body, supply a JSON representation for the [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune_onboarding_deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>

<span data-ttu-id="3c0ae-125">下表显示创建 [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune_onboarding_deviceenrollmentplatformrestrictionsconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="3c0ae-125">The following table shows the properties that are required when you create the [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune_onboarding_deviceenrollmentplatformrestrictionsconfiguration.md).</span></span>

|<span data-ttu-id="3c0ae-126">属性</span><span class="sxs-lookup"><span data-stu-id="3c0ae-126">Property</span></span>|<span data-ttu-id="3c0ae-127">类型</span><span class="sxs-lookup"><span data-stu-id="3c0ae-127">Type</span></span>|<span data-ttu-id="3c0ae-128">说明</span><span class="sxs-lookup"><span data-stu-id="3c0ae-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3c0ae-129">ID</span><span class="sxs-lookup"><span data-stu-id="3c0ae-129">id</span></span>|<span data-ttu-id="3c0ae-130">字符串</span><span class="sxs-lookup"><span data-stu-id="3c0ae-130">String</span></span>|<span data-ttu-id="3c0ae-131">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3c0ae-131">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="3c0ae-132">displayName</span><span class="sxs-lookup"><span data-stu-id="3c0ae-132">displayName</span></span>|<span data-ttu-id="3c0ae-133">字符串</span><span class="sxs-lookup"><span data-stu-id="3c0ae-133">String</span></span>|<span data-ttu-id="3c0ae-134">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3c0ae-134">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="3c0ae-135">说明</span><span class="sxs-lookup"><span data-stu-id="3c0ae-135">description</span></span>|<span data-ttu-id="3c0ae-136">字符串</span><span class="sxs-lookup"><span data-stu-id="3c0ae-136">String</span></span>|<span data-ttu-id="3c0ae-137">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3c0ae-137">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="3c0ae-138">priority</span><span class="sxs-lookup"><span data-stu-id="3c0ae-138">priority</span></span>|<span data-ttu-id="3c0ae-139">Int32</span><span class="sxs-lookup"><span data-stu-id="3c0ae-139">Int32</span></span>|<span data-ttu-id="3c0ae-140">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3c0ae-140">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="3c0ae-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3c0ae-141">createdDateTime</span></span>|<span data-ttu-id="3c0ae-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3c0ae-142">DateTimeOffset</span></span>|<span data-ttu-id="3c0ae-143">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3c0ae-143">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="3c0ae-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3c0ae-144">lastModifiedDateTime</span></span>|<span data-ttu-id="3c0ae-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3c0ae-145">DateTimeOffset</span></span>|<span data-ttu-id="3c0ae-146">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3c0ae-146">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="3c0ae-147">version</span><span class="sxs-lookup"><span data-stu-id="3c0ae-147">version</span></span>|<span data-ttu-id="3c0ae-148">Int32</span><span class="sxs-lookup"><span data-stu-id="3c0ae-148">Int32</span></span>|<span data-ttu-id="3c0ae-149">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3c0ae-149">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="3c0ae-150">iosRestriction</span><span class="sxs-lookup"><span data-stu-id="3c0ae-150">iosRestriction</span></span>|[<span data-ttu-id="3c0ae-151">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="3c0ae-151">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune_onboarding_deviceenrollmentplatformrestriction.md)|<span data-ttu-id="3c0ae-152">尚未记录</span><span class="sxs-lookup"><span data-stu-id="3c0ae-152">Not yet documented</span></span>|
|<span data-ttu-id="3c0ae-153">windowsRestriction</span><span class="sxs-lookup"><span data-stu-id="3c0ae-153">windowsRestriction</span></span>|[<span data-ttu-id="3c0ae-154">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="3c0ae-154">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune_onboarding_deviceenrollmentplatformrestriction.md)|<span data-ttu-id="3c0ae-155">尚未记录</span><span class="sxs-lookup"><span data-stu-id="3c0ae-155">Not yet documented</span></span>|
|<span data-ttu-id="3c0ae-156">windowsMobileRestriction</span><span class="sxs-lookup"><span data-stu-id="3c0ae-156">windowsMobileRestriction</span></span>|[<span data-ttu-id="3c0ae-157">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="3c0ae-157">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune_onboarding_deviceenrollmentplatformrestriction.md)|<span data-ttu-id="3c0ae-158">尚未记录</span><span class="sxs-lookup"><span data-stu-id="3c0ae-158">Not yet documented</span></span>|
|<span data-ttu-id="3c0ae-159">androidRestriction</span><span class="sxs-lookup"><span data-stu-id="3c0ae-159">androidRestriction</span></span>|[<span data-ttu-id="3c0ae-160">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="3c0ae-160">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune_onboarding_deviceenrollmentplatformrestriction.md)|<span data-ttu-id="3c0ae-161">尚未记录</span><span class="sxs-lookup"><span data-stu-id="3c0ae-161">Not yet documented</span></span>|
|<span data-ttu-id="3c0ae-162">macOSRestriction</span><span class="sxs-lookup"><span data-stu-id="3c0ae-162">macOSRestriction</span></span>|[<span data-ttu-id="3c0ae-163">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="3c0ae-163">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune_onboarding_deviceenrollmentplatformrestriction.md)|<span data-ttu-id="3c0ae-164">尚未记录</span><span class="sxs-lookup"><span data-stu-id="3c0ae-164">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="3c0ae-165">响应</span><span class="sxs-lookup"><span data-stu-id="3c0ae-165">Response</span></span>
<span data-ttu-id="3c0ae-166">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune_onboarding_deviceenrollmentplatformrestrictionsconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3c0ae-166">If successful, this method returns a `200 OK` response code and an updated [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune_onboarding_deviceenrollmentplatformrestrictionsconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3c0ae-167">示例</span><span class="sxs-lookup"><span data-stu-id="3c0ae-167">Example</span></span>
### <a name="request"></a><span data-ttu-id="3c0ae-168">请求</span><span class="sxs-lookup"><span data-stu-id="3c0ae-168">Request</span></span>
<span data-ttu-id="3c0ae-169">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3c0ae-169">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
Content-type: application/json
Content-length: 1626

{
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "version": 7,
  "iosRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  },
  "windowsRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  },
  "windowsMobileRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  },
  "androidRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  },
  "macOSRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  }
}
```

### <a name="response"></a><span data-ttu-id="3c0ae-170">响应</span><span class="sxs-lookup"><span data-stu-id="3c0ae-170">Response</span></span>
<span data-ttu-id="3c0ae-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3c0ae-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1822

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentPlatformRestrictionsConfiguration",
  "id": "3acb2d75-2d75-3acb-752d-cb3a752dcb3a",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "version": 7,
  "iosRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  },
  "windowsRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  },
  "windowsMobileRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  },
  "androidRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  },
  "macOSRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  }
}
```









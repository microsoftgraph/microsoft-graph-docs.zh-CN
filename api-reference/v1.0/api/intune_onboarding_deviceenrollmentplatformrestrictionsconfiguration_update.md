# <a name="update-deviceenrollmentplatformrestrictionsconfiguration"></a><span data-ttu-id="8655d-101">更新 deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="8655d-101">Update deviceEnrollmentPlatformRestrictionsConfiguration</span></span>

> <span data-ttu-id="8655d-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="8655d-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8655d-103">更新 [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune_onboarding_deviceenrollmentplatformrestrictionsconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="8655d-103">Update the properties of a [calendar](../resources/intune_onboarding_deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8655d-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="8655d-104">Prerequisites</span></span>
<span data-ttu-id="8655d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="8655d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="8655d-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="8655d-107">Permission type</span></span>|<span data-ttu-id="8655d-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="8655d-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8655d-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8655d-109">Delegated (work or school account)</span></span>|<span data-ttu-id="8655d-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8655d-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="8655d-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8655d-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8655d-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="8655d-112">Not supported.</span></span>|
|<span data-ttu-id="8655d-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="8655d-113">Application</span></span>|<span data-ttu-id="8655d-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="8655d-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8655d-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8655d-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="8655d-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="8655d-116">Request headers</span></span>
|<span data-ttu-id="8655d-117">标头</span><span class="sxs-lookup"><span data-stu-id="8655d-117">Header</span></span>|<span data-ttu-id="8655d-118">值</span><span class="sxs-lookup"><span data-stu-id="8655d-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8655d-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="8655d-119">Authorization</span></span>|<span data-ttu-id="8655d-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="8655d-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="8655d-121">Accept</span><span class="sxs-lookup"><span data-stu-id="8655d-121">Accept</span></span>|<span data-ttu-id="8655d-122">application/json</span><span class="sxs-lookup"><span data-stu-id="8655d-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8655d-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="8655d-123">Request body</span></span>
<span data-ttu-id="8655d-124">在请求正文中，提供 [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune_onboarding_deviceenrollmentplatformrestrictionsconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8655d-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_onboarding_deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>

<span data-ttu-id="8655d-125">下表显示创建 [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune_onboarding_deviceenrollmentplatformrestrictionsconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="8655d-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="8655d-126">属性</span><span class="sxs-lookup"><span data-stu-id="8655d-126">Property</span></span>|<span data-ttu-id="8655d-127">类型</span><span class="sxs-lookup"><span data-stu-id="8655d-127">Type</span></span>|<span data-ttu-id="8655d-128">说明</span><span class="sxs-lookup"><span data-stu-id="8655d-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8655d-129">id</span><span class="sxs-lookup"><span data-stu-id="8655d-129">id</span></span>|<span data-ttu-id="8655d-130">String</span><span class="sxs-lookup"><span data-stu-id="8655d-130">String</span></span>|<span data-ttu-id="8655d-131">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8655d-131">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="8655d-132">displayName</span><span class="sxs-lookup"><span data-stu-id="8655d-132">displayName</span></span>|<span data-ttu-id="8655d-133">String</span><span class="sxs-lookup"><span data-stu-id="8655d-133">String</span></span>|<span data-ttu-id="8655d-134">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8655d-134">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="8655d-135">description</span><span class="sxs-lookup"><span data-stu-id="8655d-135">description</span></span>|<span data-ttu-id="8655d-136">String</span><span class="sxs-lookup"><span data-stu-id="8655d-136">String</span></span>|<span data-ttu-id="8655d-137">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8655d-137">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="8655d-138">priority</span><span class="sxs-lookup"><span data-stu-id="8655d-138">priority</span></span>|<span data-ttu-id="8655d-139">Int32</span><span class="sxs-lookup"><span data-stu-id="8655d-139">Int32</span></span>|<span data-ttu-id="8655d-140">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8655d-140">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="8655d-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8655d-141">createdDateTime</span></span>|<span data-ttu-id="8655d-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8655d-142">DateTimeOffset</span></span>|<span data-ttu-id="8655d-143">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8655d-143">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="8655d-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8655d-144">lastModifiedDateTime</span></span>|<span data-ttu-id="8655d-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8655d-145">DateTimeOffset</span></span>|<span data-ttu-id="8655d-146">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8655d-146">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="8655d-147">version</span><span class="sxs-lookup"><span data-stu-id="8655d-147">version</span></span>|<span data-ttu-id="8655d-148">Int32</span><span class="sxs-lookup"><span data-stu-id="8655d-148">Int32</span></span>|<span data-ttu-id="8655d-149">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8655d-149">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="8655d-150">iosRestriction</span><span class="sxs-lookup"><span data-stu-id="8655d-150">iosRestriction</span></span>|[<span data-ttu-id="8655d-151">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="8655d-151">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune_onboarding_deviceenrollmentplatformrestriction.md)|<span data-ttu-id="8655d-152">尚未记录</span><span class="sxs-lookup"><span data-stu-id="8655d-152">Not yet documented</span></span>|
|<span data-ttu-id="8655d-153">windowsRestriction</span><span class="sxs-lookup"><span data-stu-id="8655d-153">windowsRestriction</span></span>|[<span data-ttu-id="8655d-154">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="8655d-154">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune_onboarding_deviceenrollmentplatformrestriction.md)|<span data-ttu-id="8655d-155">尚未记录</span><span class="sxs-lookup"><span data-stu-id="8655d-155">Not yet documented</span></span>|
|<span data-ttu-id="8655d-156">windowsMobileRestriction</span><span class="sxs-lookup"><span data-stu-id="8655d-156">windowsMobileRestriction</span></span>|[<span data-ttu-id="8655d-157">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="8655d-157">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune_onboarding_deviceenrollmentplatformrestriction.md)|<span data-ttu-id="8655d-158">尚未记录</span><span class="sxs-lookup"><span data-stu-id="8655d-158">Not yet documented</span></span>|
|<span data-ttu-id="8655d-159">androidRestriction</span><span class="sxs-lookup"><span data-stu-id="8655d-159">androidRestriction</span></span>|[<span data-ttu-id="8655d-160">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="8655d-160">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune_onboarding_deviceenrollmentplatformrestriction.md)|<span data-ttu-id="8655d-161">尚未记录</span><span class="sxs-lookup"><span data-stu-id="8655d-161">Not yet documented</span></span>|
|<span data-ttu-id="8655d-162">macOSRestriction</span><span class="sxs-lookup"><span data-stu-id="8655d-162">macOSRestriction</span></span>|[<span data-ttu-id="8655d-163">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="8655d-163">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune_onboarding_deviceenrollmentplatformrestriction.md)|<span data-ttu-id="8655d-164">尚未记录</span><span class="sxs-lookup"><span data-stu-id="8655d-164">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="8655d-165">响应</span><span class="sxs-lookup"><span data-stu-id="8655d-165">Response</span></span>
<span data-ttu-id="8655d-166">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune_onboarding_deviceenrollmentplatformrestrictionsconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8655d-166">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_onboarding_deviceenrollmentplatformrestrictionsconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8655d-167">示例</span><span class="sxs-lookup"><span data-stu-id="8655d-167">Example</span></span>
### <a name="request"></a><span data-ttu-id="8655d-168">请求</span><span class="sxs-lookup"><span data-stu-id="8655d-168">Request</span></span>
<span data-ttu-id="8655d-169">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8655d-169">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8655d-170">响应</span><span class="sxs-lookup"><span data-stu-id="8655d-170">Response</span></span>
<span data-ttu-id="8655d-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8655d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




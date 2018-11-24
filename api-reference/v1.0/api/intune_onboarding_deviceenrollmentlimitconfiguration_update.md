# <a name="update-deviceenrollmentlimitconfiguration"></a><span data-ttu-id="0324a-101">更新 deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="0324a-101">Update deviceEnrollmentLimitConfiguration</span></span>

> <span data-ttu-id="0324a-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="0324a-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0324a-103">更新 [deviceEnrollmentLimitConfiguration](../resources/intune_onboarding_deviceenrollmentlimitconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="0324a-103">Update the properties of a [deviceEnrollmentLimitConfiguration](../resources/intune_onboarding_deviceenrollmentlimitconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0324a-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="0324a-104">Prerequisites</span></span>
<span data-ttu-id="0324a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="0324a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="0324a-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="0324a-107">Permission type</span></span>|<span data-ttu-id="0324a-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="0324a-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0324a-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0324a-109">Delegated (work or school account)</span></span>|<span data-ttu-id="0324a-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0324a-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="0324a-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0324a-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0324a-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="0324a-112">Not supported.</span></span>|
|<span data-ttu-id="0324a-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="0324a-113">Application</span></span>|<span data-ttu-id="0324a-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="0324a-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0324a-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0324a-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="0324a-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="0324a-116">Request headers</span></span>
|<span data-ttu-id="0324a-117">标头</span><span class="sxs-lookup"><span data-stu-id="0324a-117">Header</span></span>|<span data-ttu-id="0324a-118">值</span><span class="sxs-lookup"><span data-stu-id="0324a-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0324a-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="0324a-119">Authorization</span></span>|<span data-ttu-id="0324a-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="0324a-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0324a-121">Accept</span><span class="sxs-lookup"><span data-stu-id="0324a-121">Accept</span></span>|<span data-ttu-id="0324a-122">application/json</span><span class="sxs-lookup"><span data-stu-id="0324a-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0324a-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="0324a-123">Request body</span></span>
<span data-ttu-id="0324a-124">在请求正文中，提供 [deviceEnrollmentLimitConfiguration](../resources/intune_onboarding_deviceenrollmentlimitconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0324a-124">In the request body, supply a JSON representation for the [deviceEnrollmentLimitConfiguration](../resources/intune_onboarding_deviceenrollmentlimitconfiguration.md) object.</span></span>

<span data-ttu-id="0324a-125">下表显示创建 [deviceEnrollmentLimitConfiguration](../resources/intune_onboarding_deviceenrollmentlimitconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="0324a-125">The following table shows the properties that are required when you create the [deviceEnrollmentLimitConfiguration](../resources/intune_onboarding_deviceenrollmentlimitconfiguration.md).</span></span>

|<span data-ttu-id="0324a-126">属性</span><span class="sxs-lookup"><span data-stu-id="0324a-126">Property</span></span>|<span data-ttu-id="0324a-127">类型</span><span class="sxs-lookup"><span data-stu-id="0324a-127">Type</span></span>|<span data-ttu-id="0324a-128">说明</span><span class="sxs-lookup"><span data-stu-id="0324a-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0324a-129">id</span><span class="sxs-lookup"><span data-stu-id="0324a-129">id</span></span>|<span data-ttu-id="0324a-130">String</span><span class="sxs-lookup"><span data-stu-id="0324a-130">String</span></span>|<span data-ttu-id="0324a-131">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0324a-131">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="0324a-132">displayName</span><span class="sxs-lookup"><span data-stu-id="0324a-132">displayName</span></span>|<span data-ttu-id="0324a-133">String</span><span class="sxs-lookup"><span data-stu-id="0324a-133">String</span></span>|<span data-ttu-id="0324a-134">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0324a-134">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="0324a-135">description</span><span class="sxs-lookup"><span data-stu-id="0324a-135">description</span></span>|<span data-ttu-id="0324a-136">String</span><span class="sxs-lookup"><span data-stu-id="0324a-136">String</span></span>|<span data-ttu-id="0324a-137">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0324a-137">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="0324a-138">priority</span><span class="sxs-lookup"><span data-stu-id="0324a-138">priority</span></span>|<span data-ttu-id="0324a-139">Int32</span><span class="sxs-lookup"><span data-stu-id="0324a-139">Int32</span></span>|<span data-ttu-id="0324a-140">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0324a-140">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="0324a-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0324a-141">createdDateTime</span></span>|<span data-ttu-id="0324a-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0324a-142">DateTimeOffset</span></span>|<span data-ttu-id="0324a-143">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0324a-143">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="0324a-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0324a-144">lastModifiedDateTime</span></span>|<span data-ttu-id="0324a-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0324a-145">DateTimeOffset</span></span>|<span data-ttu-id="0324a-146">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0324a-146">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="0324a-147">version</span><span class="sxs-lookup"><span data-stu-id="0324a-147">version</span></span>|<span data-ttu-id="0324a-148">Int32</span><span class="sxs-lookup"><span data-stu-id="0324a-148">Int32</span></span>|<span data-ttu-id="0324a-149">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0324a-149">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="0324a-150">limit</span><span class="sxs-lookup"><span data-stu-id="0324a-150">limit</span></span>|<span data-ttu-id="0324a-151">Int32</span><span class="sxs-lookup"><span data-stu-id="0324a-151">Int32</span></span>|<span data-ttu-id="0324a-152">尚未记录</span><span class="sxs-lookup"><span data-stu-id="0324a-152">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="0324a-153">响应</span><span class="sxs-lookup"><span data-stu-id="0324a-153">Response</span></span>
<span data-ttu-id="0324a-154">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [deviceEnrollmentLimitConfiguration](../resources/intune_onboarding_deviceenrollmentlimitconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0324a-154">If successful, this method returns a `200 OK` response code and an updated [deviceEnrollmentLimitConfiguration](../resources/intune_onboarding_deviceenrollmentlimitconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0324a-155">示例</span><span class="sxs-lookup"><span data-stu-id="0324a-155">Example</span></span>
### <a name="request"></a><span data-ttu-id="0324a-156">请求</span><span class="sxs-lookup"><span data-stu-id="0324a-156">Request</span></span>
<span data-ttu-id="0324a-157">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0324a-157">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
Content-type: application/json
Content-length: 205

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentLimitConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "version": 7,
  "limit": 5
}
```

### <a name="response"></a><span data-ttu-id="0324a-158">响应</span><span class="sxs-lookup"><span data-stu-id="0324a-158">Response</span></span>
<span data-ttu-id="0324a-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0324a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 377

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentLimitConfiguration",
  "id": "4f8c4e4c-4e4c-4f8c-4c4e-8c4f4c4e8c4f",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "version": 7,
  "limit": 5
}
```




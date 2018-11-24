# <a name="create-deviceenrollmentlimitconfiguration"></a><span data-ttu-id="43f06-101">创建 deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="43f06-101">Create deviceEnrollmentLimitConfiguration</span></span>

> <span data-ttu-id="43f06-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="43f06-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="43f06-103">创建新的 [deviceEnrollmentLimitConfiguration](../resources/intune_onboarding_deviceenrollmentlimitconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="43f06-103">Create a new [deviceEnrollmentLimitConfiguration](../resources/intune_onboarding_deviceenrollmentlimitconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="43f06-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="43f06-104">Prerequisites</span></span>
<span data-ttu-id="43f06-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="43f06-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="43f06-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="43f06-107">Permission type</span></span>|<span data-ttu-id="43f06-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="43f06-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="43f06-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="43f06-109">Delegated (work or school account)</span></span>|<span data-ttu-id="43f06-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="43f06-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="43f06-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="43f06-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="43f06-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="43f06-112">Not supported.</span></span>|
|<span data-ttu-id="43f06-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="43f06-113">Application</span></span>|<span data-ttu-id="43f06-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="43f06-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="43f06-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="43f06-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="43f06-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="43f06-116">Request headers</span></span>
|<span data-ttu-id="43f06-117">标头</span><span class="sxs-lookup"><span data-stu-id="43f06-117">Header</span></span>|<span data-ttu-id="43f06-118">值</span><span class="sxs-lookup"><span data-stu-id="43f06-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="43f06-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="43f06-119">Authorization</span></span>|<span data-ttu-id="43f06-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="43f06-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="43f06-121">Accept</span><span class="sxs-lookup"><span data-stu-id="43f06-121">Accept</span></span>|<span data-ttu-id="43f06-122">application/json</span><span class="sxs-lookup"><span data-stu-id="43f06-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="43f06-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="43f06-123">Request body</span></span>
<span data-ttu-id="43f06-124">在请求正文中，提供 deviceEnrollmentLimitConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="43f06-124">In the request body, supply a JSON representation for the deviceEnrollmentLimitConfiguration object.</span></span>

<span data-ttu-id="43f06-125">下表显示创建 deviceEnrollmentLimitConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="43f06-125">The following table shows the properties that are required when you create the deviceEnrollmentLimitConfiguration.</span></span>

|<span data-ttu-id="43f06-126">属性</span><span class="sxs-lookup"><span data-stu-id="43f06-126">Property</span></span>|<span data-ttu-id="43f06-127">类型</span><span class="sxs-lookup"><span data-stu-id="43f06-127">Type</span></span>|<span data-ttu-id="43f06-128">说明</span><span class="sxs-lookup"><span data-stu-id="43f06-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="43f06-129">id</span><span class="sxs-lookup"><span data-stu-id="43f06-129">id</span></span>|<span data-ttu-id="43f06-130">String</span><span class="sxs-lookup"><span data-stu-id="43f06-130">String</span></span>|<span data-ttu-id="43f06-131">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="43f06-131">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="43f06-132">displayName</span><span class="sxs-lookup"><span data-stu-id="43f06-132">displayName</span></span>|<span data-ttu-id="43f06-133">String</span><span class="sxs-lookup"><span data-stu-id="43f06-133">String</span></span>|<span data-ttu-id="43f06-134">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="43f06-134">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="43f06-135">description</span><span class="sxs-lookup"><span data-stu-id="43f06-135">description</span></span>|<span data-ttu-id="43f06-136">String</span><span class="sxs-lookup"><span data-stu-id="43f06-136">String</span></span>|<span data-ttu-id="43f06-137">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="43f06-137">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="43f06-138">priority</span><span class="sxs-lookup"><span data-stu-id="43f06-138">priority</span></span>|<span data-ttu-id="43f06-139">Int32</span><span class="sxs-lookup"><span data-stu-id="43f06-139">Int32</span></span>|<span data-ttu-id="43f06-140">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="43f06-140">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="43f06-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="43f06-141">createdDateTime</span></span>|<span data-ttu-id="43f06-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="43f06-142">DateTimeOffset</span></span>|<span data-ttu-id="43f06-143">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="43f06-143">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="43f06-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="43f06-144">lastModifiedDateTime</span></span>|<span data-ttu-id="43f06-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="43f06-145">DateTimeOffset</span></span>|<span data-ttu-id="43f06-146">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="43f06-146">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="43f06-147">version</span><span class="sxs-lookup"><span data-stu-id="43f06-147">version</span></span>|<span data-ttu-id="43f06-148">Int32</span><span class="sxs-lookup"><span data-stu-id="43f06-148">Int32</span></span>|<span data-ttu-id="43f06-149">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="43f06-149">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="43f06-150">limit</span><span class="sxs-lookup"><span data-stu-id="43f06-150">limit</span></span>|<span data-ttu-id="43f06-151">Int32</span><span class="sxs-lookup"><span data-stu-id="43f06-151">Int32</span></span>|<span data-ttu-id="43f06-152">尚未记录</span><span class="sxs-lookup"><span data-stu-id="43f06-152">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="43f06-153">响应</span><span class="sxs-lookup"><span data-stu-id="43f06-153">Response</span></span>
<span data-ttu-id="43f06-154">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [deviceEnrollmentLimitConfiguration](../resources/intune_onboarding_deviceenrollmentlimitconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="43f06-154">If successful, this method returns a `201 Created` response code and a [deviceEnrollmentLimitConfiguration](../resources/intune_onboarding_deviceenrollmentlimitconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="43f06-155">示例</span><span class="sxs-lookup"><span data-stu-id="43f06-155">Example</span></span>
### <a name="request"></a><span data-ttu-id="43f06-156">请求</span><span class="sxs-lookup"><span data-stu-id="43f06-156">Request</span></span>
<span data-ttu-id="43f06-157">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="43f06-157">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations
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

### <a name="response"></a><span data-ttu-id="43f06-158">响应</span><span class="sxs-lookup"><span data-stu-id="43f06-158">Response</span></span>
<span data-ttu-id="43f06-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="43f06-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




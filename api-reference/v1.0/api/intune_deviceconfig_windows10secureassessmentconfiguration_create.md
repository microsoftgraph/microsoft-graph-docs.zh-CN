# <a name="create-windows10secureassessmentconfiguration"></a><span data-ttu-id="c7681-101">创建 windows10SecureAssessmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="c7681-101">Create windows10SecureAssessmentConfiguration</span></span>

> <span data-ttu-id="c7681-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="c7681-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c7681-103">创建新的 [windows10SecureAssessmentConfiguration](../resources/intune_deviceconfig_windows10secureassessmentconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c7681-103">Create a new [plannerBucket](../resources/intune_deviceconfig_windows10secureassessmentconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c7681-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="c7681-104">Prerequisites</span></span>
<span data-ttu-id="c7681-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="c7681-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="c7681-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="c7681-107">Permission type</span></span>|<span data-ttu-id="c7681-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c7681-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c7681-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c7681-109">Delegated (work or school account)</span></span>|<span data-ttu-id="c7681-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c7681-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c7681-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c7681-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c7681-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="c7681-112">Not supported.</span></span>|
|<span data-ttu-id="c7681-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="c7681-113">Application</span></span>|<span data-ttu-id="c7681-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="c7681-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c7681-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c7681-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="c7681-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="c7681-116">Request headers</span></span>
|<span data-ttu-id="c7681-117">标头</span><span class="sxs-lookup"><span data-stu-id="c7681-117">Header</span></span>|<span data-ttu-id="c7681-118">值</span><span class="sxs-lookup"><span data-stu-id="c7681-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c7681-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="c7681-119">Authorization</span></span>|<span data-ttu-id="c7681-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c7681-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="c7681-121">Accept</span><span class="sxs-lookup"><span data-stu-id="c7681-121">Accept</span></span>|<span data-ttu-id="c7681-122">application/json</span><span class="sxs-lookup"><span data-stu-id="c7681-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c7681-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="c7681-123">Request body</span></span>
<span data-ttu-id="c7681-124">在请求正文中，提供 windows10SecureAssessmentConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c7681-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="c7681-125">下表显示创建 windows10SecureAssessmentConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="c7681-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="c7681-126">属性</span><span class="sxs-lookup"><span data-stu-id="c7681-126">Property</span></span>|<span data-ttu-id="c7681-127">类型</span><span class="sxs-lookup"><span data-stu-id="c7681-127">Type</span></span>|<span data-ttu-id="c7681-128">说明</span><span class="sxs-lookup"><span data-stu-id="c7681-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c7681-129">id</span><span class="sxs-lookup"><span data-stu-id="c7681-129">id</span></span>|<span data-ttu-id="c7681-130">String</span><span class="sxs-lookup"><span data-stu-id="c7681-130">String</span></span>|<span data-ttu-id="c7681-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="c7681-131">Key of the setting.</span></span> <span data-ttu-id="c7681-132">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c7681-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c7681-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c7681-133">lastModifiedDateTime</span></span>|<span data-ttu-id="c7681-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c7681-134">DateTimeOffset</span></span>|<span data-ttu-id="c7681-135">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="c7681-135">Indicates the date the object was last modified.</span></span> <span data-ttu-id="c7681-136">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c7681-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c7681-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c7681-137">createdDateTime</span></span>|<span data-ttu-id="c7681-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c7681-138">DateTimeOffset</span></span>|<span data-ttu-id="c7681-139">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="c7681-139">DateTime the object was created.</span></span> <span data-ttu-id="c7681-140">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c7681-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c7681-141">description</span><span class="sxs-lookup"><span data-stu-id="c7681-141">description</span></span>|<span data-ttu-id="c7681-142">String</span><span class="sxs-lookup"><span data-stu-id="c7681-142">String</span></span>|<span data-ttu-id="c7681-143">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="c7681-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c7681-144">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c7681-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c7681-145">displayName</span><span class="sxs-lookup"><span data-stu-id="c7681-145">displayName</span></span>|<span data-ttu-id="c7681-146">String</span><span class="sxs-lookup"><span data-stu-id="c7681-146">String</span></span>|<span data-ttu-id="c7681-147">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="c7681-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c7681-148">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c7681-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c7681-149">version</span><span class="sxs-lookup"><span data-stu-id="c7681-149">version</span></span>|<span data-ttu-id="c7681-150">Int32</span><span class="sxs-lookup"><span data-stu-id="c7681-150">Int32</span></span>|<span data-ttu-id="c7681-151">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="c7681-151">Version of the device configuration.</span></span> <span data-ttu-id="c7681-152">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c7681-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c7681-153">launchUri</span><span class="sxs-lookup"><span data-stu-id="c7681-153">launchUri</span></span>|<span data-ttu-id="c7681-154">String</span><span class="sxs-lookup"><span data-stu-id="c7681-154">String</span></span>|<span data-ttu-id="c7681-155">启动安全评估浏览器时指向自动加载的评估的 URL 链接。</span><span class="sxs-lookup"><span data-stu-id="c7681-155">Url link to an assessment that's automatically loaded when the secure assessment browser is launched.</span></span> <span data-ttu-id="c7681-156">它必须是有效的 URL (http\[s\]://msdn.microsoft.com/)。</span><span class="sxs-lookup"><span data-stu-id="c7681-156">It has to be a valid Url (http\[s\]://msdn.microsoft.com/).</span></span>|
|<span data-ttu-id="c7681-157">configurationAccount</span><span class="sxs-lookup"><span data-stu-id="c7681-157">configurationAccount</span></span>|<span data-ttu-id="c7681-158">String</span><span class="sxs-lookup"><span data-stu-id="c7681-158">String</span></span>|<span data-ttu-id="c7681-159">用于配置 Windows 设备进行测试的帐户。</span><span class="sxs-lookup"><span data-stu-id="c7681-159">The account used to configure the Windows device for taking the test.</span></span> <span data-ttu-id="c7681-160">用户可以是域帐户（域\用户）、AAD 帐户 (username@tenant.com) 或本地帐户（用户名）。</span><span class="sxs-lookup"><span data-stu-id="c7681-160">The user can be a domain account (domain\user), an AAD account (username@tenant.com) or a local account (username).</span></span>|
|<span data-ttu-id="c7681-161">allowPrinting</span><span class="sxs-lookup"><span data-stu-id="c7681-161">allowPrinting</span></span>|<span data-ttu-id="c7681-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="c7681-162">Boolean</span></span>|<span data-ttu-id="c7681-163">指示在测试期间是否允许应用打印。</span><span class="sxs-lookup"><span data-stu-id="c7681-163">Indicates whether or not to allow the app from printing during the test.</span></span>|
|<span data-ttu-id="c7681-164">allowScreenCapture</span><span class="sxs-lookup"><span data-stu-id="c7681-164">allowScreenCapture</span></span>|<span data-ttu-id="c7681-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="c7681-165">Boolean</span></span>|<span data-ttu-id="c7681-166">指示在测试期间是否允许屏幕捕获功能。</span><span class="sxs-lookup"><span data-stu-id="c7681-166">Indicates whether or not to allow screen capture capability during a test.</span></span>|
|<span data-ttu-id="c7681-167">allowTextSuggestion</span><span class="sxs-lookup"><span data-stu-id="c7681-167">allowTextSuggestion</span></span>|<span data-ttu-id="c7681-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="c7681-168">Boolean</span></span>|<span data-ttu-id="c7681-169">指示在测试期间是否允许文本建议。</span><span class="sxs-lookup"><span data-stu-id="c7681-169">Indicates whether or not to allow text suggestions during the test.</span></span>|



## <a name="response"></a><span data-ttu-id="c7681-170">响应</span><span class="sxs-lookup"><span data-stu-id="c7681-170">Response</span></span>
<span data-ttu-id="c7681-171">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [windows10SecureAssessmentConfiguration](../resources/intune_deviceconfig_windows10secureassessmentconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c7681-171">If successful, this method returns a `201 Created` response code and a [directoryObject](../resources/intune_deviceconfig_windows10secureassessmentconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c7681-172">示例</span><span class="sxs-lookup"><span data-stu-id="c7681-172">Example</span></span>
### <a name="request"></a><span data-ttu-id="c7681-173">请求</span><span class="sxs-lookup"><span data-stu-id="c7681-173">Request</span></span>
<span data-ttu-id="c7681-174">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c7681-174">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 423

{
  "@odata.type": "#microsoft.graph.windows10SecureAssessmentConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "launchUri": "Launch Uri value",
  "configurationAccount": "Configuration Account value",
  "allowPrinting": true,
  "allowScreenCapture": true,
  "allowTextSuggestion": true
}
```

### <a name="response"></a><span data-ttu-id="c7681-175">响应</span><span class="sxs-lookup"><span data-stu-id="c7681-175">Response</span></span>
<span data-ttu-id="c7681-p110">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c7681-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 531

{
  "@odata.type": "#microsoft.graph.windows10SecureAssessmentConfiguration",
  "id": "f60d71be-71be-f60d-be71-0df6be710df6",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "launchUri": "Launch Uri value",
  "configurationAccount": "Configuration Account value",
  "allowPrinting": true,
  "allowScreenCapture": true,
  "allowTextSuggestion": true
}
```




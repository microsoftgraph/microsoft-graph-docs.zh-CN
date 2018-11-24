# <a name="update-windows10enterprisemodernappmanagementconfiguration"></a><span data-ttu-id="fbc43-101">更新 windows10EnterpriseModernAppManagementConfiguration</span><span class="sxs-lookup"><span data-stu-id="fbc43-101">Update windows10EnterpriseModernAppManagementConfiguration</span></span>

> <span data-ttu-id="fbc43-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="fbc43-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fbc43-103">更新 [windows10EnterpriseModernAppManagementConfiguration](../resources/intune_deviceconfig_windows10enterprisemodernappmanagementconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="fbc43-103">Update the properties of a [windows10EnterpriseModernAppManagementConfiguration](../resources/intune_deviceconfig_windows10enterprisemodernappmanagementconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fbc43-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="fbc43-104">Prerequisites</span></span>
<span data-ttu-id="fbc43-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="fbc43-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="fbc43-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="fbc43-107">Permission type</span></span>|<span data-ttu-id="fbc43-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="fbc43-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fbc43-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fbc43-109">Delegated (work or school account)</span></span>|<span data-ttu-id="fbc43-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fbc43-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="fbc43-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fbc43-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fbc43-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="fbc43-112">Not supported.</span></span>|
|<span data-ttu-id="fbc43-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="fbc43-113">Application</span></span>|<span data-ttu-id="fbc43-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="fbc43-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fbc43-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fbc43-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="fbc43-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="fbc43-116">Request headers</span></span>
|<span data-ttu-id="fbc43-117">标头</span><span class="sxs-lookup"><span data-stu-id="fbc43-117">Header</span></span>|<span data-ttu-id="fbc43-118">值</span><span class="sxs-lookup"><span data-stu-id="fbc43-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fbc43-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="fbc43-119">Authorization</span></span>|<span data-ttu-id="fbc43-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="fbc43-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fbc43-121">Accept</span><span class="sxs-lookup"><span data-stu-id="fbc43-121">Accept</span></span>|<span data-ttu-id="fbc43-122">application/json</span><span class="sxs-lookup"><span data-stu-id="fbc43-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fbc43-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="fbc43-123">Request body</span></span>
<span data-ttu-id="fbc43-124">在请求正文中，提供 [windows10EnterpriseModernAppManagementConfiguration](../resources/intune_deviceconfig_windows10enterprisemodernappmanagementconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fbc43-124">In the request body, supply a JSON representation for the [windows10EnterpriseModernAppManagementConfiguration](../resources/intune_deviceconfig_windows10enterprisemodernappmanagementconfiguration.md) object.</span></span>

<span data-ttu-id="fbc43-125">下表显示创建 [windows10EnterpriseModernAppManagementConfiguration](../resources/intune_deviceconfig_windows10enterprisemodernappmanagementconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="fbc43-125">The following table shows the properties that are required when you create the [windows10EnterpriseModernAppManagementConfiguration](../resources/intune_deviceconfig_windows10enterprisemodernappmanagementconfiguration.md).</span></span>

|<span data-ttu-id="fbc43-126">属性</span><span class="sxs-lookup"><span data-stu-id="fbc43-126">Property</span></span>|<span data-ttu-id="fbc43-127">类型</span><span class="sxs-lookup"><span data-stu-id="fbc43-127">Type</span></span>|<span data-ttu-id="fbc43-128">说明</span><span class="sxs-lookup"><span data-stu-id="fbc43-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fbc43-129">id</span><span class="sxs-lookup"><span data-stu-id="fbc43-129">id</span></span>|<span data-ttu-id="fbc43-130">String</span><span class="sxs-lookup"><span data-stu-id="fbc43-130">String</span></span>|<span data-ttu-id="fbc43-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="fbc43-131">Key of the entity.</span></span> <span data-ttu-id="fbc43-132">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fbc43-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fbc43-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fbc43-133">lastModifiedDateTime</span></span>|<span data-ttu-id="fbc43-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fbc43-134">DateTimeOffset</span></span>|<span data-ttu-id="fbc43-135">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="fbc43-135">DateTime the object was last modified.</span></span> <span data-ttu-id="fbc43-136">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fbc43-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fbc43-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fbc43-137">createdDateTime</span></span>|<span data-ttu-id="fbc43-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fbc43-138">DateTimeOffset</span></span>|<span data-ttu-id="fbc43-139">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="fbc43-139">DateTime the object was created.</span></span> <span data-ttu-id="fbc43-140">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fbc43-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fbc43-141">description</span><span class="sxs-lookup"><span data-stu-id="fbc43-141">description</span></span>|<span data-ttu-id="fbc43-142">String</span><span class="sxs-lookup"><span data-stu-id="fbc43-142">String</span></span>|<span data-ttu-id="fbc43-143">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="fbc43-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="fbc43-144">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fbc43-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fbc43-145">displayName</span><span class="sxs-lookup"><span data-stu-id="fbc43-145">displayName</span></span>|<span data-ttu-id="fbc43-146">String</span><span class="sxs-lookup"><span data-stu-id="fbc43-146">String</span></span>|<span data-ttu-id="fbc43-147">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="fbc43-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="fbc43-148">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fbc43-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fbc43-149">version</span><span class="sxs-lookup"><span data-stu-id="fbc43-149">version</span></span>|<span data-ttu-id="fbc43-150">Int32</span><span class="sxs-lookup"><span data-stu-id="fbc43-150">Int32</span></span>|<span data-ttu-id="fbc43-151">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="fbc43-151">Version of the device configuration.</span></span> <span data-ttu-id="fbc43-152">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fbc43-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fbc43-153">uninstallBuiltInApps</span><span class="sxs-lookup"><span data-stu-id="fbc43-153">uninstallBuiltInApps</span></span>|<span data-ttu-id="fbc43-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="fbc43-154">Boolean</span></span>|<span data-ttu-id="fbc43-155">指示是否卸载内置 Windows 应用的固定列表。</span><span class="sxs-lookup"><span data-stu-id="fbc43-155">Indicates whether or not to uninstall a fixed list of built-in Windows apps.</span></span>|



## <a name="response"></a><span data-ttu-id="fbc43-156">响应</span><span class="sxs-lookup"><span data-stu-id="fbc43-156">Response</span></span>
<span data-ttu-id="fbc43-157">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [windows10EnterpriseModernAppManagementConfiguration](../resources/intune_deviceconfig_windows10enterprisemodernappmanagementconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="fbc43-157">If successful, this method returns a `200 OK` response code and an updated [windows10EnterpriseModernAppManagementConfiguration](../resources/intune_deviceconfig_windows10enterprisemodernappmanagementconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fbc43-158">示例</span><span class="sxs-lookup"><span data-stu-id="fbc43-158">Example</span></span>
### <a name="request"></a><span data-ttu-id="fbc43-159">请求</span><span class="sxs-lookup"><span data-stu-id="fbc43-159">Request</span></span>
<span data-ttu-id="fbc43-160">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="fbc43-160">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 222

{
  "@odata.type": "#microsoft.graph.windows10EnterpriseModernAppManagementConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "uninstallBuiltInApps": true
}
```

### <a name="response"></a><span data-ttu-id="fbc43-161">响应</span><span class="sxs-lookup"><span data-stu-id="fbc43-161">Response</span></span>
<span data-ttu-id="fbc43-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="fbc43-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 394

{
  "@odata.type": "#microsoft.graph.windows10EnterpriseModernAppManagementConfiguration",
  "id": "d6577687-7687-d657-8776-57d6877657d6",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "uninstallBuiltInApps": true
}
```




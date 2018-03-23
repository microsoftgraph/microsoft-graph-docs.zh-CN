# <a name="update-androidcustomconfiguration"></a><span data-ttu-id="8222a-101">更新 androidCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="8222a-101">Update androidCustomConfiguration</span></span>

> <span data-ttu-id="8222a-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="8222a-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8222a-103">更新 [androidCustomConfiguration](../resources/intune_deviceconfig_androidcustomconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="8222a-103">Update the properties of a [calendar](../resources/intune_deviceconfig_androidcustomconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8222a-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="8222a-104">Prerequisites</span></span>
<span data-ttu-id="8222a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="8222a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="8222a-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="8222a-107">Permission type</span></span>|<span data-ttu-id="8222a-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="8222a-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8222a-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8222a-109">Delegated (work or school account)</span></span>|<span data-ttu-id="8222a-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8222a-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8222a-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8222a-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8222a-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="8222a-112">Not supported.</span></span>|
|<span data-ttu-id="8222a-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="8222a-113">Application</span></span>|<span data-ttu-id="8222a-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="8222a-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8222a-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8222a-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="8222a-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="8222a-116">Request headers</span></span>
|<span data-ttu-id="8222a-117">标头</span><span class="sxs-lookup"><span data-stu-id="8222a-117">Header</span></span>|<span data-ttu-id="8222a-118">值</span><span class="sxs-lookup"><span data-stu-id="8222a-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8222a-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="8222a-119">Authorization</span></span>|<span data-ttu-id="8222a-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="8222a-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="8222a-121">Accept</span><span class="sxs-lookup"><span data-stu-id="8222a-121">Accept</span></span>|<span data-ttu-id="8222a-122">application/json</span><span class="sxs-lookup"><span data-stu-id="8222a-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8222a-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="8222a-123">Request body</span></span>
<span data-ttu-id="8222a-124">在请求正文中，提供 [androidCustomConfiguration](../resources/intune_deviceconfig_androidcustomconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8222a-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_deviceconfig_androidcustomconfiguration.md) object.</span></span>

<span data-ttu-id="8222a-125">下表显示了创建 [androidCustomConfiguration](../resources/intune_deviceconfig_androidcustomconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="8222a-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="8222a-126">属性</span><span class="sxs-lookup"><span data-stu-id="8222a-126">Property</span></span>|<span data-ttu-id="8222a-127">类型</span><span class="sxs-lookup"><span data-stu-id="8222a-127">Type</span></span>|<span data-ttu-id="8222a-128">说明</span><span class="sxs-lookup"><span data-stu-id="8222a-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8222a-129">id</span><span class="sxs-lookup"><span data-stu-id="8222a-129">id</span></span>|<span data-ttu-id="8222a-130">String</span><span class="sxs-lookup"><span data-stu-id="8222a-130">String</span></span>|<span data-ttu-id="8222a-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="8222a-131">Key of the setting.</span></span> <span data-ttu-id="8222a-132">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8222a-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8222a-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8222a-133">lastModifiedDateTime</span></span>|<span data-ttu-id="8222a-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8222a-134">DateTimeOffset</span></span>|<span data-ttu-id="8222a-135">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="8222a-135">Indicates the date the object was last modified.</span></span> <span data-ttu-id="8222a-136">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8222a-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8222a-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8222a-137">createdDateTime</span></span>|<span data-ttu-id="8222a-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8222a-138">DateTimeOffset</span></span>|<span data-ttu-id="8222a-139">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="8222a-139">DateTime the object was created.</span></span> <span data-ttu-id="8222a-140">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8222a-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8222a-141">description</span><span class="sxs-lookup"><span data-stu-id="8222a-141">description</span></span>|<span data-ttu-id="8222a-142">String</span><span class="sxs-lookup"><span data-stu-id="8222a-142">String</span></span>|<span data-ttu-id="8222a-143">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="8222a-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="8222a-144">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8222a-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8222a-145">displayName</span><span class="sxs-lookup"><span data-stu-id="8222a-145">displayName</span></span>|<span data-ttu-id="8222a-146">String</span><span class="sxs-lookup"><span data-stu-id="8222a-146">String</span></span>|<span data-ttu-id="8222a-147">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="8222a-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="8222a-148">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8222a-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8222a-149">version</span><span class="sxs-lookup"><span data-stu-id="8222a-149">version</span></span>|<span data-ttu-id="8222a-150">Int32</span><span class="sxs-lookup"><span data-stu-id="8222a-150">Int32</span></span>|<span data-ttu-id="8222a-151">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="8222a-151">Version of the device configuration.</span></span> <span data-ttu-id="8222a-152">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8222a-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8222a-153">omaSettings</span><span class="sxs-lookup"><span data-stu-id="8222a-153">omaSettings</span></span>|<span data-ttu-id="8222a-154">[omaSetting](../resources/intune_deviceconfig_omasetting.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8222a-154">[omaSetting](../resources/intune_deviceconfig_omasetting.md) collection</span></span>|<span data-ttu-id="8222a-155">OMA 设置。</span><span class="sxs-lookup"><span data-stu-id="8222a-155">OMA settings.</span></span> <span data-ttu-id="8222a-156">该集合最多可包含 1000 个元素。</span><span class="sxs-lookup"><span data-stu-id="8222a-156">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="8222a-157">响应</span><span class="sxs-lookup"><span data-stu-id="8222a-157">Response</span></span>
<span data-ttu-id="8222a-158">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [androidCustomConfiguration](../resources/intune_deviceconfig_androidcustomconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8222a-158">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_deviceconfig_androidcustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8222a-159">示例</span><span class="sxs-lookup"><span data-stu-id="8222a-159">Example</span></span>
### <a name="request"></a><span data-ttu-id="8222a-160">请求</span><span class="sxs-lookup"><span data-stu-id="8222a-160">Request</span></span>
<span data-ttu-id="8222a-161">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8222a-161">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 401

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "omaSettings": [
    {
      "@odata.type": "microsoft.graph.omaSettingInteger",
      "displayName": "Display Name value",
      "description": "Description value",
      "omaUri": "Oma Uri value",
      "value": 5
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="8222a-162">响应</span><span class="sxs-lookup"><span data-stu-id="8222a-162">Response</span></span>
<span data-ttu-id="8222a-p109">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8222a-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 574

{
  "@odata.type": "#microsoft.graph.androidCustomConfiguration",
  "id": "619b5e6d-5e6d-619b-6d5e-9b616d5e9b61",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "omaSettings": [
    {
      "@odata.type": "microsoft.graph.omaSettingInteger",
      "displayName": "Display Name value",
      "description": "Description value",
      "omaUri": "Oma Uri value",
      "value": 5
    }
  ]
}
```




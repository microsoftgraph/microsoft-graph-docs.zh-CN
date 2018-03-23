# <a name="create-windowsphone81customconfiguration"></a><span data-ttu-id="d0074-101">创建 windowsPhone81CustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="d0074-101">Create windowsPhone81CustomConfiguration</span></span>

> <span data-ttu-id="d0074-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="d0074-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d0074-103">创建新的 [windowsPhone81CustomConfiguration](../resources/intune_deviceconfig_windowsphone81customconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d0074-103">Create a new [plannerBucket](../resources/intune_deviceconfig_windowsphone81customconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d0074-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="d0074-104">Prerequisites</span></span>
<span data-ttu-id="d0074-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="d0074-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="d0074-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="d0074-107">Permission type</span></span>|<span data-ttu-id="d0074-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d0074-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d0074-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d0074-109">Delegated (work or school account)</span></span>|<span data-ttu-id="d0074-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0074-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d0074-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d0074-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d0074-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="d0074-112">Not supported.</span></span>|
|<span data-ttu-id="d0074-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="d0074-113">Application</span></span>|<span data-ttu-id="d0074-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="d0074-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d0074-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d0074-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="d0074-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="d0074-116">Request headers</span></span>
|<span data-ttu-id="d0074-117">标头</span><span class="sxs-lookup"><span data-stu-id="d0074-117">Header</span></span>|<span data-ttu-id="d0074-118">值</span><span class="sxs-lookup"><span data-stu-id="d0074-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d0074-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="d0074-119">Authorization</span></span>|<span data-ttu-id="d0074-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d0074-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="d0074-121">Accept</span><span class="sxs-lookup"><span data-stu-id="d0074-121">Accept</span></span>|<span data-ttu-id="d0074-122">application/json</span><span class="sxs-lookup"><span data-stu-id="d0074-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d0074-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="d0074-123">Request body</span></span>
<span data-ttu-id="d0074-124">在请求正文中，提供 windowsPhone81CustomConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d0074-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="d0074-125">下表显示了创建 windowsPhone81CustomConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="d0074-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="d0074-126">属性</span><span class="sxs-lookup"><span data-stu-id="d0074-126">Property</span></span>|<span data-ttu-id="d0074-127">类型</span><span class="sxs-lookup"><span data-stu-id="d0074-127">Type</span></span>|<span data-ttu-id="d0074-128">说明</span><span class="sxs-lookup"><span data-stu-id="d0074-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d0074-129">id</span><span class="sxs-lookup"><span data-stu-id="d0074-129">id</span></span>|<span data-ttu-id="d0074-130">String</span><span class="sxs-lookup"><span data-stu-id="d0074-130">String</span></span>|<span data-ttu-id="d0074-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="d0074-131">Key of the setting.</span></span> <span data-ttu-id="d0074-132">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d0074-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d0074-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d0074-133">lastModifiedDateTime</span></span>|<span data-ttu-id="d0074-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d0074-134">DateTimeOffset</span></span>|<span data-ttu-id="d0074-135">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="d0074-135">Indicates the date the object was last modified.</span></span> <span data-ttu-id="d0074-136">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d0074-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d0074-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d0074-137">createdDateTime</span></span>|<span data-ttu-id="d0074-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d0074-138">DateTimeOffset</span></span>|<span data-ttu-id="d0074-139">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="d0074-139">DateTime the object was created.</span></span> <span data-ttu-id="d0074-140">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d0074-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d0074-141">description</span><span class="sxs-lookup"><span data-stu-id="d0074-141">description</span></span>|<span data-ttu-id="d0074-142">String</span><span class="sxs-lookup"><span data-stu-id="d0074-142">String</span></span>|<span data-ttu-id="d0074-143">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="d0074-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d0074-144">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d0074-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d0074-145">displayName</span><span class="sxs-lookup"><span data-stu-id="d0074-145">displayName</span></span>|<span data-ttu-id="d0074-146">String</span><span class="sxs-lookup"><span data-stu-id="d0074-146">String</span></span>|<span data-ttu-id="d0074-147">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="d0074-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d0074-148">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d0074-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d0074-149">version</span><span class="sxs-lookup"><span data-stu-id="d0074-149">version</span></span>|<span data-ttu-id="d0074-150">Int32</span><span class="sxs-lookup"><span data-stu-id="d0074-150">Int32</span></span>|<span data-ttu-id="d0074-151">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="d0074-151">Version of the device configuration.</span></span> <span data-ttu-id="d0074-152">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d0074-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d0074-153">omaSettings</span><span class="sxs-lookup"><span data-stu-id="d0074-153">omaSettings</span></span>|<span data-ttu-id="d0074-154">[omaSetting](../resources/intune_deviceconfig_omasetting.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d0074-154">[omaSetting](../resources/intune_deviceconfig_omasetting.md) collection</span></span>|<span data-ttu-id="d0074-155">OMA 设置。</span><span class="sxs-lookup"><span data-stu-id="d0074-155">OMA settings.</span></span> <span data-ttu-id="d0074-156">该集合最多可包含 1000 个元素。</span><span class="sxs-lookup"><span data-stu-id="d0074-156">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="d0074-157">响应</span><span class="sxs-lookup"><span data-stu-id="d0074-157">Response</span></span>
<span data-ttu-id="d0074-158">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [windowsPhone81CustomConfiguration](../resources/intune_deviceconfig_windowsphone81customconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d0074-158">If successful, this method returns a `201 Created` response code and a [directoryObject](../resources/intune_deviceconfig_windowsphone81customconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d0074-159">示例</span><span class="sxs-lookup"><span data-stu-id="d0074-159">Example</span></span>
### <a name="request"></a><span data-ttu-id="d0074-160">请求</span><span class="sxs-lookup"><span data-stu-id="d0074-160">Request</span></span>
<span data-ttu-id="d0074-161">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d0074-161">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 473

{
  "@odata.type": "#microsoft.graph.windowsPhone81CustomConfiguration",
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

### <a name="response"></a><span data-ttu-id="d0074-162">响应</span><span class="sxs-lookup"><span data-stu-id="d0074-162">Response</span></span>
<span data-ttu-id="d0074-p109">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d0074-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 581

{
  "@odata.type": "#microsoft.graph.windowsPhone81CustomConfiguration",
  "id": "0d98693c-693c-0d98-3c69-980d3c69980d",
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




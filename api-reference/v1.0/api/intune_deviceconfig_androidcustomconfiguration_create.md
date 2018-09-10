# <a name="create-androidcustomconfiguration"></a><span data-ttu-id="f2374-101">创建 androidCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="f2374-101">Create androidCustomConfiguration</span></span>

> <span data-ttu-id="f2374-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="f2374-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f2374-103">创建新的 [androidCustomConfiguration](../resources/intune_deviceconfig_androidcustomconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f2374-103">Create a new [androidCustomConfiguration](../resources/intune_deviceconfig_androidcustomconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f2374-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="f2374-104">Prerequisites</span></span>
<span data-ttu-id="f2374-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="f2374-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f2374-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="f2374-107">Permission type</span></span>|<span data-ttu-id="f2374-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f2374-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f2374-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f2374-109">Delegated (work or school account)</span></span>|<span data-ttu-id="f2374-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2374-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f2374-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f2374-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f2374-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="f2374-112">Not supported.</span></span>|
|<span data-ttu-id="f2374-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="f2374-113">Application</span></span>|<span data-ttu-id="f2374-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f2374-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f2374-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f2374-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="f2374-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="f2374-116">Request headers</span></span>
|<span data-ttu-id="f2374-117">标头</span><span class="sxs-lookup"><span data-stu-id="f2374-117">Header</span></span>|<span data-ttu-id="f2374-118">值</span><span class="sxs-lookup"><span data-stu-id="f2374-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f2374-119">授权</span><span class="sxs-lookup"><span data-stu-id="f2374-119">Authorization</span></span>|<span data-ttu-id="f2374-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f2374-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f2374-121">Accept</span><span class="sxs-lookup"><span data-stu-id="f2374-121">Accept</span></span>|<span data-ttu-id="f2374-122">application/json</span><span class="sxs-lookup"><span data-stu-id="f2374-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f2374-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="f2374-123">Request body</span></span>
<span data-ttu-id="f2374-124">在请求正文中，提供 androidCustomConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f2374-124">In the request body, supply a JSON representation for the androidCustomConfiguration object.</span></span>

<span data-ttu-id="f2374-125">下表显示了创建 androidCustomConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="f2374-125">The following table shows the properties that are required when you create the androidCustomConfiguration.</span></span>

|<span data-ttu-id="f2374-126">属性</span><span class="sxs-lookup"><span data-stu-id="f2374-126">Property</span></span>|<span data-ttu-id="f2374-127">类型</span><span class="sxs-lookup"><span data-stu-id="f2374-127">Type</span></span>|<span data-ttu-id="f2374-128">说明</span><span class="sxs-lookup"><span data-stu-id="f2374-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f2374-129">ID</span><span class="sxs-lookup"><span data-stu-id="f2374-129">id</span></span>|<span data-ttu-id="f2374-130">字符串</span><span class="sxs-lookup"><span data-stu-id="f2374-130">String</span></span>|<span data-ttu-id="f2374-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="f2374-131">Key of the entity.</span></span> <span data-ttu-id="f2374-132">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f2374-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f2374-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f2374-133">lastModifiedDateTime</span></span>|<span data-ttu-id="f2374-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f2374-134">DateTimeOffset</span></span>|<span data-ttu-id="f2374-135">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="f2374-135">DateTime the object was last modified.</span></span> <span data-ttu-id="f2374-136">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f2374-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f2374-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f2374-137">createdDateTime</span></span>|<span data-ttu-id="f2374-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f2374-138">DateTimeOffset</span></span>|<span data-ttu-id="f2374-139">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="f2374-139">DateTime the object was created.</span></span> <span data-ttu-id="f2374-140">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f2374-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f2374-141">说明</span><span class="sxs-lookup"><span data-stu-id="f2374-141">description</span></span>|<span data-ttu-id="f2374-142">字符串</span><span class="sxs-lookup"><span data-stu-id="f2374-142">String</span></span>|<span data-ttu-id="f2374-143">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="f2374-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f2374-144">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f2374-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f2374-145">displayName</span><span class="sxs-lookup"><span data-stu-id="f2374-145">displayName</span></span>|<span data-ttu-id="f2374-146">字符串</span><span class="sxs-lookup"><span data-stu-id="f2374-146">String</span></span>|<span data-ttu-id="f2374-147">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="f2374-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f2374-148">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f2374-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f2374-149">version</span><span class="sxs-lookup"><span data-stu-id="f2374-149">version</span></span>|<span data-ttu-id="f2374-150">Int32</span><span class="sxs-lookup"><span data-stu-id="f2374-150">Int32</span></span>|<span data-ttu-id="f2374-151">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="f2374-151">Version of the device configuration.</span></span> <span data-ttu-id="f2374-152">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f2374-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f2374-153">omaSettings</span><span class="sxs-lookup"><span data-stu-id="f2374-153">omaSettings</span></span>|<span data-ttu-id="f2374-154">[omaSetting](../resources/intune_deviceconfig_omasetting.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f2374-154">[omaSetting](../resources/intune_deviceconfig_omasetting.md) collection</span></span>|<span data-ttu-id="f2374-155">OMA 设置。</span><span class="sxs-lookup"><span data-stu-id="f2374-155">OMA settings.</span></span> <span data-ttu-id="f2374-156">该集合最多可包含 1000 个元素。</span><span class="sxs-lookup"><span data-stu-id="f2374-156">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="f2374-157">响应</span><span class="sxs-lookup"><span data-stu-id="f2374-157">Response</span></span>
<span data-ttu-id="f2374-158">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [androidCustomConfiguration](../resources/intune_deviceconfig_androidcustomconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f2374-158">If successful, this method returns a `201 Created` response code and a [androidCustomConfiguration](../resources/intune_deviceconfig_androidcustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f2374-159">示例</span><span class="sxs-lookup"><span data-stu-id="f2374-159">Example</span></span>
### <a name="request"></a><span data-ttu-id="f2374-160">请求</span><span class="sxs-lookup"><span data-stu-id="f2374-160">Request</span></span>
<span data-ttu-id="f2374-161">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f2374-161">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 466

{
  "@odata.type": "#microsoft.graph.androidCustomConfiguration",
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

### <a name="response"></a><span data-ttu-id="f2374-162">响应</span><span class="sxs-lookup"><span data-stu-id="f2374-162">Response</span></span>
<span data-ttu-id="f2374-p109">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f2374-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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









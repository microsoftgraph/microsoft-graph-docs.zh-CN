# <a name="update-androidworkprofilecustomconfiguration"></a><span data-ttu-id="ad4b4-101">更新 androidWorkProfileCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="ad4b4-101">Update androidWorkProfileCustomConfiguration</span></span>

> <span data-ttu-id="ad4b4-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="ad4b4-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ad4b4-103">更新[androidWorkProfileCustomConfiguration](../resources/intune_deviceconfig_androidworkprofilecustomconfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="ad4b4-103">Update the properties of a [androidWorkProfileCustomConfiguration](../resources/intune_deviceconfig_androidworkprofilecustomconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ad4b4-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="ad4b4-104">Prerequisites</span></span>
<span data-ttu-id="ad4b4-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](../../../concepts/permissions_reference.md)。
</span><span class="sxs-lookup"><span data-stu-id="ad4b4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ad4b4-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="ad4b4-107">Permission type</span></span>|<span data-ttu-id="ad4b4-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ad4b4-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ad4b4-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ad4b4-109">Delegated (work or school account)</span></span>|<span data-ttu-id="ad4b4-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad4b4-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ad4b4-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ad4b4-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ad4b4-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="ad4b4-112">Not supported.</span></span>|
|<span data-ttu-id="ad4b4-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="ad4b4-113">Application</span></span>|<span data-ttu-id="ad4b4-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="ad4b4-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ad4b4-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ad4b4-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="ad4b4-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="ad4b4-116">Request headers</span></span>
|<span data-ttu-id="ad4b4-117">标头</span><span class="sxs-lookup"><span data-stu-id="ad4b4-117">Header</span></span>|<span data-ttu-id="ad4b4-118">值</span><span class="sxs-lookup"><span data-stu-id="ad4b4-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ad4b4-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="ad4b4-119">Authorization</span></span>|<span data-ttu-id="ad4b4-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ad4b4-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ad4b4-121">Accept</span><span class="sxs-lookup"><span data-stu-id="ad4b4-121">Accept</span></span>|<span data-ttu-id="ad4b4-122">application/json</span><span class="sxs-lookup"><span data-stu-id="ad4b4-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ad4b4-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="ad4b4-123">Request body</span></span>
<span data-ttu-id="ad4b4-124">在请求正文中，提供[androidWorkProfileCustomConfiguration](../resources/intune_deviceconfig_androidworkprofilecustomconfiguration.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ad4b4-124">In the request body, supply a JSON representation for the [androidWorkProfileCustomConfiguration](../resources/intune_deviceconfig_androidworkprofilecustomconfiguration.md) object.</span></span>

<span data-ttu-id="ad4b4-125">下表显示时创建[androidWorkProfileCustomConfiguration](../resources/intune_deviceconfig_androidworkprofilecustomconfiguration.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="ad4b4-125">The following table shows the properties that are required when you create the [androidWorkProfileCustomConfiguration](../resources/intune_deviceconfig_androidworkprofilecustomconfiguration.md).</span></span>

|<span data-ttu-id="ad4b4-126">属性</span><span class="sxs-lookup"><span data-stu-id="ad4b4-126">Property</span></span>|<span data-ttu-id="ad4b4-127">类型</span><span class="sxs-lookup"><span data-stu-id="ad4b4-127">Type</span></span>|<span data-ttu-id="ad4b4-128">说明</span><span class="sxs-lookup"><span data-stu-id="ad4b4-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ad4b4-129">id</span><span class="sxs-lookup"><span data-stu-id="ad4b4-129">id</span></span>|<span data-ttu-id="ad4b4-130">String</span><span class="sxs-lookup"><span data-stu-id="ad4b4-130">String</span></span>|<span data-ttu-id="ad4b4-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="ad4b4-131">Key of the entity.</span></span> <span data-ttu-id="ad4b4-132">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ad4b4-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ad4b4-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ad4b4-133">lastModifiedDateTime</span></span>|<span data-ttu-id="ad4b4-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ad4b4-134">DateTimeOffset</span></span>|<span data-ttu-id="ad4b4-135">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="ad4b4-135">DateTime the object was last modified.</span></span> <span data-ttu-id="ad4b4-136">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ad4b4-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ad4b4-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ad4b4-137">createdDateTime</span></span>|<span data-ttu-id="ad4b4-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ad4b4-138">DateTimeOffset</span></span>|<span data-ttu-id="ad4b4-139">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="ad4b4-139">DateTime the object was created.</span></span> <span data-ttu-id="ad4b4-140">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ad4b4-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ad4b4-141">description</span><span class="sxs-lookup"><span data-stu-id="ad4b4-141">description</span></span>|<span data-ttu-id="ad4b4-142">String</span><span class="sxs-lookup"><span data-stu-id="ad4b4-142">String</span></span>|<span data-ttu-id="ad4b4-143">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="ad4b4-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ad4b4-144">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ad4b4-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ad4b4-145">displayName</span><span class="sxs-lookup"><span data-stu-id="ad4b4-145">displayName</span></span>|<span data-ttu-id="ad4b4-146">String</span><span class="sxs-lookup"><span data-stu-id="ad4b4-146">String</span></span>|<span data-ttu-id="ad4b4-147">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="ad4b4-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ad4b4-148">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ad4b4-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ad4b4-149">version</span><span class="sxs-lookup"><span data-stu-id="ad4b4-149">version</span></span>|<span data-ttu-id="ad4b4-150">Int32</span><span class="sxs-lookup"><span data-stu-id="ad4b4-150">Int32</span></span>|<span data-ttu-id="ad4b4-151">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="ad4b4-151">Version of the device configuration.</span></span> <span data-ttu-id="ad4b4-152">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ad4b4-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ad4b4-153">omaSettings</span><span class="sxs-lookup"><span data-stu-id="ad4b4-153">omaSettings</span></span>|<span data-ttu-id="ad4b4-154">[omaSetting](../resources/intune_deviceconfig_omasetting.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ad4b4-154">[omaSetting](../resources/intune_deviceconfig_omasetting.md) collection</span></span>|<span data-ttu-id="ad4b4-155">OMA 设置。</span><span class="sxs-lookup"><span data-stu-id="ad4b4-155">OMA settings.</span></span> <span data-ttu-id="ad4b4-156">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="ad4b4-156">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="ad4b4-157">响应</span><span class="sxs-lookup"><span data-stu-id="ad4b4-157">Response</span></span>
<span data-ttu-id="ad4b4-158">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[androidWorkProfileCustomConfiguration](../resources/intune_deviceconfig_androidworkprofilecustomconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="ad4b4-158">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileCustomConfiguration](../resources/intune_deviceconfig_androidworkprofilecustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ad4b4-159">示例</span><span class="sxs-lookup"><span data-stu-id="ad4b4-159">Example</span></span>
### <a name="request"></a><span data-ttu-id="ad4b4-160">请求</span><span class="sxs-lookup"><span data-stu-id="ad4b4-160">Request</span></span>
<span data-ttu-id="ad4b4-161">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ad4b4-161">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 413

{
  "@odata.type": "#microsoft.graph.androidWorkProfileCustomConfiguration",
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

### <a name="response"></a><span data-ttu-id="ad4b4-162">响应</span><span class="sxs-lookup"><span data-stu-id="ad4b4-162">Response</span></span>
<span data-ttu-id="ad4b4-p109">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ad4b4-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 585

{
  "@odata.type": "#microsoft.graph.androidWorkProfileCustomConfiguration",
  "id": "76c5d59b-d59b-76c5-9bd5-c5769bd5c576",
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




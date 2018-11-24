# <a name="create-macoscustomconfiguration"></a><span data-ttu-id="e7609-101">创建 macOSCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="e7609-101">Create macOSCustomConfiguration</span></span>

> <span data-ttu-id="e7609-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="e7609-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e7609-103">创建新的 [macOSCustomConfiguration](../resources/intune_deviceconfig_macoscustomconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e7609-103">Create a new [macOSCustomConfiguration](../resources/intune_deviceconfig_macoscustomconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e7609-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="e7609-104">Prerequisites</span></span>
<span data-ttu-id="e7609-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="e7609-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e7609-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="e7609-107">Permission type</span></span>|<span data-ttu-id="e7609-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e7609-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e7609-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e7609-109">Delegated (work or school account)</span></span>|<span data-ttu-id="e7609-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e7609-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e7609-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e7609-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e7609-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="e7609-112">Not supported.</span></span>|
|<span data-ttu-id="e7609-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="e7609-113">Application</span></span>|<span data-ttu-id="e7609-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="e7609-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e7609-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e7609-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="e7609-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="e7609-116">Request headers</span></span>
|<span data-ttu-id="e7609-117">标头</span><span class="sxs-lookup"><span data-stu-id="e7609-117">Header</span></span>|<span data-ttu-id="e7609-118">值</span><span class="sxs-lookup"><span data-stu-id="e7609-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e7609-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="e7609-119">Authorization</span></span>|<span data-ttu-id="e7609-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e7609-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e7609-121">Accept</span><span class="sxs-lookup"><span data-stu-id="e7609-121">Accept</span></span>|<span data-ttu-id="e7609-122">application/json</span><span class="sxs-lookup"><span data-stu-id="e7609-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e7609-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="e7609-123">Request body</span></span>
<span data-ttu-id="e7609-124">在请求正文中，提供 macOSCustomConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e7609-124">In the request body, supply a JSON representation for the macOSCustomConfiguration object.</span></span>

<span data-ttu-id="e7609-125">下表显示了创建 macOSCustomConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="e7609-125">The following table shows the properties that are required when you create the macOSCustomConfiguration.</span></span>

|<span data-ttu-id="e7609-126">属性</span><span class="sxs-lookup"><span data-stu-id="e7609-126">Property</span></span>|<span data-ttu-id="e7609-127">类型</span><span class="sxs-lookup"><span data-stu-id="e7609-127">Type</span></span>|<span data-ttu-id="e7609-128">说明</span><span class="sxs-lookup"><span data-stu-id="e7609-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e7609-129">id</span><span class="sxs-lookup"><span data-stu-id="e7609-129">id</span></span>|<span data-ttu-id="e7609-130">String</span><span class="sxs-lookup"><span data-stu-id="e7609-130">String</span></span>|<span data-ttu-id="e7609-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="e7609-131">Key of the entity.</span></span> <span data-ttu-id="e7609-132">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e7609-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e7609-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e7609-133">lastModifiedDateTime</span></span>|<span data-ttu-id="e7609-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e7609-134">DateTimeOffset</span></span>|<span data-ttu-id="e7609-135">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="e7609-135">DateTime the object was last modified.</span></span> <span data-ttu-id="e7609-136">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e7609-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e7609-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e7609-137">createdDateTime</span></span>|<span data-ttu-id="e7609-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e7609-138">DateTimeOffset</span></span>|<span data-ttu-id="e7609-139">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="e7609-139">DateTime the object was created.</span></span> <span data-ttu-id="e7609-140">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e7609-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e7609-141">description</span><span class="sxs-lookup"><span data-stu-id="e7609-141">description</span></span>|<span data-ttu-id="e7609-142">String</span><span class="sxs-lookup"><span data-stu-id="e7609-142">String</span></span>|<span data-ttu-id="e7609-143">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="e7609-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="e7609-144">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e7609-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e7609-145">displayName</span><span class="sxs-lookup"><span data-stu-id="e7609-145">displayName</span></span>|<span data-ttu-id="e7609-146">String</span><span class="sxs-lookup"><span data-stu-id="e7609-146">String</span></span>|<span data-ttu-id="e7609-147">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="e7609-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="e7609-148">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e7609-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e7609-149">version</span><span class="sxs-lookup"><span data-stu-id="e7609-149">version</span></span>|<span data-ttu-id="e7609-150">Int32</span><span class="sxs-lookup"><span data-stu-id="e7609-150">Int32</span></span>|<span data-ttu-id="e7609-151">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="e7609-151">Version of the device configuration.</span></span> <span data-ttu-id="e7609-152">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e7609-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e7609-153">payloadName</span><span class="sxs-lookup"><span data-stu-id="e7609-153">payloadName</span></span>|<span data-ttu-id="e7609-154">String</span><span class="sxs-lookup"><span data-stu-id="e7609-154">String</span></span>|<span data-ttu-id="e7609-155">向用户显示的名称。</span><span class="sxs-lookup"><span data-stu-id="e7609-155">Name that is displayed to the user.</span></span>|
|<span data-ttu-id="e7609-156">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="e7609-156">payloadFileName</span></span>|<span data-ttu-id="e7609-157">String</span><span class="sxs-lookup"><span data-stu-id="e7609-157">String</span></span>|<span data-ttu-id="e7609-158">有效负载文件名 (\*.mobileconfig</span><span class="sxs-lookup"><span data-stu-id="e7609-158">Payload file name (\*.mobileconfig</span></span> | <span data-ttu-id="e7609-159">\*.xml)。</span><span class="sxs-lookup"><span data-stu-id="e7609-159">\*.xml).</span></span>|
|<span data-ttu-id="e7609-160">payload</span><span class="sxs-lookup"><span data-stu-id="e7609-160">payload</span></span>|<span data-ttu-id="e7609-161">Binary</span><span class="sxs-lookup"><span data-stu-id="e7609-161">Binary</span></span>|<span data-ttu-id="e7609-162">有效负载。</span><span class="sxs-lookup"><span data-stu-id="e7609-162">Payload.</span></span> <span data-ttu-id="e7609-163">（UTF8 编码的字节数组）</span><span class="sxs-lookup"><span data-stu-id="e7609-163">(UTF8 encoded byte array)</span></span>|



## <a name="response"></a><span data-ttu-id="e7609-164">响应</span><span class="sxs-lookup"><span data-stu-id="e7609-164">Response</span></span>
<span data-ttu-id="e7609-165">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [macOSCustomConfiguration](../resources/intune_deviceconfig_macoscustomconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e7609-165">If successful, this method returns a `201 Created` response code and a [macOSCustomConfiguration](../resources/intune_deviceconfig_macoscustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e7609-166">示例</span><span class="sxs-lookup"><span data-stu-id="e7609-166">Example</span></span>
### <a name="request"></a><span data-ttu-id="e7609-167">请求</span><span class="sxs-lookup"><span data-stu-id="e7609-167">Request</span></span>
<span data-ttu-id="e7609-168">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e7609-168">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 281

{
  "@odata.type": "#microsoft.graph.macOSCustomConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "payloadName": "Payload Name value",
  "payloadFileName": "Payload File Name value",
  "payload": "cGF5bG9hZA=="
}
```

### <a name="response"></a><span data-ttu-id="e7609-169">响应</span><span class="sxs-lookup"><span data-stu-id="e7609-169">Response</span></span>
<span data-ttu-id="e7609-p109">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e7609-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 453

{
  "@odata.type": "#microsoft.graph.macOSCustomConfiguration",
  "id": "a253835d-835d-a253-5d83-53a25d8353a2",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "payloadName": "Payload Name value",
  "payloadFileName": "Payload File Name value",
  "payload": "cGF5bG9hZA=="
}
```




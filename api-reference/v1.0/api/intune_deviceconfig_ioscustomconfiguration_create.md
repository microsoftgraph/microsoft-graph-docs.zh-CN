# <a name="create-ioscustomconfiguration"></a><span data-ttu-id="6c97a-101">创建 iosCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="6c97a-101">Create iosCustomConfiguration</span></span>

> <span data-ttu-id="6c97a-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="6c97a-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6c97a-103">创建新的 [iosCustomConfiguration](../resources/intune_deviceconfig_ioscustomconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6c97a-103">Create a new [iosCustomConfiguration](../resources/intune_deviceconfig_ioscustomconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6c97a-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="6c97a-104">Prerequisites</span></span>
<span data-ttu-id="6c97a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="6c97a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="6c97a-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="6c97a-107">Permission type</span></span>|<span data-ttu-id="6c97a-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="6c97a-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6c97a-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6c97a-109">Delegated (work or school account)</span></span>|<span data-ttu-id="6c97a-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c97a-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6c97a-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6c97a-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6c97a-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="6c97a-112">Not supported.</span></span>|
|<span data-ttu-id="6c97a-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="6c97a-113">Application</span></span>|<span data-ttu-id="6c97a-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="6c97a-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6c97a-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6c97a-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="6c97a-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="6c97a-116">Request headers</span></span>
|<span data-ttu-id="6c97a-117">标头</span><span class="sxs-lookup"><span data-stu-id="6c97a-117">Header</span></span>|<span data-ttu-id="6c97a-118">值</span><span class="sxs-lookup"><span data-stu-id="6c97a-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6c97a-119">授权</span><span class="sxs-lookup"><span data-stu-id="6c97a-119">Authorization</span></span>|<span data-ttu-id="6c97a-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6c97a-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6c97a-121">Accept</span><span class="sxs-lookup"><span data-stu-id="6c97a-121">Accept</span></span>|<span data-ttu-id="6c97a-122">application/json</span><span class="sxs-lookup"><span data-stu-id="6c97a-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6c97a-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="6c97a-123">Request body</span></span>
<span data-ttu-id="6c97a-124">在请求正文中，提供 iosCustomConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6c97a-124">In the request body, supply a JSON representation for the iosCustomConfiguration object.</span></span>

<span data-ttu-id="6c97a-125">下表显示创建 iosCustomConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="6c97a-125">The following table shows the properties that are required when you create the iosCustomConfiguration.</span></span>

|<span data-ttu-id="6c97a-126">属性</span><span class="sxs-lookup"><span data-stu-id="6c97a-126">Property</span></span>|<span data-ttu-id="6c97a-127">类型</span><span class="sxs-lookup"><span data-stu-id="6c97a-127">Type</span></span>|<span data-ttu-id="6c97a-128">说明</span><span class="sxs-lookup"><span data-stu-id="6c97a-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6c97a-129">ID</span><span class="sxs-lookup"><span data-stu-id="6c97a-129">id</span></span>|<span data-ttu-id="6c97a-130">字符串</span><span class="sxs-lookup"><span data-stu-id="6c97a-130">String</span></span>|<span data-ttu-id="6c97a-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="6c97a-131">Key of the entity.</span></span> <span data-ttu-id="6c97a-132">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6c97a-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6c97a-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6c97a-133">lastModifiedDateTime</span></span>|<span data-ttu-id="6c97a-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6c97a-134">DateTimeOffset</span></span>|<span data-ttu-id="6c97a-135">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="6c97a-135">DateTime the object was last modified.</span></span> <span data-ttu-id="6c97a-136">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6c97a-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6c97a-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6c97a-137">createdDateTime</span></span>|<span data-ttu-id="6c97a-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6c97a-138">DateTimeOffset</span></span>|<span data-ttu-id="6c97a-139">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="6c97a-139">DateTime the object was created.</span></span> <span data-ttu-id="6c97a-140">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6c97a-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6c97a-141">说明</span><span class="sxs-lookup"><span data-stu-id="6c97a-141">description</span></span>|<span data-ttu-id="6c97a-142">字符串</span><span class="sxs-lookup"><span data-stu-id="6c97a-142">String</span></span>|<span data-ttu-id="6c97a-143">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="6c97a-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6c97a-144">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6c97a-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6c97a-145">displayName</span><span class="sxs-lookup"><span data-stu-id="6c97a-145">displayName</span></span>|<span data-ttu-id="6c97a-146">字符串</span><span class="sxs-lookup"><span data-stu-id="6c97a-146">String</span></span>|<span data-ttu-id="6c97a-147">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="6c97a-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6c97a-148">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6c97a-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6c97a-149">version</span><span class="sxs-lookup"><span data-stu-id="6c97a-149">version</span></span>|<span data-ttu-id="6c97a-150">Int32</span><span class="sxs-lookup"><span data-stu-id="6c97a-150">Int32</span></span>|<span data-ttu-id="6c97a-151">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="6c97a-151">Version of the device configuration.</span></span> <span data-ttu-id="6c97a-152">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6c97a-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6c97a-153">payloadName</span><span class="sxs-lookup"><span data-stu-id="6c97a-153">payloadName</span></span>|<span data-ttu-id="6c97a-154">字符串</span><span class="sxs-lookup"><span data-stu-id="6c97a-154">String</span></span>|<span data-ttu-id="6c97a-155">向用户显示的名称。</span><span class="sxs-lookup"><span data-stu-id="6c97a-155">Name that is displayed to the user.</span></span>|
|<span data-ttu-id="6c97a-156">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="6c97a-156">payloadFileName</span></span>|<span data-ttu-id="6c97a-157">字符串</span><span class="sxs-lookup"><span data-stu-id="6c97a-157">String</span></span>|<span data-ttu-id="6c97a-158">有效负载文件名 (\*.mobileconfig</span><span class="sxs-lookup"><span data-stu-id="6c97a-158">Payload file name (\*.mobileconfig</span></span> | <span data-ttu-id="6c97a-159">\*.xml)。</span><span class="sxs-lookup"><span data-stu-id="6c97a-159">\*.xml).</span></span>|
|<span data-ttu-id="6c97a-160">负载</span><span class="sxs-lookup"><span data-stu-id="6c97a-160">payload</span></span>|<span data-ttu-id="6c97a-161">二进制</span><span class="sxs-lookup"><span data-stu-id="6c97a-161">Binary</span></span>|<span data-ttu-id="6c97a-162">有效负载。</span><span class="sxs-lookup"><span data-stu-id="6c97a-162">Payload.</span></span> <span data-ttu-id="6c97a-163">（UTF8 编码的字节数组）</span><span class="sxs-lookup"><span data-stu-id="6c97a-163">(UTF8 encoded byte array)</span></span>|



## <a name="response"></a><span data-ttu-id="6c97a-164">响应</span><span class="sxs-lookup"><span data-stu-id="6c97a-164">Response</span></span>
<span data-ttu-id="6c97a-165">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [iosCustomConfiguration](../resources/intune_deviceconfig_ioscustomconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6c97a-165">If successful, this method returns a `201 Created` response code and a [iosCustomConfiguration](../resources/intune_deviceconfig_ioscustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6c97a-166">示例</span><span class="sxs-lookup"><span data-stu-id="6c97a-166">Example</span></span>
### <a name="request"></a><span data-ttu-id="6c97a-167">请求</span><span class="sxs-lookup"><span data-stu-id="6c97a-167">Request</span></span>
<span data-ttu-id="6c97a-168">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6c97a-168">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 343

{
  "@odata.type": "#microsoft.graph.iosCustomConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "payloadName": "Payload Name value",
  "payloadFileName": "Payload File Name value",
  "payload": "cGF5bG9hZA=="
}
```

### <a name="response"></a><span data-ttu-id="6c97a-169">响应</span><span class="sxs-lookup"><span data-stu-id="6c97a-169">Response</span></span>
<span data-ttu-id="6c97a-p109">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6c97a-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 451

{
  "@odata.type": "#microsoft.graph.iosCustomConfiguration",
  "id": "f34428e3-28e3-f344-e328-44f3e32844f3",
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









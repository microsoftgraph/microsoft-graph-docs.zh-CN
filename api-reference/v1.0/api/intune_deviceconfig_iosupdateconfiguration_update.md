# <a name="update-iosupdateconfiguration"></a><span data-ttu-id="00248-101">更新 iosUpdateConfiguration</span><span class="sxs-lookup"><span data-stu-id="00248-101">Update iosUpdateConfiguration</span></span>

> <span data-ttu-id="00248-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="00248-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="00248-103">更新 [iosUpdateConfiguration](../resources/intune_deviceconfig_iosupdateconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="00248-103">Update the properties of a [iosUpdateConfiguration](../resources/intune_deviceconfig_iosupdateconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="00248-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="00248-104">Prerequisites</span></span>
<span data-ttu-id="00248-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="00248-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="00248-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="00248-107">Permission type</span></span>|<span data-ttu-id="00248-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="00248-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="00248-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="00248-109">Delegated (work or school account)</span></span>|<span data-ttu-id="00248-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00248-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="00248-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="00248-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="00248-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="00248-112">Not supported.</span></span>|
|<span data-ttu-id="00248-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="00248-113">Application</span></span>|<span data-ttu-id="00248-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="00248-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="00248-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="00248-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="00248-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="00248-116">Request headers</span></span>
|<span data-ttu-id="00248-117">标头</span><span class="sxs-lookup"><span data-stu-id="00248-117">Header</span></span>|<span data-ttu-id="00248-118">值</span><span class="sxs-lookup"><span data-stu-id="00248-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="00248-119">授权</span><span class="sxs-lookup"><span data-stu-id="00248-119">Authorization</span></span>|<span data-ttu-id="00248-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="00248-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="00248-121">接受</span><span class="sxs-lookup"><span data-stu-id="00248-121">Accept</span></span>|<span data-ttu-id="00248-122">application/json</span><span class="sxs-lookup"><span data-stu-id="00248-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="00248-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="00248-123">Request body</span></span>
<span data-ttu-id="00248-124">在请求正文中，提供 [iosUpdateConfiguration](../resources/intune_deviceconfig_iosupdateconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="00248-124">In the request body, supply a JSON representation for the [iosUpdateConfiguration](../resources/intune_deviceconfig_iosupdateconfiguration.md) object.</span></span>

<span data-ttu-id="00248-125">下表显示创建 [iosUpdateConfiguration](../resources/intune_deviceconfig_iosupdateconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="00248-125">The following table shows the properties that are required when you create the [iosUpdateConfiguration](../resources/intune_deviceconfig_iosupdateconfiguration.md).</span></span>

|<span data-ttu-id="00248-126">属性</span><span class="sxs-lookup"><span data-stu-id="00248-126">Property</span></span>|<span data-ttu-id="00248-127">类型</span><span class="sxs-lookup"><span data-stu-id="00248-127">Type</span></span>|<span data-ttu-id="00248-128">说明</span><span class="sxs-lookup"><span data-stu-id="00248-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="00248-129">ID</span><span class="sxs-lookup"><span data-stu-id="00248-129">id</span></span>|<span data-ttu-id="00248-130">字符串</span><span class="sxs-lookup"><span data-stu-id="00248-130">String</span></span>|<span data-ttu-id="00248-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="00248-131">Key of the entity.</span></span> <span data-ttu-id="00248-132">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="00248-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="00248-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="00248-133">lastModifiedDateTime</span></span>|<span data-ttu-id="00248-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="00248-134">DateTimeOffset</span></span>|<span data-ttu-id="00248-135">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="00248-135">DateTime the object was last modified.</span></span> <span data-ttu-id="00248-136">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="00248-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="00248-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="00248-137">createdDateTime</span></span>|<span data-ttu-id="00248-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="00248-138">DateTimeOffset</span></span>|<span data-ttu-id="00248-139">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="00248-139">DateTime the object was created.</span></span> <span data-ttu-id="00248-140">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="00248-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="00248-141">description</span><span class="sxs-lookup"><span data-stu-id="00248-141">description</span></span>|<span data-ttu-id="00248-142">字符串</span><span class="sxs-lookup"><span data-stu-id="00248-142">String</span></span>|<span data-ttu-id="00248-143">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="00248-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="00248-144">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="00248-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="00248-145">displayName</span><span class="sxs-lookup"><span data-stu-id="00248-145">displayName</span></span>|<span data-ttu-id="00248-146">字符串</span><span class="sxs-lookup"><span data-stu-id="00248-146">String</span></span>|<span data-ttu-id="00248-147">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="00248-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="00248-148">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="00248-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="00248-149">version</span><span class="sxs-lookup"><span data-stu-id="00248-149">version</span></span>|<span data-ttu-id="00248-150">Int32</span><span class="sxs-lookup"><span data-stu-id="00248-150">Int32</span></span>|<span data-ttu-id="00248-151">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="00248-151">Version of the device configuration.</span></span> <span data-ttu-id="00248-152">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="00248-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="00248-153">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="00248-153">activeHoursStart</span></span>|<span data-ttu-id="00248-154">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="00248-154">TimeOfDay</span></span>|<span data-ttu-id="00248-155">使用时段开始时间（使用时段表示不应发生更新安装的时间范围）</span><span class="sxs-lookup"><span data-stu-id="00248-155">Active Hours Start (active hours mean the time window when updates install should not happen)</span></span>|
|<span data-ttu-id="00248-156">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="00248-156">activeHoursEnd</span></span>|<span data-ttu-id="00248-157">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="00248-157">TimeOfDay</span></span>|<span data-ttu-id="00248-158">使用时段结束时间（使用时段表示不应发生更新安装的时间范围）</span><span class="sxs-lookup"><span data-stu-id="00248-158">Active Hours End (active hours mean the time window when updates install should not happen)</span></span>|
|<span data-ttu-id="00248-159">scheduledInstallDays</span><span class="sxs-lookup"><span data-stu-id="00248-159">scheduledInstallDays</span></span>|<span data-ttu-id="00248-160">[dayOfWeek](../resources/intune_deviceconfig_dayofweek.md) 集合</span><span class="sxs-lookup"><span data-stu-id="00248-160">dayOfWeek collection</span></span>|<span data-ttu-id="00248-p108">配置为使用时段所对应的一周的某一天。该集合最多可包含 7 个元素。可取值为：`sunday`、`monday`、`tuesday`、`wednesday`、`thursday`、`friday`、`saturday`。</span><span class="sxs-lookup"><span data-stu-id="00248-p108">Days in week for which active hours are configured. This collection can contain a maximum of 7 elements. The possible values are: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="00248-164">utcTimeOffsetInMinutes</span><span class="sxs-lookup"><span data-stu-id="00248-164">utcTimeOffsetInMinutes</span></span>|<span data-ttu-id="00248-165">Int32</span><span class="sxs-lookup"><span data-stu-id="00248-165">Int32</span></span>|<span data-ttu-id="00248-166">UTC 时间偏移，用分钟表示</span><span class="sxs-lookup"><span data-stu-id="00248-166">UTC Time Offset indicated in minutes</span></span>|



## <a name="response"></a><span data-ttu-id="00248-167">响应</span><span class="sxs-lookup"><span data-stu-id="00248-167">Response</span></span>
<span data-ttu-id="00248-168">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [iosUpdateConfiguration](../resources/intune_deviceconfig_iosupdateconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="00248-168">If successful, this method returns a `200 OK` response code and an updated [iosUpdateConfiguration](../resources/intune_deviceconfig_iosupdateconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="00248-169">示例</span><span class="sxs-lookup"><span data-stu-id="00248-169">Example</span></span>
### <a name="request"></a><span data-ttu-id="00248-170">请求</span><span class="sxs-lookup"><span data-stu-id="00248-170">Request</span></span>
<span data-ttu-id="00248-171">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="00248-171">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 328

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "activeHoursStart": "12:00:05.5020000",
  "activeHoursEnd": "11:59:00.8990000",
  "scheduledInstallDays": [
    "monday"
  ],
  "utcTimeOffsetInMinutes": 6
}
```

### <a name="response"></a><span data-ttu-id="00248-172">响应</span><span class="sxs-lookup"><span data-stu-id="00248-172">Response</span></span>
<span data-ttu-id="00248-p109">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="00248-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 497

{
  "@odata.type": "#microsoft.graph.iosUpdateConfiguration",
  "id": "321aef09-ef09-321a-09ef-1a3209ef1a32",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "activeHoursStart": "12:00:05.5020000",
  "activeHoursEnd": "11:59:00.8990000",
  "scheduledInstallDays": [
    "monday"
  ],
  "utcTimeOffsetInMinutes": 6
}
```









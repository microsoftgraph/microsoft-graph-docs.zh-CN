# <a name="create-deviceconfigurationdevicestatus"></a><span data-ttu-id="48cb7-101">创建 deviceConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="48cb7-101">Create deviceConfigurationDeviceStatus</span></span>

> <span data-ttu-id="48cb7-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="48cb7-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="48cb7-103">创建新的 [deviceConfigurationDeviceStatus](../resources/intune_deviceconfig_deviceconfigurationdevicestatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="48cb7-103">Create a new [deviceConfigurationDeviceStatus](../resources/intune_deviceconfig_deviceconfigurationdevicestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="48cb7-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="48cb7-104">Prerequisites</span></span>
<span data-ttu-id="48cb7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="48cb7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="48cb7-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="48cb7-107">Permission type</span></span>|<span data-ttu-id="48cb7-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="48cb7-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="48cb7-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="48cb7-109">Delegated (work or school account)</span></span>|<span data-ttu-id="48cb7-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48cb7-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="48cb7-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="48cb7-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="48cb7-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="48cb7-112">Not supported.</span></span>|
|<span data-ttu-id="48cb7-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="48cb7-113">Application</span></span>|<span data-ttu-id="48cb7-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="48cb7-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="48cb7-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="48cb7-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="48cb7-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="48cb7-116">Request headers</span></span>
|<span data-ttu-id="48cb7-117">标头</span><span class="sxs-lookup"><span data-stu-id="48cb7-117">Header</span></span>|<span data-ttu-id="48cb7-118">值</span><span class="sxs-lookup"><span data-stu-id="48cb7-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="48cb7-119">授权</span><span class="sxs-lookup"><span data-stu-id="48cb7-119">Authorization</span></span>|<span data-ttu-id="48cb7-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="48cb7-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="48cb7-121">接受</span><span class="sxs-lookup"><span data-stu-id="48cb7-121">Accept</span></span>|<span data-ttu-id="48cb7-122">application/json</span><span class="sxs-lookup"><span data-stu-id="48cb7-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="48cb7-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="48cb7-123">Request body</span></span>
<span data-ttu-id="48cb7-124">在请求正文中，提供 deviceConfigurationDeviceStatus 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="48cb7-124">In the request body, supply a JSON representation for the deviceConfigurationDeviceStatus object.</span></span>

<span data-ttu-id="48cb7-125">下表显示创建 deviceConfigurationDeviceStatus 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="48cb7-125">The following table shows the properties that are required when you create the deviceConfigurationDeviceStatus.</span></span>

|<span data-ttu-id="48cb7-126">属性</span><span class="sxs-lookup"><span data-stu-id="48cb7-126">Property</span></span>|<span data-ttu-id="48cb7-127">类型</span><span class="sxs-lookup"><span data-stu-id="48cb7-127">Type</span></span>|<span data-ttu-id="48cb7-128">说明</span><span class="sxs-lookup"><span data-stu-id="48cb7-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="48cb7-129">id</span><span class="sxs-lookup"><span data-stu-id="48cb7-129">id</span></span>|<span data-ttu-id="48cb7-130">字符串</span><span class="sxs-lookup"><span data-stu-id="48cb7-130">String</span></span>|<span data-ttu-id="48cb7-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="48cb7-131">Key of the entity.</span></span>|
|<span data-ttu-id="48cb7-132">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="48cb7-132">deviceDisplayName</span></span>|<span data-ttu-id="48cb7-133">字符串</span><span class="sxs-lookup"><span data-stu-id="48cb7-133">String</span></span>|<span data-ttu-id="48cb7-134">DevicePolicyStatus 的设备名。</span><span class="sxs-lookup"><span data-stu-id="48cb7-134">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="48cb7-135">userName</span><span class="sxs-lookup"><span data-stu-id="48cb7-135">userName</span></span>|<span data-ttu-id="48cb7-136">字符串</span><span class="sxs-lookup"><span data-stu-id="48cb7-136">String</span></span>|<span data-ttu-id="48cb7-137">报告的用户名</span><span class="sxs-lookup"><span data-stu-id="48cb7-137">The User Name that is being reported</span></span>|
|<span data-ttu-id="48cb7-138">deviceModel</span><span class="sxs-lookup"><span data-stu-id="48cb7-138">deviceModel</span></span>|<span data-ttu-id="48cb7-139">字符串</span><span class="sxs-lookup"><span data-stu-id="48cb7-139">String</span></span>|<span data-ttu-id="48cb7-140">报告的设备模型</span><span class="sxs-lookup"><span data-stu-id="48cb7-140">The device model that is being reported</span></span>|
|<span data-ttu-id="48cb7-141">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="48cb7-141">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="48cb7-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="48cb7-142">DateTimeOffset</span></span>|<span data-ttu-id="48cb7-143">设备符合性宽限期的到期日期/时间</span><span class="sxs-lookup"><span data-stu-id="48cb7-143">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="48cb7-144">status</span><span class="sxs-lookup"><span data-stu-id="48cb7-144">status</span></span>|[<span data-ttu-id="48cb7-145">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="48cb7-145">complianceStatus</span></span>](../resources/intune_shared_compliancestatus.md)|<span data-ttu-id="48cb7-146">策略报告的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="48cb7-146">Compliance status of the policy report.</span></span> <span data-ttu-id="48cb7-147">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`。</span><span class="sxs-lookup"><span data-stu-id="48cb7-147">The possible values are `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, , , , , or .</span></span>|
|<span data-ttu-id="48cb7-148">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="48cb7-148">lastReportedDateTime</span></span>|<span data-ttu-id="48cb7-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="48cb7-149">DateTimeOffset</span></span>|<span data-ttu-id="48cb7-150">策略报告的上次修改日期时间。</span><span class="sxs-lookup"><span data-stu-id="48cb7-150">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="48cb7-151">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="48cb7-151">userPrincipalName</span></span>|<span data-ttu-id="48cb7-152">字符串</span><span class="sxs-lookup"><span data-stu-id="48cb7-152">String</span></span>|<span data-ttu-id="48cb7-153">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="48cb7-153">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="48cb7-154">响应</span><span class="sxs-lookup"><span data-stu-id="48cb7-154">Response</span></span>
<span data-ttu-id="48cb7-155">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [deviceConfigurationDeviceStatus](../resources/intune_deviceconfig_deviceconfigurationdevicestatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="48cb7-155">If successful, this method returns a `201 Created` response code and a [deviceConfigurationDeviceStatus](../resources/intune_deviceconfig_deviceconfigurationdevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="48cb7-156">示例</span><span class="sxs-lookup"><span data-stu-id="48cb7-156">Example</span></span>
### <a name="request"></a><span data-ttu-id="48cb7-157">请求</span><span class="sxs-lookup"><span data-stu-id="48cb7-157">Request</span></span>
<span data-ttu-id="48cb7-158">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="48cb7-158">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses
Content-type: application/json
Content-length: 429

{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceStatus",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="48cb7-159">响应</span><span class="sxs-lookup"><span data-stu-id="48cb7-159">Response</span></span>
<span data-ttu-id="48cb7-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="48cb7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 478

{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceStatus",
  "id": "674e98e5-98e5-674e-e598-4e67e5984e67",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```




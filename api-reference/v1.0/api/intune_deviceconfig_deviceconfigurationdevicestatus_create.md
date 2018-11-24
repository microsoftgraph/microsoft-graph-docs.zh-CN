# <a name="create-deviceconfigurationdevicestatus"></a><span data-ttu-id="06e22-101">创建 deviceConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="06e22-101">Create deviceConfigurationDeviceStatus</span></span>

> <span data-ttu-id="06e22-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="06e22-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="06e22-103">创建新的 [deviceConfigurationDeviceStatus](../resources/intune_deviceconfig_deviceconfigurationdevicestatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="06e22-103">Create a new [deviceConfigurationDeviceStatus](../resources/intune_deviceconfig_deviceconfigurationdevicestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="06e22-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="06e22-104">Prerequisites</span></span>
<span data-ttu-id="06e22-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="06e22-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="06e22-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="06e22-107">Permission type</span></span>|<span data-ttu-id="06e22-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="06e22-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="06e22-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="06e22-109">Delegated (work or school account)</span></span>|<span data-ttu-id="06e22-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06e22-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="06e22-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="06e22-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="06e22-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="06e22-112">Not supported.</span></span>|
|<span data-ttu-id="06e22-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="06e22-113">Application</span></span>|<span data-ttu-id="06e22-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="06e22-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="06e22-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="06e22-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="06e22-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="06e22-116">Request headers</span></span>
|<span data-ttu-id="06e22-117">标头</span><span class="sxs-lookup"><span data-stu-id="06e22-117">Header</span></span>|<span data-ttu-id="06e22-118">值</span><span class="sxs-lookup"><span data-stu-id="06e22-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="06e22-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="06e22-119">Authorization</span></span>|<span data-ttu-id="06e22-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="06e22-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="06e22-121">Accept</span><span class="sxs-lookup"><span data-stu-id="06e22-121">Accept</span></span>|<span data-ttu-id="06e22-122">application/json</span><span class="sxs-lookup"><span data-stu-id="06e22-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="06e22-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="06e22-123">Request body</span></span>
<span data-ttu-id="06e22-124">在请求正文中，提供 deviceConfigurationDeviceStatus 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="06e22-124">In the request body, supply a JSON representation for the deviceConfigurationDeviceStatus object.</span></span>

<span data-ttu-id="06e22-125">下表显示创建 deviceConfigurationDeviceStatus 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="06e22-125">The following table shows the properties that are required when you create the deviceConfigurationDeviceStatus.</span></span>

|<span data-ttu-id="06e22-126">属性</span><span class="sxs-lookup"><span data-stu-id="06e22-126">Property</span></span>|<span data-ttu-id="06e22-127">类型</span><span class="sxs-lookup"><span data-stu-id="06e22-127">Type</span></span>|<span data-ttu-id="06e22-128">说明</span><span class="sxs-lookup"><span data-stu-id="06e22-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06e22-129">id</span><span class="sxs-lookup"><span data-stu-id="06e22-129">id</span></span>|<span data-ttu-id="06e22-130">String</span><span class="sxs-lookup"><span data-stu-id="06e22-130">String</span></span>|<span data-ttu-id="06e22-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="06e22-131">Key of the entity.</span></span>|
|<span data-ttu-id="06e22-132">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="06e22-132">deviceDisplayName</span></span>|<span data-ttu-id="06e22-133">String</span><span class="sxs-lookup"><span data-stu-id="06e22-133">String</span></span>|<span data-ttu-id="06e22-134">DevicePolicyStatus 的设备名。</span><span class="sxs-lookup"><span data-stu-id="06e22-134">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="06e22-135">userName</span><span class="sxs-lookup"><span data-stu-id="06e22-135">userName</span></span>|<span data-ttu-id="06e22-136">String</span><span class="sxs-lookup"><span data-stu-id="06e22-136">String</span></span>|<span data-ttu-id="06e22-137">报告的用户名</span><span class="sxs-lookup"><span data-stu-id="06e22-137">The User Name that is being reported</span></span>|
|<span data-ttu-id="06e22-138">deviceModel</span><span class="sxs-lookup"><span data-stu-id="06e22-138">deviceModel</span></span>|<span data-ttu-id="06e22-139">String</span><span class="sxs-lookup"><span data-stu-id="06e22-139">String</span></span>|<span data-ttu-id="06e22-140">报告的设备模型</span><span class="sxs-lookup"><span data-stu-id="06e22-140">The device model that is being reported</span></span>|
|<span data-ttu-id="06e22-141">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="06e22-141">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="06e22-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="06e22-142">DateTimeOffset</span></span>|<span data-ttu-id="06e22-143">设备符合性宽限期的到期日期/时间</span><span class="sxs-lookup"><span data-stu-id="06e22-143">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="06e22-144">status</span><span class="sxs-lookup"><span data-stu-id="06e22-144">status</span></span>|[<span data-ttu-id="06e22-145">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="06e22-145">complianceStatus</span></span>](../resources/intune_shared_compliancestatus.md)|<span data-ttu-id="06e22-146">策略报告的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="06e22-146">Compliance status of the policy report.</span></span> <span data-ttu-id="06e22-147">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="06e22-147">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="06e22-148">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="06e22-148">lastReportedDateTime</span></span>|<span data-ttu-id="06e22-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="06e22-149">DateTimeOffset</span></span>|<span data-ttu-id="06e22-150">策略报告的上次修改日期时间。</span><span class="sxs-lookup"><span data-stu-id="06e22-150">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="06e22-151">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="06e22-151">userPrincipalName</span></span>|<span data-ttu-id="06e22-152">String</span><span class="sxs-lookup"><span data-stu-id="06e22-152">String</span></span>|<span data-ttu-id="06e22-153">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="06e22-153">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="06e22-154">响应</span><span class="sxs-lookup"><span data-stu-id="06e22-154">Response</span></span>
<span data-ttu-id="06e22-155">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [deviceConfigurationDeviceStatus](../resources/intune_deviceconfig_deviceconfigurationdevicestatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="06e22-155">If successful, this method returns a `201 Created` response code and a [deviceConfigurationDeviceStatus](../resources/intune_deviceconfig_deviceconfigurationdevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="06e22-156">示例</span><span class="sxs-lookup"><span data-stu-id="06e22-156">Example</span></span>
### <a name="request"></a><span data-ttu-id="06e22-157">请求</span><span class="sxs-lookup"><span data-stu-id="06e22-157">Request</span></span>
<span data-ttu-id="06e22-158">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="06e22-158">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="06e22-159">响应</span><span class="sxs-lookup"><span data-stu-id="06e22-159">Response</span></span>
<span data-ttu-id="06e22-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="06e22-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




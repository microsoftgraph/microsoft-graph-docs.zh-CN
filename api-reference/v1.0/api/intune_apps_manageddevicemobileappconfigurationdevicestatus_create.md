# <a name="create-manageddevicemobileappconfigurationdevicestatus"></a><span data-ttu-id="b654f-101">创建 managedDeviceMobileAppConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="b654f-101">Create managedDeviceMobileAppConfigurationDeviceStatus</span></span>

> <span data-ttu-id="b654f-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="b654f-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b654f-103">创建新的 [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune_apps_manageddevicemobileappconfigurationdevicestatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b654f-103">Create a new [deviceCompliancePolicyAssignment](../resources/intune_apps_manageddevicemobileappconfigurationdevicestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b654f-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="b654f-104">Prerequisites</span></span>
<span data-ttu-id="b654f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="b654f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b654f-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="b654f-107">Permission type</span></span>|<span data-ttu-id="b654f-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b654f-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b654f-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b654f-109">Delegated (work or school account)</span></span>|<span data-ttu-id="b654f-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b654f-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b654f-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b654f-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b654f-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="b654f-112">Not supported.</span></span>|
|<span data-ttu-id="b654f-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="b654f-113">Application</span></span>|<span data-ttu-id="b654f-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="b654f-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b654f-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b654f-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="b654f-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="b654f-116">Request headers</span></span>
|<span data-ttu-id="b654f-117">标头</span><span class="sxs-lookup"><span data-stu-id="b654f-117">Header</span></span>|<span data-ttu-id="b654f-118">值</span><span class="sxs-lookup"><span data-stu-id="b654f-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b654f-119">授权</span><span class="sxs-lookup"><span data-stu-id="b654f-119">Authorization</span></span>|<span data-ttu-id="b654f-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b654f-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b654f-121">接受</span><span class="sxs-lookup"><span data-stu-id="b654f-121">Accept</span></span>|<span data-ttu-id="b654f-122">application/json</span><span class="sxs-lookup"><span data-stu-id="b654f-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b654f-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="b654f-123">Request body</span></span>
<span data-ttu-id="b654f-124">在请求正文中，为 managedDeviceMobileAppConfigurationDeviceStatus 对象提供 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b654f-124">In the request body, supply a JSON representation for the user object.</span></span>

<span data-ttu-id="b654f-125">下表显示创建 managedDeviceMobileAppConfigurationDeviceStatus 时必需的属性。</span><span class="sxs-lookup"><span data-stu-id="b654f-125">The following table shows the properties that are required when you create the deviceAppManagement.</span></span>

|<span data-ttu-id="b654f-126">属性</span><span class="sxs-lookup"><span data-stu-id="b654f-126">Property</span></span>|<span data-ttu-id="b654f-127">类型</span><span class="sxs-lookup"><span data-stu-id="b654f-127">Type</span></span>|<span data-ttu-id="b654f-128">说明</span><span class="sxs-lookup"><span data-stu-id="b654f-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b654f-129">id</span><span class="sxs-lookup"><span data-stu-id="b654f-129">id</span></span>|<span data-ttu-id="b654f-130">字符串</span><span class="sxs-lookup"><span data-stu-id="b654f-130">String</span></span>|<span data-ttu-id="b654f-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="b654f-131">Key of the entity.</span></span>|
|<span data-ttu-id="b654f-132">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="b654f-132">deviceDisplayName</span></span>|<span data-ttu-id="b654f-133">字符串</span><span class="sxs-lookup"><span data-stu-id="b654f-133">String</span></span>|<span data-ttu-id="b654f-134">DevicePolicyStatus 的设备名。</span><span class="sxs-lookup"><span data-stu-id="b654f-134">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="b654f-135">userName</span><span class="sxs-lookup"><span data-stu-id="b654f-135">userName</span></span>|<span data-ttu-id="b654f-136">字符串</span><span class="sxs-lookup"><span data-stu-id="b654f-136">String</span></span>|<span data-ttu-id="b654f-137">报告的用户名</span><span class="sxs-lookup"><span data-stu-id="b654f-137">The User Name that is being reported</span></span>|
|<span data-ttu-id="b654f-138">deviceModel</span><span class="sxs-lookup"><span data-stu-id="b654f-138">deviceModel</span></span>|<span data-ttu-id="b654f-139">字符串</span><span class="sxs-lookup"><span data-stu-id="b654f-139">String</span></span>|<span data-ttu-id="b654f-140">报告的设备模型</span><span class="sxs-lookup"><span data-stu-id="b654f-140">The device model that is being reported</span></span>|
|<span data-ttu-id="b654f-141">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="b654f-141">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="b654f-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b654f-142">DateTimeOffset</span></span>|<span data-ttu-id="b654f-143">设备符合性宽限期的到期日期/时间</span><span class="sxs-lookup"><span data-stu-id="b654f-143">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="b654f-144">状态</span><span class="sxs-lookup"><span data-stu-id="b654f-144">status</span></span>|[<span data-ttu-id="b654f-145">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="b654f-145">complianceStatus</span></span>](../resources/intune_shared_compliancestatus.md)|<span data-ttu-id="b654f-146">策略报告的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="b654f-146">Compliance status of the policy report.</span></span> <span data-ttu-id="b654f-147">可能的值为： `unknown` 、 `notApplicable` 、 `compliant` 、 `remediated` 、 `nonCompliant` 、 `error` 、 `conflict` 。</span><span class="sxs-lookup"><span data-stu-id="b654f-147">The possible values are `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, , , , , or .</span></span>|
|<span data-ttu-id="b654f-148">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="b654f-148">lastReportedDateTime</span></span>|<span data-ttu-id="b654f-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b654f-149">DateTimeOffset</span></span>|<span data-ttu-id="b654f-150">策略报告的上次修改日期时间。</span><span class="sxs-lookup"><span data-stu-id="b654f-150">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="b654f-151">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b654f-151">userPrincipalName</span></span>|<span data-ttu-id="b654f-152">字符串</span><span class="sxs-lookup"><span data-stu-id="b654f-152">String</span></span>|<span data-ttu-id="b654f-153">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="b654f-153">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="b654f-154">响应</span><span class="sxs-lookup"><span data-stu-id="b654f-154">Response</span></span>
<span data-ttu-id="b654f-155">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune_apps_manageddevicemobileappconfigurationdevicestatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b654f-155">If successful, this method returns a `201 Created` response code and a [deviceConfigurationAssignment](../resources/intune_apps_manageddevicemobileappconfigurationdevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b654f-156">示例</span><span class="sxs-lookup"><span data-stu-id="b654f-156">Example</span></span>
### <a name="request"></a><span data-ttu-id="b654f-157">请求</span><span class="sxs-lookup"><span data-stu-id="b654f-157">Request</span></span>
<span data-ttu-id="b654f-158">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b654f-158">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses
Content-type: application/json
Content-length: 445

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationDeviceStatus",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="b654f-159">响应</span><span class="sxs-lookup"><span data-stu-id="b654f-159">Response</span></span>
<span data-ttu-id="b654f-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b654f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 494

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationDeviceStatus",
  "id": "477d3651-3651-477d-5136-7d4751367d47",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```




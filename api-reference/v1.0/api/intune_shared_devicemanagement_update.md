# <a name="update-devicemanagement"></a><span data-ttu-id="fe8ff-101">更新 deviceManagement</span><span class="sxs-lookup"><span data-stu-id="fe8ff-101">Update deviceManagement</span></span>

> <span data-ttu-id="fe8ff-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="fe8ff-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fe8ff-103">更新 [deviceManagement](../resources/intune_shared_devicemanagement.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="fe8ff-103">Update the properties of a [deviceManagement](../resources/intune_shared_devicemanagement.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fe8ff-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="fe8ff-104">Prerequisites</span></span>
<span data-ttu-id="fe8ff-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="fe8ff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="fe8ff-107">权限&nbsp;类型&nbsp;（通过&nbsp;工作流）</span><span class="sxs-lookup"><span data-stu-id="fe8ff-107">Permission&nbsp;type&nbsp;(by&nbsp;workflow)</span></span> | <span data-ttu-id="fe8ff-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="fe8ff-108">Permissions (from most to least privileged)</span></span> |
|:---|:---|
| <span data-ttu-id="fe8ff-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fe8ff-109">Delegated (work or school account)</span></span> |
| <span data-ttu-id="fe8ff-110">&nbsp; &nbsp; 审核</span><span class="sxs-lookup"><span data-stu-id="fe8ff-110">&nbsp; &nbsp;Auditing</span></span> | <span data-ttu-id="fe8ff-111">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe8ff-111">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="fe8ff-112">&nbsp; &nbsp; 公司条款</span><span class="sxs-lookup"><span data-stu-id="fe8ff-112">&nbsp; &nbsp; Company terms</span></span> | <span data-ttu-id="fe8ff-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe8ff-113">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="fe8ff-114">&nbsp; &nbsp; 公司注册</span><span class="sxs-lookup"><span data-stu-id="fe8ff-114">&nbsp; &nbsp; Corporate enrollment</span></span> | <span data-ttu-id="fe8ff-115">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe8ff-115">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="fe8ff-116">&nbsp; &nbsp; 设备配置</span><span class="sxs-lookup"><span data-stu-id="fe8ff-116">&nbsp; &nbsp;Device configuration</span></span> | <span data-ttu-id="fe8ff-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe8ff-117">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="fe8ff-118">&nbsp; &nbsp; 设备管理</span><span class="sxs-lookup"><span data-stu-id="fe8ff-118">&nbsp; &nbsp;Device management</span></span> | <span data-ttu-id="fe8ff-119">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe8ff-119">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="fe8ff-120">&nbsp; &nbsp; 端点保护</span><span class="sxs-lookup"><span data-stu-id="fe8ff-120">&nbsp; &nbsp;Endpoint Protection</span></span> | <span data-ttu-id="fe8ff-121">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe8ff-121">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="fe8ff-122">&nbsp; &nbsp; 注册</span><span class="sxs-lookup"><span data-stu-id="fe8ff-122">&nbsp; &nbsp;Enrollment</span></span> | <span data-ttu-id="fe8ff-123">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe8ff-123">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="fe8ff-124">&nbsp; &nbsp; 通知</span><span class="sxs-lookup"><span data-stu-id="fe8ff-124">&nbsp; &nbsp;Notification</span></span> | <span data-ttu-id="fe8ff-125">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe8ff-125">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="fe8ff-126">&nbsp; &nbsp; 加入</span><span class="sxs-lookup"><span data-stu-id="fe8ff-126">&nbsp; &nbsp; On-boarding</span></span> | <span data-ttu-id="fe8ff-127">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe8ff-127">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="fe8ff-128">&nbsp; &nbsp; RBAC</span><span class="sxs-lookup"><span data-stu-id="fe8ff-128">&nbsp; &nbsp;RBAC</span></span> | <span data-ttu-id="fe8ff-129">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe8ff-129">DeviceManagementRBAC.ReadWrite.All</span></span> |
| <span data-ttu-id="fe8ff-130">&nbsp; &nbsp; 远程协助</span><span class="sxs-lookup"><span data-stu-id="fe8ff-130">remote assistance,</span></span> | <span data-ttu-id="fe8ff-131">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe8ff-131">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="fe8ff-132">&nbsp; &nbsp; 电信费用管理</span><span class="sxs-lookup"><span data-stu-id="fe8ff-132">&nbsp; &nbsp;Telecom expense management partner</span></span> | <span data-ttu-id="fe8ff-133">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe8ff-133">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="fe8ff-134">&nbsp; &nbsp; 疑难解答</span><span class="sxs-lookup"><span data-stu-id="fe8ff-134">&nbsp; &nbsp;Troubleshooting</span></span> | <span data-ttu-id="fe8ff-135">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe8ff-135">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="fe8ff-136">&nbsp; &nbsp; Windows 信息保护</span><span class="sxs-lookup"><span data-stu-id="fe8ff-136">Windows information protection</span></span> | <span data-ttu-id="fe8ff-137">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe8ff-137">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="fe8ff-138">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fe8ff-138">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fe8ff-139">不支持。</span><span class="sxs-lookup"><span data-stu-id="fe8ff-139">Not supported.</span></span>|
| <span data-ttu-id="fe8ff-140">应用程序</span><span class="sxs-lookup"><span data-stu-id="fe8ff-140">Application</span></span> | <span data-ttu-id="fe8ff-141">不支持。</span><span class="sxs-lookup"><span data-stu-id="fe8ff-141">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fe8ff-142">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fe8ff-142">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement
```

## <a name="request-headers"></a><span data-ttu-id="fe8ff-143">请求标头</span><span class="sxs-lookup"><span data-stu-id="fe8ff-143">Request headers</span></span>
|<span data-ttu-id="fe8ff-144">标头</span><span class="sxs-lookup"><span data-stu-id="fe8ff-144">Header</span></span>|<span data-ttu-id="fe8ff-145">值</span><span class="sxs-lookup"><span data-stu-id="fe8ff-145">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fe8ff-146">授权</span><span class="sxs-lookup"><span data-stu-id="fe8ff-146">Authorization</span></span>|<span data-ttu-id="fe8ff-147">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="fe8ff-147">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fe8ff-148">接受</span><span class="sxs-lookup"><span data-stu-id="fe8ff-148">Accept</span></span>|<span data-ttu-id="fe8ff-149">application/json</span><span class="sxs-lookup"><span data-stu-id="fe8ff-149">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fe8ff-150">请求正文</span><span class="sxs-lookup"><span data-stu-id="fe8ff-150">Request body</span></span>
<span data-ttu-id="fe8ff-151">在请求正文中，提供 [deviceManagement](../resources/intune_shared_devicemanagement.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fe8ff-151">In the request body, supply a JSON representation for the [deviceManagement](../resources/intune_shared_devicemanagement.md) object.</span></span>

<span data-ttu-id="fe8ff-152">下表显示创建 [deviceManagement](../resources/intune_shared_devicemanagement.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="fe8ff-152">The following table shows the properties that are required when you create the [deviceManagement](../resources/intune_shared_devicemanagement.md).</span></span>

|<span data-ttu-id="fe8ff-153">属性</span><span class="sxs-lookup"><span data-stu-id="fe8ff-153">Property</span></span>|<span data-ttu-id="fe8ff-154">类型</span><span class="sxs-lookup"><span data-stu-id="fe8ff-154">Type</span></span>|<span data-ttu-id="fe8ff-155">说明</span><span class="sxs-lookup"><span data-stu-id="fe8ff-155">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fe8ff-156">id</span><span class="sxs-lookup"><span data-stu-id="fe8ff-156">id</span></span>|<span data-ttu-id="fe8ff-157">字符串</span><span class="sxs-lookup"><span data-stu-id="fe8ff-157">String</span></span>|<span data-ttu-id="fe8ff-158">设备唯一标识符</span><span class="sxs-lookup"><span data-stu-id="fe8ff-158">Unique Identifier for the device</span></span>|
|<span data-ttu-id="fe8ff-159">**设备配置**</span><span class="sxs-lookup"><span data-stu-id="fe8ff-159">**Device configuration**</span></span>|
|<span data-ttu-id="fe8ff-160">settings</span><span class="sxs-lookup"><span data-stu-id="fe8ff-160">settings</span></span>|[<span data-ttu-id="fe8ff-161">deviceManagementSettings</span><span class="sxs-lookup"><span data-stu-id="fe8ff-161">deviceManagementSettings</span></span>](../resources/intune_deviceconfig_devicemanagementsettings.md)|<span data-ttu-id="fe8ff-162">帐户级别设置。</span><span class="sxs-lookup"><span data-stu-id="fe8ff-162">Account level settings.</span></span>|
|<span data-ttu-id="fe8ff-163">**设备管理**</span><span class="sxs-lookup"><span data-stu-id="fe8ff-163">**Device management**</span></span>|
|<span data-ttu-id="fe8ff-164">subscriptionState</span><span class="sxs-lookup"><span data-stu-id="fe8ff-164">subscriptionState</span></span>|[<span data-ttu-id="fe8ff-165">deviceManagementSubscriptionState</span><span class="sxs-lookup"><span data-stu-id="fe8ff-165">deviceManagementSubscriptionState</span></span>](../resources/intune_devices_devicemanagementsubscriptionstate.md)|<span data-ttu-id="fe8ff-166">租户移动设备管理订阅状态。</span><span class="sxs-lookup"><span data-stu-id="fe8ff-166">Tenant mobile device management subscription state.</span></span> <span data-ttu-id="fe8ff-167">可取值为：`pending`、`active`、`warning`、`disabled`、`deleted`、`blocked`、`lockedOut`。</span><span class="sxs-lookup"><span data-stu-id="fe8ff-167">The possible values are `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`, , , , , or .</span></span>|
|<span data-ttu-id="fe8ff-168">**加入**</span><span class="sxs-lookup"><span data-stu-id="fe8ff-168">**On-boarding**</span></span>|
|<span data-ttu-id="fe8ff-169">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="fe8ff-169">intuneBrand</span></span>|[<span data-ttu-id="fe8ff-170">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="fe8ff-170">intuneBrand</span></span>](../resources/intune_onboarding_intunebrand.md)|<span data-ttu-id="fe8ff-171">intuneBrand 包含在自定义公司门户应用程序以及最终用户 Web 门户的外观时使用的数据。</span><span class="sxs-lookup"><span data-stu-id="fe8ff-171">intuneBrand contains data which is used in customizing the appearance of the Company Portal applications as well as the end user web portal.</span></span>|

<span data-ttu-id="fe8ff-172">请求正文属性支持根据工作流而有所不同。</span><span class="sxs-lookup"><span data-stu-id="fe8ff-172">Request body property support varies according to context.</span></span>

## <a name="response"></a><span data-ttu-id="fe8ff-173">响应</span><span class="sxs-lookup"><span data-stu-id="fe8ff-173">Response</span></span>
<span data-ttu-id="fe8ff-174">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [deviceManagement](../resources/intune_shared_devicemanagement.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="fe8ff-174">If successful, this method returns a `200 OK` response code and an updated [deviceManagement](../resources/intune_shared_devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fe8ff-175">示例</span><span class="sxs-lookup"><span data-stu-id="fe8ff-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="fe8ff-176">请求</span><span class="sxs-lookup"><span data-stu-id="fe8ff-176">Request</span></span>
<span data-ttu-id="fe8ff-177">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="fe8ff-177">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement
Content-type: application/json
Content-length: 751

{
  "subscriptionState": "active",
  "subscriptions": "intune",
  "adminConsent": {
    "@odata.type": "microsoft.graph.adminConsent",
    "shareAPNSData": "granted"
  },
  "deviceProtectionOverview": {
    "@odata.type": "microsoft.graph.deviceProtectionOverview",
    "totalReportedDeviceCount": 8,
    "inactiveThreatAgentDeviceCount": 14,
    "unknownStateThreatAgentDeviceCount": 2,
    "pendingSignatureUpdateDeviceCount": 1,
    "cleanDeviceCount": 0,
    "pendingFullScanDeviceCount": 10,
    "pendingRestartDeviceCount": 9,
    "pendingManualStepsDeviceCount": 13,
    "pendingOfflineScanDeviceCount": 13,
    "criticalFailuresDeviceCount": 11
  },
  "accountMoveCompletionDateTime": "2017-01-01T00:01:17.9006709-08:00"
}
```

### <a name="response"></a><span data-ttu-id="fe8ff-178">响应</span><span class="sxs-lookup"><span data-stu-id="fe8ff-178">Response</span></span>

<span data-ttu-id="fe8ff-179">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="fe8ff-179">Here is an example of the response.</span></span> <span data-ttu-id="fe8ff-180">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="fe8ff-180">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="fe8ff-181">返回的属性根据工作流和上下文而有所不同。</span><span class="sxs-lookup"><span data-stu-id="fe8ff-181">Returned properties vary according to workflow and context.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 855

{
  "@odata.type": "#microsoft.graph.deviceManagement",
  "id": "0b283420-3420-0b28-2034-280b2034280b",
  "subscriptionState": "active",
  "subscriptions": "intune",
  "adminConsent": {
    "@odata.type": "microsoft.graph.adminConsent",
    "shareAPNSData": "granted"
  },
  "deviceProtectionOverview": {
    "@odata.type": "microsoft.graph.deviceProtectionOverview",
    "totalReportedDeviceCount": 8,
    "inactiveThreatAgentDeviceCount": 14,
    "unknownStateThreatAgentDeviceCount": 2,
    "pendingSignatureUpdateDeviceCount": 1,
    "cleanDeviceCount": 0,
    "pendingFullScanDeviceCount": 10,
    "pendingRestartDeviceCount": 9,
    "pendingManualStepsDeviceCount": 13,
    "pendingOfflineScanDeviceCount": 13,
    "criticalFailuresDeviceCount": 11
  },
  "accountMoveCompletionDateTime": "2017-01-01T00:01:17.9006709-08:00"
}
```




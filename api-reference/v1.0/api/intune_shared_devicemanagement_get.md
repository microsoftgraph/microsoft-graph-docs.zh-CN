# <a name="get-devicemanagement"></a><span data-ttu-id="83ff1-101">获取 deviceManagement</span><span class="sxs-lookup"><span data-stu-id="83ff1-101">Get deviceManagement</span></span>

> <span data-ttu-id="83ff1-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="83ff1-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="83ff1-103">读取 [deviceManagement](../resources/intune_shared_devicemanagement.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="83ff1-103">Read properties and relationships of the [deviceManagement](../resources/intune_shared_devicemanagement.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="83ff1-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="83ff1-104">Prerequisites</span></span>
<span data-ttu-id="83ff1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="83ff1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="83ff1-107">权限&nbsp;类型&nbsp;（通过&nbsp;工作流）</span><span class="sxs-lookup"><span data-stu-id="83ff1-107">Permission&nbsp;type&nbsp;(by&nbsp;workflow)</span></span> | <span data-ttu-id="83ff1-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="83ff1-108">Permissions (from most to least privileged)</span></span> |
|:---|:---|
| <span data-ttu-id="83ff1-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="83ff1-109">Delegated (work or school account)</span></span> | |
| <span data-ttu-id="83ff1-110">&nbsp; &nbsp; 审核</span><span class="sxs-lookup"><span data-stu-id="83ff1-110">&nbsp; &nbsp;Auditing</span></span> | <span data-ttu-id="83ff1-111">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="83ff1-111">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="83ff1-112">&nbsp; &nbsp; 公司条款</span><span class="sxs-lookup"><span data-stu-id="83ff1-112">&nbsp; &nbsp; Company terms</span></span> | <span data-ttu-id="83ff1-113">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="83ff1-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="83ff1-114">&nbsp; &nbsp; 设备配置</span><span class="sxs-lookup"><span data-stu-id="83ff1-114">&nbsp; &nbsp;Device Configuration.</span></span> | <span data-ttu-id="83ff1-115">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="83ff1-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="83ff1-116">&nbsp; &nbsp; 设备管理</span><span class="sxs-lookup"><span data-stu-id="83ff1-116">&nbsp; &nbsp;Device management</span></span> | <span data-ttu-id="83ff1-117">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="83ff1-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="83ff1-118">&nbsp; &nbsp; 注册</span><span class="sxs-lookup"><span data-stu-id="83ff1-118">&nbsp; &nbsp;Enrollment</span></span> | <span data-ttu-id="83ff1-119">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="83ff1-119">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="83ff1-120">&nbsp; &nbsp; 通知</span><span class="sxs-lookup"><span data-stu-id="83ff1-120">&nbsp; &nbsp;Notification</span></span> | <span data-ttu-id="83ff1-121">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="83ff1-121">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="83ff1-122">&nbsp; &nbsp; 参与／有份</span><span class="sxs-lookup"><span data-stu-id="83ff1-122">&nbsp; &nbsp; On-boarding</span></span> | <span data-ttu-id="83ff1-123">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="83ff1-123">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="83ff1-124">&nbsp; &nbsp; RBAC</span><span class="sxs-lookup"><span data-stu-id="83ff1-124">&nbsp; &nbsp;RBAC</span></span> | <span data-ttu-id="83ff1-125">DeviceManagementRBAC.ReadWrite.All、DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="83ff1-125">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span> |
| <span data-ttu-id="83ff1-126">&nbsp; &nbsp; 远程协助</span><span class="sxs-lookup"><span data-stu-id="83ff1-126">remote assistance,</span></span> | <span data-ttu-id="83ff1-127">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="83ff1-127">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="83ff1-128">&nbsp; &nbsp; 电信费用管理</span><span class="sxs-lookup"><span data-stu-id="83ff1-128">&nbsp; &nbsp;Telecom expense management partner</span></span> | <span data-ttu-id="83ff1-129">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="83ff1-129">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="83ff1-130">&nbsp; &nbsp; 疑难解答</span><span class="sxs-lookup"><span data-stu-id="83ff1-130">&nbsp; &nbsp;Troubleshooting</span></span> | <span data-ttu-id="83ff1-131">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="83ff1-131">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
| <span data-ttu-id="83ff1-132">&nbsp; &nbsp; Windows 信息保护</span><span class="sxs-lookup"><span data-stu-id="83ff1-132">Windows information protection</span></span> | <span data-ttu-id="83ff1-133">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="83ff1-133">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
| <span data-ttu-id="83ff1-134">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="83ff1-134">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="83ff1-135">不支持。</span><span class="sxs-lookup"><span data-stu-id="83ff1-135">Not supported.</span></span>|
| <span data-ttu-id="83ff1-136">应用程序</span><span class="sxs-lookup"><span data-stu-id="83ff1-136">Application</span></span> | <span data-ttu-id="83ff1-137">不支持。</span><span class="sxs-lookup"><span data-stu-id="83ff1-137">Not supported.</span></span> |



## <a name="http-request"></a><span data-ttu-id="83ff1-138">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="83ff1-138">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement
```

## <a name="optional-query-parameters"></a><span data-ttu-id="83ff1-139">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="83ff1-139">Optional query parameters</span></span>
<span data-ttu-id="83ff1-140">此方法支持 [OData 查询参数](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="83ff1-140">This method supports the [OData Query Parameters](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="83ff1-141">请求标头</span><span class="sxs-lookup"><span data-stu-id="83ff1-141">Request headers</span></span>
|<span data-ttu-id="83ff1-142">标头</span><span class="sxs-lookup"><span data-stu-id="83ff1-142">Header</span></span>|<span data-ttu-id="83ff1-143">值</span><span class="sxs-lookup"><span data-stu-id="83ff1-143">Value</span></span>|
|:---|:---|
|<span data-ttu-id="83ff1-144">授权</span><span class="sxs-lookup"><span data-stu-id="83ff1-144">Authorization</span></span>|<span data-ttu-id="83ff1-145">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="83ff1-145">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="83ff1-146">Accept</span><span class="sxs-lookup"><span data-stu-id="83ff1-146">Accept</span></span>|<span data-ttu-id="83ff1-147">application/json</span><span class="sxs-lookup"><span data-stu-id="83ff1-147">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="83ff1-148">请求正文</span><span class="sxs-lookup"><span data-stu-id="83ff1-148">Request body</span></span>
<span data-ttu-id="83ff1-149">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="83ff1-149">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="83ff1-150">响应</span><span class="sxs-lookup"><span data-stu-id="83ff1-150">Response</span></span>
<span data-ttu-id="83ff1-151">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和 [deviceManagement](../resources/intune_shared_devicemanagement.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="83ff1-151">If successful, this method returns a `200 OK` response code and [deviceManagement](../resources/intune_shared_devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="83ff1-152">示例</span><span class="sxs-lookup"><span data-stu-id="83ff1-152">Example</span></span>
### <a name="request"></a><span data-ttu-id="83ff1-153">请求</span><span class="sxs-lookup"><span data-stu-id="83ff1-153">Request</span></span>
<span data-ttu-id="83ff1-154">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="83ff1-154">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement
```

### <a name="response"></a><span data-ttu-id="83ff1-155">响应</span><span class="sxs-lookup"><span data-stu-id="83ff1-155">Response</span></span>
<span data-ttu-id="83ff1-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="83ff1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 918

{
  "value": {
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
}
```




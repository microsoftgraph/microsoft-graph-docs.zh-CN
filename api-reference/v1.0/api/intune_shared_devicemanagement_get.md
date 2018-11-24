# <a name="get-devicemanagement"></a><span data-ttu-id="0bcb8-101">获取 deviceManagement</span><span class="sxs-lookup"><span data-stu-id="0bcb8-101">Get deviceManagement</span></span>

> <span data-ttu-id="0bcb8-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="0bcb8-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0bcb8-103">读取 [deviceManagement](../resources/intune_shared_devicemanagement.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0bcb8-103">Read properties and relationships of the [deviceManagement](../resources/intune_shared_devicemanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0bcb8-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="0bcb8-104">Prerequisites</span></span>
<span data-ttu-id="0bcb8-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](../../../concepts/permissions_reference.md)。
</span><span class="sxs-lookup"><span data-stu-id="0bcb8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="0bcb8-107">权限&nbsp;类型&nbsp;(通过&nbsp;工作流)</span><span class="sxs-lookup"><span data-stu-id="0bcb8-107">Permission&nbsp;type&nbsp;(by&nbsp;workflow)</span></span> | <span data-ttu-id="0bcb8-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="0bcb8-108">Permissions (from most to least privileged)</span></span> |
|:---|:---|
| <span data-ttu-id="0bcb8-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0bcb8-109">Delegated (work or school account)</span></span> | |
| <span data-ttu-id="0bcb8-110">&nbsp;&nbsp;审核</span><span class="sxs-lookup"><span data-stu-id="0bcb8-110">&nbsp; &nbsp; Auditing</span></span> | <span data-ttu-id="0bcb8-111">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="0bcb8-111">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="0bcb8-112">&nbsp;&nbsp;公司术语</span><span class="sxs-lookup"><span data-stu-id="0bcb8-112">&nbsp; &nbsp; Company terms</span></span> | <span data-ttu-id="0bcb8-113">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="0bcb8-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="0bcb8-114">&nbsp;&nbsp;设备配置</span><span class="sxs-lookup"><span data-stu-id="0bcb8-114">&nbsp; &nbsp; Device configuration</span></span> | <span data-ttu-id="0bcb8-115">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="0bcb8-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="0bcb8-116">&nbsp;&nbsp;设备管理</span><span class="sxs-lookup"><span data-stu-id="0bcb8-116">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="0bcb8-117">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="0bcb8-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="0bcb8-118">&nbsp;&nbsp;注册</span><span class="sxs-lookup"><span data-stu-id="0bcb8-118">&nbsp; &nbsp; Enrollment</span></span> | <span data-ttu-id="0bcb8-119">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="0bcb8-119">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="0bcb8-120">&nbsp;&nbsp;通知</span><span class="sxs-lookup"><span data-stu-id="0bcb8-120">&nbsp; &nbsp; Notification</span></span> | <span data-ttu-id="0bcb8-121">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="0bcb8-121">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="0bcb8-122">&nbsp;&nbsp;入职培训</span><span class="sxs-lookup"><span data-stu-id="0bcb8-122">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="0bcb8-123">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="0bcb8-123">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="0bcb8-124">&nbsp;&nbsp; RBAC</span><span class="sxs-lookup"><span data-stu-id="0bcb8-124">&nbsp; &nbsp; RBAC</span></span> | <span data-ttu-id="0bcb8-125">DeviceManagementRBAC.ReadWrite.All、DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="0bcb8-125">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span> |
| <span data-ttu-id="0bcb8-126">&nbsp;&nbsp;远程协助</span><span class="sxs-lookup"><span data-stu-id="0bcb8-126">&nbsp; &nbsp; Remote assistance</span></span> | <span data-ttu-id="0bcb8-127">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="0bcb8-127">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="0bcb8-128">&nbsp;&nbsp;电信支出管理</span><span class="sxs-lookup"><span data-stu-id="0bcb8-128">&nbsp; &nbsp; Telecom expense management</span></span> | <span data-ttu-id="0bcb8-129">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="0bcb8-129">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="0bcb8-130">&nbsp;&nbsp;疑难解答</span><span class="sxs-lookup"><span data-stu-id="0bcb8-130">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="0bcb8-131">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="0bcb8-131">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
| <span data-ttu-id="0bcb8-132">&nbsp;&nbsp; Windows 信息保护</span><span class="sxs-lookup"><span data-stu-id="0bcb8-132">&nbsp; &nbsp; Windows Information Protection</span></span> | <span data-ttu-id="0bcb8-133">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="0bcb8-133">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
| <span data-ttu-id="0bcb8-134">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0bcb8-134">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0bcb8-135">不支持。</span><span class="sxs-lookup"><span data-stu-id="0bcb8-135">Not supported.</span></span>|
| <span data-ttu-id="0bcb8-136">应用程序</span><span class="sxs-lookup"><span data-stu-id="0bcb8-136">Application</span></span> | <span data-ttu-id="0bcb8-137">不支持。</span><span class="sxs-lookup"><span data-stu-id="0bcb8-137">Not supported.</span></span> |



## <a name="http-request"></a><span data-ttu-id="0bcb8-138">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0bcb8-138">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0bcb8-139">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="0bcb8-139">Optional query parameters</span></span>
<span data-ttu-id="0bcb8-140">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="0bcb8-140">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="0bcb8-141">请求标头</span><span class="sxs-lookup"><span data-stu-id="0bcb8-141">Request headers</span></span>
|<span data-ttu-id="0bcb8-142">标头</span><span class="sxs-lookup"><span data-stu-id="0bcb8-142">Header</span></span>|<span data-ttu-id="0bcb8-143">值</span><span class="sxs-lookup"><span data-stu-id="0bcb8-143">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0bcb8-144">Authorization</span><span class="sxs-lookup"><span data-stu-id="0bcb8-144">Authorization</span></span>|<span data-ttu-id="0bcb8-145">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="0bcb8-145">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0bcb8-146">Accept</span><span class="sxs-lookup"><span data-stu-id="0bcb8-146">Accept</span></span>|<span data-ttu-id="0bcb8-147">application/json</span><span class="sxs-lookup"><span data-stu-id="0bcb8-147">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0bcb8-148">请求正文</span><span class="sxs-lookup"><span data-stu-id="0bcb8-148">Request body</span></span>
<span data-ttu-id="0bcb8-149">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0bcb8-149">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0bcb8-150">响应</span><span class="sxs-lookup"><span data-stu-id="0bcb8-150">Response</span></span>
<span data-ttu-id="0bcb8-151">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和 [deviceManagement](../resources/intune_shared_devicemanagement.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0bcb8-151">If successful, this method returns a `200 OK` response code and [deviceManagement](../resources/intune_shared_devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0bcb8-152">示例</span><span class="sxs-lookup"><span data-stu-id="0bcb8-152">Example</span></span>
### <a name="request"></a><span data-ttu-id="0bcb8-153">请求</span><span class="sxs-lookup"><span data-stu-id="0bcb8-153">Request</span></span>
<span data-ttu-id="0bcb8-154">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0bcb8-154">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement
```

### <a name="response"></a><span data-ttu-id="0bcb8-155">响应</span><span class="sxs-lookup"><span data-stu-id="0bcb8-155">Response</span></span>
<span data-ttu-id="0bcb8-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0bcb8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




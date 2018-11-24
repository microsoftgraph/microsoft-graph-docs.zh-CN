# <a name="list-manageddevicemobileappconfigurationdevicestatuses"></a><span data-ttu-id="f29a8-101">列表 managedDeviceMobileAppConfigurationDeviceStatuses</span><span class="sxs-lookup"><span data-stu-id="f29a8-101">List managedDeviceMobileAppConfigurationDeviceStatuses</span></span>

> <span data-ttu-id="f29a8-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="f29a8-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f29a8-103">列出属性和[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune_apps_manageddevicemobileappconfigurationdevicestatus.md)对象之间的关系。</span><span class="sxs-lookup"><span data-stu-id="f29a8-103">List properties and relationships of the [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune_apps_manageddevicemobileappconfigurationdevicestatus.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f29a8-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="f29a8-104">Prerequisites</span></span>
<span data-ttu-id="f29a8-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](../../../concepts/permissions_reference.md)。
</span><span class="sxs-lookup"><span data-stu-id="f29a8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f29a8-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="f29a8-107">Permission type</span></span>|<span data-ttu-id="f29a8-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f29a8-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f29a8-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f29a8-109">Delegated (work or school account)</span></span>|<span data-ttu-id="f29a8-110">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="f29a8-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="f29a8-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f29a8-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f29a8-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="f29a8-112">Not supported.</span></span>|
|<span data-ttu-id="f29a8-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="f29a8-113">Application</span></span>|<span data-ttu-id="f29a8-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f29a8-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f29a8-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f29a8-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="f29a8-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="f29a8-116">Request headers</span></span>
|<span data-ttu-id="f29a8-117">标头</span><span class="sxs-lookup"><span data-stu-id="f29a8-117">Header</span></span>|<span data-ttu-id="f29a8-118">值</span><span class="sxs-lookup"><span data-stu-id="f29a8-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f29a8-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="f29a8-119">Authorization</span></span>|<span data-ttu-id="f29a8-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f29a8-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f29a8-121">Accept</span><span class="sxs-lookup"><span data-stu-id="f29a8-121">Accept</span></span>|<span data-ttu-id="f29a8-122">application/json</span><span class="sxs-lookup"><span data-stu-id="f29a8-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f29a8-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="f29a8-123">Request body</span></span>
<span data-ttu-id="f29a8-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f29a8-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f29a8-125">响应</span><span class="sxs-lookup"><span data-stu-id="f29a8-125">Response</span></span>
<span data-ttu-id="f29a8-126">如果成功，此方法返回`200 OK`响应代码和响应正文中的[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune_apps_manageddevicemobileappconfigurationdevicestatus.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="f29a8-126">If successful, this method returns a `200 OK` response code and a collection of [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune_apps_manageddevicemobileappconfigurationdevicestatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f29a8-127">示例</span><span class="sxs-lookup"><span data-stu-id="f29a8-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="f29a8-128">请求</span><span class="sxs-lookup"><span data-stu-id="f29a8-128">Request</span></span>
<span data-ttu-id="f29a8-129">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f29a8-129">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses
```

### <a name="response"></a><span data-ttu-id="f29a8-130">响应</span><span class="sxs-lookup"><span data-stu-id="f29a8-130">Response</span></span>
<span data-ttu-id="f29a8-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f29a8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 563

{
  "value": [
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
  ]
}
```




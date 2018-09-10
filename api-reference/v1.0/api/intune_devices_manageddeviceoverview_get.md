# <a name="get-manageddeviceoverview"></a><span data-ttu-id="f4f71-101">获取 managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="f4f71-101">Get managedDeviceOverview</span></span>

> <span data-ttu-id="f4f71-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="f4f71-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f4f71-103">读取 [managedDeviceOverview](../resources/intune_devices_manageddeviceoverview.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f4f71-103">Read properties and relationships of the [managedDeviceOverview](../resources/intune_devices_manageddeviceoverview.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f4f71-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="f4f71-104">Prerequisites</span></span>
<span data-ttu-id="f4f71-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="f4f71-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f4f71-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="f4f71-107">Permission type</span></span>|<span data-ttu-id="f4f71-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f4f71-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f4f71-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f4f71-109">Delegated (work or school account)</span></span>|<span data-ttu-id="f4f71-110">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="f4f71-110">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="f4f71-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f4f71-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f4f71-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="f4f71-112">Not supported.</span></span>|
|<span data-ttu-id="f4f71-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="f4f71-113">Application</span></span>|<span data-ttu-id="f4f71-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f4f71-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f4f71-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f4f71-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managedDeviceOverview
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f4f71-116">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="f4f71-116">Optional query parameters</span></span>
<span data-ttu-id="f4f71-117">此方法支持 [OData 查询参数](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="f4f71-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="f4f71-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="f4f71-118">Request headers</span></span>
|<span data-ttu-id="f4f71-119">标头</span><span class="sxs-lookup"><span data-stu-id="f4f71-119">Header</span></span>|<span data-ttu-id="f4f71-120">值</span><span class="sxs-lookup"><span data-stu-id="f4f71-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f4f71-121">授权</span><span class="sxs-lookup"><span data-stu-id="f4f71-121">Authorization</span></span>|<span data-ttu-id="f4f71-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f4f71-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f4f71-123">Accept</span><span class="sxs-lookup"><span data-stu-id="f4f71-123">Accept</span></span>|<span data-ttu-id="f4f71-124">application/json</span><span class="sxs-lookup"><span data-stu-id="f4f71-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f4f71-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="f4f71-125">Request body</span></span>
<span data-ttu-id="f4f71-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f4f71-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f4f71-127">响应</span><span class="sxs-lookup"><span data-stu-id="f4f71-127">Response</span></span>
<span data-ttu-id="f4f71-128">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [managedDeviceOverview](../resources/intune_devices_manageddeviceoverview.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f4f71-128">If successful, this method returns a `200 OK` response code and [managedDeviceOverview](../resources/intune_devices_manageddeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f4f71-129">示例</span><span class="sxs-lookup"><span data-stu-id="f4f71-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="f4f71-130">请求</span><span class="sxs-lookup"><span data-stu-id="f4f71-130">Request</span></span>
<span data-ttu-id="f4f71-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f4f71-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/managedDeviceOverview
```

### <a name="response"></a><span data-ttu-id="f4f71-132">响应</span><span class="sxs-lookup"><span data-stu-id="f4f71-132">Response</span></span>
<span data-ttu-id="f4f71-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f4f71-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 797

{
  "value": {
    "@odata.type": "#microsoft.graph.managedDeviceOverview",
    "id": "42a91653-1653-42a9-5316-a9425316a942",
    "enrolledDeviceCount": 3,
    "mdmEnrolledCount": 0,
    "dualEnrolledDeviceCount": 7,
    "deviceOperatingSystemSummary": {
      "@odata.type": "microsoft.graph.deviceOperatingSystemSummary",
      "androidCount": 12,
      "iosCount": 8,
      "macOSCount": 10,
      "windowsMobileCount": 2,
      "windowsCount": 12,
      "unknownCount": 12
    },
    "deviceExchangeAccessStateSummary": {
      "@odata.type": "microsoft.graph.deviceExchangeAccessStateSummary",
      "allowedDeviceCount": 2,
      "blockedDeviceCount": 2,
      "quarantinedDeviceCount": 6,
      "unknownDeviceCount": 2,
      "unavailableDeviceCount": 6
    }
  }
}
```









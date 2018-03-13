# <a name="get-devicecompliancedevicestatus"></a><span data-ttu-id="cc37d-101">获取 deviceComplianceDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="cc37d-101">Get deviceComplianceDeviceStatus</span></span>

> <span data-ttu-id="cc37d-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="cc37d-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cc37d-103">读取 [deviceComplianceDeviceStatus](../resources/intune_deviceconfig_devicecompliancedevicestatus.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="cc37d-103">Read properties and relationships of [plannerTaskDetails](../resources/intune_deviceconfig_devicecompliancedevicestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="cc37d-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="cc37d-104">Prerequisites</span></span>
<span data-ttu-id="cc37d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="cc37d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="cc37d-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="cc37d-107">Permission type</span></span>|<span data-ttu-id="cc37d-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="cc37d-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cc37d-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cc37d-109">Delegated (work or school account)</span></span>|<span data-ttu-id="cc37d-110">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="cc37d-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="cc37d-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cc37d-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cc37d-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="cc37d-112">Not supported.</span></span>|
|<span data-ttu-id="cc37d-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="cc37d-113">Application</span></span>|<span data-ttu-id="cc37d-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="cc37d-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cc37d-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cc37d-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses/{deviceComplianceDeviceStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cc37d-116">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="cc37d-116">Optional query parameters</span></span>
<span data-ttu-id="cc37d-117">此方法支持 [OData 查询参数](https://developer.microsoft.com/zh-CN/graph/docs/overview/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="cc37d-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/zh-CN/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="cc37d-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="cc37d-118">Request headers</span></span>
|<span data-ttu-id="cc37d-119">标头</span><span class="sxs-lookup"><span data-stu-id="cc37d-119">Header</span></span>|<span data-ttu-id="cc37d-120">值</span><span class="sxs-lookup"><span data-stu-id="cc37d-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cc37d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="cc37d-121">Authorization</span></span>|<span data-ttu-id="cc37d-122">需要持有者&lt;令牌&gt;。</span><span class="sxs-lookup"><span data-stu-id="cc37d-122">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="cc37d-123">Accept</span><span class="sxs-lookup"><span data-stu-id="cc37d-123">Accept</span></span>|<span data-ttu-id="cc37d-124">application/json</span><span class="sxs-lookup"><span data-stu-id="cc37d-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cc37d-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="cc37d-125">Request body</span></span>
<span data-ttu-id="cc37d-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="cc37d-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cc37d-127">响应</span><span class="sxs-lookup"><span data-stu-id="cc37d-127">Response</span></span>
<span data-ttu-id="cc37d-128">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [deviceComplianceDeviceStatus](../resources/intune_deviceconfig_devicecompliancedevicestatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="cc37d-128">If successful, this method returns a `200 OK` response code and a [ListItemVersion](../resources/intune_deviceconfig_devicecompliancedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cc37d-129">示例</span><span class="sxs-lookup"><span data-stu-id="cc37d-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="cc37d-130">请求</span><span class="sxs-lookup"><span data-stu-id="cc37d-130">Request</span></span>
<span data-ttu-id="cc37d-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="cc37d-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses/{deviceComplianceDeviceStatusId}
```

### <a name="response"></a><span data-ttu-id="cc37d-132">响应</span><span class="sxs-lookup"><span data-stu-id="cc37d-132">Response</span></span>
<span data-ttu-id="cc37d-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="cc37d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 512

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceComplianceDeviceStatus",
    "id": "c6c78124-8124-c6c7-2481-c7c62481c7c6",
    "deviceDisplayName": "Device Display Name value",
    "userName": "User Name value",
    "deviceModel": "Device Model value",
    "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
    "status": "notApplicable",
    "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
    "userPrincipalName": "User Principal Name value"
  }
}
```




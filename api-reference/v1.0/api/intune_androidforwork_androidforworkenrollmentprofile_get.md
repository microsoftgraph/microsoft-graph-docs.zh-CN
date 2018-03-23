# <a name="get-androidforworkenrollmentprofile"></a><span data-ttu-id="a85e8-101">获取 androidForWorkEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="a85e8-101">Get androidForWorkEnrollmentProfile</span></span>

> <span data-ttu-id="a85e8-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="a85e8-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a85e8-103">读取 [androidForWorkEnrollmentProfile](../resources/intune_androidforwork_androidforworkenrollmentprofile.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a85e8-103">Read properties and relationships of [plannerTaskDetails](../resources/intune_androidforwork_androidforworkenrollmentprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a85e8-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="a85e8-104">Prerequisites</span></span>
<span data-ttu-id="a85e8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="a85e8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a85e8-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="a85e8-107">Permission type</span></span>|<span data-ttu-id="a85e8-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a85e8-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a85e8-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a85e8-109">Delegated (work or school account)</span></span>|<span data-ttu-id="a85e8-110">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a85e8-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="a85e8-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a85e8-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a85e8-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="a85e8-112">Not supported.</span></span>|
|<span data-ttu-id="a85e8-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="a85e8-113">Application</span></span>|<span data-ttu-id="a85e8-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="a85e8-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a85e8-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a85e8-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/androidForWorkEnrollmentProfiles/{androidForWorkEnrollmentProfileId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a85e8-116">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="a85e8-116">Optional query parameters</span></span>
<span data-ttu-id="a85e8-117">此方法支持 [OData 查询参数](https://developer.microsoft.com/zh-CN/graph/docs/overview/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="a85e8-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/zh-CN/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="a85e8-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="a85e8-118">Request headers</span></span>
|<span data-ttu-id="a85e8-119">标头</span><span class="sxs-lookup"><span data-stu-id="a85e8-119">Header</span></span>|<span data-ttu-id="a85e8-120">值</span><span class="sxs-lookup"><span data-stu-id="a85e8-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a85e8-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a85e8-121">Authorization</span></span>|<span data-ttu-id="a85e8-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a85e8-122">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="a85e8-123">Accept</span><span class="sxs-lookup"><span data-stu-id="a85e8-123">Accept</span></span>|<span data-ttu-id="a85e8-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a85e8-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a85e8-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="a85e8-125">Request body</span></span>
<span data-ttu-id="a85e8-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a85e8-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a85e8-127">响应</span><span class="sxs-lookup"><span data-stu-id="a85e8-127">Response</span></span>
<span data-ttu-id="a85e8-128">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [androidForWorkEnrollmentProfile](../resources/intune_androidforwork_androidforworkenrollmentprofile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a85e8-128">If successful, this method returns a `200 OK` response code and a [ListItemVersion](../resources/intune_androidforwork_androidforworkenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a85e8-129">示例</span><span class="sxs-lookup"><span data-stu-id="a85e8-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="a85e8-130">请求</span><span class="sxs-lookup"><span data-stu-id="a85e8-130">Request</span></span>
<span data-ttu-id="a85e8-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a85e8-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/androidForWorkEnrollmentProfiles/{androidForWorkEnrollmentProfileId}
```

### <a name="response"></a><span data-ttu-id="a85e8-132">响应</span><span class="sxs-lookup"><span data-stu-id="a85e8-132">Response</span></span>
<span data-ttu-id="a85e8-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a85e8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 872

{
  "value": {
    "@odata.type": "#microsoft.graph.androidForWorkEnrollmentProfile",
    "accountId": "Account Id value",
    "id": "e6742553-2553-e674-5325-74e6532574e6",
    "name": "Name value",
    "displayName": "Display Name value",
    "description": "Description value",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "tokenValue": "Token Value value",
    "tokenExpirationDateTime": "2016-12-31T23:59:54.0590989-08:00",
    "totalEnrollmentCount": 4,
    "enrolledDeviceCount": 3,
    "qrCode": "Qr Code value",
    "qrCodeContent": "Qr Code Content value",
    "qrCodeImage": {
      "@odata.type": "microsoft.graph.mimeContent",
      "type": "Type value",
      "value": "dmFsdWU="
    }
  }
}
```




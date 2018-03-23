# <a name="get-softwareupdatestatussummary"></a><span data-ttu-id="655f3-101">获取 softwareUpdateStatusSummary</span><span class="sxs-lookup"><span data-stu-id="655f3-101">Get softwareUpdateStatusSummary</span></span>

> <span data-ttu-id="655f3-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="655f3-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="655f3-103">读取 [softwareUpdateStatusSummary](../resources/intune_deviceconfig_softwareupdatestatussummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="655f3-103">Read properties and relationships of [plannerProgressTaskBoardTaskFormat](../resources/intune_deviceconfig_softwareupdatestatussummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="655f3-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="655f3-104">Prerequisites</span></span>
<span data-ttu-id="655f3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="655f3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="655f3-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="655f3-107">Permission type</span></span>|<span data-ttu-id="655f3-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="655f3-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="655f3-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="655f3-109">Delegated (work or school account)</span></span>|<span data-ttu-id="655f3-110">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="655f3-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="655f3-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="655f3-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="655f3-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="655f3-112">Not supported.</span></span>|
|<span data-ttu-id="655f3-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="655f3-113">Application</span></span>|<span data-ttu-id="655f3-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="655f3-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="655f3-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="655f3-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/softwareUpdateStatusSummary
```

## <a name="optional-query-parameters"></a><span data-ttu-id="655f3-116">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="655f3-116">Optional query parameters</span></span>
<span data-ttu-id="655f3-117">此方法支持 [OData 查询参数](https://developer.microsoft.com/zh-CN/graph/docs/overview/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="655f3-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/zh-CN/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="655f3-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="655f3-118">Request headers</span></span>
|<span data-ttu-id="655f3-119">标头</span><span class="sxs-lookup"><span data-stu-id="655f3-119">Header</span></span>|<span data-ttu-id="655f3-120">值</span><span class="sxs-lookup"><span data-stu-id="655f3-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="655f3-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="655f3-121">Authorization</span></span>|<span data-ttu-id="655f3-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="655f3-122">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="655f3-123">Accept</span><span class="sxs-lookup"><span data-stu-id="655f3-123">Accept</span></span>|<span data-ttu-id="655f3-124">application/json</span><span class="sxs-lookup"><span data-stu-id="655f3-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="655f3-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="655f3-125">Request body</span></span>
<span data-ttu-id="655f3-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="655f3-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="655f3-127">响应</span><span class="sxs-lookup"><span data-stu-id="655f3-127">Response</span></span>
<span data-ttu-id="655f3-128">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [softwareUpdateStatusSummary](../resources/intune_deviceconfig_softwareupdatestatussummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="655f3-128">If successful, this method returns a `200 OK` response code and a [DriveItemVersion](../resources/intune_deviceconfig_softwareupdatestatussummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="655f3-129">示例</span><span class="sxs-lookup"><span data-stu-id="655f3-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="655f3-130">请求</span><span class="sxs-lookup"><span data-stu-id="655f3-130">Request</span></span>
<span data-ttu-id="655f3-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="655f3-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/softwareUpdateStatusSummary
```

### <a name="response"></a><span data-ttu-id="655f3-132">响应</span><span class="sxs-lookup"><span data-stu-id="655f3-132">Response</span></span>
<span data-ttu-id="655f3-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="655f3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 620

{
  "value": {
    "@odata.type": "#microsoft.graph.softwareUpdateStatusSummary",
    "id": "4f71421f-421f-4f71-1f42-714f1f42714f",
    "displayName": "Display Name value",
    "compliantDeviceCount": 4,
    "nonCompliantDeviceCount": 7,
    "remediatedDeviceCount": 5,
    "errorDeviceCount": 0,
    "unknownDeviceCount": 2,
    "conflictDeviceCount": 3,
    "notApplicableDeviceCount": 8,
    "compliantUserCount": 2,
    "nonCompliantUserCount": 5,
    "remediatedUserCount": 3,
    "errorUserCount": 14,
    "unknownUserCount": 0,
    "conflictUserCount": 1,
    "notApplicableUserCount": 6
  }
}
```




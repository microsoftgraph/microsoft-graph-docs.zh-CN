# <a name="get-devicemanagementtroubleshootingevent"></a><span data-ttu-id="ceddf-101">获取 deviceManagementTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="ceddf-101">Get deviceManagementTroubleshootingEvent</span></span>

> <span data-ttu-id="ceddf-102">**重要说明：**Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="ceddf-102">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ceddf-103">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ceddf-103">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ceddf-104">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="ceddf-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ceddf-105">读取 [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ceddf-105">Read properties and relationships of the [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ceddf-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="ceddf-106">Prerequisites</span></span>
<span data-ttu-id="ceddf-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="ceddf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ceddf-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="ceddf-109">Permission type</span></span>|<span data-ttu-id="ceddf-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ceddf-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ceddf-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ceddf-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ceddf-112">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="ceddf-112">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="ceddf-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ceddf-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ceddf-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="ceddf-114">Not supported.</span></span>|
|<span data-ttu-id="ceddf-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="ceddf-115">Application</span></span>|<span data-ttu-id="ceddf-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ceddf-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ceddf-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ceddf-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ceddf-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="ceddf-118">Optional query parameters</span></span>
<span data-ttu-id="ceddf-119">此方法支持 [OData 查询参数](https://developer.microsoft.com/zh-CN/graph/docs/overview/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="ceddf-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/zh-CN/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="ceddf-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="ceddf-120">Request headers</span></span>
|<span data-ttu-id="ceddf-121">标头</span><span class="sxs-lookup"><span data-stu-id="ceddf-121">Header</span></span>|<span data-ttu-id="ceddf-122">值</span><span class="sxs-lookup"><span data-stu-id="ceddf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ceddf-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ceddf-123">Authorization</span></span>|<span data-ttu-id="ceddf-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ceddf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ceddf-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ceddf-125">Accept</span></span>|<span data-ttu-id="ceddf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ceddf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ceddf-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="ceddf-127">Request body</span></span>
<span data-ttu-id="ceddf-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ceddf-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ceddf-129">响应</span><span class="sxs-lookup"><span data-stu-id="ceddf-129">Response</span></span>
<span data-ttu-id="ceddf-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ceddf-130">If successful, this method returns a `200 OK` response code and [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ceddf-131">示例</span><span class="sxs-lookup"><span data-stu-id="ceddf-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="ceddf-132">请求</span><span class="sxs-lookup"><span data-stu-id="ceddf-132">Request</span></span>
<span data-ttu-id="ceddf-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ceddf-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

### <a name="response"></a><span data-ttu-id="ceddf-134">响应</span><span class="sxs-lookup"><span data-stu-id="ceddf-134">Response</span></span>
<span data-ttu-id="ceddf-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ceddf-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 255

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementTroubleshootingEvent",
    "id": "fb26dcee-dcee-fb26-eedc-26fbeedc26fb",
    "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
    "correlationId": "Correlation Id value"
  }
}
```




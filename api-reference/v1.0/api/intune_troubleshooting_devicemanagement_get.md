# <a name="get-devicemanagement"></a><span data-ttu-id="ba3ae-101">获取 deviceManagement</span><span class="sxs-lookup"><span data-stu-id="ba3ae-101">Get deviceManagement</span></span>

> <span data-ttu-id="ba3ae-102">**重要说明：**Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="ba3ae-102">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ba3ae-103">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ba3ae-103">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ba3ae-104">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="ba3ae-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ba3ae-105">读取 [deviceManagement](../resources/intune_troubleshooting_devicemanagement.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ba3ae-105">Read properties and relationships of the [deviceManagement](../resources/intune_troubleshooting_devicemanagement.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ba3ae-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="ba3ae-106">Prerequisites</span></span>
<span data-ttu-id="ba3ae-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="ba3ae-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ba3ae-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="ba3ae-109">Permission type</span></span>|<span data-ttu-id="ba3ae-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ba3ae-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ba3ae-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ba3ae-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ba3ae-112">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="ba3ae-112">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="ba3ae-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ba3ae-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ba3ae-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="ba3ae-114">Not supported.</span></span>|
|<span data-ttu-id="ba3ae-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="ba3ae-115">Application</span></span>|<span data-ttu-id="ba3ae-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ba3ae-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ba3ae-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ba3ae-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ba3ae-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="ba3ae-118">Optional query parameters</span></span>
<span data-ttu-id="ba3ae-119">此方法支持 [OData 查询参数](https://developer.microsoft.com/zh-CN/graph/docs/overview/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="ba3ae-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/zh-CN/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="ba3ae-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="ba3ae-120">Request headers</span></span>
|<span data-ttu-id="ba3ae-121">标头</span><span class="sxs-lookup"><span data-stu-id="ba3ae-121">Header</span></span>|<span data-ttu-id="ba3ae-122">值</span><span class="sxs-lookup"><span data-stu-id="ba3ae-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ba3ae-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ba3ae-123">Authorization</span></span>|<span data-ttu-id="ba3ae-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ba3ae-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ba3ae-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ba3ae-125">Accept</span></span>|<span data-ttu-id="ba3ae-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ba3ae-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ba3ae-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="ba3ae-127">Request body</span></span>
<span data-ttu-id="ba3ae-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ba3ae-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ba3ae-129">响应</span><span class="sxs-lookup"><span data-stu-id="ba3ae-129">Response</span></span>
<span data-ttu-id="ba3ae-130">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和 [deviceManagement](../resources/intune_troubleshooting_devicemanagement.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ba3ae-130">If successful, this method returns a `200 OK` response code and [deviceManagement](../resources/intune_troubleshooting_devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ba3ae-131">示例</span><span class="sxs-lookup"><span data-stu-id="ba3ae-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="ba3ae-132">请求</span><span class="sxs-lookup"><span data-stu-id="ba3ae-132">Request</span></span>
<span data-ttu-id="ba3ae-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ba3ae-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement
```

### <a name="response"></a><span data-ttu-id="ba3ae-134">响应</span><span class="sxs-lookup"><span data-stu-id="ba3ae-134">Response</span></span>
<span data-ttu-id="ba3ae-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ba3ae-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 130

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagement",
    "id": "0b283420-3420-0b28-2034-280b2034280b"
  }
}
```




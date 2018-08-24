# <a name="get-devicecategory"></a><span data-ttu-id="a7561-101">获取 deviceCategory</span><span class="sxs-lookup"><span data-stu-id="a7561-101">Get deviceCategory</span></span>

> <span data-ttu-id="a7561-102">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="a7561-102">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a7561-103">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a7561-103">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a7561-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="a7561-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a7561-105">读取 [deviceCategory](../resources/intune_shared_devicecategory.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a7561-105">Read properties and relationships of the [deviceCategory](../resources/intune_shared_devicecategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a7561-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="a7561-106">Prerequisites</span></span>
<span data-ttu-id="a7561-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="a7561-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a7561-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="a7561-109">Permission type</span></span>|<span data-ttu-id="a7561-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a7561-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a7561-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a7561-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a7561-112">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="a7561-112">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="a7561-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a7561-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a7561-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="a7561-114">Not supported.</span></span>|
|<span data-ttu-id="a7561-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="a7561-115">Application</span></span>|<span data-ttu-id="a7561-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a7561-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a7561-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a7561-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/deviceCategory
GET /deviceManagement/deviceCategories/{deviceCategoryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a7561-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="a7561-118">Optional query parameters</span></span>
<span data-ttu-id="a7561-119">此方法支持 [OData 查询参数](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="a7561-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a7561-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="a7561-120">Request headers</span></span>
|<span data-ttu-id="a7561-121">标头</span><span class="sxs-lookup"><span data-stu-id="a7561-121">Header</span></span>|<span data-ttu-id="a7561-122">值</span><span class="sxs-lookup"><span data-stu-id="a7561-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a7561-123">授权</span><span class="sxs-lookup"><span data-stu-id="a7561-123">Authorization</span></span>|<span data-ttu-id="a7561-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a7561-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a7561-125">接受</span><span class="sxs-lookup"><span data-stu-id="a7561-125">Accept</span></span>|<span data-ttu-id="a7561-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a7561-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a7561-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="a7561-127">Request body</span></span>
<span data-ttu-id="a7561-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a7561-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a7561-129">响应</span><span class="sxs-lookup"><span data-stu-id="a7561-129">Response</span></span>
<span data-ttu-id="a7561-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [deviceCategory](../resources/intune_shared_devicecategory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a7561-130">If successful, this method returns a `200 OK` response code and [deviceCategory](../resources/intune_shared_devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a7561-131">示例</span><span class="sxs-lookup"><span data-stu-id="a7561-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="a7561-132">请求</span><span class="sxs-lookup"><span data-stu-id="a7561-132">Request</span></span>
<span data-ttu-id="a7561-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a7561-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCategories/{deviceCategoryId}
```

### <a name="response"></a><span data-ttu-id="a7561-134">响应</span><span class="sxs-lookup"><span data-stu-id="a7561-134">Response</span></span>
<span data-ttu-id="a7561-135">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="a7561-135">Here is an example of the response.</span></span> <span data-ttu-id="a7561-136">注意：为简洁起见，可能会截断此处展示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="a7561-136">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="a7561-137">从实际的调用返回的属性根据上下文而有所不同。</span><span class="sxs-lookup"><span data-stu-id="a7561-137">Properties returned from an actual call vary according to context.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 211

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceCategory",
    "id": "f881b841-b841-f881-41b8-81f841b881f8",
    "displayName": "Display Name value",
    "description": "Description value"
  }
}
```




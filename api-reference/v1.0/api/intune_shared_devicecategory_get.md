# <a name="get-devicecategory"></a><span data-ttu-id="fed15-101">获取 deviceCategory</span><span class="sxs-lookup"><span data-stu-id="fed15-101">Get deviceCategory</span></span>



> <span data-ttu-id="fed15-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="fed15-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fed15-103">读取 [deviceCategory](../resources/intune_shared_devicecategory.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="fed15-103">Read properties and relationships of the [deviceCategory](../resources/intune_shared_devicecategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fed15-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="fed15-104">Prerequisites</span></span>
<span data-ttu-id="fed15-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](../../../concepts/permissions_reference.md)。
</span><span class="sxs-lookup"><span data-stu-id="fed15-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="fed15-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="fed15-107">Permission type</span></span>|<span data-ttu-id="fed15-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="fed15-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fed15-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fed15-109">Delegated (work or school account)</span></span>||
| <span data-ttu-id="fed15-110">&nbsp; &nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="fed15-110">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="fed15-111">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="fed15-111">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
| <span data-ttu-id="fed15-112">&nbsp;&nbsp; **入职培训**</span><span class="sxs-lookup"><span data-stu-id="fed15-112">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="fed15-113">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="fed15-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="fed15-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fed15-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fed15-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="fed15-115">Not supported.</span></span>|
|<span data-ttu-id="fed15-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="fed15-116">Application</span></span>|<span data-ttu-id="fed15-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="fed15-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fed15-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fed15-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/deviceCategory
GET /deviceManagement/deviceCategories/{deviceCategoryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fed15-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="fed15-119">Optional query parameters</span></span>
<span data-ttu-id="fed15-120">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="fed15-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fed15-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="fed15-121">Request headers</span></span>
|<span data-ttu-id="fed15-122">标头</span><span class="sxs-lookup"><span data-stu-id="fed15-122">Header</span></span>|<span data-ttu-id="fed15-123">值</span><span class="sxs-lookup"><span data-stu-id="fed15-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fed15-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="fed15-124">Authorization</span></span>|<span data-ttu-id="fed15-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="fed15-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fed15-126">Accept</span><span class="sxs-lookup"><span data-stu-id="fed15-126">Accept</span></span>|<span data-ttu-id="fed15-127">application/json</span><span class="sxs-lookup"><span data-stu-id="fed15-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fed15-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="fed15-128">Request body</span></span>
<span data-ttu-id="fed15-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="fed15-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fed15-130">响应</span><span class="sxs-lookup"><span data-stu-id="fed15-130">Response</span></span>
<span data-ttu-id="fed15-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [deviceCategory](../resources/intune_shared_devicecategory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="fed15-131">If successful, this method returns a `200 OK` response code and [deviceCategory](../resources/intune_shared_devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fed15-132">示例</span><span class="sxs-lookup"><span data-stu-id="fed15-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="fed15-133">请求</span><span class="sxs-lookup"><span data-stu-id="fed15-133">Request</span></span>
<span data-ttu-id="fed15-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="fed15-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/deviceCategory
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCategories/{deviceCategoryId}

```

### <a name="response"></a><span data-ttu-id="fed15-135">响应</span><span class="sxs-lookup"><span data-stu-id="fed15-135">Response</span></span>
<span data-ttu-id="fed15-136">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="fed15-136">Here is an example of the response.</span></span> <span data-ttu-id="fed15-137">注意：为简洁起见，可能会截断此处展示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="fed15-137">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="fed15-138">从实际的调用返回的属性有所不同根据上下文。</span><span class="sxs-lookup"><span data-stu-id="fed15-138">Properties returned from an actual call vary according to context.</span></span>

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




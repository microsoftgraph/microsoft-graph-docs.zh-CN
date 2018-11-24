# <a name="get-reportroot"></a><span data-ttu-id="54b88-101">获取 reportRoot</span><span class="sxs-lookup"><span data-stu-id="54b88-101">Get reportRoot</span></span>

> <span data-ttu-id="54b88-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="54b88-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="54b88-103">读取 [reportRoot](../resources/intune_shared_reportroot.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="54b88-103">Read properties and relationships of the [reportRoot](../resources/intune_shared_reportroot.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="54b88-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="54b88-104">Prerequisites</span></span>
<span data-ttu-id="54b88-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](../../../concepts/permissions_reference.md)。
</span><span class="sxs-lookup"><span data-stu-id="54b88-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="54b88-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="54b88-107">Permission type</span></span>|<span data-ttu-id="54b88-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="54b88-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="54b88-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="54b88-109">Delegated (work or school account)</span></span>||
| <span data-ttu-id="54b88-110">&nbsp;&nbsp;设备配置</span><span class="sxs-lookup"><span data-stu-id="54b88-110">&nbsp; &nbsp; Device configuration</span></span> | <span data-ttu-id="54b88-111">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="54b88-111">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="54b88-112">&nbsp;&nbsp;疑难解答</span><span class="sxs-lookup"><span data-stu-id="54b88-112">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="54b88-113">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="54b88-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="54b88-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="54b88-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="54b88-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="54b88-115">Not supported.</span></span>|
|<span data-ttu-id="54b88-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="54b88-116">Application</span></span>|<span data-ttu-id="54b88-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="54b88-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="54b88-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="54b88-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports
```

## <a name="optional-query-parameters"></a><span data-ttu-id="54b88-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="54b88-119">Optional query parameters</span></span>
<span data-ttu-id="54b88-120">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="54b88-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="54b88-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="54b88-121">Request headers</span></span>
|<span data-ttu-id="54b88-122">标头</span><span class="sxs-lookup"><span data-stu-id="54b88-122">Header</span></span>|<span data-ttu-id="54b88-123">值</span><span class="sxs-lookup"><span data-stu-id="54b88-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="54b88-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="54b88-124">Authorization</span></span>|<span data-ttu-id="54b88-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="54b88-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="54b88-126">Accept</span><span class="sxs-lookup"><span data-stu-id="54b88-126">Accept</span></span>|<span data-ttu-id="54b88-127">application/json</span><span class="sxs-lookup"><span data-stu-id="54b88-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="54b88-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="54b88-128">Request body</span></span>
<span data-ttu-id="54b88-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="54b88-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="54b88-130">响应</span><span class="sxs-lookup"><span data-stu-id="54b88-130">Response</span></span>
<span data-ttu-id="54b88-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [reportRoot](../resources/intune_shared_reportroot.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="54b88-131">If successful, this method returns a `200 OK` response code and [reportRoot](../resources/intune_shared_reportroot.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="54b88-132">示例</span><span class="sxs-lookup"><span data-stu-id="54b88-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="54b88-133">请求</span><span class="sxs-lookup"><span data-stu-id="54b88-133">Request</span></span>
<span data-ttu-id="54b88-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="54b88-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/reports
```

### <a name="response"></a><span data-ttu-id="54b88-135">响应</span><span class="sxs-lookup"><span data-stu-id="54b88-135">Response</span></span>
<span data-ttu-id="54b88-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="54b88-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 124

{
  "value": {
    "@odata.type": "#microsoft.graph.reportRoot",
    "id": "9ab6b3dd-b3dd-9ab6-ddb3-b69addb3b69a"
  }
}
```









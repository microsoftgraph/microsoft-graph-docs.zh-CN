# <a name="get-deviceappmanagement"></a><span data-ttu-id="e8a30-101">获取 deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="e8a30-101">Get deviceAppManagement</span></span>

> <span data-ttu-id="e8a30-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="e8a30-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e8a30-103">读取 [deviceAppManagement](../resources/intune_shared_deviceappmanagement.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e8a30-103">Read properties and relationships of the [deviceAppManagement](../resources/intune_shared_deviceappmanagement.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e8a30-104">必要条件</span><span class="sxs-lookup"><span data-stu-id="e8a30-104">Prerequisites</span></span>
<span data-ttu-id="e8a30-105">以下权限之一需要调用此 API。</span><span class="sxs-lookup"><span data-stu-id="e8a30-105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see Permissions.</span></span> <span data-ttu-id="e8a30-106">若要了解详细信息，包括如何选择权限，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="e8a30-106">To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>  <span data-ttu-id="e8a30-107">请注意，相应权限根据工作流而有所不同。</span><span class="sxs-lookup"><span data-stu-id="e8a30-107">Note that the appropriate permission varies according to the workflow.</span></span>

|<span data-ttu-id="e8a30-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="e8a30-108">Permission type</span></span>|<span data-ttu-id="e8a30-109">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e8a30-109">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e8a30-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e8a30-110">Delegated (work or school account)</span></span>|<span data-ttu-id="e8a30-111">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="e8a30-111">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
|<span data-ttu-id="e8a30-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e8a30-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e8a30-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="e8a30-113">Not supported.</span></span>|
|<span data-ttu-id="e8a30-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="e8a30-114">Application</span></span>|<span data-ttu-id="e8a30-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="e8a30-115">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e8a30-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e8a30-116">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e8a30-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="e8a30-117">Optional query parameters</span></span>
<span data-ttu-id="e8a30-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="e8a30-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="e8a30-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="e8a30-119">Request headers</span></span>
|<span data-ttu-id="e8a30-120">标头</span><span class="sxs-lookup"><span data-stu-id="e8a30-120">Header</span></span>|<span data-ttu-id="e8a30-121">值</span><span class="sxs-lookup"><span data-stu-id="e8a30-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e8a30-122">授权</span><span class="sxs-lookup"><span data-stu-id="e8a30-122">Authorization</span></span>|<span data-ttu-id="e8a30-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e8a30-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e8a30-124">接受</span><span class="sxs-lookup"><span data-stu-id="e8a30-124">Accept</span></span>|<span data-ttu-id="e8a30-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e8a30-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e8a30-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="e8a30-126">Request body</span></span>
<span data-ttu-id="e8a30-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e8a30-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e8a30-128">响应</span><span class="sxs-lookup"><span data-stu-id="e8a30-128">Response</span></span>
<span data-ttu-id="e8a30-129">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和 [deviceAppManagement](../resources/intune_shared_deviceappmanagement.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e8a30-129">If successful, this method returns a `200 OK` response code and [deviceAppManagement](../resources/intune_shared_deviceappmanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e8a30-130">示例</span><span class="sxs-lookup"><span data-stu-id="e8a30-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="e8a30-131">请求</span><span class="sxs-lookup"><span data-stu-id="e8a30-131">Request</span></span>
<span data-ttu-id="e8a30-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e8a30-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement
```

### <a name="response"></a><span data-ttu-id="e8a30-133">响应</span><span class="sxs-lookup"><span data-stu-id="e8a30-133">Response</span></span>
<span data-ttu-id="e8a30-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e8a30-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 133

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceAppManagement",
    "id": "bbb801a3-01a3-bbb8-a301-b8bba301b8bb"
  }
}
```




# <a name="get-deviceappmanagement"></a><span data-ttu-id="6da02-101">获取 deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="6da02-101">Get deviceAppManagement</span></span>

> <span data-ttu-id="6da02-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="6da02-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6da02-103">读取 [deviceAppManagement](../resources/intune_shared_deviceappmanagement.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="6da02-103">Read properties and relationships of the [deviceAppManagement](../resources/intune_shared_deviceappmanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6da02-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="6da02-104">Prerequisites</span></span>

<span data-ttu-id="6da02-105">以下权限之一需要调用此 API。</span><span class="sxs-lookup"><span data-stu-id="6da02-105">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="6da02-106">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="6da02-106">To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>  <span data-ttu-id="6da02-107">请注意，在相应权限根据工作流而有所不同。</span><span class="sxs-lookup"><span data-stu-id="6da02-107">Note that the appropriate permission varies according to the workflow.</span></span>

|<span data-ttu-id="6da02-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="6da02-108">Permission type</span></span>|<span data-ttu-id="6da02-109">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="6da02-109">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6da02-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6da02-110">Delegated (work or school account)</span></span>|<span data-ttu-id="6da02-111">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="6da02-111">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
|<span data-ttu-id="6da02-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6da02-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6da02-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="6da02-113">Not supported.</span></span>|
|<span data-ttu-id="6da02-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="6da02-114">Application</span></span>|<span data-ttu-id="6da02-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="6da02-115">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6da02-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6da02-116">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6da02-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="6da02-117">Optional query parameters</span></span>
<span data-ttu-id="6da02-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="6da02-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6da02-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="6da02-119">Request headers</span></span>
|<span data-ttu-id="6da02-120">标头</span><span class="sxs-lookup"><span data-stu-id="6da02-120">Header</span></span>|<span data-ttu-id="6da02-121">值</span><span class="sxs-lookup"><span data-stu-id="6da02-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6da02-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6da02-122">Authorization</span></span>|<span data-ttu-id="6da02-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6da02-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6da02-124">Accept</span><span class="sxs-lookup"><span data-stu-id="6da02-124">Accept</span></span>|<span data-ttu-id="6da02-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6da02-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6da02-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="6da02-126">Request body</span></span>
<span data-ttu-id="6da02-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6da02-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6da02-128">响应</span><span class="sxs-lookup"><span data-stu-id="6da02-128">Response</span></span>
<span data-ttu-id="6da02-129">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和 [deviceAppManagement](../resources/intune_shared_deviceappmanagement.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6da02-129">If successful, this method returns a `200 OK` response code and [deviceAppManagement](../resources/intune_shared_deviceappmanagement.md) object in the response body.</span></span>

## <a name="example-request"></a><span data-ttu-id="6da02-130">示例请求</span><span class="sxs-lookup"><span data-stu-id="6da02-130">Example request</span></span>

``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement
```

## <a name="example-response"></a><span data-ttu-id="6da02-131">响应示例</span><span class="sxs-lookup"><span data-stu-id="6da02-131">Example response</span></span>
<span data-ttu-id="6da02-132">为简便起见，如下所示的响应对象可能会被截断。</span><span class="sxs-lookup"><span data-stu-id="6da02-132">The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="6da02-133">从实际的呼叫，将返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6da02-133">All properties will be returned from an actual call.</span></span>

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




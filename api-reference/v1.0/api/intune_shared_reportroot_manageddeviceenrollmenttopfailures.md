# <a name="manageddeviceenrollmenttopfailures-function"></a><span data-ttu-id="99135-101">managedDeviceEnrollmentTopFailures 函数</span><span class="sxs-lookup"><span data-stu-id="99135-101">managedDeviceEnrollmentTopFailures function</span></span>

> <span data-ttu-id="99135-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="99135-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="99135-103">尚未记录</span><span class="sxs-lookup"><span data-stu-id="99135-103">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="99135-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="99135-104">Prerequisites</span></span>
<span data-ttu-id="99135-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="99135-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="99135-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="99135-107">Permission type</span></span>|<span data-ttu-id="99135-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="99135-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="99135-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="99135-109">Delegated (work or school account)</span></span>||
| <span data-ttu-id="99135-110">&nbsp; &nbsp; 疑难解答</span><span class="sxs-lookup"><span data-stu-id="99135-110">&nbsp; &nbsp;Troubleshooting</span></span> | <span data-ttu-id="99135-111">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="99135-111">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="99135-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="99135-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="99135-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="99135-113">Not supported.</span></span>|
|<span data-ttu-id="99135-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="99135-114">Application</span></span>|<span data-ttu-id="99135-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="99135-115">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="99135-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="99135-116">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentTopFailures
```

## <a name="request-headers"></a><span data-ttu-id="99135-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="99135-117">Request headers</span></span>
|<span data-ttu-id="99135-118">标头</span><span class="sxs-lookup"><span data-stu-id="99135-118">Header</span></span>|<span data-ttu-id="99135-119">值</span><span class="sxs-lookup"><span data-stu-id="99135-119">Value</span></span>|
|:---|:---|
|<span data-ttu-id="99135-120">授权</span><span class="sxs-lookup"><span data-stu-id="99135-120">Authorization</span></span>|<span data-ttu-id="99135-121">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="99135-121">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="99135-122">接受</span><span class="sxs-lookup"><span data-stu-id="99135-122">Accept</span></span>|<span data-ttu-id="99135-123">application/json</span><span class="sxs-lookup"><span data-stu-id="99135-123">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="99135-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="99135-124">Request body</span></span>
<span data-ttu-id="99135-125">在请求 URL 中，提供以下查询参数（含值）。</span><span class="sxs-lookup"><span data-stu-id="99135-125">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="99135-126">下表显示了可用于此函数的参数。</span><span class="sxs-lookup"><span data-stu-id="99135-126">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="99135-127">属性</span><span class="sxs-lookup"><span data-stu-id="99135-127">Property</span></span>|<span data-ttu-id="99135-128">类型</span><span class="sxs-lookup"><span data-stu-id="99135-128">Type</span></span>|<span data-ttu-id="99135-129">说明</span><span class="sxs-lookup"><span data-stu-id="99135-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="99135-130">时间段</span><span class="sxs-lookup"><span data-stu-id="99135-130">period</span></span>|<span data-ttu-id="99135-131">字符串</span><span class="sxs-lookup"><span data-stu-id="99135-131">String</span></span>|<span data-ttu-id="99135-132">尚未记录</span><span class="sxs-lookup"><span data-stu-id="99135-132">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="99135-133">响应</span><span class="sxs-lookup"><span data-stu-id="99135-133">Response</span></span>
<span data-ttu-id="99135-134">如果成功，此函数会在响应正文中返回 `200 OK` 响应代码和一个 [report](../resources/intune_shared_report.md)。</span><span class="sxs-lookup"><span data-stu-id="99135-134">If successful, this function returns a `200 OK` response code and a [report](../resources/intune_shared_report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="99135-135">示例</span><span class="sxs-lookup"><span data-stu-id="99135-135">Example</span></span>
### <a name="request"></a><span data-ttu-id="99135-136">请求</span><span class="sxs-lookup"><span data-stu-id="99135-136">Request</span></span>
<span data-ttu-id="99135-137">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="99135-137">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1/reports/managedDeviceEnrollmentTopFailures(period='parameterValue')
```

### <a name="response"></a><span data-ttu-id="99135-138">响应</span><span class="sxs-lookup"><span data-stu-id="99135-138">Response</span></span>
<span data-ttu-id="99135-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="99135-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 123

{
  "value": {
    "@odata.type": "microsoft.graph.report",
    "content": "<Unknown Primitive Type Edm.Stream>"
  }
}
```





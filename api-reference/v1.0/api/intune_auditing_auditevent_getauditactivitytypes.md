# <a name="getauditactivitytypes-function"></a><span data-ttu-id="d053e-101">getAuditActivityTypes 函数</span><span class="sxs-lookup"><span data-stu-id="d053e-101">getAuditActivityTypes function</span></span>

> <span data-ttu-id="d053e-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="d053e-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d053e-103">尚未记录</span><span class="sxs-lookup"><span data-stu-id="d053e-103">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d053e-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="d053e-104">Prerequisites</span></span>
<span data-ttu-id="d053e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="d053e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="d053e-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="d053e-107">Permission type</span></span>|<span data-ttu-id="d053e-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d053e-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d053e-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d053e-109">Delegated (work or school account)</span></span>|<span data-ttu-id="d053e-110">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="d053e-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="d053e-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d053e-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d053e-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="d053e-112">Not supported.</span></span>|
|<span data-ttu-id="d053e-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="d053e-113">Application</span></span>|<span data-ttu-id="d053e-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="d053e-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d053e-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d053e-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/auditEvents/getAuditActivityTypes
```

## <a name="request-headers"></a><span data-ttu-id="d053e-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="d053e-116">Request headers</span></span>
|<span data-ttu-id="d053e-117">标头</span><span class="sxs-lookup"><span data-stu-id="d053e-117">Header</span></span>|<span data-ttu-id="d053e-118">值</span><span class="sxs-lookup"><span data-stu-id="d053e-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d053e-119">授权</span><span class="sxs-lookup"><span data-stu-id="d053e-119">Authorization</span></span>|<span data-ttu-id="d053e-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d053e-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d053e-121">Accept</span><span class="sxs-lookup"><span data-stu-id="d053e-121">Accept</span></span>|<span data-ttu-id="d053e-122">application/json</span><span class="sxs-lookup"><span data-stu-id="d053e-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d053e-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="d053e-123">Request body</span></span>
<span data-ttu-id="d053e-124">在请求 URL 中，提供以下查询参数（含值）。</span><span class="sxs-lookup"><span data-stu-id="d053e-124">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="d053e-125">下表显示了可用于此函数的参数。</span><span class="sxs-lookup"><span data-stu-id="d053e-125">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="d053e-126">属性</span><span class="sxs-lookup"><span data-stu-id="d053e-126">Property</span></span>|<span data-ttu-id="d053e-127">类型</span><span class="sxs-lookup"><span data-stu-id="d053e-127">Type</span></span>|<span data-ttu-id="d053e-128">说明</span><span class="sxs-lookup"><span data-stu-id="d053e-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d053e-129">category</span><span class="sxs-lookup"><span data-stu-id="d053e-129">category</span></span>|<span data-ttu-id="d053e-130">字符串</span><span class="sxs-lookup"><span data-stu-id="d053e-130">String</span></span>|<span data-ttu-id="d053e-131">尚未记录</span><span class="sxs-lookup"><span data-stu-id="d053e-131">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="d053e-132">响应</span><span class="sxs-lookup"><span data-stu-id="d053e-132">Response</span></span>
<span data-ttu-id="d053e-133">如果成功，此函数会在响应正文中返回 `200 OK` 响应代码和一个 String 集合。</span><span class="sxs-lookup"><span data-stu-id="d053e-133">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d053e-134">示例</span><span class="sxs-lookup"><span data-stu-id="d053e-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="d053e-135">请求</span><span class="sxs-lookup"><span data-stu-id="d053e-135">Request</span></span>
<span data-ttu-id="d053e-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d053e-136">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/auditEvents/getAuditActivityTypes(category='parameterValue')
```

### <a name="response"></a><span data-ttu-id="d053e-137">响应</span><span class="sxs-lookup"><span data-stu-id="d053e-137">Response</span></span>
<span data-ttu-id="d053e-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d053e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 61

{
  "value": [
    "Get Audit Activity Types value"
  ]
}
```









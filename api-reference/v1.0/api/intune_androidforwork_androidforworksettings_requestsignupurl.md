# <a name="requestsignupurl-action"></a><span data-ttu-id="7988b-101">requestSignupUrl 操作</span><span class="sxs-lookup"><span data-stu-id="7988b-101">requestSignupUrl action</span></span>

> <span data-ttu-id="7988b-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="7988b-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7988b-103">生成用于注册 Android for Work 管理的注册 URL。</span><span class="sxs-lookup"><span data-stu-id="7988b-103">Generates a sign-up URL that is used to enroll in Android for Work management.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7988b-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="7988b-104">Prerequisites</span></span>
<span data-ttu-id="7988b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="7988b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="7988b-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="7988b-107">Permission type</span></span>|<span data-ttu-id="7988b-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="7988b-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7988b-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7988b-109">Delegated (work or school account)</span></span>|<span data-ttu-id="7988b-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7988b-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7988b-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7988b-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7988b-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="7988b-112">Not supported.</span></span>|
|<span data-ttu-id="7988b-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="7988b-113">Application</span></span>|<span data-ttu-id="7988b-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="7988b-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7988b-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7988b-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidForWorkSettings/requestSignupUrl
```

## <a name="request-headers"></a><span data-ttu-id="7988b-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="7988b-116">Request headers</span></span>
|<span data-ttu-id="7988b-117">标头</span><span class="sxs-lookup"><span data-stu-id="7988b-117">Header</span></span>|<span data-ttu-id="7988b-118">值</span><span class="sxs-lookup"><span data-stu-id="7988b-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7988b-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="7988b-119">Authorization</span></span>|<span data-ttu-id="7988b-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="7988b-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="7988b-121">Accept</span><span class="sxs-lookup"><span data-stu-id="7988b-121">Accept</span></span>|<span data-ttu-id="7988b-122">application/json</span><span class="sxs-lookup"><span data-stu-id="7988b-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7988b-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="7988b-123">Request body</span></span>
<span data-ttu-id="7988b-124">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7988b-124">In the request body, supply a JSON representation of the Contact object.</span></span>

<span data-ttu-id="7988b-125">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="7988b-125">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="7988b-126">属性</span><span class="sxs-lookup"><span data-stu-id="7988b-126">Property</span></span>|<span data-ttu-id="7988b-127">类型</span><span class="sxs-lookup"><span data-stu-id="7988b-127">Type</span></span>|<span data-ttu-id="7988b-128">说明</span><span class="sxs-lookup"><span data-stu-id="7988b-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7988b-129">hostName</span><span class="sxs-lookup"><span data-stu-id="7988b-129">hostname</span></span>|<span data-ttu-id="7988b-130">String</span><span class="sxs-lookup"><span data-stu-id="7988b-130">String</span></span>|<span data-ttu-id="7988b-131">成功完成注册后浏览器将被重定向到的回调 URL 的主机名。</span><span class="sxs-lookup"><span data-stu-id="7988b-131">The hostname of the callback URL to which the browser will be redirected after successfully completing sign-up.</span></span>|



## <a name="response"></a><span data-ttu-id="7988b-132">响应</span><span class="sxs-lookup"><span data-stu-id="7988b-132">Response</span></span>
<span data-ttu-id="7988b-133">如果成功，此操作会在响应正文中返回 `200 OK` 响应代码和一个 String。</span><span class="sxs-lookup"><span data-stu-id="7988b-133">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7988b-134">示例</span><span class="sxs-lookup"><span data-stu-id="7988b-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="7988b-135">请求</span><span class="sxs-lookup"><span data-stu-id="7988b-135">Request</span></span>
<span data-ttu-id="7988b-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7988b-136">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/androidForWorkSettings/requestSignupUrl

Content-type: application/json
Content-length: 37

{
  "hostName": "Host Name value"
}
```

### <a name="response"></a><span data-ttu-id="7988b-137">响应</span><span class="sxs-lookup"><span data-stu-id="7988b-137">Response</span></span>
<span data-ttu-id="7988b-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7988b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 56

{
  "value": "https://example.com/requestSignupUrl/"
}
```




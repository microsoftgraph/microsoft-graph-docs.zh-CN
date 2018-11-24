# <a name="windowsdefenderupdatesignatures-action"></a><span data-ttu-id="f36a7-101">windowsDefenderUpdateSignatures 操作</span><span class="sxs-lookup"><span data-stu-id="f36a7-101">windowsDefenderUpdateSignatures action</span></span>

> <span data-ttu-id="f36a7-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="f36a7-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f36a7-103">尚未记录</span><span class="sxs-lookup"><span data-stu-id="f36a7-103">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f36a7-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="f36a7-104">Prerequisites</span></span>
<span data-ttu-id="f36a7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="f36a7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f36a7-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="f36a7-107">Permission type</span></span>|<span data-ttu-id="f36a7-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f36a7-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f36a7-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f36a7-109">Delegated (work or school account)</span></span>|<span data-ttu-id="f36a7-110">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="f36a7-110">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="f36a7-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f36a7-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f36a7-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="f36a7-112">Not supported.</span></span>|
|<span data-ttu-id="f36a7-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="f36a7-113">Application</span></span>|<span data-ttu-id="f36a7-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f36a7-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f36a7-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f36a7-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/windowsDefenderUpdateSignatures
POST /deviceManagement/managedDevices/{managedDeviceId}/windowsDefenderUpdateSignatures
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/windowsDefenderUpdateSignatures
```

## <a name="request-headers"></a><span data-ttu-id="f36a7-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="f36a7-116">Request headers</span></span>
|<span data-ttu-id="f36a7-117">标头</span><span class="sxs-lookup"><span data-stu-id="f36a7-117">Header</span></span>|<span data-ttu-id="f36a7-118">值</span><span class="sxs-lookup"><span data-stu-id="f36a7-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f36a7-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="f36a7-119">Authorization</span></span>|<span data-ttu-id="f36a7-120">需要持有者&lt;令牌&gt;。</span><span class="sxs-lookup"><span data-stu-id="f36a7-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f36a7-121">Accept</span><span class="sxs-lookup"><span data-stu-id="f36a7-121">Accept</span></span>|<span data-ttu-id="f36a7-122">application/json</span><span class="sxs-lookup"><span data-stu-id="f36a7-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f36a7-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="f36a7-123">Request body</span></span>
<span data-ttu-id="f36a7-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f36a7-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f36a7-125">响应</span><span class="sxs-lookup"><span data-stu-id="f36a7-125">Response</span></span>
<span data-ttu-id="f36a7-126">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="f36a7-126">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f36a7-127">示例</span><span class="sxs-lookup"><span data-stu-id="f36a7-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="f36a7-128">请求</span><span class="sxs-lookup"><span data-stu-id="f36a7-128">Request</span></span>
<span data-ttu-id="f36a7-129">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f36a7-129">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices/{managedDeviceId}/windowsDefenderUpdateSignatures
```

### <a name="response"></a><span data-ttu-id="f36a7-130">响应</span><span class="sxs-lookup"><span data-stu-id="f36a7-130">Response</span></span>
<span data-ttu-id="f36a7-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f36a7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




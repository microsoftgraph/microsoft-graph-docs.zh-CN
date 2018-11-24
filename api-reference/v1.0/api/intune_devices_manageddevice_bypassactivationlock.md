# <a name="bypassactivationlock-action"></a><span data-ttu-id="149f0-101">bypassActivationLock 操作</span><span class="sxs-lookup"><span data-stu-id="149f0-101">bypassActivationLock action</span></span>

> <span data-ttu-id="149f0-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="149f0-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="149f0-103">跳过激活锁</span><span class="sxs-lookup"><span data-stu-id="149f0-103">Bypass activation lock</span></span>
## <a name="prerequisites"></a><span data-ttu-id="149f0-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="149f0-104">Prerequisites</span></span>
<span data-ttu-id="149f0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="149f0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="149f0-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="149f0-107">Permission type</span></span>|<span data-ttu-id="149f0-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="149f0-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="149f0-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="149f0-109">Delegated (work or school account)</span></span>|<span data-ttu-id="149f0-110">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="149f0-110">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="149f0-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="149f0-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="149f0-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="149f0-112">Not supported.</span></span>|
|<span data-ttu-id="149f0-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="149f0-113">Application</span></span>|<span data-ttu-id="149f0-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="149f0-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="149f0-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="149f0-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/bypassActivationLock
POST /deviceManagement/managedDevices/{managedDeviceId}/bypassActivationLock
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/bypassActivationLock
```

## <a name="request-headers"></a><span data-ttu-id="149f0-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="149f0-116">Request headers</span></span>
|<span data-ttu-id="149f0-117">标头</span><span class="sxs-lookup"><span data-stu-id="149f0-117">Header</span></span>|<span data-ttu-id="149f0-118">值</span><span class="sxs-lookup"><span data-stu-id="149f0-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="149f0-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="149f0-119">Authorization</span></span>|<span data-ttu-id="149f0-120">需要持有者&lt;令牌&gt;。</span><span class="sxs-lookup"><span data-stu-id="149f0-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="149f0-121">Accept</span><span class="sxs-lookup"><span data-stu-id="149f0-121">Accept</span></span>|<span data-ttu-id="149f0-122">application/json</span><span class="sxs-lookup"><span data-stu-id="149f0-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="149f0-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="149f0-123">Request body</span></span>
<span data-ttu-id="149f0-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="149f0-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="149f0-125">响应</span><span class="sxs-lookup"><span data-stu-id="149f0-125">Response</span></span>
<span data-ttu-id="149f0-126">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="149f0-126">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="149f0-127">示例</span><span class="sxs-lookup"><span data-stu-id="149f0-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="149f0-128">请求</span><span class="sxs-lookup"><span data-stu-id="149f0-128">Request</span></span>
<span data-ttu-id="149f0-129">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="149f0-129">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices/{managedDeviceId}/bypassActivationLock
```

### <a name="response"></a><span data-ttu-id="149f0-130">响应</span><span class="sxs-lookup"><span data-stu-id="149f0-130">Response</span></span>
<span data-ttu-id="149f0-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="149f0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




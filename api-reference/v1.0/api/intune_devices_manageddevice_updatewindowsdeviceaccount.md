# <a name="updatewindowsdeviceaccount-action"></a><span data-ttu-id="6ccf3-101">updateWindowsDeviceAccount 操作</span><span class="sxs-lookup"><span data-stu-id="6ccf3-101">updateWindowsDeviceAccount action</span></span>

> <span data-ttu-id="6ccf3-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="6ccf3-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6ccf3-103">尚未记录</span><span class="sxs-lookup"><span data-stu-id="6ccf3-103">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6ccf3-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="6ccf3-104">Prerequisites</span></span>
<span data-ttu-id="6ccf3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="6ccf3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="6ccf3-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="6ccf3-107">Permission type</span></span>|<span data-ttu-id="6ccf3-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="6ccf3-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6ccf3-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6ccf3-109">Delegated (work or school account)</span></span>|<span data-ttu-id="6ccf3-110">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="6ccf3-110">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="6ccf3-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6ccf3-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6ccf3-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="6ccf3-112">Not supported.</span></span>|
|<span data-ttu-id="6ccf3-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="6ccf3-113">Application</span></span>|<span data-ttu-id="6ccf3-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="6ccf3-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6ccf3-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6ccf3-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/updateWindowsDeviceAccount
POST /deviceManagement/managedDevices/{managedDeviceId}/updateWindowsDeviceAccount
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/updateWindowsDeviceAccount
```

## <a name="request-headers"></a><span data-ttu-id="6ccf3-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="6ccf3-116">Request headers</span></span>
|<span data-ttu-id="6ccf3-117">标头</span><span class="sxs-lookup"><span data-stu-id="6ccf3-117">Header</span></span>|<span data-ttu-id="6ccf3-118">值</span><span class="sxs-lookup"><span data-stu-id="6ccf3-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6ccf3-119">授权</span><span class="sxs-lookup"><span data-stu-id="6ccf3-119">Authorization</span></span>|<span data-ttu-id="6ccf3-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6ccf3-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6ccf3-121">Accept</span><span class="sxs-lookup"><span data-stu-id="6ccf3-121">Accept</span></span>|<span data-ttu-id="6ccf3-122">application/json</span><span class="sxs-lookup"><span data-stu-id="6ccf3-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6ccf3-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="6ccf3-123">Request body</span></span>
<span data-ttu-id="6ccf3-124">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6ccf3-124">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="6ccf3-125">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="6ccf3-125">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="6ccf3-126">属性</span><span class="sxs-lookup"><span data-stu-id="6ccf3-126">Property</span></span>|<span data-ttu-id="6ccf3-127">类型</span><span class="sxs-lookup"><span data-stu-id="6ccf3-127">Type</span></span>|<span data-ttu-id="6ccf3-128">说明</span><span class="sxs-lookup"><span data-stu-id="6ccf3-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6ccf3-129">updateWindowsDeviceAccountActionParameter</span><span class="sxs-lookup"><span data-stu-id="6ccf3-129">updateWindowsDeviceAccountActionParameter</span></span>|[<span data-ttu-id="6ccf3-130">updateWindowsDeviceAccountActionParameter</span><span class="sxs-lookup"><span data-stu-id="6ccf3-130">updateWindowsDeviceAccountActionParameter</span></span>](../resources/intune_devices_updatewindowsdeviceaccountactionparameter.md)|<span data-ttu-id="6ccf3-131">尚未记录</span><span class="sxs-lookup"><span data-stu-id="6ccf3-131">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="6ccf3-132">响应</span><span class="sxs-lookup"><span data-stu-id="6ccf3-132">Response</span></span>
<span data-ttu-id="6ccf3-133">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="6ccf3-133">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="6ccf3-134">示例</span><span class="sxs-lookup"><span data-stu-id="6ccf3-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="6ccf3-135">请求</span><span class="sxs-lookup"><span data-stu-id="6ccf3-135">Request</span></span>
<span data-ttu-id="6ccf3-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6ccf3-136">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices/{managedDeviceId}/updateWindowsDeviceAccount

Content-type: application/json
Content-length: 532

{
  "updateWindowsDeviceAccountActionParameter": {
    "@odata.type": "microsoft.graph.updateWindowsDeviceAccountActionParameter",
    "deviceAccount": {
      "@odata.type": "microsoft.graph.windowsDeviceAccount",
      "password": "Password value"
    },
    "passwordRotationEnabled": true,
    "calendarSyncEnabled": true,
    "deviceAccountEmail": "Device Account Email value",
    "exchangeServer": "Exchange Server value",
    "sessionInitiationProtocalAddress": "Session Initiation Protocal Address value"
  }
}
```

### <a name="response"></a><span data-ttu-id="6ccf3-137">响应</span><span class="sxs-lookup"><span data-stu-id="6ccf3-137">Response</span></span>
<span data-ttu-id="6ccf3-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6ccf3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```









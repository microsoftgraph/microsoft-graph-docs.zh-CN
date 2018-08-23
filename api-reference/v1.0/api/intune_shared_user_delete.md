# <a name="delete-user"></a><span data-ttu-id="d440f-101">删除 user</span><span class="sxs-lookup"><span data-stu-id="d440f-101">Delete user</span></span>

> <span data-ttu-id="d440f-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="d440f-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d440f-103">删除 [user](../resources/intune_shared_user.md)。</span><span class="sxs-lookup"><span data-stu-id="d440f-103">Deletes a [user](../resources/intune_shared_user.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d440f-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="d440f-104">Prerequisites</span></span>
<span data-ttu-id="d440f-105">需要以下权限之一才能调用此 API。</span><span class="sxs-lookup"><span data-stu-id="d440f-105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see Permissions.</span></span> <span data-ttu-id="d440f-106">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="d440f-106">To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>  <span data-ttu-id="d440f-107">所需的特定权限取决于上下文。</span><span class="sxs-lookup"><span data-stu-id="d440f-107">The specific permission required depends on context.</span></span>

|<span data-ttu-id="d440f-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="d440f-108">Permission type</span></span>|<span data-ttu-id="d440f-109">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d440f-109">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d440f-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d440f-110">Delegated (work or school account)</span></span>| <span data-ttu-id="d440f-111">_因上下文而异_</span><span class="sxs-lookup"><span data-stu-id="d440f-111">_varies by context_</span></span>|
| <span data-ttu-id="d440f-112">&nbsp; &nbsp; 设备</span><span class="sxs-lookup"><span data-stu-id="d440f-112">&nbsp;&nbsp;</span></span> | <span data-ttu-id="d440f-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d440f-113">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="d440f-114">&nbsp; &nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="d440f-114">.mam</span></span> | <span data-ttu-id="d440f-115">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d440f-115">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="d440f-116">&nbsp; &nbsp; 参与／有份</span><span class="sxs-lookup"><span data-stu-id="d440f-116">&nbsp; &nbsp; On-boarding</span></span> | <span data-ttu-id="d440f-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d440f-117">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="d440f-118">&nbsp; &nbsp; 疑难解答</span><span class="sxs-lookup"><span data-stu-id="d440f-118">&nbsp; &nbsp;Troubleshooting</span></span> | <span data-ttu-id="d440f-119">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d440f-119">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
|<span data-ttu-id="d440f-120">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d440f-120">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d440f-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="d440f-121">Not supported.</span></span>|
|<span data-ttu-id="d440f-122">应用程序</span><span class="sxs-lookup"><span data-stu-id="d440f-122">Application</span></span>|<span data-ttu-id="d440f-123">不支持。</span><span class="sxs-lookup"><span data-stu-id="d440f-123">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d440f-124">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d440f-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /users/{usersId}
```

## <a name="request-headers"></a><span data-ttu-id="d440f-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="d440f-125">Request headers</span></span>
|<span data-ttu-id="d440f-126">标头</span><span class="sxs-lookup"><span data-stu-id="d440f-126">Header</span></span>|<span data-ttu-id="d440f-127">值</span><span class="sxs-lookup"><span data-stu-id="d440f-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d440f-128">授权</span><span class="sxs-lookup"><span data-stu-id="d440f-128">Authorization</span></span>|<span data-ttu-id="d440f-129">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d440f-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d440f-130">接受</span><span class="sxs-lookup"><span data-stu-id="d440f-130">Accept</span></span>|<span data-ttu-id="d440f-131">application/json</span><span class="sxs-lookup"><span data-stu-id="d440f-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d440f-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="d440f-132">Request body</span></span>
<span data-ttu-id="d440f-133">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d440f-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d440f-134">响应</span><span class="sxs-lookup"><span data-stu-id="d440f-134">Response</span></span>
<span data-ttu-id="d440f-135">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="d440f-135">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="d440f-136">示例</span><span class="sxs-lookup"><span data-stu-id="d440f-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="d440f-137">请求</span><span class="sxs-lookup"><span data-stu-id="d440f-137">Request</span></span>
<span data-ttu-id="d440f-138">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d440f-138">Here is an example of the request.</span></span>

``` http
DELETE https://graph.microsoft.com/v1.0/users/{usersId}
```

### <a name="response"></a><span data-ttu-id="d440f-139">响应</span><span class="sxs-lookup"><span data-stu-id="d440f-139">Response</span></span>
<span data-ttu-id="d440f-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d440f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```




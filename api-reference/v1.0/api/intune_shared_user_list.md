# <a name="list-users"></a><span data-ttu-id="4b00a-101">列出 users</span><span class="sxs-lookup"><span data-stu-id="4b00a-101">List users</span></span>

> <span data-ttu-id="4b00a-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="4b00a-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4b00a-103">列出 [user](../resources/intune_shared_user.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4b00a-103">List properties and relationships of the [user](../resources/intune_shared_user.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4b00a-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="4b00a-104">Prerequisites</span></span>
<span data-ttu-id="4b00a-105">需要以下权限之一才能调用此 API。</span><span class="sxs-lookup"><span data-stu-id="4b00a-105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see Permissions.</span></span> <span data-ttu-id="4b00a-106">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="4b00a-106">To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>  <span data-ttu-id="4b00a-107">特定权限取决于上下文。</span><span class="sxs-lookup"><span data-stu-id="4b00a-107">The specific permission depends on the context.</span></span>

|<span data-ttu-id="4b00a-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="4b00a-108">Permission type</span></span>|<span data-ttu-id="4b00a-109">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="4b00a-109">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4b00a-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4b00a-110">Delegated (work or school account)</span></span>| <span data-ttu-id="4b00a-111">_因上下文而异_</span><span class="sxs-lookup"><span data-stu-id="4b00a-111">_varies by context_</span></span>|
| <span data-ttu-id="4b00a-112">&nbsp; &nbsp; 设备</span><span class="sxs-lookup"><span data-stu-id="4b00a-112">&nbsp;&nbsp;</span></span> | <span data-ttu-id="4b00a-113">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="4b00a-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="4b00a-114">&nbsp; &nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="4b00a-114">.mam</span></span> | <span data-ttu-id="4b00a-115">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="4b00a-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="4b00a-116">&nbsp; &nbsp; 起始安排</span><span class="sxs-lookup"><span data-stu-id="4b00a-116">&nbsp; &nbsp; On-boarding</span></span> | <span data-ttu-id="4b00a-117">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="4b00a-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="4b00a-118">&nbsp; &nbsp; 疑难解答</span><span class="sxs-lookup"><span data-stu-id="4b00a-118">&nbsp; &nbsp;Troubleshooting</span></span> | <span data-ttu-id="4b00a-119">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="4b00a-119">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
|<span data-ttu-id="4b00a-120">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4b00a-120">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4b00a-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="4b00a-121">Not supported.</span></span>|
|<span data-ttu-id="4b00a-122">应用程序</span><span class="sxs-lookup"><span data-stu-id="4b00a-122">Application</span></span>|<span data-ttu-id="4b00a-123">不支持。</span><span class="sxs-lookup"><span data-stu-id="4b00a-123">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4b00a-124">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4b00a-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users
```

## <a name="request-headers"></a><span data-ttu-id="4b00a-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="4b00a-125">Request headers</span></span>
|<span data-ttu-id="4b00a-126">标头</span><span class="sxs-lookup"><span data-stu-id="4b00a-126">Header</span></span>|<span data-ttu-id="4b00a-127">值</span><span class="sxs-lookup"><span data-stu-id="4b00a-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4b00a-128">授权</span><span class="sxs-lookup"><span data-stu-id="4b00a-128">Authorization</span></span>|<span data-ttu-id="4b00a-129">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="4b00a-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4b00a-130">接受</span><span class="sxs-lookup"><span data-stu-id="4b00a-130">Accept</span></span>|<span data-ttu-id="4b00a-131">application/json</span><span class="sxs-lookup"><span data-stu-id="4b00a-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4b00a-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="4b00a-132">Request body</span></span>
<span data-ttu-id="4b00a-133">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4b00a-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4b00a-134">响应</span><span class="sxs-lookup"><span data-stu-id="4b00a-134">Response</span></span>
<span data-ttu-id="4b00a-135">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [user](../resources/intune_shared_user.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="4b00a-135">If successful, this method returns a `200 OK` response code and a collection of [user](../resources/intune_shared_user.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4b00a-136">示例</span><span class="sxs-lookup"><span data-stu-id="4b00a-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="4b00a-137">请求</span><span class="sxs-lookup"><span data-stu-id="4b00a-137">Request</span></span>
<span data-ttu-id="4b00a-138">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4b00a-138">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/v1.0/users
```

### <a name="response"></a><span data-ttu-id="4b00a-139">响应</span><span class="sxs-lookup"><span data-stu-id="4b00a-139">Response</span></span>
<span data-ttu-id="4b00a-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4b00a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 136

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.user",
      "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
    }
  ]
}
```




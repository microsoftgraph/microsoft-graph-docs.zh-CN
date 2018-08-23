# <a name="get-user"></a><span data-ttu-id="5592d-101">获取 user</span><span class="sxs-lookup"><span data-stu-id="5592d-101">Get user</span></span>

> <span data-ttu-id="5592d-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="5592d-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5592d-103">读取 [user](../resources/intune_shared_user.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5592d-103">Read properties and relationships of the [user](../resources/intune_shared_user.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5592d-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="5592d-104">Prerequisites</span></span>
<span data-ttu-id="5592d-105">需要以下权限之一才能调用此 API。</span><span class="sxs-lookup"><span data-stu-id="5592d-105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see Permissions.</span></span> <span data-ttu-id="5592d-106">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="5592d-106">To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>  <span data-ttu-id="5592d-107">特定权限取决于上下文。</span><span class="sxs-lookup"><span data-stu-id="5592d-107">The specific permission depends on the context.</span></span>

|<span data-ttu-id="5592d-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="5592d-108">Permission type</span></span>|<span data-ttu-id="5592d-109">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="5592d-109">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5592d-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5592d-110">Delegated (work or school account)</span></span>| <span data-ttu-id="5592d-111">_因上下文而异_</span><span class="sxs-lookup"><span data-stu-id="5592d-111">_varies by context_</span></span>|
| <span data-ttu-id="5592d-112">&nbsp; &nbsp; 设备</span><span class="sxs-lookup"><span data-stu-id="5592d-112">&nbsp;&nbsp;</span></span> | <span data-ttu-id="5592d-113">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="5592d-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="5592d-114">&nbsp; &nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="5592d-114">.mam</span></span> | <span data-ttu-id="5592d-115">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="5592d-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="5592d-116">&nbsp; &nbsp; 加入</span><span class="sxs-lookup"><span data-stu-id="5592d-116">&nbsp; &nbsp; On-boarding</span></span> | <span data-ttu-id="5592d-117">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="5592d-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="5592d-118">&nbsp; &nbsp; 疑难解答</span><span class="sxs-lookup"><span data-stu-id="5592d-118">&nbsp; &nbsp;Troubleshooting</span></span> | <span data-ttu-id="5592d-119">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="5592d-119">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
|<span data-ttu-id="5592d-120">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5592d-120">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5592d-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="5592d-121">Not supported.</span></span>|
|<span data-ttu-id="5592d-122">应用程序</span><span class="sxs-lookup"><span data-stu-id="5592d-122">Application</span></span>|<span data-ttu-id="5592d-123">不支持。</span><span class="sxs-lookup"><span data-stu-id="5592d-123">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5592d-124">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5592d-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5592d-125">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="5592d-125">Optional query parameters</span></span>
<span data-ttu-id="5592d-126">此方法支持 [OData 查询参数](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="5592d-126">This method supports the [OData Query Parameters](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="5592d-127">请求标头</span><span class="sxs-lookup"><span data-stu-id="5592d-127">Request headers</span></span>
|<span data-ttu-id="5592d-128">标头</span><span class="sxs-lookup"><span data-stu-id="5592d-128">Header</span></span>|<span data-ttu-id="5592d-129">值</span><span class="sxs-lookup"><span data-stu-id="5592d-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5592d-130">授权</span><span class="sxs-lookup"><span data-stu-id="5592d-130">Authorization</span></span>|<span data-ttu-id="5592d-131">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="5592d-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5592d-132">接受</span><span class="sxs-lookup"><span data-stu-id="5592d-132">Accept</span></span>|<span data-ttu-id="5592d-133">application/json</span><span class="sxs-lookup"><span data-stu-id="5592d-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5592d-134">请求正文</span><span class="sxs-lookup"><span data-stu-id="5592d-134">Request body</span></span>
<span data-ttu-id="5592d-135">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5592d-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5592d-136">响应</span><span class="sxs-lookup"><span data-stu-id="5592d-136">Response</span></span>
<span data-ttu-id="5592d-137">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [user](../resources/intune_shared_user.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5592d-137">If successful, this method returns a `200 OK` response code and [user](../resources/intune_shared_user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5592d-138">示例</span><span class="sxs-lookup"><span data-stu-id="5592d-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="5592d-139">请求</span><span class="sxs-lookup"><span data-stu-id="5592d-139">Request</span></span>
<span data-ttu-id="5592d-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5592d-140">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/v1.0/users/{usersId}
```

### <a name="response"></a><span data-ttu-id="5592d-141">响应</span><span class="sxs-lookup"><span data-stu-id="5592d-141">Response</span></span>
<span data-ttu-id="5592d-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5592d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 118

{
  "value": {
    "@odata.type": "#microsoft.graph.user",
    "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
  }
}
```




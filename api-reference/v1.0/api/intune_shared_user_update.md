# <a name="update-user"></a><span data-ttu-id="9e53c-101">更新 user</span><span class="sxs-lookup"><span data-stu-id="9e53c-101">Update user</span></span>

> <span data-ttu-id="9e53c-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="9e53c-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9e53c-103">更新 [user](../resources/intune_shared_user.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="9e53c-103">Update the properties of a [user](../resources/intune_shared_user.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9e53c-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="9e53c-104">Prerequisites</span></span>
<span data-ttu-id="9e53c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="9e53c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="9e53c-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="9e53c-107">Permission type</span></span>|<span data-ttu-id="9e53c-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="9e53c-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9e53c-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9e53c-109">Delegated (work or school account)</span></span>| <span data-ttu-id="9e53c-110">_因上下文而异_</span><span class="sxs-lookup"><span data-stu-id="9e53c-110">_varies by context_</span></span>|
| <span data-ttu-id="9e53c-111">&nbsp; &nbsp; 设备</span><span class="sxs-lookup"><span data-stu-id="9e53c-111">&nbsp;&nbsp;</span></span> | <span data-ttu-id="9e53c-112">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9e53c-112">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="9e53c-113">&nbsp; &nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="9e53c-113">.mam</span></span> | <span data-ttu-id="9e53c-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9e53c-114">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="9e53c-115">&nbsp; &nbsp; 加入</span><span class="sxs-lookup"><span data-stu-id="9e53c-115">&nbsp; &nbsp; On-boarding</span></span> | <span data-ttu-id="9e53c-116">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9e53c-116">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="9e53c-117">&nbsp; &nbsp; 疑难解答</span><span class="sxs-lookup"><span data-stu-id="9e53c-117">&nbsp; &nbsp;Troubleshooting</span></span> | <span data-ttu-id="9e53c-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9e53c-118">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
|<span data-ttu-id="9e53c-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9e53c-119">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9e53c-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="9e53c-120">Not supported.</span></span>|
|<span data-ttu-id="9e53c-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="9e53c-121">Application</span></span>|<span data-ttu-id="9e53c-122">不支持。</span><span class="sxs-lookup"><span data-stu-id="9e53c-122">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9e53c-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9e53c-123">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /users/{usersId}
```

## <a name="request-headers"></a><span data-ttu-id="9e53c-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="9e53c-124">Request headers</span></span>
|<span data-ttu-id="9e53c-125">标头</span><span class="sxs-lookup"><span data-stu-id="9e53c-125">Header</span></span>|<span data-ttu-id="9e53c-126">值</span><span class="sxs-lookup"><span data-stu-id="9e53c-126">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9e53c-127">授权</span><span class="sxs-lookup"><span data-stu-id="9e53c-127">Authorization</span></span>|<span data-ttu-id="9e53c-128">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="9e53c-128">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9e53c-129">接受</span><span class="sxs-lookup"><span data-stu-id="9e53c-129">Accept</span></span>|<span data-ttu-id="9e53c-130">application/json</span><span class="sxs-lookup"><span data-stu-id="9e53c-130">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9e53c-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="9e53c-131">Request body</span></span>
<span data-ttu-id="9e53c-132">在请求正文中，提供 [user](../resources/intune_shared_user.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9e53c-132">In the request body, supply a JSON representation for the [user](../resources/intune_shared_user.md) object.</span></span>

<span data-ttu-id="9e53c-133">下表显示创建 [user](../resources/intune_shared_user.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="9e53c-133">The following table shows the properties that are required when you create the [user](../resources/intune_shared_user.md).</span></span>

|<span data-ttu-id="9e53c-134">属性</span><span class="sxs-lookup"><span data-stu-id="9e53c-134">Property</span></span>|<span data-ttu-id="9e53c-135">类型</span><span class="sxs-lookup"><span data-stu-id="9e53c-135">Type</span></span>|<span data-ttu-id="9e53c-136">说明</span><span class="sxs-lookup"><span data-stu-id="9e53c-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9e53c-137">id</span><span class="sxs-lookup"><span data-stu-id="9e53c-137">id</span></span>|<span data-ttu-id="9e53c-138">字符串</span><span class="sxs-lookup"><span data-stu-id="9e53c-138">String</span></span>|<span data-ttu-id="9e53c-139">用户的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="9e53c-139">Unique identifier of the user.</span></span>|
|<span data-ttu-id="9e53c-140">**加入**</span><span class="sxs-lookup"><span data-stu-id="9e53c-140">**On-boarding**</span></span>|
|<span data-ttu-id="9e53c-141">deviceEnrollmentLimit</span><span class="sxs-lookup"><span data-stu-id="9e53c-141">deviceEnrollmentLimit</span></span>|<span data-ttu-id="9e53c-142">Int32</span><span class="sxs-lookup"><span data-stu-id="9e53c-142">Int32</span></span>|<span data-ttu-id="9e53c-143">允许用户注册的最大设备数的限制。</span><span class="sxs-lookup"><span data-stu-id="9e53c-143">The limit on the maximum number of devices that the user is permitted to enroll.</span></span> <span data-ttu-id="9e53c-144">允许的值为 5 或 1000。</span><span class="sxs-lookup"><span data-stu-id="9e53c-144">Allowed values are 5 or 1000.</span></span>|

## <a name="response"></a><span data-ttu-id="9e53c-145">响应</span><span class="sxs-lookup"><span data-stu-id="9e53c-145">Response</span></span>
<span data-ttu-id="9e53c-146">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [user](../resources/intune_shared_user.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9e53c-146">If successful, this method returns a `200 OK` response code and an updated [user](../resources/intune_shared_user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9e53c-147">示例</span><span class="sxs-lookup"><span data-stu-id="9e53c-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="9e53c-148">请求</span><span class="sxs-lookup"><span data-stu-id="9e53c-148">Request</span></span>
<span data-ttu-id="9e53c-149">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9e53c-149">Here is an example of the request.</span></span>

``` http
PATCH https://graph.microsoft.com/v1.0/users/{usersId}
Content-type: application/json
Content-length: 2

{}
```

### <a name="response"></a><span data-ttu-id="9e53c-150">响应</span><span class="sxs-lookup"><span data-stu-id="9e53c-150">Response</span></span>
<span data-ttu-id="9e53c-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9e53c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 95

{
  "@odata.type": "#microsoft.graph.user",
  "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
}
```




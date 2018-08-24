# <a name="create-user"></a><span data-ttu-id="33991-101">创建 user</span><span class="sxs-lookup"><span data-stu-id="33991-101">Create user</span></span>

> <span data-ttu-id="33991-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="33991-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="33991-103">创建新的 [user](../resources/intune_shared_user.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="33991-103">Create a new [user](../resources/intune_shared_user.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="33991-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="33991-104">Prerequisites</span></span>
<span data-ttu-id="33991-105">需要以下权限之一才能调用此 API。</span><span class="sxs-lookup"><span data-stu-id="33991-105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see Permissions.</span></span> <span data-ttu-id="33991-106">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="33991-106">To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>  <span data-ttu-id="33991-107">所需的特定权限取决于上下文。</span><span class="sxs-lookup"><span data-stu-id="33991-107">The specific permission required depends on the context.</span></span>

|<span data-ttu-id="33991-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="33991-108">Permission type</span></span>|<span data-ttu-id="33991-109">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="33991-109">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="33991-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="33991-110">Delegated (work or school account)</span></span>| <span data-ttu-id="33991-111">_因上下文而异_</span><span class="sxs-lookup"><span data-stu-id="33991-111">_varies by context_</span></span> |
| <span data-ttu-id="33991-112">&nbsp; &nbsp; 设备</span><span class="sxs-lookup"><span data-stu-id="33991-112">&nbsp;&nbsp;</span></span> | <span data-ttu-id="33991-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="33991-113">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="33991-114">&nbsp; &nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="33991-114">.mam</span></span> | <span data-ttu-id="33991-115">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="33991-115">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="33991-116">&nbsp; &nbsp; 加入</span><span class="sxs-lookup"><span data-stu-id="33991-116">&nbsp; &nbsp; On-boarding</span></span> | <span data-ttu-id="33991-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="33991-117">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="33991-118">&nbsp; &nbsp; 疑难解答</span><span class="sxs-lookup"><span data-stu-id="33991-118">&nbsp; &nbsp;Troubleshooting</span></span> | <span data-ttu-id="33991-119">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="33991-119">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
|<span data-ttu-id="33991-120">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="33991-120">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="33991-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="33991-121">Not supported.</span></span>|
|<span data-ttu-id="33991-122">应用程序</span><span class="sxs-lookup"><span data-stu-id="33991-122">Application</span></span>|<span data-ttu-id="33991-123">不支持。</span><span class="sxs-lookup"><span data-stu-id="33991-123">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="33991-124">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="33991-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users
```

## <a name="request-headers"></a><span data-ttu-id="33991-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="33991-125">Request headers</span></span>
|<span data-ttu-id="33991-126">标头</span><span class="sxs-lookup"><span data-stu-id="33991-126">Header</span></span>|<span data-ttu-id="33991-127">值</span><span class="sxs-lookup"><span data-stu-id="33991-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="33991-128">授权</span><span class="sxs-lookup"><span data-stu-id="33991-128">Authorization</span></span>|<span data-ttu-id="33991-129">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="33991-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="33991-130">接受</span><span class="sxs-lookup"><span data-stu-id="33991-130">Accept</span></span>|<span data-ttu-id="33991-131">application/json</span><span class="sxs-lookup"><span data-stu-id="33991-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="33991-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="33991-132">Request body</span></span>
<span data-ttu-id="33991-133">在请求正文中，提供 user 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="33991-133">In the request body, supply a JSON representation for the user object.</span></span>

<span data-ttu-id="33991-134">下表显示创建 user 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="33991-134">The following table shows the properties that are required when you create the user.</span></span>

|<span data-ttu-id="33991-135">属性</span><span class="sxs-lookup"><span data-stu-id="33991-135">Property</span></span>|<span data-ttu-id="33991-136">类型</span><span class="sxs-lookup"><span data-stu-id="33991-136">Type</span></span>|<span data-ttu-id="33991-137">说明</span><span class="sxs-lookup"><span data-stu-id="33991-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="33991-138">id</span><span class="sxs-lookup"><span data-stu-id="33991-138">id</span></span>|<span data-ttu-id="33991-139">字符串</span><span class="sxs-lookup"><span data-stu-id="33991-139">String</span></span>|<span data-ttu-id="33991-140">用户的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="33991-140">Unique identifier of the user.</span></span>|
|<span data-ttu-id="33991-141">**加入**</span><span class="sxs-lookup"><span data-stu-id="33991-141">**On-boarding**</span></span>|
|<span data-ttu-id="33991-142">deviceEnrollmentLimit</span><span class="sxs-lookup"><span data-stu-id="33991-142">deviceEnrollmentLimit</span></span>|<span data-ttu-id="33991-143">Int32</span><span class="sxs-lookup"><span data-stu-id="33991-143">Int32</span></span>|<span data-ttu-id="33991-144">允许用户注册的最大设备数的限制。</span><span class="sxs-lookup"><span data-stu-id="33991-144">The limit on the maximum number of devices that the user is permitted to enroll.</span></span> <span data-ttu-id="33991-145">允许的值为 5 或 1000。</span><span class="sxs-lookup"><span data-stu-id="33991-145">Allowed values are 5 or 1000.</span></span>|

<span data-ttu-id="33991-146">请求正文属性支持根据上下文而有所不同。</span><span class="sxs-lookup"><span data-stu-id="33991-146">Request body property support varies according to context.</span></span>

## <a name="response"></a><span data-ttu-id="33991-147">响应</span><span class="sxs-lookup"><span data-stu-id="33991-147">Response</span></span>
<span data-ttu-id="33991-148">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [user](../resources/intune_shared_user.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="33991-148">If successful, this method returns a `201 Created` response code and a [user](../resources/intune_shared_user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="33991-149">示例</span><span class="sxs-lookup"><span data-stu-id="33991-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="33991-150">请求</span><span class="sxs-lookup"><span data-stu-id="33991-150">Request</span></span>
<span data-ttu-id="33991-151">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="33991-151">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/v1.0/users
Content-type: application/json
Content-length: 46

{
  "@odata.type": "#microsoft.graph.user"
}
```

### <a name="response"></a><span data-ttu-id="33991-152">响应</span><span class="sxs-lookup"><span data-stu-id="33991-152">Response</span></span>
<span data-ttu-id="33991-153">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="33991-153">Here is an example of the response.</span></span> <span data-ttu-id="33991-154">注意：为简洁起见，可能会截断此处展示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="33991-154">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="33991-155">从实际调用返回的属性根据上下文而有所不同。</span><span class="sxs-lookup"><span data-stu-id="33991-155">Properties returned from an actual call vary according to context.</span></span>

``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 95

{
  "@odata.type": "#microsoft.graph.user",
  "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
}
```




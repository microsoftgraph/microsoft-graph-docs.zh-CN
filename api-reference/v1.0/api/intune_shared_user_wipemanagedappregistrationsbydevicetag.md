# <a name="wipemanagedappregistrationsbydevicetag-action"></a><span data-ttu-id="1c868-101">wipeManagedAppRegistrationsByDeviceTag 操作</span><span class="sxs-lookup"><span data-stu-id="1c868-101">wipeManagedAppRegistrationsByDeviceTag action</span></span>

> <span data-ttu-id="1c868-102">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="1c868-102">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1c868-103">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="1c868-103">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1c868-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="1c868-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1c868-105">对包含指定设备标记的应用注册发布擦除操作。</span><span class="sxs-lookup"><span data-stu-id="1c868-105">Issues a wipe operation on an app registration with specified device tag.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1c868-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="1c868-106">Prerequisites</span></span>
<span data-ttu-id="1c868-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="1c868-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="1c868-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="1c868-109">Permission type</span></span>|<span data-ttu-id="1c868-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="1c868-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1c868-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1c868-111">Delegated (work or school account)</span></span>| <span data-ttu-id="1c868-112">_因上下文而异_</span><span class="sxs-lookup"><span data-stu-id="1c868-112">_varies by context_</span></span> |
| <span data-ttu-id="1c868-113">&nbsp; &nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="1c868-113">.mam</span></span> | <span data-ttu-id="1c868-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1c868-114">DeviceManagementApps.ReadWrite.All</span></span> |
|<span data-ttu-id="1c868-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1c868-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1c868-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="1c868-116">Not supported.</span></span>|
|<span data-ttu-id="1c868-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="1c868-117">Application</span></span>|<span data-ttu-id="1c868-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="1c868-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1c868-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1c868-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/wipeManagedAppRegistrationsByDeviceTag
```

## <a name="request-headers"></a><span data-ttu-id="1c868-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="1c868-120">Request headers</span></span>
|<span data-ttu-id="1c868-121">标头</span><span class="sxs-lookup"><span data-stu-id="1c868-121">Header</span></span>|<span data-ttu-id="1c868-122">值</span><span class="sxs-lookup"><span data-stu-id="1c868-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1c868-123">授权</span><span class="sxs-lookup"><span data-stu-id="1c868-123">Authorization</span></span>|<span data-ttu-id="1c868-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="1c868-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1c868-125">接受</span><span class="sxs-lookup"><span data-stu-id="1c868-125">Accept</span></span>|<span data-ttu-id="1c868-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1c868-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1c868-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="1c868-127">Request body</span></span>
<span data-ttu-id="1c868-128">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1c868-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="1c868-129">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="1c868-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="1c868-130">属性</span><span class="sxs-lookup"><span data-stu-id="1c868-130">Property</span></span>|<span data-ttu-id="1c868-131">类型</span><span class="sxs-lookup"><span data-stu-id="1c868-131">Type</span></span>|<span data-ttu-id="1c868-132">说明</span><span class="sxs-lookup"><span data-stu-id="1c868-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1c868-133">deviceTag</span><span class="sxs-lookup"><span data-stu-id="1c868-133">deviceTag</span></span>|<span data-ttu-id="1c868-134">字符串</span><span class="sxs-lookup"><span data-stu-id="1c868-134">String</span></span>|<span data-ttu-id="1c868-135">设备标记</span><span class="sxs-lookup"><span data-stu-id="1c868-135">device tag</span></span>|

## <a name="response"></a><span data-ttu-id="1c868-136">响应</span><span class="sxs-lookup"><span data-stu-id="1c868-136">Response</span></span>
<span data-ttu-id="1c868-137">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="1c868-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="1c868-138">示例</span><span class="sxs-lookup"><span data-stu-id="1c868-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="1c868-139">请求</span><span class="sxs-lookup"><span data-stu-id="1c868-139">Request</span></span>
<span data-ttu-id="1c868-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1c868-140">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/beta/users/{usersId}/wipeManagedAppRegistrationsByDeviceTag

Content-type: application/json
Content-length: 39

{
  "deviceTag": "Device Tag value"
}
```

### <a name="response"></a><span data-ttu-id="1c868-141">响应</span><span class="sxs-lookup"><span data-stu-id="1c868-141">Response</span></span>
<span data-ttu-id="1c868-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1c868-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```




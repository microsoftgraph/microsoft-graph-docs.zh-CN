# <a name="wipemanagedappregistrationsbydevicetag-action"></a><span data-ttu-id="25c59-101">wipeManagedAppRegistrationsByDeviceTag 操作</span><span class="sxs-lookup"><span data-stu-id="25c59-101">wipeManagedAppRegistrationsByDeviceTag action</span></span>

> <span data-ttu-id="25c59-102">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="25c59-102">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="25c59-103">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="25c59-103">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="25c59-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="25c59-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="25c59-105">对包含指定设备标记的应用注册发布擦除操作。</span><span class="sxs-lookup"><span data-stu-id="25c59-105">Issues a wipe operation on an app registration with specified device tag.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="25c59-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="25c59-106">Prerequisites</span></span>
<span data-ttu-id="25c59-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="25c59-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="25c59-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="25c59-109">Permission type</span></span>|<span data-ttu-id="25c59-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="25c59-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="25c59-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="25c59-111">Delegated (work or school account)</span></span>|<span data-ttu-id="25c59-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25c59-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="25c59-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="25c59-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="25c59-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="25c59-114">Not supported.</span></span>|
|<span data-ttu-id="25c59-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="25c59-115">Application</span></span>|<span data-ttu-id="25c59-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="25c59-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="25c59-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="25c59-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/wipeManagedAppRegistrationsByDeviceTag
```

## <a name="request-headers"></a><span data-ttu-id="25c59-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="25c59-118">Request headers</span></span>
|<span data-ttu-id="25c59-119">标头</span><span class="sxs-lookup"><span data-stu-id="25c59-119">Header</span></span>|<span data-ttu-id="25c59-120">值</span><span class="sxs-lookup"><span data-stu-id="25c59-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="25c59-121">授权</span><span class="sxs-lookup"><span data-stu-id="25c59-121">Authorization</span></span>|<span data-ttu-id="25c59-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="25c59-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="25c59-123">接受</span><span class="sxs-lookup"><span data-stu-id="25c59-123">Accept</span></span>|<span data-ttu-id="25c59-124">application/json</span><span class="sxs-lookup"><span data-stu-id="25c59-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="25c59-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="25c59-125">Request body</span></span>
<span data-ttu-id="25c59-126">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="25c59-126">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="25c59-127">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="25c59-127">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="25c59-128">属性</span><span class="sxs-lookup"><span data-stu-id="25c59-128">Property</span></span>|<span data-ttu-id="25c59-129">类型</span><span class="sxs-lookup"><span data-stu-id="25c59-129">Type</span></span>|<span data-ttu-id="25c59-130">说明</span><span class="sxs-lookup"><span data-stu-id="25c59-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="25c59-131">deviceTag</span><span class="sxs-lookup"><span data-stu-id="25c59-131">deviceTag</span></span>|<span data-ttu-id="25c59-132">字符串</span><span class="sxs-lookup"><span data-stu-id="25c59-132">String</span></span>|<span data-ttu-id="25c59-133">设备标记</span><span class="sxs-lookup"><span data-stu-id="25c59-133">device tag</span></span>|

## <a name="response"></a><span data-ttu-id="25c59-134">响应</span><span class="sxs-lookup"><span data-stu-id="25c59-134">Response</span></span>
<span data-ttu-id="25c59-135">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="25c59-135">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="25c59-136">示例</span><span class="sxs-lookup"><span data-stu-id="25c59-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="25c59-137">请求</span><span class="sxs-lookup"><span data-stu-id="25c59-137">Request</span></span>
<span data-ttu-id="25c59-138">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="25c59-138">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/beta/users/{usersId}/wipeManagedAppRegistrationsByDeviceTag

Content-type: application/json
Content-length: 39

{
  "deviceTag": "Device Tag value"
}
```

### <a name="response"></a><span data-ttu-id="25c59-139">响应</span><span class="sxs-lookup"><span data-stu-id="25c59-139">Response</span></span>
<span data-ttu-id="25c59-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="25c59-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```




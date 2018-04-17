# <a name="delete-enrollmenttroubleshootingevent"></a><span data-ttu-id="e8f06-101">删除 enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="e8f06-101">Delete enrollmentTroubleshootingEvent</span></span>

> <span data-ttu-id="e8f06-102">**重要说明：**Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="e8f06-102">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e8f06-103">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="e8f06-103">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e8f06-104">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="e8f06-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e8f06-105">删除 [enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md)。</span><span class="sxs-lookup"><span data-stu-id="e8f06-105">Deletes a [enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e8f06-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="e8f06-106">Prerequisites</span></span>
<span data-ttu-id="e8f06-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="e8f06-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e8f06-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="e8f06-109">Permission type</span></span>|<span data-ttu-id="e8f06-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e8f06-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e8f06-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e8f06-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e8f06-112">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8f06-112">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="e8f06-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e8f06-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e8f06-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="e8f06-114">Not supported.</span></span>|
|<span data-ttu-id="e8f06-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="e8f06-115">Application</span></span>|<span data-ttu-id="e8f06-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e8f06-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e8f06-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e8f06-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="e8f06-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="e8f06-118">Request headers</span></span>
|<span data-ttu-id="e8f06-119">标头</span><span class="sxs-lookup"><span data-stu-id="e8f06-119">Header</span></span>|<span data-ttu-id="e8f06-120">值</span><span class="sxs-lookup"><span data-stu-id="e8f06-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e8f06-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e8f06-121">Authorization</span></span>|<span data-ttu-id="e8f06-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e8f06-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e8f06-123">Accept</span><span class="sxs-lookup"><span data-stu-id="e8f06-123">Accept</span></span>|<span data-ttu-id="e8f06-124">application/json</span><span class="sxs-lookup"><span data-stu-id="e8f06-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e8f06-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="e8f06-125">Request body</span></span>
<span data-ttu-id="e8f06-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e8f06-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e8f06-127">响应</span><span class="sxs-lookup"><span data-stu-id="e8f06-127">Response</span></span>
<span data-ttu-id="e8f06-128">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="e8f06-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="e8f06-129">示例</span><span class="sxs-lookup"><span data-stu-id="e8f06-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="e8f06-130">请求</span><span class="sxs-lookup"><span data-stu-id="e8f06-130">Request</span></span>
<span data-ttu-id="e8f06-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e8f06-131">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

### <a name="response"></a><span data-ttu-id="e8f06-132">响应</span><span class="sxs-lookup"><span data-stu-id="e8f06-132">Response</span></span>
<span data-ttu-id="e8f06-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e8f06-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




# <a name="create-devicemanagementtroubleshootingevent"></a><span data-ttu-id="d1899-101">创建 deviceManagementTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="d1899-101">Create deviceManagementTroubleshootingEvent</span></span>

> <span data-ttu-id="d1899-102">**重要说明：**Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="d1899-102">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d1899-103">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d1899-103">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d1899-104">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="d1899-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d1899-105">创建新的 [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d1899-105">Create a new [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d1899-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="d1899-106">Prerequisites</span></span>
<span data-ttu-id="d1899-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="d1899-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="d1899-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d1899-109">Permission type</span></span>|<span data-ttu-id="d1899-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d1899-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d1899-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d1899-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d1899-112">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1899-112">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="d1899-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d1899-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d1899-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="d1899-114">Not supported.</span></span>|
|<span data-ttu-id="d1899-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="d1899-115">Application</span></span>|<span data-ttu-id="d1899-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d1899-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d1899-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d1899-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/troubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="d1899-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="d1899-118">Request headers</span></span>
|<span data-ttu-id="d1899-119">标头</span><span class="sxs-lookup"><span data-stu-id="d1899-119">Header</span></span>|<span data-ttu-id="d1899-120">值</span><span class="sxs-lookup"><span data-stu-id="d1899-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d1899-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d1899-121">Authorization</span></span>|<span data-ttu-id="d1899-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d1899-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d1899-123">Accept</span><span class="sxs-lookup"><span data-stu-id="d1899-123">Accept</span></span>|<span data-ttu-id="d1899-124">application/json</span><span class="sxs-lookup"><span data-stu-id="d1899-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d1899-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="d1899-125">Request body</span></span>
<span data-ttu-id="d1899-126">在请求正文中，提供 deviceManagementTroubleshootingEvent 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d1899-126">In the request body, supply a JSON representation for the deviceManagementTroubleshootingEvent object.</span></span>

<span data-ttu-id="d1899-127">下表显示创建 deviceManagementTroubleshootingEvent 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="d1899-127">The following table shows the properties that are required when you create the deviceManagementTroubleshootingEvent.</span></span>

|<span data-ttu-id="d1899-128">属性</span><span class="sxs-lookup"><span data-stu-id="d1899-128">Property</span></span>|<span data-ttu-id="d1899-129">类型</span><span class="sxs-lookup"><span data-stu-id="d1899-129">Type</span></span>|<span data-ttu-id="d1899-130">说明</span><span class="sxs-lookup"><span data-stu-id="d1899-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d1899-131">id</span><span class="sxs-lookup"><span data-stu-id="d1899-131">id</span></span>|<span data-ttu-id="d1899-132">String</span><span class="sxs-lookup"><span data-stu-id="d1899-132">String</span></span>|<span data-ttu-id="d1899-133">对象的 UUID</span><span class="sxs-lookup"><span data-stu-id="d1899-133">UUID for the object</span></span>|
|<span data-ttu-id="d1899-134">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="d1899-134">eventDateTime</span></span>|<span data-ttu-id="d1899-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d1899-135">DateTimeOffset</span></span>|<span data-ttu-id="d1899-136">事件发生的时间。</span><span class="sxs-lookup"><span data-stu-id="d1899-136">Time when the event occurred .</span></span>|
|<span data-ttu-id="d1899-137">correlationId</span><span class="sxs-lookup"><span data-stu-id="d1899-137">correlationId</span></span>|<span data-ttu-id="d1899-138">String</span><span class="sxs-lookup"><span data-stu-id="d1899-138">String</span></span>|<span data-ttu-id="d1899-139">用于跟踪服务中的故障的 ID。</span><span class="sxs-lookup"><span data-stu-id="d1899-139">Id used for tracing the failure in the service.</span></span>|



## <a name="response"></a><span data-ttu-id="d1899-140">响应</span><span class="sxs-lookup"><span data-stu-id="d1899-140">Response</span></span>
<span data-ttu-id="d1899-141">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d1899-141">If successful, this method returns a `201 Created` response code and a [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d1899-142">示例</span><span class="sxs-lookup"><span data-stu-id="d1899-142">Example</span></span>
### <a name="request"></a><span data-ttu-id="d1899-143">请求</span><span class="sxs-lookup"><span data-stu-id="d1899-143">Request</span></span>
<span data-ttu-id="d1899-144">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d1899-144">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents
Content-type: application/json
Content-length: 179

{
  "@odata.type": "#microsoft.graph.deviceManagementTroubleshootingEvent",
  "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
  "correlationId": "Correlation Id value"
}
```

### <a name="response"></a><span data-ttu-id="d1899-145">响应</span><span class="sxs-lookup"><span data-stu-id="d1899-145">Response</span></span>
<span data-ttu-id="d1899-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d1899-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 228

{
  "@odata.type": "#microsoft.graph.deviceManagementTroubleshootingEvent",
  "id": "fb26dcee-dcee-fb26-eedc-26fbeedc26fb",
  "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
  "correlationId": "Correlation Id value"
}
```




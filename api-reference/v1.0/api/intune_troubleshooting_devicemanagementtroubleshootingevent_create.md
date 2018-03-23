# <a name="create-devicemanagementtroubleshootingevent"></a><span data-ttu-id="b2d97-101">创建 deviceManagementTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="b2d97-101">Create deviceManagementTroubleshootingEvent</span></span>

> <span data-ttu-id="b2d97-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="b2d97-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b2d97-103">创建新的 [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b2d97-103">Create a new [plannerBucket](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b2d97-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="b2d97-104">Prerequisites</span></span>
<span data-ttu-id="b2d97-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="b2d97-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b2d97-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="b2d97-107">Permission type</span></span>|<span data-ttu-id="b2d97-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b2d97-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b2d97-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b2d97-109">Delegated (work or school account)</span></span>|<span data-ttu-id="b2d97-110">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b2d97-110">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="b2d97-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b2d97-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b2d97-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="b2d97-112">Not supported.</span></span>|
|<span data-ttu-id="b2d97-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="b2d97-113">Application</span></span>|<span data-ttu-id="b2d97-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="b2d97-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b2d97-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b2d97-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/troubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="b2d97-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="b2d97-116">Request headers</span></span>
|<span data-ttu-id="b2d97-117">标头</span><span class="sxs-lookup"><span data-stu-id="b2d97-117">Header</span></span>|<span data-ttu-id="b2d97-118">值</span><span class="sxs-lookup"><span data-stu-id="b2d97-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b2d97-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="b2d97-119">Authorization</span></span>|<span data-ttu-id="b2d97-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b2d97-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="b2d97-121">Accept</span><span class="sxs-lookup"><span data-stu-id="b2d97-121">Accept</span></span>|<span data-ttu-id="b2d97-122">application/json</span><span class="sxs-lookup"><span data-stu-id="b2d97-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b2d97-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="b2d97-123">Request body</span></span>
<span data-ttu-id="b2d97-124">在请求正文中，提供 deviceManagementTroubleshootingEvent 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b2d97-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="b2d97-125">下表显示创建 deviceManagementTroubleshootingEvent 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="b2d97-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="b2d97-126">属性</span><span class="sxs-lookup"><span data-stu-id="b2d97-126">Property</span></span>|<span data-ttu-id="b2d97-127">类型</span><span class="sxs-lookup"><span data-stu-id="b2d97-127">Type</span></span>|<span data-ttu-id="b2d97-128">说明</span><span class="sxs-lookup"><span data-stu-id="b2d97-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b2d97-129">id</span><span class="sxs-lookup"><span data-stu-id="b2d97-129">id</span></span>|<span data-ttu-id="b2d97-130">String</span><span class="sxs-lookup"><span data-stu-id="b2d97-130">String</span></span>|<span data-ttu-id="b2d97-131">对象的 UUID</span><span class="sxs-lookup"><span data-stu-id="b2d97-131">UUID for the object</span></span>|
|<span data-ttu-id="b2d97-132">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="b2d97-132">eventDateTime</span></span>|<span data-ttu-id="b2d97-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b2d97-133">DateTimeOffset</span></span>|<span data-ttu-id="b2d97-134">事件发生的时间。</span><span class="sxs-lookup"><span data-stu-id="b2d97-134">Time when the event occurred .</span></span>|
|<span data-ttu-id="b2d97-135">correlationId</span><span class="sxs-lookup"><span data-stu-id="b2d97-135">correlationId</span></span>|<span data-ttu-id="b2d97-136">String</span><span class="sxs-lookup"><span data-stu-id="b2d97-136">String</span></span>|<span data-ttu-id="b2d97-137">用于跟踪服务中的故障的 ID。</span><span class="sxs-lookup"><span data-stu-id="b2d97-137">Id used for tracing the failure in the service.</span></span>|



## <a name="response"></a><span data-ttu-id="b2d97-138">响应</span><span class="sxs-lookup"><span data-stu-id="b2d97-138">Response</span></span>
<span data-ttu-id="b2d97-139">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b2d97-139">If successful, this method returns a `201 Created` response code and a [DriveItemVersion](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b2d97-140">示例</span><span class="sxs-lookup"><span data-stu-id="b2d97-140">Example</span></span>
### <a name="request"></a><span data-ttu-id="b2d97-141">请求</span><span class="sxs-lookup"><span data-stu-id="b2d97-141">Request</span></span>
<span data-ttu-id="b2d97-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b2d97-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/troubleshootingEvents
Content-type: application/json
Content-length: 179

{
  "@odata.type": "#microsoft.graph.deviceManagementTroubleshootingEvent",
  "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
  "correlationId": "Correlation Id value"
}
```

### <a name="response"></a><span data-ttu-id="b2d97-143">响应</span><span class="sxs-lookup"><span data-stu-id="b2d97-143">Response</span></span>
<span data-ttu-id="b2d97-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b2d97-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




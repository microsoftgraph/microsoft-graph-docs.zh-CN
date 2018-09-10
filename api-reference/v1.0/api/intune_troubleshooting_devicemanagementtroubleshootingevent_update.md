# <a name="update-devicemanagementtroubleshootingevent"></a><span data-ttu-id="4774f-101">更新 deviceManagementTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="4774f-101">Update deviceManagementTroubleshootingEvent</span></span>

> <span data-ttu-id="4774f-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="4774f-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4774f-103">更新 [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="4774f-103">Update the properties of a [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4774f-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="4774f-104">Prerequisites</span></span>
<span data-ttu-id="4774f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="4774f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="4774f-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="4774f-107">Permission type</span></span>|<span data-ttu-id="4774f-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="4774f-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4774f-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4774f-109">Delegated (work or school account)</span></span>|<span data-ttu-id="4774f-110">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4774f-110">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="4774f-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4774f-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4774f-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="4774f-112">Not supported.</span></span>|
|<span data-ttu-id="4774f-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="4774f-113">Application</span></span>|<span data-ttu-id="4774f-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="4774f-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4774f-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4774f-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="4774f-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="4774f-116">Request headers</span></span>
|<span data-ttu-id="4774f-117">标头</span><span class="sxs-lookup"><span data-stu-id="4774f-117">Header</span></span>|<span data-ttu-id="4774f-118">值</span><span class="sxs-lookup"><span data-stu-id="4774f-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4774f-119">授权</span><span class="sxs-lookup"><span data-stu-id="4774f-119">Authorization</span></span>|<span data-ttu-id="4774f-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="4774f-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4774f-121">Accept</span><span class="sxs-lookup"><span data-stu-id="4774f-121">Accept</span></span>|<span data-ttu-id="4774f-122">application/json</span><span class="sxs-lookup"><span data-stu-id="4774f-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4774f-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="4774f-123">Request body</span></span>
<span data-ttu-id="4774f-124">在请求正文中，提供 [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4774f-124">In the request body, supply a JSON representation for the [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md) object.</span></span>

<span data-ttu-id="4774f-125">下表显示创建 [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="4774f-125">The following table shows the properties that are required when you create the [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md).</span></span>

|<span data-ttu-id="4774f-126">属性</span><span class="sxs-lookup"><span data-stu-id="4774f-126">Property</span></span>|<span data-ttu-id="4774f-127">类型</span><span class="sxs-lookup"><span data-stu-id="4774f-127">Type</span></span>|<span data-ttu-id="4774f-128">说明</span><span class="sxs-lookup"><span data-stu-id="4774f-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4774f-129">ID</span><span class="sxs-lookup"><span data-stu-id="4774f-129">id</span></span>|<span data-ttu-id="4774f-130">字符串</span><span class="sxs-lookup"><span data-stu-id="4774f-130">String</span></span>|<span data-ttu-id="4774f-131">对象的 UUID</span><span class="sxs-lookup"><span data-stu-id="4774f-131">UUID for the object</span></span>|
|<span data-ttu-id="4774f-132">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="4774f-132">eventDateTime</span></span>|<span data-ttu-id="4774f-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4774f-133">DateTimeOffset</span></span>|<span data-ttu-id="4774f-134">事件发生的时间。</span><span class="sxs-lookup"><span data-stu-id="4774f-134">Time when the event occurred .</span></span>|
|<span data-ttu-id="4774f-135">correlationId</span><span class="sxs-lookup"><span data-stu-id="4774f-135">correlationId</span></span>|<span data-ttu-id="4774f-136">字符串</span><span class="sxs-lookup"><span data-stu-id="4774f-136">String</span></span>|<span data-ttu-id="4774f-137">用于跟踪服务中的故障的 ID。</span><span class="sxs-lookup"><span data-stu-id="4774f-137">Id used for tracing the failure in the service.</span></span>|



## <a name="response"></a><span data-ttu-id="4774f-138">响应</span><span class="sxs-lookup"><span data-stu-id="4774f-138">Response</span></span>
<span data-ttu-id="4774f-139">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4774f-139">If successful, this method returns a `200 OK` response code and an updated [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4774f-140">示例</span><span class="sxs-lookup"><span data-stu-id="4774f-140">Example</span></span>
### <a name="request"></a><span data-ttu-id="4774f-141">请求</span><span class="sxs-lookup"><span data-stu-id="4774f-141">Request</span></span>
<span data-ttu-id="4774f-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4774f-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1/deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
Content-type: application/json
Content-length: 104

{
  "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
  "correlationId": "Correlation Id value"
}
```

### <a name="response"></a><span data-ttu-id="4774f-143">响应</span><span class="sxs-lookup"><span data-stu-id="4774f-143">Response</span></span>
<span data-ttu-id="4774f-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4774f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 228

{
  "@odata.type": "#microsoft.graph.deviceManagementTroubleshootingEvent",
  "id": "fb26dcee-dcee-fb26-eedc-26fbeedc26fb",
  "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
  "correlationId": "Correlation Id value"
}
```





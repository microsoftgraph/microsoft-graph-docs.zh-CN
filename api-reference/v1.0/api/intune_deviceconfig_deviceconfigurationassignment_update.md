# <a name="update-deviceconfigurationassignment"></a><span data-ttu-id="9bbf6-101">更新 deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="9bbf6-101">Update deviceConfigurationAssignment</span></span>

> <span data-ttu-id="9bbf6-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="9bbf6-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9bbf6-103">更新 [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="9bbf6-103">Update the properties of a [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9bbf6-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="9bbf6-104">Prerequisites</span></span>
<span data-ttu-id="9bbf6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="9bbf6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="9bbf6-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="9bbf6-107">Permission type</span></span>|<span data-ttu-id="9bbf6-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="9bbf6-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9bbf6-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9bbf6-109">Delegated (work or school account)</span></span>|<span data-ttu-id="9bbf6-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9bbf6-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9bbf6-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9bbf6-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9bbf6-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="9bbf6-112">Not supported.</span></span>|
|<span data-ttu-id="9bbf6-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="9bbf6-113">Application</span></span>|<span data-ttu-id="9bbf6-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="9bbf6-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9bbf6-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9bbf6-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments/{deviceConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="9bbf6-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="9bbf6-116">Request headers</span></span>
|<span data-ttu-id="9bbf6-117">标头</span><span class="sxs-lookup"><span data-stu-id="9bbf6-117">Header</span></span>|<span data-ttu-id="9bbf6-118">值</span><span class="sxs-lookup"><span data-stu-id="9bbf6-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9bbf6-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="9bbf6-119">Authorization</span></span>|<span data-ttu-id="9bbf6-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="9bbf6-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9bbf6-121">Accept</span><span class="sxs-lookup"><span data-stu-id="9bbf6-121">Accept</span></span>|<span data-ttu-id="9bbf6-122">application/json</span><span class="sxs-lookup"><span data-stu-id="9bbf6-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9bbf6-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="9bbf6-123">Request body</span></span>
<span data-ttu-id="9bbf6-124">在请求正文中，提供 [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9bbf6-124">In the request body, supply a JSON representation for the [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md) object.</span></span>

<span data-ttu-id="9bbf6-125">下表显示创建 [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="9bbf6-125">The following table shows the properties that are required when you create the [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md).</span></span>

|<span data-ttu-id="9bbf6-126">属性</span><span class="sxs-lookup"><span data-stu-id="9bbf6-126">Property</span></span>|<span data-ttu-id="9bbf6-127">类型</span><span class="sxs-lookup"><span data-stu-id="9bbf6-127">Type</span></span>|<span data-ttu-id="9bbf6-128">说明</span><span class="sxs-lookup"><span data-stu-id="9bbf6-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9bbf6-129">id</span><span class="sxs-lookup"><span data-stu-id="9bbf6-129">id</span></span>|<span data-ttu-id="9bbf6-130">String</span><span class="sxs-lookup"><span data-stu-id="9bbf6-130">String</span></span>|<span data-ttu-id="9bbf6-131">分配的键。</span><span class="sxs-lookup"><span data-stu-id="9bbf6-131">The key of the assignment.</span></span>|
|<span data-ttu-id="9bbf6-132">target</span><span class="sxs-lookup"><span data-stu-id="9bbf6-132">target</span></span>|[<span data-ttu-id="9bbf6-133">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="9bbf6-133">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune_shared_deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="9bbf6-134">设备配置的分配目标。</span><span class="sxs-lookup"><span data-stu-id="9bbf6-134">The assignment target for the device configuration.</span></span>|



## <a name="response"></a><span data-ttu-id="9bbf6-135">响应</span><span class="sxs-lookup"><span data-stu-id="9bbf6-135">Response</span></span>
<span data-ttu-id="9bbf6-136">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9bbf6-136">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9bbf6-137">示例</span><span class="sxs-lookup"><span data-stu-id="9bbf6-137">Example</span></span>
### <a name="request"></a><span data-ttu-id="9bbf6-138">请求</span><span class="sxs-lookup"><span data-stu-id="9bbf6-138">Request</span></span>
<span data-ttu-id="9bbf6-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9bbf6-139">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments/{deviceConfigurationAssignmentId}
Content-type: application/json
Content-length: 169

{
  "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="9bbf6-140">响应</span><span class="sxs-lookup"><span data-stu-id="9bbf6-140">Response</span></span>
<span data-ttu-id="9bbf6-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9bbf6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 218

{
  "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
  "id": "d59b6342-6342-d59b-4263-9bd542639bd5",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```




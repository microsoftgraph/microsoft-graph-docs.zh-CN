# <a name="update-manageddevicemobileappconfigurationassignment"></a><span data-ttu-id="9eada-101">更新 managedDeviceMobileAppConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="9eada-101">Update managedDeviceMobileAppConfigurationAssignment</span></span>

> <span data-ttu-id="9eada-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="9eada-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9eada-103">更新 [managedDeviceMobileAppConfigurationAssignment](../resources/intune_apps_manageddevicemobileappconfigurationassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="9eada-103">Update the properties of a [managedDeviceMobileAppConfigurationAssignment](../resources/intune_apps_manageddevicemobileappconfigurationassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9eada-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="9eada-104">Prerequisites</span></span>
<span data-ttu-id="9eada-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="9eada-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="9eada-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="9eada-107">Permission type</span></span>|<span data-ttu-id="9eada-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="9eada-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9eada-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9eada-109">Delegated (work or school account)</span></span>|<span data-ttu-id="9eada-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9eada-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="9eada-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9eada-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9eada-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="9eada-112">Not supported.</span></span>|
|<span data-ttu-id="9eada-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="9eada-113">Application</span></span>|<span data-ttu-id="9eada-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="9eada-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9eada-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9eada-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments/{managedDeviceMobileAppConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="9eada-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="9eada-116">Request headers</span></span>
|<span data-ttu-id="9eada-117">标头</span><span class="sxs-lookup"><span data-stu-id="9eada-117">Header</span></span>|<span data-ttu-id="9eada-118">值</span><span class="sxs-lookup"><span data-stu-id="9eada-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9eada-119">授权</span><span class="sxs-lookup"><span data-stu-id="9eada-119">Authorization</span></span>|<span data-ttu-id="9eada-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="9eada-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9eada-121">接受</span><span class="sxs-lookup"><span data-stu-id="9eada-121">Accept</span></span>|<span data-ttu-id="9eada-122">application/json</span><span class="sxs-lookup"><span data-stu-id="9eada-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9eada-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="9eada-123">Request body</span></span>
<span data-ttu-id="9eada-124">在请求正文中，提供 [managedDeviceMobileAppConfigurationAssignment](../resources/intune_apps_manageddevicemobileappconfigurationassignment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9eada-124">In the request body, supply a JSON representation for the [managedDeviceMobileAppConfigurationAssignment](../resources/intune_apps_manageddevicemobileappconfigurationassignment.md) object.</span></span>

<span data-ttu-id="9eada-125">下表显示创建 [managedDeviceMobileAppConfigurationAssignment](../resources/intune_apps_manageddevicemobileappconfigurationassignment.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="9eada-125">The following table shows the properties that are required when you create the [managedDeviceMobileAppConfigurationAssignment](../resources/intune_apps_manageddevicemobileappconfigurationassignment.md).</span></span>

|<span data-ttu-id="9eada-126">属性</span><span class="sxs-lookup"><span data-stu-id="9eada-126">Property</span></span>|<span data-ttu-id="9eada-127">类型</span><span class="sxs-lookup"><span data-stu-id="9eada-127">Type</span></span>|<span data-ttu-id="9eada-128">说明</span><span class="sxs-lookup"><span data-stu-id="9eada-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9eada-129">ID</span><span class="sxs-lookup"><span data-stu-id="9eada-129">id</span></span>|<span data-ttu-id="9eada-130">字符串</span><span class="sxs-lookup"><span data-stu-id="9eada-130">String</span></span>|<span data-ttu-id="9eada-131">实体的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="9eada-131">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="9eada-132">目标</span><span class="sxs-lookup"><span data-stu-id="9eada-132">target</span></span>|[<span data-ttu-id="9eada-133">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="9eada-133">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune_shared_deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="9eada-134">将 T&C 策略分配到的分配目标。</span><span class="sxs-lookup"><span data-stu-id="9eada-134">Assignment target that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="9eada-135">响应</span><span class="sxs-lookup"><span data-stu-id="9eada-135">Response</span></span>
<span data-ttu-id="9eada-136">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [managedDeviceMobileAppConfigurationAssignment](../resources/intune_apps_manageddevicemobileappconfigurationassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9eada-136">If successful, this method returns a `200 OK` response code and an updated [managedDeviceMobileAppConfigurationAssignment](../resources/intune_apps_manageddevicemobileappconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9eada-137">示例</span><span class="sxs-lookup"><span data-stu-id="9eada-137">Example</span></span>
### <a name="request"></a><span data-ttu-id="9eada-138">请求</span><span class="sxs-lookup"><span data-stu-id="9eada-138">Request</span></span>
<span data-ttu-id="9eada-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9eada-139">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments/{managedDeviceMobileAppConfigurationAssignmentId}
Content-type: application/json
Content-length: 101

{
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="9eada-140">响应</span><span class="sxs-lookup"><span data-stu-id="9eada-140">Response</span></span>
<span data-ttu-id="9eada-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9eada-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 234

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationAssignment",
  "id": "4df81c9c-1c9c-4df8-9c1c-f84d9c1cf84d",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```









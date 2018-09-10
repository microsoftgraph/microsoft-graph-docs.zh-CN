# <a name="create-enrollmentconfigurationassignment"></a><span data-ttu-id="deb84-101">创建 enrollmentConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="deb84-101">Create enrollmentConfigurationAssignment</span></span>

> <span data-ttu-id="deb84-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="deb84-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="deb84-103">创建新的 [enrollmentConfigurationAssignment](../resources/intune_onboarding_enrollmentconfigurationassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="deb84-103">Create a new [enrollmentConfigurationAssignment](../resources/intune_onboarding_enrollmentconfigurationassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="deb84-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="deb84-104">Prerequisites</span></span>
<span data-ttu-id="deb84-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="deb84-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="deb84-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="deb84-107">Permission type</span></span>|<span data-ttu-id="deb84-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="deb84-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="deb84-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="deb84-109">Delegated (work or school account)</span></span>|<span data-ttu-id="deb84-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="deb84-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="deb84-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="deb84-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="deb84-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="deb84-112">Not supported.</span></span>|
|<span data-ttu-id="deb84-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="deb84-113">Application</span></span>|<span data-ttu-id="deb84-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="deb84-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="deb84-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="deb84-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="deb84-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="deb84-116">Request headers</span></span>
|<span data-ttu-id="deb84-117">标头</span><span class="sxs-lookup"><span data-stu-id="deb84-117">Header</span></span>|<span data-ttu-id="deb84-118">值</span><span class="sxs-lookup"><span data-stu-id="deb84-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="deb84-119">授权</span><span class="sxs-lookup"><span data-stu-id="deb84-119">Authorization</span></span>|<span data-ttu-id="deb84-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="deb84-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="deb84-121">接受</span><span class="sxs-lookup"><span data-stu-id="deb84-121">Accept</span></span>|<span data-ttu-id="deb84-122">application/json</span><span class="sxs-lookup"><span data-stu-id="deb84-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="deb84-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="deb84-123">Request body</span></span>
<span data-ttu-id="deb84-124">在请求正文中，提供 enrollmentConfigurationAssignment 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="deb84-124">In the request body, supply a JSON representation for the enrollmentConfigurationAssignment object.</span></span>

<span data-ttu-id="deb84-125">下表显示创建 enrollmentConfigurationAssignment 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="deb84-125">The following table shows the properties that are required when you create the enrollmentConfigurationAssignment.</span></span>

|<span data-ttu-id="deb84-126">属性</span><span class="sxs-lookup"><span data-stu-id="deb84-126">Property</span></span>|<span data-ttu-id="deb84-127">类型</span><span class="sxs-lookup"><span data-stu-id="deb84-127">Type</span></span>|<span data-ttu-id="deb84-128">说明</span><span class="sxs-lookup"><span data-stu-id="deb84-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="deb84-129">ID</span><span class="sxs-lookup"><span data-stu-id="deb84-129">id</span></span>|<span data-ttu-id="deb84-130">字符串</span><span class="sxs-lookup"><span data-stu-id="deb84-130">String</span></span>|<span data-ttu-id="deb84-131">尚未记录</span><span class="sxs-lookup"><span data-stu-id="deb84-131">Not yet documented</span></span>|
|<span data-ttu-id="deb84-132">目标</span><span class="sxs-lookup"><span data-stu-id="deb84-132">target</span></span>|[<span data-ttu-id="deb84-133">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="deb84-133">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune_shared_deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="deb84-134">尚未记录</span><span class="sxs-lookup"><span data-stu-id="deb84-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="deb84-135">响应</span><span class="sxs-lookup"><span data-stu-id="deb84-135">Response</span></span>
<span data-ttu-id="deb84-136">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [enrollmentConfigurationAssignment](../resources/intune_onboarding_enrollmentconfigurationassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="deb84-136">If successful, this method returns a `201 Created` response code and a [enrollmentConfigurationAssignment](../resources/intune_onboarding_enrollmentconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="deb84-137">示例</span><span class="sxs-lookup"><span data-stu-id="deb84-137">Example</span></span>
### <a name="request"></a><span data-ttu-id="deb84-138">请求</span><span class="sxs-lookup"><span data-stu-id="deb84-138">Request</span></span>
<span data-ttu-id="deb84-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="deb84-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments
Content-type: application/json
Content-length: 173

{
  "@odata.type": "#microsoft.graph.enrollmentConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="deb84-140">响应</span><span class="sxs-lookup"><span data-stu-id="deb84-140">Response</span></span>
<span data-ttu-id="deb84-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="deb84-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 222

{
  "@odata.type": "#microsoft.graph.enrollmentConfigurationAssignment",
  "id": "705b021c-021c-705b-1c02-5b701c025b70",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```









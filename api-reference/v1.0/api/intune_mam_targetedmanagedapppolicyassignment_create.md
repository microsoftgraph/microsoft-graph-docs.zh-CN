# <a name="create-targetedmanagedapppolicyassignment"></a><span data-ttu-id="8673b-101">创建 targetedManagedAppPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="8673b-101">Create targetedManagedAppPolicyAssignment</span></span>

> <span data-ttu-id="8673b-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="8673b-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8673b-103">创建新的 [targetedManagedAppPolicyAssignment](../resources/intune_mam_targetedmanagedapppolicyassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8673b-103">Create a new [targetedManagedAppPolicyAssignment](../resources/intune_mam_targetedmanagedapppolicyassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8673b-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="8673b-104">Prerequisites</span></span>
<span data-ttu-id="8673b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="8673b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="8673b-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="8673b-107">Permission type</span></span>|<span data-ttu-id="8673b-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="8673b-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8673b-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8673b-109">Delegated (work or school account)</span></span>|<span data-ttu-id="8673b-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8673b-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="8673b-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8673b-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8673b-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="8673b-112">Not supported.</span></span>|
|<span data-ttu-id="8673b-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="8673b-113">Application</span></span>|<span data-ttu-id="8673b-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="8673b-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8673b-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8673b-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/assignments
POST /deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}/assignments
POST /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/assignments
POST /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/assignments
POST /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="8673b-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="8673b-116">Request headers</span></span>
|<span data-ttu-id="8673b-117">标头</span><span class="sxs-lookup"><span data-stu-id="8673b-117">Header</span></span>|<span data-ttu-id="8673b-118">值</span><span class="sxs-lookup"><span data-stu-id="8673b-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8673b-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="8673b-119">Authorization</span></span>|<span data-ttu-id="8673b-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="8673b-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8673b-121">Accept</span><span class="sxs-lookup"><span data-stu-id="8673b-121">Accept</span></span>|<span data-ttu-id="8673b-122">application/json</span><span class="sxs-lookup"><span data-stu-id="8673b-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8673b-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="8673b-123">Request body</span></span>
<span data-ttu-id="8673b-124">在请求正文中，提供 targetedManagedAppPolicyAssignment 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8673b-124">In the request body, supply a JSON representation for the targetedManagedAppPolicyAssignment object.</span></span>

<span data-ttu-id="8673b-125">下表显示创建 targetedManagedAppPolicyAssignment 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="8673b-125">The following table shows the properties that are required when you create the targetedManagedAppPolicyAssignment.</span></span>

|<span data-ttu-id="8673b-126">属性</span><span class="sxs-lookup"><span data-stu-id="8673b-126">Property</span></span>|<span data-ttu-id="8673b-127">类型</span><span class="sxs-lookup"><span data-stu-id="8673b-127">Type</span></span>|<span data-ttu-id="8673b-128">说明</span><span class="sxs-lookup"><span data-stu-id="8673b-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8673b-129">id</span><span class="sxs-lookup"><span data-stu-id="8673b-129">id</span></span>|<span data-ttu-id="8673b-130">String</span><span class="sxs-lookup"><span data-stu-id="8673b-130">String</span></span>|<span data-ttu-id="8673b-131">ID</span><span class="sxs-lookup"><span data-stu-id="8673b-131">Id</span></span>|
|<span data-ttu-id="8673b-132">target</span><span class="sxs-lookup"><span data-stu-id="8673b-132">target</span></span>|[<span data-ttu-id="8673b-133">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="8673b-133">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune_mam_deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="8673b-134">组或应用的部署标识符</span><span class="sxs-lookup"><span data-stu-id="8673b-134">Identifier for deployment of a group or app</span></span>|



## <a name="response"></a><span data-ttu-id="8673b-135">响应</span><span class="sxs-lookup"><span data-stu-id="8673b-135">Response</span></span>
<span data-ttu-id="8673b-136">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [targetedManagedAppPolicyAssignment](../resources/intune_mam_targetedmanagedapppolicyassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8673b-136">If successful, this method returns a `201 Created` response code and a [targetedManagedAppPolicyAssignment](../resources/intune_mam_targetedmanagedapppolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8673b-137">示例</span><span class="sxs-lookup"><span data-stu-id="8673b-137">Example</span></span>
### <a name="request"></a><span data-ttu-id="8673b-138">请求</span><span class="sxs-lookup"><span data-stu-id="8673b-138">Request</span></span>
<span data-ttu-id="8673b-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8673b-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/assignments
Content-type: application/json
Content-length: 174

{
  "@odata.type": "#microsoft.graph.targetedManagedAppPolicyAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="8673b-140">响应</span><span class="sxs-lookup"><span data-stu-id="8673b-140">Response</span></span>
<span data-ttu-id="8673b-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8673b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 223

{
  "@odata.type": "#microsoft.graph.targetedManagedAppPolicyAssignment",
  "id": "8b68c4a6-c4a6-8b68-a6c4-688ba6c4688b",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```




# <a name="update-devicecompliancepolicyassignment"></a><span data-ttu-id="b1370-101">更新 deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="b1370-101">Update deviceCompliancePolicyAssignment</span></span>

> <span data-ttu-id="b1370-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="b1370-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b1370-103">更新 [deviceCompliancePolicyAssignment](../resources/intune_deviceconfig_devicecompliancepolicyassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b1370-103">Update the properties of a [deviceCompliancePolicyAssignment](../resources/intune_deviceconfig_devicecompliancepolicyassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b1370-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="b1370-104">Prerequisites</span></span>
<span data-ttu-id="b1370-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="b1370-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b1370-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="b1370-107">Permission type</span></span>|<span data-ttu-id="b1370-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b1370-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b1370-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b1370-109">Delegated (work or school account)</span></span>|<span data-ttu-id="b1370-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1370-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b1370-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b1370-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b1370-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="b1370-112">Not supported.</span></span>|
|<span data-ttu-id="b1370-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="b1370-113">Application</span></span>|<span data-ttu-id="b1370-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="b1370-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b1370-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b1370-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments/{deviceCompliancePolicyAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="b1370-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="b1370-116">Request headers</span></span>
|<span data-ttu-id="b1370-117">标头</span><span class="sxs-lookup"><span data-stu-id="b1370-117">Header</span></span>|<span data-ttu-id="b1370-118">值</span><span class="sxs-lookup"><span data-stu-id="b1370-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b1370-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="b1370-119">Authorization</span></span>|<span data-ttu-id="b1370-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b1370-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b1370-121">Accept</span><span class="sxs-lookup"><span data-stu-id="b1370-121">Accept</span></span>|<span data-ttu-id="b1370-122">application/json</span><span class="sxs-lookup"><span data-stu-id="b1370-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b1370-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="b1370-123">Request body</span></span>
<span data-ttu-id="b1370-124">在请求正文中，提供 [deviceCompliancePolicyAssignment](../resources/intune_deviceconfig_devicecompliancepolicyassignment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b1370-124">In the request body, supply a JSON representation for the [deviceCompliancePolicyAssignment](../resources/intune_deviceconfig_devicecompliancepolicyassignment.md) object.</span></span>

<span data-ttu-id="b1370-125">下表显示创建 [deviceCompliancePolicyAssignment](../resources/intune_deviceconfig_devicecompliancepolicyassignment.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="b1370-125">The following table shows the properties that are required when you create the [deviceCompliancePolicyAssignment](../resources/intune_deviceconfig_devicecompliancepolicyassignment.md).</span></span>

|<span data-ttu-id="b1370-126">属性</span><span class="sxs-lookup"><span data-stu-id="b1370-126">Property</span></span>|<span data-ttu-id="b1370-127">类型</span><span class="sxs-lookup"><span data-stu-id="b1370-127">Type</span></span>|<span data-ttu-id="b1370-128">说明</span><span class="sxs-lookup"><span data-stu-id="b1370-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b1370-129">id</span><span class="sxs-lookup"><span data-stu-id="b1370-129">id</span></span>|<span data-ttu-id="b1370-130">String</span><span class="sxs-lookup"><span data-stu-id="b1370-130">String</span></span>|<span data-ttu-id="b1370-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="b1370-131">Key of the entity.</span></span>|
|<span data-ttu-id="b1370-132">target</span><span class="sxs-lookup"><span data-stu-id="b1370-132">target</span></span>|[<span data-ttu-id="b1370-133">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="b1370-133">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune_shared_deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="b1370-134">符合性策略分配目标。</span><span class="sxs-lookup"><span data-stu-id="b1370-134">Target for the compliance policy assignment.</span></span>|



## <a name="response"></a><span data-ttu-id="b1370-135">响应</span><span class="sxs-lookup"><span data-stu-id="b1370-135">Response</span></span>
<span data-ttu-id="b1370-136">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [deviceCompliancePolicyAssignment](../resources/intune_deviceconfig_devicecompliancepolicyassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b1370-136">If successful, this method returns a `200 OK` response code and an updated [deviceCompliancePolicyAssignment](../resources/intune_deviceconfig_devicecompliancepolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b1370-137">示例</span><span class="sxs-lookup"><span data-stu-id="b1370-137">Example</span></span>
### <a name="request"></a><span data-ttu-id="b1370-138">请求</span><span class="sxs-lookup"><span data-stu-id="b1370-138">Request</span></span>
<span data-ttu-id="b1370-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b1370-139">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments/{deviceCompliancePolicyAssignmentId}
Content-type: application/json
Content-length: 172

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="b1370-140">响应</span><span class="sxs-lookup"><span data-stu-id="b1370-140">Response</span></span>
<span data-ttu-id="b1370-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b1370-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 221

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyAssignment",
  "id": "92dc3fef-3fef-92dc-ef3f-dc92ef3fdc92",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```




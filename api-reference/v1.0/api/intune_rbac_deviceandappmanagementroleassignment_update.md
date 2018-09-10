# <a name="update-deviceandappmanagementroleassignment"></a><span data-ttu-id="89fa0-101">更新 deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="89fa0-101">Update deviceAndAppManagementRoleAssignment</span></span>

> <span data-ttu-id="89fa0-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="89fa0-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="89fa0-103">更新 [deviceAndAppManagementRoleAssignment](../resources/intune_rbac_deviceandappmanagementroleassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="89fa0-103">Update the properties of a [deviceAndAppManagementRoleAssignment](../resources/intune_rbac_deviceandappmanagementroleassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="89fa0-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="89fa0-104">Prerequisites</span></span>
<span data-ttu-id="89fa0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="89fa0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="89fa0-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="89fa0-107">Permission type</span></span>|<span data-ttu-id="89fa0-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="89fa0-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="89fa0-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="89fa0-109">Delegated (work or school account)</span></span>|<span data-ttu-id="89fa0-110">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89fa0-110">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="89fa0-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="89fa0-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="89fa0-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="89fa0-112">Not supported.</span></span>|
|<span data-ttu-id="89fa0-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="89fa0-113">Application</span></span>|<span data-ttu-id="89fa0-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="89fa0-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="89fa0-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="89fa0-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleAssignments/{deviceAndAppManagementRoleAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="89fa0-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="89fa0-116">Request headers</span></span>
|<span data-ttu-id="89fa0-117">标头</span><span class="sxs-lookup"><span data-stu-id="89fa0-117">Header</span></span>|<span data-ttu-id="89fa0-118">值</span><span class="sxs-lookup"><span data-stu-id="89fa0-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="89fa0-119">授权</span><span class="sxs-lookup"><span data-stu-id="89fa0-119">Authorization</span></span>|<span data-ttu-id="89fa0-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="89fa0-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="89fa0-121">Accept</span><span class="sxs-lookup"><span data-stu-id="89fa0-121">Accept</span></span>|<span data-ttu-id="89fa0-122">application/json</span><span class="sxs-lookup"><span data-stu-id="89fa0-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="89fa0-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="89fa0-123">Request body</span></span>
<span data-ttu-id="89fa0-124">在请求正文中，提供 [deviceAndAppManagementRoleAssignment](../resources/intune_rbac_deviceandappmanagementroleassignment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="89fa0-124">In the request body, supply a JSON representation for the [deviceAndAppManagementRoleAssignment](../resources/intune_rbac_deviceandappmanagementroleassignment.md) object.</span></span>

<span data-ttu-id="89fa0-125">下表显示创建 [deviceAndAppManagementRoleAssignment](../resources/intune_rbac_deviceandappmanagementroleassignment.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="89fa0-125">The following table shows the properties that are required when you create the [deviceAndAppManagementRoleAssignment](../resources/intune_rbac_deviceandappmanagementroleassignment.md).</span></span>

|<span data-ttu-id="89fa0-126">属性</span><span class="sxs-lookup"><span data-stu-id="89fa0-126">Property</span></span>|<span data-ttu-id="89fa0-127">类型</span><span class="sxs-lookup"><span data-stu-id="89fa0-127">Type</span></span>|<span data-ttu-id="89fa0-128">说明</span><span class="sxs-lookup"><span data-stu-id="89fa0-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="89fa0-129">ID</span><span class="sxs-lookup"><span data-stu-id="89fa0-129">id</span></span>|<span data-ttu-id="89fa0-130">字符串</span><span class="sxs-lookup"><span data-stu-id="89fa0-130">String</span></span>|<span data-ttu-id="89fa0-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="89fa0-131">Key of the entity.</span></span> <span data-ttu-id="89fa0-132">此为只读，且自动生成。</span><span class="sxs-lookup"><span data-stu-id="89fa0-132">This is read-only and automatically generated.</span></span> <span data-ttu-id="89fa0-133">继承自 [roleAssignment](../resources/intune_rbac_roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="89fa0-133">Inherited from [roleAssignment](../resources/intune_rbac_roleassignment.md)</span></span>|
|<span data-ttu-id="89fa0-134">displayName</span><span class="sxs-lookup"><span data-stu-id="89fa0-134">displayName</span></span>|<span data-ttu-id="89fa0-135">字符串</span><span class="sxs-lookup"><span data-stu-id="89fa0-135">String</span></span>|<span data-ttu-id="89fa0-136">角色分配的显示或友好名称。</span><span class="sxs-lookup"><span data-stu-id="89fa0-136">The display or friendly name of the role Assignment.</span></span> <span data-ttu-id="89fa0-137">继承自 [roleAssignment](../resources/intune_rbac_roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="89fa0-137">Inherited from [roleAssignment](../resources/intune_rbac_roleassignment.md)</span></span>|
|<span data-ttu-id="89fa0-138">说明</span><span class="sxs-lookup"><span data-stu-id="89fa0-138">description</span></span>|<span data-ttu-id="89fa0-139">字符串</span><span class="sxs-lookup"><span data-stu-id="89fa0-139">String</span></span>|<span data-ttu-id="89fa0-140">角色分配的说明。</span><span class="sxs-lookup"><span data-stu-id="89fa0-140">Description of the Role Assignment.</span></span> <span data-ttu-id="89fa0-141">继承自 [roleAssignment](../resources/intune_rbac_roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="89fa0-141">Inherited from [roleAssignment](../resources/intune_rbac_roleassignment.md)</span></span>|
|<span data-ttu-id="89fa0-142">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="89fa0-142">resourceScopes</span></span>|<span data-ttu-id="89fa0-143">String 集合</span><span class="sxs-lookup"><span data-stu-id="89fa0-143">String collection</span></span>|<span data-ttu-id="89fa0-144">角色作用域成员安全组的 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="89fa0-144">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="89fa0-145">这些是 Azure Active Directory 中的 ID。</span><span class="sxs-lookup"><span data-stu-id="89fa0-145">These are IDs from Azure Active Directory.</span></span> <span data-ttu-id="89fa0-146">继承自 [roleAssignment](../resources/intune_rbac_roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="89fa0-146">Inherited from [roleAssignment](../resources/intune_rbac_roleassignment.md)</span></span>|
|<span data-ttu-id="89fa0-147">成员</span><span class="sxs-lookup"><span data-stu-id="89fa0-147">members</span></span>|<span data-ttu-id="89fa0-148">String 集合</span><span class="sxs-lookup"><span data-stu-id="89fa0-148">String collection</span></span>|<span data-ttu-id="89fa0-149">角色成员安全组的 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="89fa0-149">The list of ids of role member security groups.</span></span> <span data-ttu-id="89fa0-150">这些是 Azure Active Directory 中的 ID。</span><span class="sxs-lookup"><span data-stu-id="89fa0-150">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="89fa0-151">响应</span><span class="sxs-lookup"><span data-stu-id="89fa0-151">Response</span></span>
<span data-ttu-id="89fa0-152">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [deviceAndAppManagementRoleAssignment](../resources/intune_rbac_deviceandappmanagementroleassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="89fa0-152">If successful, this method returns a `200 OK` response code and an updated [deviceAndAppManagementRoleAssignment](../resources/intune_rbac_deviceandappmanagementroleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="89fa0-153">示例</span><span class="sxs-lookup"><span data-stu-id="89fa0-153">Example</span></span>
### <a name="request"></a><span data-ttu-id="89fa0-154">请求</span><span class="sxs-lookup"><span data-stu-id="89fa0-154">Request</span></span>
<span data-ttu-id="89fa0-155">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="89fa0-155">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/roleAssignments/{deviceAndAppManagementRoleAssignmentId}
Content-type: application/json
Content-length: 183

{
  "displayName": "Display Name value",
  "description": "Description value",
  "resourceScopes": [
    "Resource Scopes value"
  ],
  "members": [
    "Members value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="89fa0-156">响应</span><span class="sxs-lookup"><span data-stu-id="89fa0-156">Response</span></span>
<span data-ttu-id="89fa0-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="89fa0-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 307

{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleAssignment",
  "id": "a12e8ebb-8ebb-a12e-bb8e-2ea1bb8e2ea1",
  "displayName": "Display Name value",
  "description": "Description value",
  "resourceScopes": [
    "Resource Scopes value"
  ],
  "members": [
    "Members value"
  ]
}
```









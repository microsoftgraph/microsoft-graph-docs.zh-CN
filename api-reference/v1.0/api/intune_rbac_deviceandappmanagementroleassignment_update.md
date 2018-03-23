# <a name="update-deviceandappmanagementroleassignment"></a><span data-ttu-id="e6aeb-101">更新 deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="e6aeb-101">Update deviceAndAppManagementRoleAssignment</span></span>

> <span data-ttu-id="e6aeb-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="e6aeb-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e6aeb-103">更新 [deviceAndAppManagementRoleAssignment](../resources/intune_rbac_deviceandappmanagementroleassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="e6aeb-103">Update the properties of a [calendar](../resources/intune_rbac_deviceandappmanagementroleassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e6aeb-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="e6aeb-104">Prerequisites</span></span>
<span data-ttu-id="e6aeb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="e6aeb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e6aeb-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="e6aeb-107">Permission type</span></span>|<span data-ttu-id="e6aeb-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e6aeb-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e6aeb-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e6aeb-109">Delegated (work or school account)</span></span>|<span data-ttu-id="e6aeb-110">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e6aeb-110">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="e6aeb-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e6aeb-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e6aeb-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="e6aeb-112">Not supported.</span></span>|
|<span data-ttu-id="e6aeb-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="e6aeb-113">Application</span></span>|<span data-ttu-id="e6aeb-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="e6aeb-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e6aeb-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e6aeb-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleAssignments/{deviceAndAppManagementRoleAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="e6aeb-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="e6aeb-116">Request headers</span></span>
|<span data-ttu-id="e6aeb-117">标头</span><span class="sxs-lookup"><span data-stu-id="e6aeb-117">Header</span></span>|<span data-ttu-id="e6aeb-118">值</span><span class="sxs-lookup"><span data-stu-id="e6aeb-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e6aeb-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="e6aeb-119">Authorization</span></span>|<span data-ttu-id="e6aeb-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e6aeb-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="e6aeb-121">Accept</span><span class="sxs-lookup"><span data-stu-id="e6aeb-121">Accept</span></span>|<span data-ttu-id="e6aeb-122">application/json</span><span class="sxs-lookup"><span data-stu-id="e6aeb-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e6aeb-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="e6aeb-123">Request body</span></span>
<span data-ttu-id="e6aeb-124">在请求正文中，提供 [deviceAndAppManagementRoleAssignment](../resources/intune_rbac_deviceandappmanagementroleassignment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e6aeb-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_rbac_deviceandappmanagementroleassignment.md) object.</span></span>

<span data-ttu-id="e6aeb-125">下表显示创建 [deviceAndAppManagementRoleAssignment](../resources/intune_rbac_deviceandappmanagementroleassignment.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="e6aeb-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="e6aeb-126">属性</span><span class="sxs-lookup"><span data-stu-id="e6aeb-126">Property</span></span>|<span data-ttu-id="e6aeb-127">类型</span><span class="sxs-lookup"><span data-stu-id="e6aeb-127">Type</span></span>|<span data-ttu-id="e6aeb-128">说明</span><span class="sxs-lookup"><span data-stu-id="e6aeb-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e6aeb-129">id</span><span class="sxs-lookup"><span data-stu-id="e6aeb-129">id</span></span>|<span data-ttu-id="e6aeb-130">String</span><span class="sxs-lookup"><span data-stu-id="e6aeb-130">String</span></span>|<span data-ttu-id="e6aeb-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="e6aeb-131">Key of the setting.</span></span> <span data-ttu-id="e6aeb-132">此为只读，且自动生成。</span><span class="sxs-lookup"><span data-stu-id="e6aeb-132">This is read-only and automatically generated.</span></span> <span data-ttu-id="e6aeb-133">继承自 [roleAssignment](../resources/intune_rbac_roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="e6aeb-133">Inherited from [roleAssignment](../resources/intune_rbac_roleassignment.md)</span></span>|
|<span data-ttu-id="e6aeb-134">displayName</span><span class="sxs-lookup"><span data-stu-id="e6aeb-134">displayName</span></span>|<span data-ttu-id="e6aeb-135">String</span><span class="sxs-lookup"><span data-stu-id="e6aeb-135">String</span></span>|<span data-ttu-id="e6aeb-136">角色分配的显示或友好名称。</span><span class="sxs-lookup"><span data-stu-id="e6aeb-136">The display or friendly name of the role Assignment.</span></span> <span data-ttu-id="e6aeb-137">继承自 [roleAssignment](../resources/intune_rbac_roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="e6aeb-137">Inherited from [roleAssignment](../resources/intune_rbac_roleassignment.md)</span></span>|
|<span data-ttu-id="e6aeb-138">description</span><span class="sxs-lookup"><span data-stu-id="e6aeb-138">description</span></span>|<span data-ttu-id="e6aeb-139">String</span><span class="sxs-lookup"><span data-stu-id="e6aeb-139">String</span></span>|<span data-ttu-id="e6aeb-140">角色分配的说明。</span><span class="sxs-lookup"><span data-stu-id="e6aeb-140">Description of the Role Assignment.</span></span> <span data-ttu-id="e6aeb-141">继承自 [roleAssignment](../resources/intune_rbac_roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="e6aeb-141">Inherited from [roleAssignment](../resources/intune_rbac_roleassignment.md)</span></span>|
|<span data-ttu-id="e6aeb-142">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="e6aeb-142">resourceScopes</span></span>|<span data-ttu-id="e6aeb-143">String 集合</span><span class="sxs-lookup"><span data-stu-id="e6aeb-143">String collection</span></span>|<span data-ttu-id="e6aeb-144">角色作用域成员安全组的 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="e6aeb-144">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="e6aeb-145">这些是 Azure Active Directory 中的 ID。</span><span class="sxs-lookup"><span data-stu-id="e6aeb-145">These are IDs from Azure Active Directory.</span></span> <span data-ttu-id="e6aeb-146">继承自 [roleAssignment](../resources/intune_rbac_roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="e6aeb-146">Inherited from [roleAssignment](../resources/intune_rbac_roleassignment.md)</span></span>|
|<span data-ttu-id="e6aeb-147">members</span><span class="sxs-lookup"><span data-stu-id="e6aeb-147">members</span></span>|<span data-ttu-id="e6aeb-148">String 集合</span><span class="sxs-lookup"><span data-stu-id="e6aeb-148">String collection</span></span>|<span data-ttu-id="e6aeb-149">角色成员安全组的 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="e6aeb-149">The list of ids of role member security groups.</span></span> <span data-ttu-id="e6aeb-150">这些是 Azure Active Directory 中的 ID。</span><span class="sxs-lookup"><span data-stu-id="e6aeb-150">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="e6aeb-151">响应</span><span class="sxs-lookup"><span data-stu-id="e6aeb-151">Response</span></span>
<span data-ttu-id="e6aeb-152">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [deviceAndAppManagementRoleAssignment](../resources/intune_rbac_deviceandappmanagementroleassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e6aeb-152">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_rbac_deviceandappmanagementroleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e6aeb-153">示例</span><span class="sxs-lookup"><span data-stu-id="e6aeb-153">Example</span></span>
### <a name="request"></a><span data-ttu-id="e6aeb-154">请求</span><span class="sxs-lookup"><span data-stu-id="e6aeb-154">Request</span></span>
<span data-ttu-id="e6aeb-155">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e6aeb-155">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e6aeb-156">响应</span><span class="sxs-lookup"><span data-stu-id="e6aeb-156">Response</span></span>
<span data-ttu-id="e6aeb-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e6aeb-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




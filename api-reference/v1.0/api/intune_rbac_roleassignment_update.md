# <a name="update-roleassignment"></a><span data-ttu-id="20d1d-101">更新 roleAssignment</span><span class="sxs-lookup"><span data-stu-id="20d1d-101">Update roleAssignment</span></span>

> <span data-ttu-id="20d1d-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="20d1d-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="20d1d-103">更新 [roleAssignment](../resources/intune_rbac_roleassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="20d1d-103">Update the properties of a [roleAssignment](../resources/intune_rbac_roleassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="20d1d-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="20d1d-104">Prerequisites</span></span>
<span data-ttu-id="20d1d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="20d1d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="20d1d-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="20d1d-107">Permission type</span></span>|<span data-ttu-id="20d1d-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="20d1d-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="20d1d-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="20d1d-109">Delegated (work or school account)</span></span>|<span data-ttu-id="20d1d-110">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="20d1d-110">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="20d1d-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="20d1d-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="20d1d-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="20d1d-112">Not supported.</span></span>|
|<span data-ttu-id="20d1d-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="20d1d-113">Application</span></span>|<span data-ttu-id="20d1d-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="20d1d-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="20d1d-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="20d1d-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="20d1d-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="20d1d-116">Request headers</span></span>
|<span data-ttu-id="20d1d-117">标头</span><span class="sxs-lookup"><span data-stu-id="20d1d-117">Header</span></span>|<span data-ttu-id="20d1d-118">值</span><span class="sxs-lookup"><span data-stu-id="20d1d-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="20d1d-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="20d1d-119">Authorization</span></span>|<span data-ttu-id="20d1d-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="20d1d-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="20d1d-121">Accept</span><span class="sxs-lookup"><span data-stu-id="20d1d-121">Accept</span></span>|<span data-ttu-id="20d1d-122">application/json</span><span class="sxs-lookup"><span data-stu-id="20d1d-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="20d1d-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="20d1d-123">Request body</span></span>
<span data-ttu-id="20d1d-124">在请求正文中，提供 [roleAssignment](../resources/intune_rbac_roleassignment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="20d1d-124">In the request body, supply a JSON representation for the [roleAssignment](../resources/intune_rbac_roleassignment.md) object.</span></span>

<span data-ttu-id="20d1d-125">下表显示创建 [roleAssignment](../resources/intune_rbac_roleassignment.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="20d1d-125">The following table shows the properties that are required when you create the [roleAssignment](../resources/intune_rbac_roleassignment.md).</span></span>

|<span data-ttu-id="20d1d-126">属性</span><span class="sxs-lookup"><span data-stu-id="20d1d-126">Property</span></span>|<span data-ttu-id="20d1d-127">类型</span><span class="sxs-lookup"><span data-stu-id="20d1d-127">Type</span></span>|<span data-ttu-id="20d1d-128">说明</span><span class="sxs-lookup"><span data-stu-id="20d1d-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="20d1d-129">id</span><span class="sxs-lookup"><span data-stu-id="20d1d-129">id</span></span>|<span data-ttu-id="20d1d-130">String</span><span class="sxs-lookup"><span data-stu-id="20d1d-130">String</span></span>|<span data-ttu-id="20d1d-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="20d1d-131">Key of the entity.</span></span> <span data-ttu-id="20d1d-132">此为只读，且自动生成。</span><span class="sxs-lookup"><span data-stu-id="20d1d-132">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="20d1d-133">displayName</span><span class="sxs-lookup"><span data-stu-id="20d1d-133">displayName</span></span>|<span data-ttu-id="20d1d-134">String</span><span class="sxs-lookup"><span data-stu-id="20d1d-134">String</span></span>|<span data-ttu-id="20d1d-135">角色分配的显示或友好名称。</span><span class="sxs-lookup"><span data-stu-id="20d1d-135">The display or friendly name of the role Assignment.</span></span>|
|<span data-ttu-id="20d1d-136">description</span><span class="sxs-lookup"><span data-stu-id="20d1d-136">description</span></span>|<span data-ttu-id="20d1d-137">String</span><span class="sxs-lookup"><span data-stu-id="20d1d-137">String</span></span>|<span data-ttu-id="20d1d-138">角色分配的说明。</span><span class="sxs-lookup"><span data-stu-id="20d1d-138">Description of the Role Assignment.</span></span>|
|<span data-ttu-id="20d1d-139">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="20d1d-139">resourceScopes</span></span>|<span data-ttu-id="20d1d-140">String 集合</span><span class="sxs-lookup"><span data-stu-id="20d1d-140">String collection</span></span>|<span data-ttu-id="20d1d-141">角色作用域成员安全组的 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="20d1d-141">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="20d1d-142">这些是 Azure Active Directory 中的 ID。</span><span class="sxs-lookup"><span data-stu-id="20d1d-142">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="20d1d-143">响应</span><span class="sxs-lookup"><span data-stu-id="20d1d-143">Response</span></span>
<span data-ttu-id="20d1d-144">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [roleAssignment](../resources/intune_rbac_roleassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="20d1d-144">If successful, this method returns a `200 OK` response code and an updated [roleAssignment](../resources/intune_rbac_roleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="20d1d-145">示例</span><span class="sxs-lookup"><span data-stu-id="20d1d-145">Example</span></span>
### <a name="request"></a><span data-ttu-id="20d1d-146">请求</span><span class="sxs-lookup"><span data-stu-id="20d1d-146">Request</span></span>
<span data-ttu-id="20d1d-147">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="20d1d-147">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}
Content-type: application/json
Content-length: 193

{
  "@odata.type": "#microsoft.graph.roleAssignment",
  "displayName": "Display Name value",
  "description": "Description value",
  "resourceScopes": [
    "Resource Scopes value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="20d1d-148">响应</span><span class="sxs-lookup"><span data-stu-id="20d1d-148">Response</span></span>
<span data-ttu-id="20d1d-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="20d1d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 242

{
  "@odata.type": "#microsoft.graph.roleAssignment",
  "id": "b3234d24-4d24-b323-244d-23b3244d23b3",
  "displayName": "Display Name value",
  "description": "Description value",
  "resourceScopes": [
    "Resource Scopes value"
  ]
}
```




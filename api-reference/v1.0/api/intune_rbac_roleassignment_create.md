# <a name="create-roleassignment"></a><span data-ttu-id="05f7b-101">创建 roleAssignment</span><span class="sxs-lookup"><span data-stu-id="05f7b-101">Create roleAssignment</span></span>

> <span data-ttu-id="05f7b-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="05f7b-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="05f7b-103">创建新的 [roleAssignment](../resources/intune_rbac_roleassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="05f7b-103">Create a new [plannerBucket](../resources/intune_rbac_roleassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="05f7b-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="05f7b-104">Prerequisites</span></span>
<span data-ttu-id="05f7b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="05f7b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="05f7b-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="05f7b-107">Permission type</span></span>|<span data-ttu-id="05f7b-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="05f7b-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="05f7b-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="05f7b-109">Delegated (work or school account)</span></span>|<span data-ttu-id="05f7b-110">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05f7b-110">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="05f7b-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="05f7b-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="05f7b-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="05f7b-112">Not supported.</span></span>|
|<span data-ttu-id="05f7b-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="05f7b-113">Application</span></span>|<span data-ttu-id="05f7b-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="05f7b-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="05f7b-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="05f7b-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="05f7b-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="05f7b-116">Request headers</span></span>
|<span data-ttu-id="05f7b-117">标头</span><span class="sxs-lookup"><span data-stu-id="05f7b-117">Header</span></span>|<span data-ttu-id="05f7b-118">值</span><span class="sxs-lookup"><span data-stu-id="05f7b-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="05f7b-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="05f7b-119">Authorization</span></span>|<span data-ttu-id="05f7b-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="05f7b-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="05f7b-121">Accept</span><span class="sxs-lookup"><span data-stu-id="05f7b-121">Accept</span></span>|<span data-ttu-id="05f7b-122">application/json</span><span class="sxs-lookup"><span data-stu-id="05f7b-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="05f7b-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="05f7b-123">Request body</span></span>
<span data-ttu-id="05f7b-124">在请求正文中，提供 roleAssignment 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="05f7b-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="05f7b-125">下表显示创建 roleAssignment 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="05f7b-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="05f7b-126">属性</span><span class="sxs-lookup"><span data-stu-id="05f7b-126">Property</span></span>|<span data-ttu-id="05f7b-127">类型</span><span class="sxs-lookup"><span data-stu-id="05f7b-127">Type</span></span>|<span data-ttu-id="05f7b-128">说明</span><span class="sxs-lookup"><span data-stu-id="05f7b-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="05f7b-129">id</span><span class="sxs-lookup"><span data-stu-id="05f7b-129">id</span></span>|<span data-ttu-id="05f7b-130">String</span><span class="sxs-lookup"><span data-stu-id="05f7b-130">String</span></span>|<span data-ttu-id="05f7b-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="05f7b-131">Key of the setting.</span></span> <span data-ttu-id="05f7b-132">此为只读，且自动生成。</span><span class="sxs-lookup"><span data-stu-id="05f7b-132">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="05f7b-133">displayName</span><span class="sxs-lookup"><span data-stu-id="05f7b-133">displayName</span></span>|<span data-ttu-id="05f7b-134">String</span><span class="sxs-lookup"><span data-stu-id="05f7b-134">String</span></span>|<span data-ttu-id="05f7b-135">角色分配的显示或友好名称。</span><span class="sxs-lookup"><span data-stu-id="05f7b-135">The display or friendly name of the role Assignment.</span></span>|
|<span data-ttu-id="05f7b-136">description</span><span class="sxs-lookup"><span data-stu-id="05f7b-136">description</span></span>|<span data-ttu-id="05f7b-137">String</span><span class="sxs-lookup"><span data-stu-id="05f7b-137">String</span></span>|<span data-ttu-id="05f7b-138">角色分配的说明。</span><span class="sxs-lookup"><span data-stu-id="05f7b-138">Description of the Role Assignment.</span></span>|
|<span data-ttu-id="05f7b-139">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="05f7b-139">resourceScopes</span></span>|<span data-ttu-id="05f7b-140">String 集合</span><span class="sxs-lookup"><span data-stu-id="05f7b-140">String collection</span></span>|<span data-ttu-id="05f7b-141">角色作用域成员安全组的 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="05f7b-141">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="05f7b-142">这些是 Azure Active Directory 中的 ID。</span><span class="sxs-lookup"><span data-stu-id="05f7b-142">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="05f7b-143">响应</span><span class="sxs-lookup"><span data-stu-id="05f7b-143">Response</span></span>
<span data-ttu-id="05f7b-144">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [roleAssignment](../resources/intune_rbac_roleassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="05f7b-144">If successful, this method returns a `201 Created` response code and a [directoryObject](../resources/intune_rbac_roleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="05f7b-145">示例</span><span class="sxs-lookup"><span data-stu-id="05f7b-145">Example</span></span>
### <a name="request"></a><span data-ttu-id="05f7b-146">请求</span><span class="sxs-lookup"><span data-stu-id="05f7b-146">Request</span></span>
<span data-ttu-id="05f7b-147">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="05f7b-147">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments
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

### <a name="response"></a><span data-ttu-id="05f7b-148">响应</span><span class="sxs-lookup"><span data-stu-id="05f7b-148">Response</span></span>
<span data-ttu-id="05f7b-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="05f7b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




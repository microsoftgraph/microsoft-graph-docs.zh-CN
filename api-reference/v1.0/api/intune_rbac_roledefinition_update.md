# <a name="update-roledefinition"></a><span data-ttu-id="63538-101">更新 roleDefinition</span><span class="sxs-lookup"><span data-stu-id="63538-101">Update roleDefinition</span></span>

> <span data-ttu-id="63538-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="63538-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="63538-103">更新 [roleDefinition](../resources/intune_rbac_roledefinition.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="63538-103">Update the properties of a [roleDefinition](../resources/intune_rbac_roledefinition.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="63538-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="63538-104">Prerequisites</span></span>
<span data-ttu-id="63538-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="63538-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="63538-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="63538-107">Permission type</span></span>|<span data-ttu-id="63538-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="63538-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="63538-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="63538-109">Delegated (work or school account)</span></span>|<span data-ttu-id="63538-110">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63538-110">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="63538-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="63538-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="63538-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="63538-112">Not supported.</span></span>|
|<span data-ttu-id="63538-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="63538-113">Application</span></span>|<span data-ttu-id="63538-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="63538-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="63538-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="63538-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/roleDefinition
```

## <a name="request-headers"></a><span data-ttu-id="63538-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="63538-116">Request headers</span></span>
|<span data-ttu-id="63538-117">标头</span><span class="sxs-lookup"><span data-stu-id="63538-117">Header</span></span>|<span data-ttu-id="63538-118">值</span><span class="sxs-lookup"><span data-stu-id="63538-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="63538-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="63538-119">Authorization</span></span>|<span data-ttu-id="63538-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="63538-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="63538-121">Accept</span><span class="sxs-lookup"><span data-stu-id="63538-121">Accept</span></span>|<span data-ttu-id="63538-122">application/json</span><span class="sxs-lookup"><span data-stu-id="63538-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="63538-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="63538-123">Request body</span></span>
<span data-ttu-id="63538-124">在请求正文中，提供 [roleDefinition](../resources/intune_rbac_roledefinition.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="63538-124">In the request body, supply a JSON representation for the [roleDefinition](../resources/intune_rbac_roledefinition.md) object.</span></span>

<span data-ttu-id="63538-125">下表显示创建 [roleDefinition](../resources/intune_rbac_roledefinition.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="63538-125">The following table shows the properties that are required when you create the [roleDefinition](../resources/intune_rbac_roledefinition.md).</span></span>

|<span data-ttu-id="63538-126">属性</span><span class="sxs-lookup"><span data-stu-id="63538-126">Property</span></span>|<span data-ttu-id="63538-127">类型</span><span class="sxs-lookup"><span data-stu-id="63538-127">Type</span></span>|<span data-ttu-id="63538-128">说明</span><span class="sxs-lookup"><span data-stu-id="63538-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="63538-129">id</span><span class="sxs-lookup"><span data-stu-id="63538-129">id</span></span>|<span data-ttu-id="63538-130">String</span><span class="sxs-lookup"><span data-stu-id="63538-130">String</span></span>|<span data-ttu-id="63538-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="63538-131">Key of the entity.</span></span> <span data-ttu-id="63538-132">此为只读，且自动生成。</span><span class="sxs-lookup"><span data-stu-id="63538-132">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="63538-133">displayName</span><span class="sxs-lookup"><span data-stu-id="63538-133">displayName</span></span>|<span data-ttu-id="63538-134">String</span><span class="sxs-lookup"><span data-stu-id="63538-134">String</span></span>|<span data-ttu-id="63538-135">角色定义的显示名称。</span><span class="sxs-lookup"><span data-stu-id="63538-135">Display Name of the Role definition.</span></span>|
|<span data-ttu-id="63538-136">description</span><span class="sxs-lookup"><span data-stu-id="63538-136">description</span></span>|<span data-ttu-id="63538-137">String</span><span class="sxs-lookup"><span data-stu-id="63538-137">String</span></span>|<span data-ttu-id="63538-138">角色定义的说明。</span><span class="sxs-lookup"><span data-stu-id="63538-138">Description of the Role definition.</span></span>|
|<span data-ttu-id="63538-139">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="63538-139">rolePermissions</span></span>|<span data-ttu-id="63538-140">[rolePermission](../resources/intune_rbac_rolepermission.md) 集合</span><span class="sxs-lookup"><span data-stu-id="63538-140">[rolePermission](../resources/intune_rbac_rolepermission.md) collection</span></span>|<span data-ttu-id="63538-141">允许此角色执行的角色权限列表。</span><span class="sxs-lookup"><span data-stu-id="63538-141">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="63538-142">它们必须与定义为 rolePermission 一部分的 actionName 匹配。</span><span class="sxs-lookup"><span data-stu-id="63538-142">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="63538-143">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="63538-143">isBuiltIn</span></span>|<span data-ttu-id="63538-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="63538-144">Boolean</span></span>|<span data-ttu-id="63538-145">角色类型。</span><span class="sxs-lookup"><span data-stu-id="63538-145">Type of Role.</span></span> <span data-ttu-id="63538-146">如果是内置角色，则设置为 True；如果是自定义角色定义，则设置为 False。</span><span class="sxs-lookup"><span data-stu-id="63538-146">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|



## <a name="response"></a><span data-ttu-id="63538-147">响应</span><span class="sxs-lookup"><span data-stu-id="63538-147">Response</span></span>
<span data-ttu-id="63538-148">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [roleDefinition](../resources/intune_rbac_roledefinition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="63538-148">If successful, this method returns a `200 OK` response code and an updated [roleDefinition](../resources/intune_rbac_roledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="63538-149">示例</span><span class="sxs-lookup"><span data-stu-id="63538-149">Example</span></span>
### <a name="request"></a><span data-ttu-id="63538-150">请求</span><span class="sxs-lookup"><span data-stu-id="63538-150">Request</span></span>
<span data-ttu-id="63538-151">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="63538-151">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/roleDefinitions/{roleDefinitionId}
Content-type: application/json
Content-length: 580

{
  "@odata.type": "#microsoft.graph.roleDefinition",
  "displayName": "Display Name value",
  "description": "Description value",
  "rolePermissions": [
    {
      "@odata.type": "microsoft.graph.rolePermission",
      "resourceActions": [
        {
          "@odata.type": "microsoft.graph.resourceAction",
          "allowedResourceActions": [
            "Allowed Resource Actions value"
          ],
          "notAllowedResourceActions": [
            "Not Allowed Resource Actions value"
          ]
        }
      ]
    }
  ],
  "isBuiltIn": true
}
```

### <a name="response"></a><span data-ttu-id="63538-152">响应</span><span class="sxs-lookup"><span data-stu-id="63538-152">Response</span></span>
<span data-ttu-id="63538-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="63538-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 629

{
  "@odata.type": "#microsoft.graph.roleDefinition",
  "id": "70fdcd08-cd08-70fd-08cd-fd7008cdfd70",
  "displayName": "Display Name value",
  "description": "Description value",
  "rolePermissions": [
    {
      "@odata.type": "microsoft.graph.rolePermission",
      "resourceActions": [
        {
          "@odata.type": "microsoft.graph.resourceAction",
          "allowedResourceActions": [
            "Allowed Resource Actions value"
          ],
          "notAllowedResourceActions": [
            "Not Allowed Resource Actions value"
          ]
        }
      ]
    }
  ],
  "isBuiltIn": true
}
```




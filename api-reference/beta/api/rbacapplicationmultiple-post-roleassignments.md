---
title: 创建 unifiedRoleAssignmentMultiple
description: 创建新的 unifiedRoleAssignmentMultiple 对象。
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: bc09a9c514ab504d81f65983791ae947db313267
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2021
ms.locfileid: "52868961"
---
# <a name="create-unifiedroleassignmentmultiple"></a><span data-ttu-id="c6f48-103">创建 unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="c6f48-103">Create unifiedRoleAssignmentMultiple</span></span>

<span data-ttu-id="c6f48-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c6f48-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c6f48-105">为 RBAC 提供程序创建新的 [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c6f48-105">Create a new [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) object for an RBAC provider.</span></span> 

<span data-ttu-id="c6f48-106">目前支持以下 RBAC 提供程序：</span><span class="sxs-lookup"><span data-stu-id="c6f48-106">The following RBAC providers are currently supported:</span></span>
- <span data-ttu-id="c6f48-107">云电脑</span><span class="sxs-lookup"><span data-stu-id="c6f48-107">cloud PC</span></span> 
- <span data-ttu-id="c6f48-108">Intune (设备) </span><span class="sxs-lookup"><span data-stu-id="c6f48-108">device management (Intune)</span></span>

<span data-ttu-id="c6f48-109">For other Microsoft 365 applications (like Azure AD) ， use [unifiedRoleAssignment](../resources/unifiedroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="c6f48-109">For other Microsoft 365 applications (like Azure AD), use [unifiedRoleAssignment](../resources/unifiedroleassignment.md).</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="c6f48-110">权限</span><span class="sxs-lookup"><span data-stu-id="c6f48-110">Permissions</span></span>

<span data-ttu-id="c6f48-111">根据 RBAC 提供程序以及 (或应用程序) 的权限类型，从下表中选择调用此 API 所需的最低特权权限。</span><span class="sxs-lookup"><span data-stu-id="c6f48-111">Depending on the RBAC provider and the permission type (delegated or application) that is needed, choose from the following table the least privileged permission required to call this API.</span></span> <span data-ttu-id="c6f48-112">若要了解详细信息，包括在选择更多特权之前的[注意事项](/graph/auth/auth-concepts#best-practices-for-requesting-permissions)，请在“[权限](/graph/permissions-reference)”中搜索以下权限。</span><span class="sxs-lookup"><span data-stu-id="c6f48-112">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in [Permissions](/graph/permissions-reference).</span></span> 

|<span data-ttu-id="c6f48-113">支持的提供程序</span><span class="sxs-lookup"><span data-stu-id="c6f48-113">Supported provider</span></span>      | <span data-ttu-id="c6f48-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c6f48-114">Delegated (work or school account)</span></span>  | <span data-ttu-id="c6f48-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c6f48-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c6f48-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="c6f48-116">Application</span></span> |
|:-----------------------|:------------------------------------|:---------------------------------------|:------------|
| <span data-ttu-id="c6f48-117">Cloud PC</span><span class="sxs-lookup"><span data-stu-id="c6f48-117">Cloud PC</span></span> | <span data-ttu-id="c6f48-118">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c6f48-118">CloudPC.ReadWrite.All</span></span> | <span data-ttu-id="c6f48-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="c6f48-119">Not supported.</span></span> | <span data-ttu-id="c6f48-120">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c6f48-120">CloudPC.ReadWrite.All</span></span> |
| <span data-ttu-id="c6f48-121">Intune</span><span class="sxs-lookup"><span data-stu-id="c6f48-121">Intune</span></span> | <span data-ttu-id="c6f48-122">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c6f48-122">DeviceManagementRBAC.ReadWrite.All</span></span> | <span data-ttu-id="c6f48-123">不支持。</span><span class="sxs-lookup"><span data-stu-id="c6f48-123">Not supported.</span></span>| <span data-ttu-id="c6f48-124">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c6f48-124">DeviceManagementRBAC.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c6f48-125">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c6f48-125">HTTP request</span></span>

<span data-ttu-id="c6f48-126">若要为角色分配创建云电脑提供商：</span><span class="sxs-lookup"><span data-stu-id="c6f48-126">To create role assignment for a cloud PC provider:</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /roleManagement/cloudPC/roleAssignments
```

<span data-ttu-id="c6f48-127">若要为角色分配创建一个 Intune 提供程序：</span><span class="sxs-lookup"><span data-stu-id="c6f48-127">To create role assignment for an Intune provider:</span></span>
<!-- { "blockType": "ignored" } -->

```http
POST /roleManagement/deviceManagement/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="c6f48-128">请求标头</span><span class="sxs-lookup"><span data-stu-id="c6f48-128">Request headers</span></span>

| <span data-ttu-id="c6f48-129">名称</span><span class="sxs-lookup"><span data-stu-id="c6f48-129">Name</span></span> | <span data-ttu-id="c6f48-130">说明</span><span class="sxs-lookup"><span data-stu-id="c6f48-130">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="c6f48-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="c6f48-131">Authorization</span></span> | <span data-ttu-id="c6f48-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c6f48-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c6f48-134">Content-type</span><span class="sxs-lookup"><span data-stu-id="c6f48-134">Content-type</span></span> | <span data-ttu-id="c6f48-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="c6f48-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c6f48-137">请求正文</span><span class="sxs-lookup"><span data-stu-id="c6f48-137">Request body</span></span>

<span data-ttu-id="c6f48-138">在请求正文中，提供 [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c6f48-138">In the request body, supply a JSON representation of [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) object.</span></span> <span data-ttu-id="c6f48-139">请求必须具有在 Azure AD 中定义的作用域（如 ）或特定于应用程序的范围（ `directoryScopeIds` 如 `appScopeId` ）。</span><span class="sxs-lookup"><span data-stu-id="c6f48-139">The request must have either a scope defined in Azure AD, such as `directoryScopeIds`, or an application-specific scope, such as `appScopeId`.</span></span> <span data-ttu-id="c6f48-140">Azure AD 范围的示例包括租户 (/") 、管理单元或应用程序。</span><span class="sxs-lookup"><span data-stu-id="c6f48-140">Examples of Azure AD scope are tenant ("/"), administrative units, or applications.</span></span> 

## <a name="response"></a><span data-ttu-id="c6f48-141">响应</span><span class="sxs-lookup"><span data-stu-id="c6f48-141">Response</span></span>

<span data-ttu-id="c6f48-142">如果成功，此方法在响应正文中返回 响应代码和新的 `201 Created` [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c6f48-142">If successful, this method returns a `201 Created` response code and a new [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c6f48-143">示例</span><span class="sxs-lookup"><span data-stu-id="c6f48-143">Examples</span></span>

### <a name="example-1-create-a-role-assignment-in-intune-over-two-scope-groups-which-are-azure-ad-objects"></a><span data-ttu-id="c6f48-144">示例 1：在 Intune 角色分配两个作用域组上创建一个 (组，即 Azure AD 对象) </span><span class="sxs-lookup"><span data-stu-id="c6f48-144">Example 1: Create a role assignment in Intune over two scope groups (which are Azure AD objects)</span></span>

#### <a name="request"></a><span data-ttu-id="c6f48-145">请求</span><span class="sxs-lookup"><span data-stu-id="c6f48-145">Request</span></span>

<span data-ttu-id="c6f48-146">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c6f48-146">The following is an example of the request.</span></span>
> <span data-ttu-id="c6f48-147">**注意\*\*\*\*：roleDefinitionId** 的 **roleTemplateId 的使用**。</span><span class="sxs-lookup"><span data-stu-id="c6f48-147">**Note:** the use of the **roleTemplateId** for **roleDefinitionId**.</span></span> <span data-ttu-id="c6f48-148">**roleDefinitionId** 可以是服务范围的模板 ID 或特定于目录 **的 roleDefinitionId**。</span><span class="sxs-lookup"><span data-stu-id="c6f48-148">**roleDefinitionId** can be either the service-wide template ID or the directory-specific **roleDefinitionId**.</span></span>


# <a name="http"></a>[<span data-ttu-id="c6f48-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="c6f48-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_unifiedroleassignmentmultiple_from_rbacapplication"
}-->

```http
POST https://graph.microsoft.com/beta/roleManagement/deviceManagement/roleAssignments
Content-type: application/json

{ 
    "@odata.type": "#microsoft.graph.unifiedRoleAssignmentMultiple",
    "displayName": "My test role assignment 1",
    "roleDefinitionId": "c2cf284d-6c41-4e6b-afac-4b80928c9034",
    "principalIds": ["f8ca5a85-489a-49a0-b555-0a6d81e56f0d", "c1518aa9-4da5-4c84-a902-a31404023890"],
    "directoryScopeIds": ["28ca5a85-489a-49a0-b555-0a6d81e56f0d", "8152656a-cf9a-4928-a457-1512d4cae295"],
}
```
# <a name="c"></a>[<span data-ttu-id="c6f48-150">C#</span><span class="sxs-lookup"><span data-stu-id="c6f48-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-unifiedroleassignmentmultiple-from-rbacapplication-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c6f48-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c6f48-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-unifiedroleassignmentmultiple-from-rbacapplication-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c6f48-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c6f48-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-unifiedroleassignmentmultiple-from-rbacapplication-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c6f48-153">Java</span><span class="sxs-lookup"><span data-stu-id="c6f48-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-unifiedroleassignmentmultiple-from-rbacapplication-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c6f48-154">响应</span><span class="sxs-lookup"><span data-stu-id="c6f48-154">Response</span></span>

<span data-ttu-id="c6f48-155">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="c6f48-155">The following is an example of the response.</span></span>
> <span data-ttu-id="c6f48-156">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="c6f48-156">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignmentMultiple"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#roleManagement/deviceManagement/roleAssignments/$entity",
    "@odata.type": "#microsoft.graph.unifiedRoleAssignmentMultiple",
    "id": "28ca5a85-489a-49a0-b555-0a6d81e56f0d",
    "roleDefinitionId": "c2cf284d-6c41-4e6b-afac-4b80928c9034",
    "principalIds": ["f8ca5a85-489a-49a0-b555-0a6d81e56f0d", "c1518aa9-4da5-4c84-a902-a31404023890"],
    "directoryScopeIds": ["28ca5a85-489a-49a0-b555-0a6d81e56f0d", "8152656a-cf9a-4928-a457-1512d4cae295"]
}
```

### <a name="example-2-create-a-role-assignment-in-intune-at-intune-specific-scope-of-all-devices"></a><span data-ttu-id="c6f48-157">示例 2：在 Intune 角色分配"所有设备"的 Intune 中创建一个应用</span><span class="sxs-lookup"><span data-stu-id="c6f48-157">Example 2: Create a role assignment in Intune at Intune-specific scope of "all Devices"</span></span>

<span data-ttu-id="c6f48-158">使用以下信息创建 Intune 角色分配：</span><span class="sxs-lookup"><span data-stu-id="c6f48-158">Use the following information for creating Intune role assignments:</span></span>
- <span data-ttu-id="c6f48-159">若要允许在所有 Intune 设备上进行分配，请使用 `AllDevices` **appScopeIds 中的值**。</span><span class="sxs-lookup"><span data-stu-id="c6f48-159">To allow assignments over all Intune devices, use the `AllDevices` value in **appScopeIds**.</span></span>
- <span data-ttu-id="c6f48-160">若要允许分配所有 Intune 许可用户，请使用 `AllLicensedUsers` **appScopeIds 中的值**。</span><span class="sxs-lookup"><span data-stu-id="c6f48-160">To allow assignments over all Intune licensed users, use the `AllLicensedUsers` value in **appScopeIds**.</span></span>
- <span data-ttu-id="c6f48-161">若要允许分配所有 Intune 设备和许可用户，请使用 `/` **directoryScopeIds 中的值**。</span><span class="sxs-lookup"><span data-stu-id="c6f48-161">To allow assignments over all Intune devices and licensed users, use the `/` value in **directoryScopeIds**.</span></span>

#### <a name="request"></a><span data-ttu-id="c6f48-162">请求</span><span class="sxs-lookup"><span data-stu-id="c6f48-162">Request</span></span>

<span data-ttu-id="c6f48-163">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c6f48-163">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="c6f48-164">HTTP</span><span class="sxs-lookup"><span data-stu-id="c6f48-164">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_unifiedroleassignmentmultiple_intune_specific"
}-->

```http
POST https://graph.microsoft.com/beta/roleManagement/deviceManagement/roleAssignments
Content-type: application/json

{
    "@odata.type": "#microsoft.graph.unifiedRoleAssignmentMultiple",
    "displayName": "My test role assignment 1",
    "roleDefinitionId": "c2cf284d-6c41-4e6b-afac-4b80928c9034",
    "principalIds": ["f8ca5a85-489a-49a0-b555-0a6d81e56f0d", "c1518aa9-4da5-4c84-a902-a31404023890"],
    "appScopeIds": ["allDevices"]
}
```
# <a name="c"></a>[<span data-ttu-id="c6f48-165">C#</span><span class="sxs-lookup"><span data-stu-id="c6f48-165">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-unifiedroleassignmentmultiple-intune-specific-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c6f48-166">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c6f48-166">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-unifiedroleassignmentmultiple-intune-specific-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c6f48-167">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c6f48-167">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-unifiedroleassignmentmultiple-intune-specific-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c6f48-168">Java</span><span class="sxs-lookup"><span data-stu-id="c6f48-168">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-unifiedroleassignmentmultiple-intune-specific-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c6f48-169">响应</span><span class="sxs-lookup"><span data-stu-id="c6f48-169">Response</span></span>

<span data-ttu-id="c6f48-170">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="c6f48-170">The following is an example of the response.</span></span>
> <span data-ttu-id="c6f48-171">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="c6f48-171">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignmentMultiple"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#roleManagement/deviceManagement/roleAssignments/$entity",
    "@odata.type": "#microsoft.graph.unifiedRoleAssignmentMultiple",
    "id": "28ca5a85-489a-49a0-b555-0a6d81e56f0d",
    "roleDefinitionId": "c2cf284d-6c41-4e6b-afac-4b80928c9034",
    "principalIds": ["f8ca5a85-489a-49a0-b555-0a6d81e56f0d", "c1518aa9-4da5-4c84-a902-a31404023890"],
    "appScopeIds": ["allDevices"]
}
```

### <a name="example-3-create-a-role-assignment-for-a-cloud-pc-provider"></a><span data-ttu-id="c6f48-172">示例 3：角色分配云电脑提供商</span><span class="sxs-lookup"><span data-stu-id="c6f48-172">Example 3: Create a role assignment for a cloud PC provider</span></span>

#### <a name="request"></a><span data-ttu-id="c6f48-173">请求</span><span class="sxs-lookup"><span data-stu-id="c6f48-173">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="c6f48-174">HTTP</span><span class="sxs-lookup"><span data-stu-id="c6f48-174">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_unifiedroleassignmentmultiple_from_rbacapplication_cloudpc"
}-->

```http
POST https://graph.microsoft.com/beta/roleManagement/cloudPC/roleAssignments
Content-type: application/json

{ 
    "@odata.type": "#microsoft.graph.unifiedRoleAssignmentMultiple",
    "displayName": "My test role assignment 1",
    "description": "My role assignment description",
    "roleDefinitionId": "b5c08161-a7af-481c-ace2-a20a69a48fb1",
    "principalIds": ["f8ca5a85-489a-49a0-b555-0a6d81e56f0d", "c1518aa9-4da5-4c84-a902-a31404023890"]
}
```
# <a name="c"></a>[<span data-ttu-id="c6f48-175">C#</span><span class="sxs-lookup"><span data-stu-id="c6f48-175">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-unifiedroleassignmentmultiple-from-rbacapplication-cloudpc-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c6f48-176">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c6f48-176">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-unifiedroleassignmentmultiple-from-rbacapplication-cloudpc-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c6f48-177">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c6f48-177">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-unifiedroleassignmentmultiple-from-rbacapplication-cloudpc-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c6f48-178">Java</span><span class="sxs-lookup"><span data-stu-id="c6f48-178">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-unifiedroleassignmentmultiple-from-rbacapplication-cloudpc-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="c6f48-179">响应</span><span class="sxs-lookup"><span data-stu-id="c6f48-179">Response</span></span>

<span data-ttu-id="c6f48-180">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="c6f48-180">The following is an example of the response.</span></span>
> <span data-ttu-id="c6f48-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="c6f48-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignmentMultiple"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/cloudPC/roleAssignments/$entity",
    "id": "47c88dcd-cc79-4b0c-ba7d-7af2199649c5",
    "displayName": "My role assignment",
    "description": "My role assignment description",
    "roleDefinitionId": "b5c08161-a7af-481c-ace2-a20a69a48fb1",
    "principalIds": [
        "f8ca5a85-489a-49a0-b555-0a6d81e56f0d",
        "c1518aa9-4da5-4c84-a902-a31404023890"
    ],
    "directoryScopeIds": [
        "/"
    ],
    "appScopeIds": []
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create unifiedRoleAssignmentMultiple",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->



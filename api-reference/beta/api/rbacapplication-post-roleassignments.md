---
title: 创建 unifiedRoleAssignment
description: 创建新的 unifiedRoleAssignment 对象。
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 2c1243373539fce47c2eaf9d9b3f351eac00a719
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53442188"
---
# <a name="create-unifiedroleassignment"></a><span data-ttu-id="7b238-103">创建 unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="7b238-103">Create unifiedRoleAssignment</span></span>

<span data-ttu-id="7b238-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7b238-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7b238-105">创建新的 [unifiedRoleAssignment](../resources/unifiedroleassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7b238-105">Create a new [unifiedRoleAssignment](../resources/unifiedroleassignment.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="7b238-106">权限</span><span class="sxs-lookup"><span data-stu-id="7b238-106">Permissions</span></span>

<span data-ttu-id="7b238-107">根据 RBAC 提供程序以及 (或应用程序) 的权限类型，从下表中选择调用此 API 所需的最低特权权限。</span><span class="sxs-lookup"><span data-stu-id="7b238-107">Depending on the RBAC provider and the permission type (delegated or application) that is needed, choose from the following table the least privileged permission required to call this API.</span></span> <span data-ttu-id="7b238-108">若要了解其他信息， [在](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) 特权权限之前要特别小心，在"权限" [中搜索](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7b238-108">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in [Permissions](/graph/permissions-reference).</span></span>

### <a name="for-directory-azure-ad-provider"></a><span data-ttu-id="7b238-109">对于 Azure AD (提供程序) 目录</span><span class="sxs-lookup"><span data-stu-id="7b238-109">For Directory (Azure AD) provider</span></span>

|<span data-ttu-id="7b238-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="7b238-110">Permission type</span></span>      | <span data-ttu-id="7b238-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7b238-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7b238-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7b238-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="7b238-113">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="7b238-113">RoleManagement.ReadWrite.Directory</span></span>   |
|<span data-ttu-id="7b238-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7b238-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7b238-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="7b238-115">Not supported.</span></span>    |
|<span data-ttu-id="7b238-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="7b238-116">Application</span></span> | <span data-ttu-id="7b238-117">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="7b238-117">RoleManagement.ReadWrite.Directory</span></span> |

### <a name="for-entitlement-management-provider"></a><span data-ttu-id="7b238-118">对于权利管理提供程序</span><span class="sxs-lookup"><span data-stu-id="7b238-118">For Entitlement management provider</span></span>

|<span data-ttu-id="7b238-119">权限类型</span><span class="sxs-lookup"><span data-stu-id="7b238-119">Permission type</span></span>      | <span data-ttu-id="7b238-120">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7b238-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7b238-121">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7b238-121">Delegated (work or school account)</span></span> |  <span data-ttu-id="7b238-122">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7b238-122">EntitlementManagement.ReadWrite.All</span></span>   |
|<span data-ttu-id="7b238-123">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7b238-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7b238-124">不支持。</span><span class="sxs-lookup"><span data-stu-id="7b238-124">Not supported.</span></span>    |
|<span data-ttu-id="7b238-125">应用程序</span><span class="sxs-lookup"><span data-stu-id="7b238-125">Application</span></span> | <span data-ttu-id="7b238-126">不支持。</span><span class="sxs-lookup"><span data-stu-id="7b238-126">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7b238-127">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7b238-127">HTTP request</span></span>

<span data-ttu-id="7b238-128">为角色分配创建一个目录提供程序：</span><span class="sxs-lookup"><span data-stu-id="7b238-128">Create a role assignment for the directory provider:</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /roleManagement/directory/roleAssignments
```

<span data-ttu-id="7b238-129">为角色分配提供程序创建一个权限管理提供程序：</span><span class="sxs-lookup"><span data-stu-id="7b238-129">Create a role assignment for the entitlement management provider:</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /roleManagement/entitlementManagement/roleAssignments
```


## <a name="request-headers"></a><span data-ttu-id="7b238-130">请求标头</span><span class="sxs-lookup"><span data-stu-id="7b238-130">Request headers</span></span>

| <span data-ttu-id="7b238-131">名称</span><span class="sxs-lookup"><span data-stu-id="7b238-131">Name</span></span>          | <span data-ttu-id="7b238-132">说明</span><span class="sxs-lookup"><span data-stu-id="7b238-132">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="7b238-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="7b238-133">Authorization</span></span> | <span data-ttu-id="7b238-134">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="7b238-134">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="7b238-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="7b238-135">Request body</span></span>

<span data-ttu-id="7b238-136">在请求正文中，提供 [unifiedRoleAssignment](../resources/unifiedroleassignment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7b238-136">In the request body, supply a JSON representation of a [unifiedRoleAssignment](../resources/unifiedroleassignment.md) object.</span></span> <span data-ttu-id="7b238-137">请求必须具有在 Azure AD 中定义的作用域（如 **directoryScopeId）** 或特定于应用程序的范围（如 **appScopeId）。**</span><span class="sxs-lookup"><span data-stu-id="7b238-137">The request must have either a scope defined in Azure AD, such as **directoryScopeId**, or an application-specific scope, such as **appScopeId**.</span></span> <span data-ttu-id="7b238-138">Azure AD 范围的示例包括租户 ("/") 、管理单元或应用程序。</span><span class="sxs-lookup"><span data-stu-id="7b238-138">Examples of Azure AD scopes are tenant ("/"), administrative units, or applications.</span></span> <span data-ttu-id="7b238-139">权利管理使用租户 ("/") 访问包目录范围。</span><span class="sxs-lookup"><span data-stu-id="7b238-139">Entitlement management uses tenant ("/") and access package catalog scopes.</span></span> <span data-ttu-id="7b238-140">有关详细信息，请参阅 [appScope](../resources/appscope.md)。</span><span class="sxs-lookup"><span data-stu-id="7b238-140">For more information, see [appScope](../resources/appscope.md).</span></span>

## <a name="response"></a><span data-ttu-id="7b238-141">响应</span><span class="sxs-lookup"><span data-stu-id="7b238-141">Response</span></span>

<span data-ttu-id="7b238-142">如果成功，此方法在响应正文中返回 响应代码和新的 `201 Created` [unifiedRoleAssignment](../resources/unifiedroleassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7b238-142">If successful, this method returns a `201 Created` response code and a new [unifiedRoleAssignment](../resources/unifiedroleassignment.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7b238-143">示例</span><span class="sxs-lookup"><span data-stu-id="7b238-143">Examples</span></span>

### <a name="example-1-create-a-role-assignment-at-tenant-scope"></a><span data-ttu-id="7b238-144">示例 1：在租户角色分配创建租户</span><span class="sxs-lookup"><span data-stu-id="7b238-144">Example 1: Create a role assignment at tenant scope</span></span>

#### <a name="request"></a><span data-ttu-id="7b238-145">请求</span><span class="sxs-lookup"><span data-stu-id="7b238-145">Request</span></span>

<span data-ttu-id="7b238-146">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="7b238-146">The following is an example of the request.</span></span> <span data-ttu-id="7b238-147">请注意 roleDefinitionId 的 roleTemplateId 的使用。</span><span class="sxs-lookup"><span data-stu-id="7b238-147">Note the use of the roleTemplateId for roleDefinitionId.</span></span> <span data-ttu-id="7b238-148">roleDefinitionId 可以是服务范围的模板 ID 或特定于目录的 roleDefinitionId。</span><span class="sxs-lookup"><span data-stu-id="7b238-148">roleDefinitionId can be either the service-wide template Id or the directory-specific roleDefinitionId.</span></span>


# <a name="http"></a>[<span data-ttu-id="7b238-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="7b238-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_unifiedroleassignment_from_rbacapplication"
}-->

```http
POST https://graph.microsoft.com/beta/roleManagement/directory/roleAssignments
Content-type: application/json

{ 
    "@odata.type": "#microsoft.graph.unifiedRoleAssignment",
    "roleDefinitionId": "c2cf284d-6c41-4e6b-afac-4b80928c9034",
    "principalId": "f8ca5a85-489a-49a0-b555-0a6d81e56f0d",
    "directoryScopeId": "/"
}
```
# <a name="c"></a>[<span data-ttu-id="7b238-150">C#</span><span class="sxs-lookup"><span data-stu-id="7b238-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-unifiedroleassignment-from-rbacapplication-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7b238-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7b238-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-unifiedroleassignment-from-rbacapplication-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7b238-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7b238-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-unifiedroleassignment-from-rbacapplication-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7b238-153">Java</span><span class="sxs-lookup"><span data-stu-id="7b238-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-unifiedroleassignment-from-rbacapplication-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="7b238-154">响应</span><span class="sxs-lookup"><span data-stu-id="7b238-154">Response</span></span>

<span data-ttu-id="7b238-155">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="7b238-155">The following is an example of the response.</span></span>

> <span data-ttu-id="7b238-156">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="7b238-156">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignment"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleAssignments/$entity",
    "id": "YUb1sHQtUEyvox7IA_Eu_mm3jqnUe4lEhvatluHVi2I-1",
    "roleDefinitionId": "c2cf284d-6c41-4e6b-afac-4b80928c9034",
    "principalId": "f8ca5a85-489a-49a0-b555-0a6d81e56f0d",
    "directoryScopeId": "/"
}
```

### <a name="example-2--create-a-role-assignment-over-an-administrative-unit-scope"></a><span data-ttu-id="7b238-157">示例 2：创建角色分配管理单元作用域的组</span><span class="sxs-lookup"><span data-stu-id="7b238-157">Example 2 : Create a role assignment over an administrative unit scope</span></span>

#### <a name="request"></a><span data-ttu-id="7b238-158">请求</span><span class="sxs-lookup"><span data-stu-id="7b238-158">Request</span></span>

<span data-ttu-id="7b238-159">以下示例将主要用户管理员角色分配给管理单元。</span><span class="sxs-lookup"><span data-stu-id="7b238-159">The following example assigns a principal User Admin role over an administrative unit.</span></span>


# <a name="http"></a>[<span data-ttu-id="7b238-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="7b238-160">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_unifiedroleassignment_over_administrativeunit"
}-->

```http
POST https://graph.microsoft.com/beta/roleManagement/directory/roleAssignments
Content-type: application/json

{
    "@odata.type": "#microsoft.graph.unifiedRoleAssignment",
    "roleDefinitionId": "fe930be7-5e62-47db-91af-98c3a49a38b1", //template id of User Account Administrator
    "principalId": "f8ca5a85-489a-49a0-b555-0a6d81e56f0d",
    "directoryScopeId": "/administrativeUnits/5d107bba-d8e2-4e13-b6ae-884be90e5d1a" //object id of an administrative unit
}
```
# <a name="c"></a>[<span data-ttu-id="7b238-161">C#</span><span class="sxs-lookup"><span data-stu-id="7b238-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-unifiedroleassignment-over-administrativeunit-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7b238-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7b238-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-unifiedroleassignment-over-administrativeunit-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7b238-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7b238-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-unifiedroleassignment-over-administrativeunit-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7b238-164">Java</span><span class="sxs-lookup"><span data-stu-id="7b238-164">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-unifiedroleassignment-over-administrativeunit-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="7b238-165">响应</span><span class="sxs-lookup"><span data-stu-id="7b238-165">Response</span></span>

<span data-ttu-id="7b238-166">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="7b238-166">The following is an example of the response.</span></span>

> <span data-ttu-id="7b238-167">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="7b238-167">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignment"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleAssignments/$entity",
    "id": "BH21sHQtUEyvox7IA_Eu_mm3jqnUe4lEhvatluHIWb7-1",
    "roleDefinitionId": "fe930be7-5e62-47db-91af-98c3a49a38b1",
    "principalId": "f8ca5a85-489a-49a0-b555-0a6d81e56f0d",
    "directoryScopeId": "/administrativeUnits/5d107bba-d8e2-4e13-b6ae-884be90e5d1a"
}
```


### <a name="example-3-create-a-role-assignment-at-access-package-catalog-scope"></a><span data-ttu-id="7b238-168">示例 3：在角色分配包目录范围创建应用程序</span><span class="sxs-lookup"><span data-stu-id="7b238-168">Example 3: Create a role assignment at access package catalog scope</span></span>

#### <a name="request"></a><span data-ttu-id="7b238-169">请求</span><span class="sxs-lookup"><span data-stu-id="7b238-169">Request</span></span>

<span data-ttu-id="7b238-170">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="7b238-170">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="7b238-171">HTTP</span><span class="sxs-lookup"><span data-stu-id="7b238-171">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_unifiedroleassignment3_from_rbacapplication"
}-->

```http
POST https://graph.microsoft.com/beta/roleManagement/entitlementManagement/roleAssignments
Content-type: application/json

{
    "principalId": "679a9213-c497-48a4-830a-8d3d25d94ddc",
    "roleDefinitionId": "ae79f266-94d4-4dab-b730-feca7e132178",
    "appScopeId": "/AccessPackageCatalog/beedadfe-01d5-4025-910b-84abb9369997"
}
```
# <a name="c"></a>[<span data-ttu-id="7b238-172">C#</span><span class="sxs-lookup"><span data-stu-id="7b238-172">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-unifiedroleassignment3-from-rbacapplication-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7b238-173">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7b238-173">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-unifiedroleassignment3-from-rbacapplication-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7b238-174">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7b238-174">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-unifiedroleassignment3-from-rbacapplication-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7b238-175">Java</span><span class="sxs-lookup"><span data-stu-id="7b238-175">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-unifiedroleassignment3-from-rbacapplication-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="7b238-176">响应</span><span class="sxs-lookup"><span data-stu-id="7b238-176">Response</span></span>

<span data-ttu-id="7b238-177">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="7b238-177">The following is an example of the response.</span></span>

> <span data-ttu-id="7b238-178">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="7b238-178">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignment"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/entitlementManagement/roleAssignments/$entity",
    "id": "f3092518-7874-462e-93e9-0cd6c11ffc52",
    "principalId": "679a9213-c497-48a4-830a-8d3d25d94ddc",
    "roleDefinitionId": "ae79f266-94d4-4dab-b730-feca7e132178",
    "appScopeId": "/AccessPackageCatalog/beedadfe-01d5-4025-910b-84abb9369997"
}
```


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create unifiedRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


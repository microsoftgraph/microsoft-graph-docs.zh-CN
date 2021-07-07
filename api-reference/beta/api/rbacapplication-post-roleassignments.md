---
title: 创建 unifiedRoleAssignment
description: 创建新的 unifiedRoleAssignment 对象。
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: aafcc34d288dcce1bcd0970802472a2e2e565e83
ms.sourcegitcommit: ada6eab637b9b318129aefb98edbe7316399d9ba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/07/2021
ms.locfileid: "53317201"
---
# <a name="create-unifiedroleassignment"></a><span data-ttu-id="e576c-103">创建 unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="e576c-103">Create unifiedRoleAssignment</span></span>

<span data-ttu-id="e576c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e576c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e576c-105">创建新的 [unifiedRoleAssignment](../resources/unifiedroleassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e576c-105">Create a new [unifiedRoleAssignment](../resources/unifiedroleassignment.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e576c-106">权限</span><span class="sxs-lookup"><span data-stu-id="e576c-106">Permissions</span></span>

<span data-ttu-id="e576c-107">根据 RBAC 提供程序以及 (或应用程序) 的权限类型，从下表中选择调用此 API 所需的最低特权权限。</span><span class="sxs-lookup"><span data-stu-id="e576c-107">Depending on the RBAC provider and the permission type (delegated or application) that is needed, choose from the following table the least privileged permission required to call this API.</span></span> <span data-ttu-id="e576c-108">若要了解其他信息， [在](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) 特权权限之前要特别小心，在"权限" [中搜索](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e576c-108">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e576c-109">支持的提供程序</span><span class="sxs-lookup"><span data-stu-id="e576c-109">Supported provider</span></span>      | <span data-ttu-id="e576c-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e576c-110">Delegated (work or school account)</span></span>  | <span data-ttu-id="e576c-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e576c-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e576c-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="e576c-112">Application</span></span> |
|:-----------------------|:------------------------------------|:---------------------------------------|:------------|
| <span data-ttu-id="e576c-113">目录</span><span class="sxs-lookup"><span data-stu-id="e576c-113">Directory</span></span> | <span data-ttu-id="e576c-114">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="e576c-114">RoleManagement.ReadWrite.Directory</span></span> | <span data-ttu-id="e576c-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="e576c-115">Not supported.</span></span>| <span data-ttu-id="e576c-116">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="e576c-116">RoleManagement.ReadWrite.Directory</span></span> |
| <span data-ttu-id="e576c-117">权利管理</span><span class="sxs-lookup"><span data-stu-id="e576c-117">Entitlement management</span></span> | <span data-ttu-id="e576c-118">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e576c-118">EntitlementManagement.ReadWrite.All</span></span> | <span data-ttu-id="e576c-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="e576c-119">Not supported.</span></span> | <span data-ttu-id="e576c-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="e576c-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e576c-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e576c-121">HTTP request</span></span>

<span data-ttu-id="e576c-122">为角色分配创建一个目录提供程序：</span><span class="sxs-lookup"><span data-stu-id="e576c-122">Create a role assignment for the directory provider:</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /roleManagement/directory/roleAssignments
```

<span data-ttu-id="e576c-123">为角色分配提供程序创建一个权限管理提供程序：</span><span class="sxs-lookup"><span data-stu-id="e576c-123">Create a role assignment for the entitlement management provider:</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /roleManagement/entitlementManagement/roleAssignments
```


## <a name="request-headers"></a><span data-ttu-id="e576c-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="e576c-124">Request headers</span></span>

| <span data-ttu-id="e576c-125">名称</span><span class="sxs-lookup"><span data-stu-id="e576c-125">Name</span></span>          | <span data-ttu-id="e576c-126">说明</span><span class="sxs-lookup"><span data-stu-id="e576c-126">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="e576c-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="e576c-127">Authorization</span></span> | <span data-ttu-id="e576c-128">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="e576c-128">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="e576c-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="e576c-129">Request body</span></span>

<span data-ttu-id="e576c-130">在请求正文中，提供 [unifiedRoleAssignment](../resources/unifiedroleassignment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e576c-130">In the request body, supply a JSON representation of [unifiedRoleAssignment](../resources/unifiedroleassignment.md) object.</span></span> <span data-ttu-id="e576c-131">请求必须具有在 Azure AD 中定义的作用域（如 ）或特定于应用程序的范围（ `directoryScopeId` 如 `appScopeId` ）。</span><span class="sxs-lookup"><span data-stu-id="e576c-131">The request must have either a scope defined in Azure AD, such as `directoryScopeId`, or an application-specific scope, such as `appScopeId`.</span></span> <span data-ttu-id="e576c-132">Azure AD 范围的示例包括租户 (/") 、管理单元或应用程序。</span><span class="sxs-lookup"><span data-stu-id="e576c-132">Examples of Azure AD scope are tenant ("/"), administrative units, or applications.</span></span> <span data-ttu-id="e576c-133">有关详细信息，请参阅 [appScope](../resources/appscope.md)。</span><span class="sxs-lookup"><span data-stu-id="e576c-133">For more information, see [appScope](../resources/appscope.md).</span></span>

## <a name="response"></a><span data-ttu-id="e576c-134">响应</span><span class="sxs-lookup"><span data-stu-id="e576c-134">Response</span></span>

<span data-ttu-id="e576c-135">如果成功，此方法在响应正文中返回 响应代码和新的 `201 Created` [unifiedRoleAssignment](../resources/unifiedroleassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e576c-135">If successful, this method returns a `201 Created` response code and a new [unifiedRoleAssignment](../resources/unifiedroleassignment.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e576c-136">示例</span><span class="sxs-lookup"><span data-stu-id="e576c-136">Examples</span></span>

### <a name="example-1-create-a-role-assignment-at-tenant-scope"></a><span data-ttu-id="e576c-137">示例 1：在租户角色分配创建租户</span><span class="sxs-lookup"><span data-stu-id="e576c-137">Example 1: Create a role assignment at tenant scope</span></span>

#### <a name="request"></a><span data-ttu-id="e576c-138">请求</span><span class="sxs-lookup"><span data-stu-id="e576c-138">Request</span></span>

<span data-ttu-id="e576c-139">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e576c-139">The following is an example of the request.</span></span> <span data-ttu-id="e576c-140">请注意 roleDefinitionId 的 roleTemplateId 的使用。</span><span class="sxs-lookup"><span data-stu-id="e576c-140">Note the use of the roleTemplateId for roleDefinitionId.</span></span> <span data-ttu-id="e576c-141">roleDefinitionId 可以是服务范围的模板 ID 或特定于目录的 roleDefinitionId。</span><span class="sxs-lookup"><span data-stu-id="e576c-141">roleDefinitionId can be either the service-wide template Id or the directory-specific roleDefinitionId.</span></span>


# <a name="http"></a>[<span data-ttu-id="e576c-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="e576c-142">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="e576c-143">C#</span><span class="sxs-lookup"><span data-stu-id="e576c-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-unifiedroleassignment-from-rbacapplication-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e576c-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e576c-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-unifiedroleassignment-from-rbacapplication-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e576c-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e576c-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-unifiedroleassignment-from-rbacapplication-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e576c-146">Java</span><span class="sxs-lookup"><span data-stu-id="e576c-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-unifiedroleassignment-from-rbacapplication-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e576c-147">响应</span><span class="sxs-lookup"><span data-stu-id="e576c-147">Response</span></span>

<span data-ttu-id="e576c-148">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="e576c-148">The following is an example of the response.</span></span>

> <span data-ttu-id="e576c-149">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="e576c-149">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-2--create-a-role-assignment-over-an-administrative-unit-scope"></a><span data-ttu-id="e576c-150">示例 2：创建角色分配管理单元作用域的组</span><span class="sxs-lookup"><span data-stu-id="e576c-150">Example 2 : Create a role assignment over an administrative unit scope</span></span>

#### <a name="request"></a><span data-ttu-id="e576c-151">请求</span><span class="sxs-lookup"><span data-stu-id="e576c-151">Request</span></span>

<span data-ttu-id="e576c-152">以下示例将主要用户管理员角色分配给管理单元。</span><span class="sxs-lookup"><span data-stu-id="e576c-152">The following example assigns a principal User Admin role over an administrative unit.</span></span>


# <a name="http"></a>[<span data-ttu-id="e576c-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="e576c-153">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="e576c-154">C#</span><span class="sxs-lookup"><span data-stu-id="e576c-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-unifiedroleassignment-over-administrativeunit-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e576c-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e576c-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-unifiedroleassignment-over-administrativeunit-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e576c-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e576c-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-unifiedroleassignment-over-administrativeunit-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e576c-157">Java</span><span class="sxs-lookup"><span data-stu-id="e576c-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-unifiedroleassignment-over-administrativeunit-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e576c-158">响应</span><span class="sxs-lookup"><span data-stu-id="e576c-158">Response</span></span>

<span data-ttu-id="e576c-159">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="e576c-159">The following is an example of the response.</span></span>

> <span data-ttu-id="e576c-160">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="e576c-160">**Note:** The response object shown here might be shortened for readability.</span></span>

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

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create unifiedRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->



---
title: 创建 unifiedRoleAssignment
description: 创建新的 unifiedRoleAssignment 对象。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 02e794c15ab562d61adde8a6c662c0c7e4ae4e7a
ms.sourcegitcommit: 11503211a31ea17f4e577c21ec36d364184c0580
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/08/2020
ms.locfileid: "43181159"
---
# <a name="create-unifiedroleassignment"></a><span data-ttu-id="0d0cb-103">创建 unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="0d0cb-103">Create unifiedRoleAssignment</span></span>

<span data-ttu-id="0d0cb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0d0cb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0d0cb-105">创建新的[unifiedRoleAssignment](../resources/unifiedroleassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="0d0cb-105">Create a new [unifiedRoleAssignment](../resources/unifiedroleassignment.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="0d0cb-106">权限</span><span class="sxs-lookup"><span data-stu-id="0d0cb-106">Permissions</span></span>

<span data-ttu-id="0d0cb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0d0cb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0d0cb-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="0d0cb-109">Permission type</span></span>                        | <span data-ttu-id="0d0cb-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0d0cb-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="0d0cb-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0d0cb-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="0d0cb-112">RoleManagement、RoleManagement、目录</span><span class="sxs-lookup"><span data-stu-id="0d0cb-112">RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span> |
| <span data-ttu-id="0d0cb-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0d0cb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0d0cb-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="0d0cb-114">Not supported.</span></span> |
| <span data-ttu-id="0d0cb-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="0d0cb-115">Application</span></span>                            | <span data-ttu-id="0d0cb-116">RoleManagement、RoleManagement、目录</span><span class="sxs-lookup"><span data-stu-id="0d0cb-116">RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="0d0cb-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0d0cb-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /roleManagement/directory/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="0d0cb-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="0d0cb-118">Request headers</span></span>

| <span data-ttu-id="0d0cb-119">名称</span><span class="sxs-lookup"><span data-stu-id="0d0cb-119">Name</span></span>          | <span data-ttu-id="0d0cb-120">说明</span><span class="sxs-lookup"><span data-stu-id="0d0cb-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="0d0cb-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="0d0cb-121">Authorization</span></span> | <span data-ttu-id="0d0cb-122">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="0d0cb-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="0d0cb-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="0d0cb-123">Request body</span></span>

<span data-ttu-id="0d0cb-124">在请求正文中，提供[unifiedRoleAssignment](../resources/unifiedroleassignment.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0d0cb-124">In the request body, supply a JSON representation of [unifiedRoleAssignment](../resources/unifiedroleassignment.md) object.</span></span> <span data-ttu-id="0d0cb-125">请求必须具有在 Azure AD 中定义的作用域（例如`directoryScopeId`）或特定于应用程序的作用域（例如`appScopeId`）。</span><span class="sxs-lookup"><span data-stu-id="0d0cb-125">The request must have either a scope defined in Azure AD, such as `directoryScopeId`, or an application-specific scope, such as `appScopeId`.</span></span> <span data-ttu-id="0d0cb-126">Azure AD 作用域的示例包括租户（"/"）、管理单元或应用程序。</span><span class="sxs-lookup"><span data-stu-id="0d0cb-126">Examples of Azure AD scope are tenant ("/"), administrative units, or applications.</span></span> <span data-ttu-id="0d0cb-127">有关详细信息，请参阅[appScope](../resources/appscope.md)。</span><span class="sxs-lookup"><span data-stu-id="0d0cb-127">For more information, see [appScope](../resources/appscope.md).</span></span>

## <a name="response"></a><span data-ttu-id="0d0cb-128">响应</span><span class="sxs-lookup"><span data-stu-id="0d0cb-128">Response</span></span>

<span data-ttu-id="0d0cb-129">如果成功，此方法在响应`201 Created`正文中返回响应代码和新的[unifiedRoleAssignment](../resources/unifiedroleassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="0d0cb-129">If successful, this method returns a `201 Created` response code and a new [unifiedRoleAssignment](../resources/unifiedroleassignment.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0d0cb-130">示例</span><span class="sxs-lookup"><span data-stu-id="0d0cb-130">Examples</span></span>

### <a name="example-1-create-a-role-assignment-at-tenant-scope"></a><span data-ttu-id="0d0cb-131">示例1：在租户范围创建角色分配</span><span class="sxs-lookup"><span data-stu-id="0d0cb-131">Example 1: Create a role assignment at tenant scope</span></span>

#### <a name="request"></a><span data-ttu-id="0d0cb-132">请求</span><span class="sxs-lookup"><span data-stu-id="0d0cb-132">Request</span></span>

<span data-ttu-id="0d0cb-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="0d0cb-133">The following is an example of the request.</span></span> <span data-ttu-id="0d0cb-134">请注意，使用 roleTemplateId 进行 roleDefinitionId。</span><span class="sxs-lookup"><span data-stu-id="0d0cb-134">Note the use of the roleTemplateId for roleDefinitionId.</span></span> <span data-ttu-id="0d0cb-135">roleDefinitionId 可以是服务范围的模板 Id，也可以是特定于目录的 roleDefinitionId。</span><span class="sxs-lookup"><span data-stu-id="0d0cb-135">roleDefinitionId can be either the service-wide template Id or the directory-specific roleDefinitionId.</span></span>


# <a name="http"></a>[<span data-ttu-id="0d0cb-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="0d0cb-136">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="0d0cb-137">C#</span><span class="sxs-lookup"><span data-stu-id="0d0cb-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-unifiedroleassignment-from-rbacapplication-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0d0cb-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0d0cb-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-unifiedroleassignment-from-rbacapplication-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0d0cb-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0d0cb-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-unifiedroleassignment-from-rbacapplication-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="0d0cb-140">响应</span><span class="sxs-lookup"><span data-stu-id="0d0cb-140">Response</span></span>

<span data-ttu-id="0d0cb-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="0d0cb-141">The following is an example of the response.</span></span>

> <span data-ttu-id="0d0cb-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="0d0cb-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2--create-a-role-assignment-over-an-administrative-unit-scope"></a><span data-ttu-id="0d0cb-144">示例2：在管理单元范围内创建角色分配</span><span class="sxs-lookup"><span data-stu-id="0d0cb-144">Example 2 : Create a role assignment over an administrative unit scope</span></span>

#### <a name="request"></a><span data-ttu-id="0d0cb-145">请求</span><span class="sxs-lookup"><span data-stu-id="0d0cb-145">Request</span></span>

<span data-ttu-id="0d0cb-146">下面的示例在管理单元上分配主要用户管理员角色。</span><span class="sxs-lookup"><span data-stu-id="0d0cb-146">The following example assigns a principal User Admin role over an administrative unit.</span></span>


# <a name="http"></a>[<span data-ttu-id="0d0cb-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="0d0cb-147">HTTP</span></span>](#tab/http)
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
    "directoryScopeId": "5d107bba-d8e2-4e13-b6ae-884be90e5d1a" //object id of an administrative unit
}
```
# <a name="c"></a>[<span data-ttu-id="0d0cb-148">C#</span><span class="sxs-lookup"><span data-stu-id="0d0cb-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-unifiedroleassignment-over-administrativeunit-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0d0cb-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0d0cb-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-unifiedroleassignment-over-administrativeunit-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0d0cb-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0d0cb-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-unifiedroleassignment-over-administrativeunit-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="0d0cb-151">响应</span><span class="sxs-lookup"><span data-stu-id="0d0cb-151">Response</span></span>

<span data-ttu-id="0d0cb-152">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="0d0cb-152">The following is an example of the response.</span></span>

> <span data-ttu-id="0d0cb-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="0d0cb-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
    "directoryScopeId": "5d107bba-d8e2-4e13-b6ae-884be90e5d1a"
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

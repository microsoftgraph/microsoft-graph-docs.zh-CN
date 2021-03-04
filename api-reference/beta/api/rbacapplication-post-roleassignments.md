---
title: 创建 unifiedRoleAssignment
description: 创建新的 unifiedRoleAssignment 对象。
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: d654b852358c94e4b762c794c6da114f19b091af
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50440883"
---
# <a name="create-unifiedroleassignment"></a><span data-ttu-id="9c97f-103">创建 unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="9c97f-103">Create unifiedRoleAssignment</span></span>

<span data-ttu-id="9c97f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9c97f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9c97f-105">创建新的 [unifiedRoleAssignment](../resources/unifiedroleassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9c97f-105">Create a new [unifiedRoleAssignment](../resources/unifiedroleassignment.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="9c97f-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="9c97f-106">Permissions</span></span>

<span data-ttu-id="9c97f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9c97f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9c97f-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="9c97f-109">Permission type</span></span>                        | <span data-ttu-id="9c97f-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9c97f-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="9c97f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9c97f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="9c97f-112">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="9c97f-112">RoleManagement.ReadWrite.Directory</span></span> |
| <span data-ttu-id="9c97f-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9c97f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9c97f-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="9c97f-114">Not supported.</span></span> |
| <span data-ttu-id="9c97f-115">Application</span><span class="sxs-lookup"><span data-stu-id="9c97f-115">Application</span></span>                            | <span data-ttu-id="9c97f-116">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="9c97f-116">RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="9c97f-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9c97f-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /roleManagement/directory/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="9c97f-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="9c97f-118">Request headers</span></span>

| <span data-ttu-id="9c97f-119">名称</span><span class="sxs-lookup"><span data-stu-id="9c97f-119">Name</span></span>          | <span data-ttu-id="9c97f-120">说明</span><span class="sxs-lookup"><span data-stu-id="9c97f-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="9c97f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="9c97f-121">Authorization</span></span> | <span data-ttu-id="9c97f-122">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="9c97f-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="9c97f-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="9c97f-123">Request body</span></span>

<span data-ttu-id="9c97f-124">在请求正文中，提供 [unifiedRoleAssignment](../resources/unifiedroleassignment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9c97f-124">In the request body, supply a JSON representation of [unifiedRoleAssignment](../resources/unifiedroleassignment.md) object.</span></span> <span data-ttu-id="9c97f-125">请求必须具有在 Azure AD 中定义的作用域（例如）或特定于应用程序的范围， `directoryScopeId` 例如 `appScopeId` 。</span><span class="sxs-lookup"><span data-stu-id="9c97f-125">The request must have either a scope defined in Azure AD, such as `directoryScopeId`, or an application-specific scope, such as `appScopeId`.</span></span> <span data-ttu-id="9c97f-126">Azure AD 范围的示例包括租户 ("/") 、管理单元或应用程序。</span><span class="sxs-lookup"><span data-stu-id="9c97f-126">Examples of Azure AD scope are tenant ("/"), administrative units, or applications.</span></span> <span data-ttu-id="9c97f-127">有关详细信息，请参阅 [appScope](../resources/appscope.md)。</span><span class="sxs-lookup"><span data-stu-id="9c97f-127">For more information, see [appScope](../resources/appscope.md).</span></span>

## <a name="response"></a><span data-ttu-id="9c97f-128">响应</span><span class="sxs-lookup"><span data-stu-id="9c97f-128">Response</span></span>

<span data-ttu-id="9c97f-129">如果成功，此方法在响应正文中返回响应 `201 Created` 代码和新的 [unifiedRoleAssignment](../resources/unifiedroleassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9c97f-129">If successful, this method returns a `201 Created` response code and a new [unifiedRoleAssignment](../resources/unifiedroleassignment.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9c97f-130">示例</span><span class="sxs-lookup"><span data-stu-id="9c97f-130">Examples</span></span>

### <a name="example-1-create-a-role-assignment-at-tenant-scope"></a><span data-ttu-id="9c97f-131">示例 1：在租户角色分配创建租户</span><span class="sxs-lookup"><span data-stu-id="9c97f-131">Example 1: Create a role assignment at tenant scope</span></span>

#### <a name="request"></a><span data-ttu-id="9c97f-132">请求</span><span class="sxs-lookup"><span data-stu-id="9c97f-132">Request</span></span>

<span data-ttu-id="9c97f-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="9c97f-133">The following is an example of the request.</span></span> <span data-ttu-id="9c97f-134">请注意对 roleDefinitionId 使用 roleTemplateId。</span><span class="sxs-lookup"><span data-stu-id="9c97f-134">Note the use of the roleTemplateId for roleDefinitionId.</span></span> <span data-ttu-id="9c97f-135">roleDefinitionId 可以是服务范围的模板 ID 或特定于目录的 roleDefinitionId。</span><span class="sxs-lookup"><span data-stu-id="9c97f-135">roleDefinitionId can be either the service-wide template Id or the directory-specific roleDefinitionId.</span></span>


# <a name="http"></a>[<span data-ttu-id="9c97f-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="9c97f-136">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="9c97f-137">C#</span><span class="sxs-lookup"><span data-stu-id="9c97f-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-unifiedroleassignment-from-rbacapplication-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9c97f-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9c97f-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-unifiedroleassignment-from-rbacapplication-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9c97f-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9c97f-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-unifiedroleassignment-from-rbacapplication-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9c97f-140">Java</span><span class="sxs-lookup"><span data-stu-id="9c97f-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-unifiedroleassignment-from-rbacapplication-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9c97f-141">响应</span><span class="sxs-lookup"><span data-stu-id="9c97f-141">Response</span></span>

<span data-ttu-id="9c97f-142">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="9c97f-142">The following is an example of the response.</span></span>

> <span data-ttu-id="9c97f-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="9c97f-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2--create-a-role-assignment-over-an-administrative-unit-scope"></a><span data-ttu-id="9c97f-145">示例 2：角色分配管理单元作用域创建一个管理单元</span><span class="sxs-lookup"><span data-stu-id="9c97f-145">Example 2 : Create a role assignment over an administrative unit scope</span></span>

#### <a name="request"></a><span data-ttu-id="9c97f-146">请求</span><span class="sxs-lookup"><span data-stu-id="9c97f-146">Request</span></span>

<span data-ttu-id="9c97f-147">以下示例为管理单元分配主体用户管理员角色。</span><span class="sxs-lookup"><span data-stu-id="9c97f-147">The following example assigns a principal User Admin role over an administrative unit.</span></span>


# <a name="http"></a>[<span data-ttu-id="9c97f-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="9c97f-148">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="9c97f-149">C#</span><span class="sxs-lookup"><span data-stu-id="9c97f-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-unifiedroleassignment-over-administrativeunit-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9c97f-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9c97f-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-unifiedroleassignment-over-administrativeunit-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9c97f-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9c97f-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-unifiedroleassignment-over-administrativeunit-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9c97f-152">Java</span><span class="sxs-lookup"><span data-stu-id="9c97f-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-unifiedroleassignment-over-administrativeunit-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9c97f-153">响应</span><span class="sxs-lookup"><span data-stu-id="9c97f-153">Response</span></span>

<span data-ttu-id="9c97f-154">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="9c97f-154">The following is an example of the response.</span></span>

> <span data-ttu-id="9c97f-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="9c97f-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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



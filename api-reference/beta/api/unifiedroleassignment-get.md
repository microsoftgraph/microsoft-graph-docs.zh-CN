---
title: 获取 unifiedRoleAssignment
description: 检索 unifiedRoleAssignment 对象的属性和关系。
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 238b2e1d6049ec53d779fddba830338b13b6f781
ms.sourcegitcommit: 4888ac7504533344c4fc6828e2a06a002a1d72d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/09/2021
ms.locfileid: "53351035"
---
# <a name="get-unifiedroleassignment"></a><span data-ttu-id="5eecc-103">获取 unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="5eecc-103">Get unifiedRoleAssignment</span></span>

<span data-ttu-id="5eecc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5eecc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5eecc-105">检索 [unifiedRoleAssignment](../resources/unifiedroleassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5eecc-105">Retrieve the properties and relationships of a [unifiedRoleAssignment](../resources/unifiedroleassignment.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="5eecc-106">权限</span><span class="sxs-lookup"><span data-stu-id="5eecc-106">Permissions</span></span>

<span data-ttu-id="5eecc-107">根据 RBAC 提供程序以及 (或应用程序) 的权限类型，从下表中选择调用此 API 所需的最低特权权限。</span><span class="sxs-lookup"><span data-stu-id="5eecc-107">Depending on the RBAC provider and the permission type (delegated or application) that is needed, choose from the following table the least privileged permission required to call this API.</span></span> <span data-ttu-id="5eecc-108">若要了解其他信息， [在](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) 特权权限之前要特别小心，在"权限" [中搜索](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5eecc-108">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in [Permissions](/graph/permissions-reference).</span></span>

### <a name="for-directory-azure-ad-provider"></a><span data-ttu-id="5eecc-109">对于 Azure AD (提供程序) 目录</span><span class="sxs-lookup"><span data-stu-id="5eecc-109">For Directory (Azure AD) provider</span></span>

|<span data-ttu-id="5eecc-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="5eecc-110">Permission type</span></span>      | <span data-ttu-id="5eecc-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5eecc-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5eecc-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5eecc-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="5eecc-113">RoleManagement.Read.Directory、Directory.Read.All、RoleManagement.ReadWrite.Directory、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="5eecc-113">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>   |
|<span data-ttu-id="5eecc-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5eecc-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5eecc-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="5eecc-115">Not supported.</span></span>    |
|<span data-ttu-id="5eecc-116">Application</span><span class="sxs-lookup"><span data-stu-id="5eecc-116">Application</span></span> | <span data-ttu-id="5eecc-117">RoleManagement.Read.Directory、Directory.Read.All、RoleManagement.ReadWrite.Directory、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5eecc-117">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

### <a name="for-entitlement-management-provider"></a><span data-ttu-id="5eecc-118">对于权利管理提供程序</span><span class="sxs-lookup"><span data-stu-id="5eecc-118">For Entitlement management provider</span></span>

|<span data-ttu-id="5eecc-119">权限类型</span><span class="sxs-lookup"><span data-stu-id="5eecc-119">Permission type</span></span>      | <span data-ttu-id="5eecc-120">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5eecc-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5eecc-121">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5eecc-121">Delegated (work or school account)</span></span> |  <span data-ttu-id="5eecc-122">EntitlementManagement.Read.All、EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5eecc-122">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span>  |
|<span data-ttu-id="5eecc-123">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5eecc-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5eecc-124">不支持。</span><span class="sxs-lookup"><span data-stu-id="5eecc-124">Not supported.</span></span>    |
|<span data-ttu-id="5eecc-125">Application</span><span class="sxs-lookup"><span data-stu-id="5eecc-125">Application</span></span> | <span data-ttu-id="5eecc-126">不支持。</span><span class="sxs-lookup"><span data-stu-id="5eecc-126">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5eecc-127">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5eecc-127">HTTP request</span></span>

<span data-ttu-id="5eecc-128">获取角色分配提供程序的名称：</span><span class="sxs-lookup"><span data-stu-id="5eecc-128">Get a role assignment for a directory provider:</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /roleManagement/directory/roleAssignments/{id}
```

<span data-ttu-id="5eecc-129">获取角色分配管理提供程序的信息：</span><span class="sxs-lookup"><span data-stu-id="5eecc-129">Get a role assignment for the entitlement management provider:</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /roleManagement/entitlementManagement/roleAssignments/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5eecc-130">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="5eecc-130">Optional query parameters</span></span>

<span data-ttu-id="5eecc-131">此方法支持 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="5eecc-131">This method supports OData query parameters to help customize the response.</span></span> <span data-ttu-id="5eecc-132">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="5eecc-132">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="5eecc-133">请求标头</span><span class="sxs-lookup"><span data-stu-id="5eecc-133">Request headers</span></span>

| <span data-ttu-id="5eecc-134">名称</span><span class="sxs-lookup"><span data-stu-id="5eecc-134">Name</span></span>      |<span data-ttu-id="5eecc-135">说明</span><span class="sxs-lookup"><span data-stu-id="5eecc-135">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5eecc-136">Authorization</span><span class="sxs-lookup"><span data-stu-id="5eecc-136">Authorization</span></span> | <span data-ttu-id="5eecc-137">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="5eecc-137">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="5eecc-138">请求正文</span><span class="sxs-lookup"><span data-stu-id="5eecc-138">Request body</span></span>

<span data-ttu-id="5eecc-139">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5eecc-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5eecc-140">响应</span><span class="sxs-lookup"><span data-stu-id="5eecc-140">Response</span></span>

<span data-ttu-id="5eecc-141">如果成功，此方法在响应正文中返回 响应代码和请求的 `200 OK` [unifiedRoleAssignment](../resources/unifiedroleassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5eecc-141">If successful, this method returns a `200 OK` response code and the requested [unifiedRoleAssignment](../resources/unifiedroleassignment.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5eecc-142">示例</span><span class="sxs-lookup"><span data-stu-id="5eecc-142">Examples</span></span>

### <a name="example-1--get-details-of-a-role-assignment"></a><span data-ttu-id="5eecc-143">示例 1：获取角色分配</span><span class="sxs-lookup"><span data-stu-id="5eecc-143">Example 1 : Get details of a role assignment</span></span>

#### <a name="request"></a><span data-ttu-id="5eecc-144">请求</span><span class="sxs-lookup"><span data-stu-id="5eecc-144">Request</span></span>

<span data-ttu-id="5eecc-145">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="5eecc-145">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="5eecc-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="5eecc-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_unifiedroleassignment_1"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/directory/roleAssignments/lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1
```
# <a name="c"></a>[<span data-ttu-id="5eecc-147">C#</span><span class="sxs-lookup"><span data-stu-id="5eecc-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-unifiedroleassignment-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5eecc-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5eecc-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-unifiedroleassignment-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5eecc-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5eecc-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-unifiedroleassignment-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5eecc-150">Java</span><span class="sxs-lookup"><span data-stu-id="5eecc-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-unifiedroleassignment-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="5eecc-151">响应</span><span class="sxs-lookup"><span data-stu-id="5eecc-151">Response</span></span>

<span data-ttu-id="5eecc-152">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="5eecc-152">The following is an example of the response.</span></span>

> <span data-ttu-id="5eecc-153">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="5eecc-153">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignment"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleAssignments/$entity",
    "id": "lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1",
    "roleDefinitionId": "62e90394-69f5-4237-9190-012177145e10",
    "principalId": "4ab0b690-479b-47ff-af8f-2576cf521872",
    "directoryScopeId": "28ca5a85-489a-49a0-b555-0a6d81e56f0"
}
```

### <a name="example-2-get-details-of-a-role-assignment-with-expand"></a><span data-ttu-id="5eecc-154">示例 2：使用 获取角色分配的详细信息 `$expand`</span><span class="sxs-lookup"><span data-stu-id="5eecc-154">Example 2: Get details of a role assignment with `$expand`</span></span>

#### <a name="request"></a><span data-ttu-id="5eecc-155">请求</span><span class="sxs-lookup"><span data-stu-id="5eecc-155">Request</span></span>

<span data-ttu-id="5eecc-156">下面是一个包含查询参数 `$expand` 的请求示例。</span><span class="sxs-lookup"><span data-stu-id="5eecc-156">The following is an example of the request with the `$expand` query parameter.</span></span>


# <a name="http"></a>[<span data-ttu-id="5eecc-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="5eecc-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_unifiedroleassignment_2"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/directory/roleAssignments/lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1?$expand=roleDefinition,principal,directoryScope
```
# <a name="c"></a>[<span data-ttu-id="5eecc-158">C#</span><span class="sxs-lookup"><span data-stu-id="5eecc-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-unifiedroleassignment-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5eecc-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5eecc-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-unifiedroleassignment-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5eecc-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5eecc-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-unifiedroleassignment-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5eecc-161">Java</span><span class="sxs-lookup"><span data-stu-id="5eecc-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-unifiedroleassignment-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="5eecc-162">响应</span><span class="sxs-lookup"><span data-stu-id="5eecc-162">Response</span></span>

<span data-ttu-id="5eecc-163">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="5eecc-163">The following is an example of the response.</span></span>
> <span data-ttu-id="5eecc-164">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="5eecc-164">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignment"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleAssignments/$entity",
    "@odata.type": "#microsoft.graph.unifiedRoleAssignment",
    "id": "lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1",
    "roleDefinitionId": "c2cf284d-6c41-4e6b-afac-4b80928c9034",
    "roleDefinition": {
      "id": "c2cf284d-6c41-4e6b-afac-4b80928c9034",
      "displayName": "Billing Administrator",
      "description": "Can perform common billing related tasks like updating payment information.",
      "rolePermissions": [
        {
          "allowedResourceActions": [
            "microsoft.commerce.billing/allEntities/allTasks",
            "microsoft.directory/organization/basic/update",
          ],
          "excludedResourceActions": []
        }],
      "isEnabled": true,
      },
    "principalId": "f8ca5a85-489a-49a0-b555-0a6d81e56f0d",
    "principal": {
      "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users/$entity",
      "id": "f8ca5a85-489a-49a0-b555-0a6d81e56f0d ",
      "userPrincipalName": "alice@contoso.com",
      "displayName": "Alice Smith"
    },
    "directoryScopeId": "28ca5a85-489a-49a0-b555-0a6d81e56f0d",
    "directoryScope": {
      "@odata.context": "https://graph.microsoft.com/beta/$metadata#organization/$entity",
      "id": "28ca5a85-489a-49a0-b555-0a6d81e56f0d",
      "displayName": "Contoso_Seattle_Admins"
    }
}
```
<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get unifiedRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->



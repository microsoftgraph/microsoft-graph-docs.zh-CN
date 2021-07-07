---
title: 获取 unifiedRoleAssignment
description: 检索 unifiedRoleAssignment 对象的属性和关系。
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: e24f9a2ae184502123cca58188902d0f66782b87
ms.sourcegitcommit: ada6eab637b9b318129aefb98edbe7316399d9ba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/07/2021
ms.locfileid: "53317033"
---
# <a name="get-unifiedroleassignment"></a><span data-ttu-id="eb472-103">获取 unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="eb472-103">Get unifiedRoleAssignment</span></span>

<span data-ttu-id="eb472-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eb472-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eb472-105">检索 [unifiedRoleAssignment](../resources/unifiedroleassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="eb472-105">Retrieve the properties and relationships of a [unifiedRoleAssignment](../resources/unifiedroleassignment.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="eb472-106">权限</span><span class="sxs-lookup"><span data-stu-id="eb472-106">Permissions</span></span>

<span data-ttu-id="eb472-107">根据 RBAC 提供程序以及 (或应用程序) 的权限类型，从下表中选择调用此 API 所需的最低特权权限。</span><span class="sxs-lookup"><span data-stu-id="eb472-107">Depending on the RBAC provider and the permission type (delegated or application) that is needed, choose from the following table the least privileged permission required to call this API.</span></span> <span data-ttu-id="eb472-108">若要了解其他信息， [在](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) 特权权限之前要特别小心，在"权限" [中搜索](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="eb472-108">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eb472-109">支持的提供程序</span><span class="sxs-lookup"><span data-stu-id="eb472-109">Supported provider</span></span>      | <span data-ttu-id="eb472-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="eb472-110">Delegated (work or school account)</span></span>  | <span data-ttu-id="eb472-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="eb472-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eb472-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="eb472-112">Application</span></span> |
|:-----------------------|:------------------------------------|:---------------------------------------|:------------|
| <span data-ttu-id="eb472-113">目录</span><span class="sxs-lookup"><span data-stu-id="eb472-113">Directory</span></span> | <span data-ttu-id="eb472-114">RoleManagement.Read.Directory、Directory.Read.All、RoleManagement.ReadWrite.Directory、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="eb472-114">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> | <span data-ttu-id="eb472-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="eb472-115">Not supported.</span></span>| <span data-ttu-id="eb472-116">RoleManagement.Read.Directory、Directory.Read.All、RoleManagement.ReadWrite.Directory、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eb472-116">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="eb472-117">权利管理</span><span class="sxs-lookup"><span data-stu-id="eb472-117">Entitlement management</span></span> | <span data-ttu-id="eb472-118">EntitlementManagement.Read.All、EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eb472-118">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> | <span data-ttu-id="eb472-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="eb472-119">Not supported.</span></span> | <span data-ttu-id="eb472-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="eb472-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="eb472-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="eb472-121">HTTP request</span></span>

<span data-ttu-id="eb472-122">获取角色分配提供程序的名称：</span><span class="sxs-lookup"><span data-stu-id="eb472-122">Get a role assignment for a directory provider:</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /roleManagement/directory/roleAssignments/{id}
```

<span data-ttu-id="eb472-123">获取角色分配管理提供程序的信息：</span><span class="sxs-lookup"><span data-stu-id="eb472-123">Get a role assignment for the entitlement management provider:</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /roleManagement/entitlementManagement/roleAssignments/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="eb472-124">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="eb472-124">Optional query parameters</span></span>

<span data-ttu-id="eb472-125">此方法支持 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="eb472-125">This method supports OData query parameters to help customize the response.</span></span> <span data-ttu-id="eb472-126">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="eb472-126">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="eb472-127">请求标头</span><span class="sxs-lookup"><span data-stu-id="eb472-127">Request headers</span></span>

| <span data-ttu-id="eb472-128">名称</span><span class="sxs-lookup"><span data-stu-id="eb472-128">Name</span></span>      |<span data-ttu-id="eb472-129">说明</span><span class="sxs-lookup"><span data-stu-id="eb472-129">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="eb472-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="eb472-130">Authorization</span></span> | <span data-ttu-id="eb472-131">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="eb472-131">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="eb472-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="eb472-132">Request body</span></span>

<span data-ttu-id="eb472-133">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="eb472-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eb472-134">响应</span><span class="sxs-lookup"><span data-stu-id="eb472-134">Response</span></span>

<span data-ttu-id="eb472-135">如果成功，此方法在响应正文中返回 响应代码和请求的 `200 OK` [unifiedRoleAssignment](../resources/unifiedroleassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="eb472-135">If successful, this method returns a `200 OK` response code and the requested [unifiedRoleAssignment](../resources/unifiedroleassignment.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="eb472-136">示例</span><span class="sxs-lookup"><span data-stu-id="eb472-136">Examples</span></span>

### <a name="example-1--get-details-of-a-role-assignment"></a><span data-ttu-id="eb472-137">示例 1：获取角色分配</span><span class="sxs-lookup"><span data-stu-id="eb472-137">Example 1 : Get details of a role assignment</span></span>

#### <a name="request"></a><span data-ttu-id="eb472-138">请求</span><span class="sxs-lookup"><span data-stu-id="eb472-138">Request</span></span>

<span data-ttu-id="eb472-139">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="eb472-139">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="eb472-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="eb472-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_unifiedroleassignment_1"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/directory/roleAssignments/lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1
```
# <a name="c"></a>[<span data-ttu-id="eb472-141">C#</span><span class="sxs-lookup"><span data-stu-id="eb472-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-unifiedroleassignment-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="eb472-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="eb472-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-unifiedroleassignment-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="eb472-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="eb472-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-unifiedroleassignment-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="eb472-144">Java</span><span class="sxs-lookup"><span data-stu-id="eb472-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-unifiedroleassignment-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="eb472-145">响应</span><span class="sxs-lookup"><span data-stu-id="eb472-145">Response</span></span>

<span data-ttu-id="eb472-146">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="eb472-146">The following is an example of the response.</span></span>

> <span data-ttu-id="eb472-147">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="eb472-147">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-2-get-details-of-a-role-assignment-with-expand"></a><span data-ttu-id="eb472-148">示例 2：使用 获取角色分配的详细信息 `$expand`</span><span class="sxs-lookup"><span data-stu-id="eb472-148">Example 2: Get details of a role assignment with `$expand`</span></span>

#### <a name="request"></a><span data-ttu-id="eb472-149">请求</span><span class="sxs-lookup"><span data-stu-id="eb472-149">Request</span></span>

<span data-ttu-id="eb472-150">下面是一个包含查询参数 `$expand` 的请求示例。</span><span class="sxs-lookup"><span data-stu-id="eb472-150">The following is an example of the request with the `$expand` query parameter.</span></span>


# <a name="http"></a>[<span data-ttu-id="eb472-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="eb472-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_unifiedroleassignment_2"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/directory/roleAssignments/lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1?$expand=roleDefinition,principal,directoryScope
```
# <a name="c"></a>[<span data-ttu-id="eb472-152">C#</span><span class="sxs-lookup"><span data-stu-id="eb472-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-unifiedroleassignment-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="eb472-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="eb472-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-unifiedroleassignment-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="eb472-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="eb472-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-unifiedroleassignment-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="eb472-155">Java</span><span class="sxs-lookup"><span data-stu-id="eb472-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-unifiedroleassignment-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="eb472-156">响应</span><span class="sxs-lookup"><span data-stu-id="eb472-156">Response</span></span>

<span data-ttu-id="eb472-157">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="eb472-157">The following is an example of the response.</span></span>
> <span data-ttu-id="eb472-158">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="eb472-158">**Note:** The response object shown here might be shortened for readability.</span></span>

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



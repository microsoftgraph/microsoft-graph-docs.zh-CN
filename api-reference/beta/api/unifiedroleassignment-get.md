---
title: 获取 unifiedRoleAssignment
description: 检索 unifiedRoleAssignment 对象的属性和关系。
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: f40465ac0e6c7bb4f9a2419063e3b91a647128e0
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52050743"
---
# <a name="get-unifiedroleassignment"></a><span data-ttu-id="a7dd5-103">获取 unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="a7dd5-103">Get unifiedRoleAssignment</span></span>

<span data-ttu-id="a7dd5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a7dd5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a7dd5-105">检索 [unifiedRoleAssignment](../resources/unifiedroleassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a7dd5-105">Retrieve the properties and relationships of a [unifiedRoleAssignment](../resources/unifiedroleassignment.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a7dd5-106">权限</span><span class="sxs-lookup"><span data-stu-id="a7dd5-106">Permissions</span></span>

<span data-ttu-id="a7dd5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a7dd5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a7dd5-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="a7dd5-109">Permission type</span></span>      | <span data-ttu-id="a7dd5-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a7dd5-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a7dd5-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a7dd5-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a7dd5-112">RoleManagement.Read.Directory、Directory.Read.All、RoleManagement.ReadWrite.Directory、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a7dd5-112">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a7dd5-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a7dd5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a7dd5-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="a7dd5-114">Not supported.</span></span>    |
|<span data-ttu-id="a7dd5-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="a7dd5-115">Application</span></span> | <span data-ttu-id="a7dd5-116">RoleManagement.Read.Directory、Directory.Read.All、RoleManagement.ReadWrite.Directory、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a7dd5-116">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a7dd5-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a7dd5-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /roleManagement/directory/roleAssignments/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a7dd5-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="a7dd5-118">Optional query parameters</span></span>

<span data-ttu-id="a7dd5-119">此方法支持 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="a7dd5-119">This method supports OData query parameters to help customize the response.</span></span> <span data-ttu-id="a7dd5-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="a7dd5-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="a7dd5-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="a7dd5-121">Request headers</span></span>

| <span data-ttu-id="a7dd5-122">名称</span><span class="sxs-lookup"><span data-stu-id="a7dd5-122">Name</span></span>      |<span data-ttu-id="a7dd5-123">说明</span><span class="sxs-lookup"><span data-stu-id="a7dd5-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a7dd5-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="a7dd5-124">Authorization</span></span> | <span data-ttu-id="a7dd5-125">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="a7dd5-125">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="a7dd5-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="a7dd5-126">Request body</span></span>

<span data-ttu-id="a7dd5-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a7dd5-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a7dd5-128">响应</span><span class="sxs-lookup"><span data-stu-id="a7dd5-128">Response</span></span>

<span data-ttu-id="a7dd5-129">如果成功，此方法在响应正文中返回 响应代码和请求的 `200 OK` [unifiedRoleAssignment](../resources/unifiedroleassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a7dd5-129">If successful, this method returns a `200 OK` response code and the requested [unifiedRoleAssignment](../resources/unifiedroleassignment.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a7dd5-130">示例</span><span class="sxs-lookup"><span data-stu-id="a7dd5-130">Examples</span></span>

### <a name="example-1--get-details-of-a-role-assignment"></a><span data-ttu-id="a7dd5-131">示例 1：获取角色分配</span><span class="sxs-lookup"><span data-stu-id="a7dd5-131">Example 1 : Get details of a role assignment</span></span>

#### <a name="request"></a><span data-ttu-id="a7dd5-132">请求</span><span class="sxs-lookup"><span data-stu-id="a7dd5-132">Request</span></span>

<span data-ttu-id="a7dd5-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a7dd5-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="a7dd5-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="a7dd5-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_unifiedroleassignment_1"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/directory/roleAssignments/lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1
```
# <a name="c"></a>[<span data-ttu-id="a7dd5-135">C#</span><span class="sxs-lookup"><span data-stu-id="a7dd5-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-unifiedroleassignment-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a7dd5-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a7dd5-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-unifiedroleassignment-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a7dd5-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a7dd5-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-unifiedroleassignment-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a7dd5-138">Java</span><span class="sxs-lookup"><span data-stu-id="a7dd5-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-unifiedroleassignment-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a7dd5-139">响应</span><span class="sxs-lookup"><span data-stu-id="a7dd5-139">Response</span></span>

<span data-ttu-id="a7dd5-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="a7dd5-140">The following is an example of the response.</span></span>

> <span data-ttu-id="a7dd5-141">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="a7dd5-141">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-2-get-details-of-a-role-assignment-with-expand"></a><span data-ttu-id="a7dd5-142">示例 2：使用 获取角色分配的详细信息 `$expand`</span><span class="sxs-lookup"><span data-stu-id="a7dd5-142">Example 2: Get details of a role assignment with `$expand`</span></span>

#### <a name="request"></a><span data-ttu-id="a7dd5-143">请求</span><span class="sxs-lookup"><span data-stu-id="a7dd5-143">Request</span></span>

<span data-ttu-id="a7dd5-144">下面是一个包含查询参数 `$expand` 的请求示例。</span><span class="sxs-lookup"><span data-stu-id="a7dd5-144">The following is an example of the request with the `$expand` query parameter.</span></span>


# <a name="http"></a>[<span data-ttu-id="a7dd5-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="a7dd5-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_unifiedroleassignment_2"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/directory/roleAssignments/lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1?$expand=roleDefinition,principal,directoryScope
```
# <a name="c"></a>[<span data-ttu-id="a7dd5-146">C#</span><span class="sxs-lookup"><span data-stu-id="a7dd5-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-unifiedroleassignment-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a7dd5-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a7dd5-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-unifiedroleassignment-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a7dd5-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a7dd5-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-unifiedroleassignment-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a7dd5-149">Java</span><span class="sxs-lookup"><span data-stu-id="a7dd5-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-unifiedroleassignment-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a7dd5-150">响应</span><span class="sxs-lookup"><span data-stu-id="a7dd5-150">Response</span></span>

<span data-ttu-id="a7dd5-151">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="a7dd5-151">The following is an example of the response.</span></span>
> <span data-ttu-id="a7dd5-152">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="a7dd5-152">**Note:** The response object shown here might be shortened for readability.</span></span>

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



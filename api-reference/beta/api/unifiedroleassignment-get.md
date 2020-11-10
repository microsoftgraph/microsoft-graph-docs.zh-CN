---
title: 获取 unifiedRoleAssignment
description: 检索 unifiedRoleAssignment 对象的属性和关系。
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: dda763b8b50a0a02e1bd826739095a81e9d85b22
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48978911"
---
# <a name="get-unifiedroleassignment"></a><span data-ttu-id="7226f-103">获取 unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="7226f-103">Get unifiedRoleAssignment</span></span>

<span data-ttu-id="7226f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7226f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7226f-105">检索 [unifiedRoleAssignment](../resources/unifiedroleassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="7226f-105">Retrieve the properties and relationships of a [unifiedRoleAssignment](../resources/unifiedroleassignment.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="7226f-106">权限</span><span class="sxs-lookup"><span data-stu-id="7226f-106">Permissions</span></span>

<span data-ttu-id="7226f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7226f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7226f-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="7226f-109">Permission type</span></span>      | <span data-ttu-id="7226f-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7226f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7226f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7226f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7226f-112">RoleManagement、RoleManagement、Directory.accessasuser.all、all、、all、all 和的所有子目录。</span><span class="sxs-lookup"><span data-stu-id="7226f-112">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7226f-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7226f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7226f-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="7226f-114">Not supported.</span></span>    |
|<span data-ttu-id="7226f-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="7226f-115">Application</span></span> | <span data-ttu-id="7226f-116">RoleManagement、RoleManagement、目录和所有读写的所有子目录。所有</span><span class="sxs-lookup"><span data-stu-id="7226f-116">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7226f-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7226f-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /roleManagement/directory/roleAssignments/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7226f-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="7226f-118">Optional query parameters</span></span>

<span data-ttu-id="7226f-119">此方法支持 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="7226f-119">This method supports OData query parameters to help customize the response.</span></span> <span data-ttu-id="7226f-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="7226f-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="7226f-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="7226f-121">Request headers</span></span>

| <span data-ttu-id="7226f-122">名称</span><span class="sxs-lookup"><span data-stu-id="7226f-122">Name</span></span>      |<span data-ttu-id="7226f-123">说明</span><span class="sxs-lookup"><span data-stu-id="7226f-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7226f-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="7226f-124">Authorization</span></span> | <span data-ttu-id="7226f-125">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="7226f-125">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="7226f-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="7226f-126">Request body</span></span>

<span data-ttu-id="7226f-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7226f-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7226f-128">响应</span><span class="sxs-lookup"><span data-stu-id="7226f-128">Response</span></span>

<span data-ttu-id="7226f-129">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和请求的 [unifiedRoleAssignment](../resources/unifiedroleassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7226f-129">If successful, this method returns a `200 OK` response code and the requested [unifiedRoleAssignment](../resources/unifiedroleassignment.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7226f-130">示例</span><span class="sxs-lookup"><span data-stu-id="7226f-130">Examples</span></span>

### <a name="example-1--get-details-of-a-role-assignment"></a><span data-ttu-id="7226f-131">示例1：获取角色分配的详细信息</span><span class="sxs-lookup"><span data-stu-id="7226f-131">Example 1 : Get details of a role assignment</span></span>

#### <a name="request"></a><span data-ttu-id="7226f-132">请求</span><span class="sxs-lookup"><span data-stu-id="7226f-132">Request</span></span>

<span data-ttu-id="7226f-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="7226f-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="7226f-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="7226f-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_unifiedroleassignment"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/directory/roleAssignments/lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1
```
# <a name="c"></a>[<span data-ttu-id="7226f-135">C#</span><span class="sxs-lookup"><span data-stu-id="7226f-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-unifiedroleassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7226f-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7226f-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-unifiedroleassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7226f-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7226f-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-unifiedroleassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7226f-138">Java</span><span class="sxs-lookup"><span data-stu-id="7226f-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-unifiedroleassignment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="7226f-139">响应</span><span class="sxs-lookup"><span data-stu-id="7226f-139">Response</span></span>

<span data-ttu-id="7226f-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="7226f-140">The following is an example of the response.</span></span>

> <span data-ttu-id="7226f-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="7226f-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-details-of-a-role-assignment-with-expand"></a><span data-ttu-id="7226f-143">示例2：获取角色分配的详细信息 `$expand`</span><span class="sxs-lookup"><span data-stu-id="7226f-143">Example 2: Get details of a role assignment with `$expand`</span></span>

#### <a name="request"></a><span data-ttu-id="7226f-144">请求</span><span class="sxs-lookup"><span data-stu-id="7226f-144">Request</span></span>

<span data-ttu-id="7226f-145">以下是包含查询参数的请求的示例 `$expand` 。</span><span class="sxs-lookup"><span data-stu-id="7226f-145">The following is an example of the request with the `$expand` query parameter.</span></span>


# <a name="http"></a>[<span data-ttu-id="7226f-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="7226f-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_unifiedroleassignment"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/directory/roleAssignments/lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1?$expand=roleDefinition,principal,directoryScope
```
# <a name="c"></a>[<span data-ttu-id="7226f-147">C#</span><span class="sxs-lookup"><span data-stu-id="7226f-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-unifiedroleassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7226f-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7226f-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-unifiedroleassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7226f-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7226f-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-unifiedroleassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7226f-150">Java</span><span class="sxs-lookup"><span data-stu-id="7226f-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-unifiedroleassignment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="7226f-151">响应</span><span class="sxs-lookup"><span data-stu-id="7226f-151">Response</span></span>

<span data-ttu-id="7226f-152">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="7226f-152">The following is an example of the response.</span></span>
> <span data-ttu-id="7226f-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="7226f-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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



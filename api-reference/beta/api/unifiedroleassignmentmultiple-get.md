---
title: 获取 unifiedRoleAssignmentMultiple
description: 检索 unifiedRoleAssignmentMultiple 对象的属性和关系。
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: d7d387736e1b59a4afd04558433d68a17d2bedb2
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2021
ms.locfileid: "52869966"
---
# <a name="get-unifiedroleassignmentmultiple"></a><span data-ttu-id="a3323-103">获取 unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="a3323-103">Get unifiedRoleAssignmentMultiple</span></span>

<span data-ttu-id="a3323-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a3323-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a3323-105">获取 RBAC 提供程序 [的 unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a3323-105">Get the properties and relationships of a [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) object of an RBAC provider.</span></span> 

<span data-ttu-id="a3323-106">目前支持以下 RBAC 提供程序：</span><span class="sxs-lookup"><span data-stu-id="a3323-106">The following RBAC providers are currently supported:</span></span>
- <span data-ttu-id="a3323-107">云电脑</span><span class="sxs-lookup"><span data-stu-id="a3323-107">cloud PC</span></span> 
- <span data-ttu-id="a3323-108">Intune (设备) </span><span class="sxs-lookup"><span data-stu-id="a3323-108">device management (Intune)</span></span>

<span data-ttu-id="a3323-109">For other Microsoft 365 applications (like Azure AD) ， use [unifiedRoleAssignment](../resources/unifiedroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="a3323-109">For other Microsoft 365 applications (like Azure AD), use [unifiedRoleAssignment](../resources/unifiedroleassignment.md).</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="a3323-110">权限</span><span class="sxs-lookup"><span data-stu-id="a3323-110">Permissions</span></span>

<span data-ttu-id="a3323-111">根据 RBAC 提供程序以及 (或应用程序) 的权限类型，从下表中选择调用此 API 所需的最低特权权限。</span><span class="sxs-lookup"><span data-stu-id="a3323-111">Depending on the RBAC provider and the permission type (delegated or application) that is needed, choose from the following table the least privileged permission required to call this API.</span></span> <span data-ttu-id="a3323-112">若要了解详细信息，包括在选择更多特权之前的[注意事项](/graph/auth/auth-concepts#best-practices-for-requesting-permissions)，请在“[权限](/graph/permissions-reference)”中搜索以下权限。</span><span class="sxs-lookup"><span data-stu-id="a3323-112">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in [Permissions](/graph/permissions-reference).</span></span> 

|<span data-ttu-id="a3323-113">支持的提供程序</span><span class="sxs-lookup"><span data-stu-id="a3323-113">Supported provider</span></span>      | <span data-ttu-id="a3323-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a3323-114">Delegated (work or school account)</span></span>  | <span data-ttu-id="a3323-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a3323-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a3323-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="a3323-116">Application</span></span> |
|:-----------------------|:------------------------------------|:---------------------------------------|:------------|
| <span data-ttu-id="a3323-117">Cloud PC</span><span class="sxs-lookup"><span data-stu-id="a3323-117">Cloud PC</span></span> | <span data-ttu-id="a3323-118">CloudPC.Read.All、CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a3323-118">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span> | <span data-ttu-id="a3323-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="a3323-119">Not supported.</span></span> | <span data-ttu-id="a3323-120">CloudPC.Read.All、CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a3323-120">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span> |
| <span data-ttu-id="a3323-121">Intune</span><span class="sxs-lookup"><span data-stu-id="a3323-121">Intune</span></span> | <span data-ttu-id="a3323-122">DeviceManagementRBAC.Read.All、DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a3323-122">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span></span> | <span data-ttu-id="a3323-123">不支持。</span><span class="sxs-lookup"><span data-stu-id="a3323-123">Not supported.</span></span>| <span data-ttu-id="a3323-124">DeviceManagementRBAC.Read.All、DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a3323-124">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a3323-125">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a3323-125">HTTP request</span></span>

<span data-ttu-id="a3323-126">若要获取云电脑提供商的 unifiedRoleAssignmentMultiple 的属性和关系：</span><span class="sxs-lookup"><span data-stu-id="a3323-126">To get the properties and relationships of a unifiedRoleAssignmentMultiple for a cloud PC provider:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /roleManagement/cloudPC/roleAssignments/{id}
```

<span data-ttu-id="a3323-127">若要获取 Intune 提供程序的 unifiedRoleAssignmentMultiple 的属性和关系：</span><span class="sxs-lookup"><span data-stu-id="a3323-127">To get the properties and relationships of a unifiedRoleAssignmentMultiple for an Intune provider:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /roleManagement/deviceManagement/roleAssignments/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a3323-128">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="a3323-128">Optional query parameters</span></span>

<span data-ttu-id="a3323-129">此方法支持 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="a3323-129">This method supports OData query parameters to help customize the response.</span></span> <span data-ttu-id="a3323-130">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="a3323-130">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="a3323-131">请求标头</span><span class="sxs-lookup"><span data-stu-id="a3323-131">Request headers</span></span>

| <span data-ttu-id="a3323-132">名称</span><span class="sxs-lookup"><span data-stu-id="a3323-132">Name</span></span>  | <span data-ttu-id="a3323-133">说明</span><span class="sxs-lookup"><span data-stu-id="a3323-133">Description</span></span> |
|:----- |:----------- |
| <span data-ttu-id="a3323-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="a3323-134">Authorization</span></span> | <span data-ttu-id="a3323-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a3323-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a3323-137">请求正文</span><span class="sxs-lookup"><span data-stu-id="a3323-137">Request body</span></span>

<span data-ttu-id="a3323-138">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a3323-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a3323-139">响应</span><span class="sxs-lookup"><span data-stu-id="a3323-139">Response</span></span>

<span data-ttu-id="a3323-140">如果成功，此方法在响应正文中返回 响应代码和请求的 `200 OK` [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a3323-140">If successful, this method returns a `200 OK` response code and the requested [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a3323-141">示例</span><span class="sxs-lookup"><span data-stu-id="a3323-141">Examples</span></span>

### <a name="example-1-get-a-directory-scoped-roleassignmentmultiple-in-an-intune-provider"></a><span data-ttu-id="a3323-142">示例 1：获取 Intune 提供程序中的目录作用域角色AssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="a3323-142">Example 1: Get a directory-scoped roleAssignmentMultiple in an Intune provider</span></span>

#### <a name="request"></a><span data-ttu-id="a3323-143">请求</span><span class="sxs-lookup"><span data-stu-id="a3323-143">Request</span></span>

<span data-ttu-id="a3323-144">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a3323-144">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="a3323-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="a3323-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_unifiedroleassignmentmultiple_1"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/deviceManagement/roleAssignments/lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1
```
# <a name="c"></a>[<span data-ttu-id="a3323-146">C#</span><span class="sxs-lookup"><span data-stu-id="a3323-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-unifiedroleassignmentmultiple-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a3323-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a3323-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-unifiedroleassignmentmultiple-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a3323-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a3323-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-unifiedroleassignmentmultiple-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a3323-149">Java</span><span class="sxs-lookup"><span data-stu-id="a3323-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-unifiedroleassignmentmultiple-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a3323-150">响应</span><span class="sxs-lookup"><span data-stu-id="a3323-150">Response</span></span>

<span data-ttu-id="a3323-151">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="a3323-151">The following is an example of the response.</span></span>
> <span data-ttu-id="a3323-152">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="a3323-152">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignment"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/deviceManagement/roleAssignments/$entity",
    "@odata.type": "#microsoft.graph.unifiedRoleAssignmentMultiple",
    "id": "lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1",
    "roleDefinitionId": "62e90394-69f5-4237-9190-012177145e10",
    "principalIds[]": ["4ab0b690-479b-47ff-af8f-2576cf521872", "f8ca5a85-489a-49a0-b555-0a6d81e56f0d"],
    "directoryScopeIds[]": ["28ca5a85-489a-49a0-b555-0a6d81e56f0", "8152656a-cf9a-4928-a457-1512d4cae295"]
}
```

### <a name="example-2-get-a-roleassignmentmultiple-assigned-to-a-group-in-an-intune-provider"></a><span data-ttu-id="a3323-153">示例 2：获取分配给 Intune 提供程序中的组的 roleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="a3323-153">Example 2: Get a roleAssignmentMultiple assigned to a group in an Intune provider</span></span>

#### <a name="request"></a><span data-ttu-id="a3323-154">请求</span><span class="sxs-lookup"><span data-stu-id="a3323-154">Request</span></span>

<span data-ttu-id="a3323-155">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a3323-155">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="a3323-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="a3323-156">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_unifiedroleassignmentmultiple_2"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/deviceManagement/roleAssignments?$filter = principalIds/any(x:x eq '564ae70c-73d9-476b-820b-fb61eb7384b9')
```
# <a name="c"></a>[<span data-ttu-id="a3323-157">C#</span><span class="sxs-lookup"><span data-stu-id="a3323-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-unifiedroleassignmentmultiple-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a3323-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a3323-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-unifiedroleassignmentmultiple-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a3323-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a3323-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-unifiedroleassignmentmultiple-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a3323-160">Java</span><span class="sxs-lookup"><span data-stu-id="a3323-160">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-unifiedroleassignmentmultiple-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a3323-161">响应</span><span class="sxs-lookup"><span data-stu-id="a3323-161">Response</span></span>

<span data-ttu-id="a3323-162">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="a3323-162">The following is an example of the response.</span></span>
> <span data-ttu-id="a3323-163">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="a3323-163">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignment"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/deviceManagement/roleAssignments",
    "@odata.count": 7,
    "value": [
        {
            "id": "893fc648-73fc-482b-b964-ddd1cabf0db4",
            "condition": null,
            "displayName": "Assign Contoso_App_Admin to School Admin",
            "description": "test",
            "roleDefinitionId": "2f9f4f7e-2d13-427b-adf2-361a1eef7ae8",
            "principalIds": [
                "564ae70c-73d9-476b-820b-fb61eb7384b9"
            ],
            "directoryScopeIds": [],
            "appScopeIds": [
                "0",
                "AllLicensedUsers"
            ]
        }
    ]
}
```

### <a name="example-3-get-a-directory-scoped-roleassignmentmultiple-in-an-intune-provider-with-expand"></a><span data-ttu-id="a3323-164">示例 3：获取 Intune 提供程序中具有的目录作用域角色AssignmentMultiple `$expand`</span><span class="sxs-lookup"><span data-stu-id="a3323-164">Example 3: Get a directory-scoped roleAssignmentMultiple in an Intune provider with `$expand`</span></span>

#### <a name="request"></a><span data-ttu-id="a3323-165">请求</span><span class="sxs-lookup"><span data-stu-id="a3323-165">Request</span></span>

<span data-ttu-id="a3323-166">下面是一个包含查询参数 `$expand` 的请求示例。</span><span class="sxs-lookup"><span data-stu-id="a3323-166">The following is an example of the request with the `$expand` query parameter.</span></span>


# <a name="http"></a>[<span data-ttu-id="a3323-167">HTTP</span><span class="sxs-lookup"><span data-stu-id="a3323-167">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_unifiedroleassignment_3"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/deviceManagement/roleAssignments/lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1?$expand=roleDefinition,principals,directoryScopes
```
# <a name="c"></a>[<span data-ttu-id="a3323-168">C#</span><span class="sxs-lookup"><span data-stu-id="a3323-168">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-unifiedroleassignment-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a3323-169">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a3323-169">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-unifiedroleassignment-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a3323-170">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a3323-170">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-unifiedroleassignment-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a3323-171">Java</span><span class="sxs-lookup"><span data-stu-id="a3323-171">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-unifiedroleassignment-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a3323-172">响应</span><span class="sxs-lookup"><span data-stu-id="a3323-172">Response</span></span>

<span data-ttu-id="a3323-173">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="a3323-173">The following is an example of the response.</span></span>
> <span data-ttu-id="a3323-174">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="a3323-174">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignment"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#roleManagement/deviceManagement/roleAssignments/$entity",
  "@odata.type": "#microsoft.graph.unifiedRoleAssignmentMultiple",
  "id": "lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1",
  "roleDefinitionId": "c2cf284d-6c41-4e6b-afac-4b80928c9034",
  "roleDefinition": {
    "id": "c2cf284d-6c41-4e6b-afac-4b80928c9034",
    "displayName": "Application Manager",
    "description": "Manages mobile and managed applications",
    "rolePermissions": [
      {
        "allowedResourceActions": [],
        "excludedResourceActions": [],
    }],
    "isEnabled": true,
    "isBuiltIn": true,
  },
  "principalIds": ["f8ca5a85-489a-49a0-b555-0a6d81e56f0d", "c1518aa9-4da5-4c84-a902-a31404023890"],
  "principals": [
    {
      "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups/$entity",
      "id": "f8ca5a85-489a-49a0-b555-0a6d81e56f0d",
      "displayName": "Global IT"
    },
    {
      "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups/$entity",
      "id": "c1518aa9-4da5-4c84-a902-a31404023890",
      "displayName": "Americas IT"
    }
],
  "directoryScopeIds": ["28ca5a85-489a-49a0-b555-0a6d81e56f0d", "8152656a-cf9a-4928-a457-1512d4cae295"],
  "directoryScopes": [
    {
      "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups/$entity",
      "id": "28ca5a85-489a-49a0-b555-0a6d81e56f0d",
      "displayName": "Washington Sales Region"
    },
    {
      "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups/$entity",
      "id": "8152656a-cf9a-4928-a457-1512d4cae295",
      "displayName": "Oregon Sales Region"
    }
  ]
}
```
### <a name="example-4-get-a-roleassignmentmultiple-in-a-cloud-pc-provider"></a><span data-ttu-id="a3323-175">示例 4：获取云电脑提供商中的 roleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="a3323-175">Example 4: Get a roleAssignmentMultiple in a cloud PC provider</span></span>

#### <a name="request"></a><span data-ttu-id="a3323-176">请求</span><span class="sxs-lookup"><span data-stu-id="a3323-176">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="a3323-177">HTTP</span><span class="sxs-lookup"><span data-stu-id="a3323-177">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_unifiedroleassignmentmultiple_1"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/cloudPC/roleAssignments/dbe9d288-fd87-41f4-b33d-b498ed207096
```
# <a name="c"></a>[<span data-ttu-id="a3323-178">C#</span><span class="sxs-lookup"><span data-stu-id="a3323-178">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-unifiedroleassignmentmultiple-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a3323-179">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a3323-179">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-unifiedroleassignmentmultiple-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a3323-180">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a3323-180">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-unifiedroleassignmentmultiple-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a3323-181">Java</span><span class="sxs-lookup"><span data-stu-id="a3323-181">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-unifiedroleassignmentmultiple-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a3323-182">响应</span><span class="sxs-lookup"><span data-stu-id="a3323-182">Response</span></span>
> <span data-ttu-id="a3323-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="a3323-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignment"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/cloudPC/roleAssignments/$entity",
    "id": "dbe9d288-fd87-41f4-b33d-b498ed207096",
    "description": null,
    "displayName": "My test role assignment 1",
    "roleDefinitionId": "b5c08161-a7af-481c-ace2-a20a69a48fb1",
    "principalIds": [
        "8e811502-ebda-4782-8f81-071d17f0f892",
        "30e3492f-964c-4d73-88c6-986a53c6e2a0"
    ],
    "directoryScopeIds": [
        "/"
    ],
    "appScopeIds": []
}
```

### <a name="example-5-get-a-roleassignmentmultiple-in-a-cloud-pc-provider-with-expand"></a><span data-ttu-id="a3323-185">示例 5：在云电脑提供商获取 roleAssignmentMultiple `$expand`</span><span class="sxs-lookup"><span data-stu-id="a3323-185">Example 5: Get a roleAssignmentMultiple in a cloud PC provider with `$expand`</span></span>

#### <a name="request"></a><span data-ttu-id="a3323-186">请求</span><span class="sxs-lookup"><span data-stu-id="a3323-186">Request</span></span>

<span data-ttu-id="a3323-187">下面是一个包含查询参数 `$expand` 的请求示例。</span><span class="sxs-lookup"><span data-stu-id="a3323-187">The following is an example of the request with the `$expand` query parameter.</span></span>


# <a name="http"></a>[<span data-ttu-id="a3323-188">HTTP</span><span class="sxs-lookup"><span data-stu-id="a3323-188">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_unifiedroleassignment_3"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/cloudPC/roleAssignments/dbe9d288-fd87-41f4-b33d-b498ed207096?$expand=roleDefinition
```
# <a name="c"></a>[<span data-ttu-id="a3323-189">C#</span><span class="sxs-lookup"><span data-stu-id="a3323-189">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-unifiedroleassignment-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a3323-190">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a3323-190">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-unifiedroleassignment-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a3323-191">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a3323-191">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-unifiedroleassignment-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a3323-192">Java</span><span class="sxs-lookup"><span data-stu-id="a3323-192">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-unifiedroleassignment-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a3323-193">响应</span><span class="sxs-lookup"><span data-stu-id="a3323-193">Response</span></span>
> <span data-ttu-id="a3323-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="a3323-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignment"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/cloudPC/roleAssignments/$entity",
    "@odata.type": "#microsoft.graph.unifiedRoleAssignmentMultiple",
    "id": "dbe9d288-fd87-41f4-b33d-b498ed207096",
    "roleDefinitionId": "b5c08161-a7af-481c-ace2-a20a69a48fb1",
    "principalIds": ["8e811502-ebda-4782-8f81-071d17f0f892", "30e3492f-964c-4d73-88c6-986a53c6e2a0"],
    "directoryScopeIds": [
        "/"
    ],
    "appScopeIds": [],
    "roleDefinitions": {
        "id": "b5c08161-a7af-481c-ace2-a20a69a48fb1",
        "description": "Have read and write access to all Cloud PC features.",
        "displayName": "Cloud PC Administrator",
        "isBuiltIn": true,
        "isEnabled": true,
        "resourceScopes": [
            "/"
        ],
        "templateId": "b5c08161-a7af-481c-ace2-a20a69a48fb1",
        "version": null,
        "rolePermissions": [
            {
                "allowedResourceActions": [
                    "Microsoft.CloudPC/CloudPCs/Read",
                    "Microsoft.CloudPC/CloudPCs/Reprovision",
                    "Microsoft.CloudPC/DeviceImages/Create",
                    "Microsoft.CloudPC/DeviceImages/Delete",
                    "Microsoft.CloudPC/DeviceImages/Read",
                    "Microsoft.CloudPC/OnPremisesConnections/Create",
                    "Microsoft.CloudPC/OnPremisesConnections/Delete",
                    "Microsoft.CloudPC/OnPremisesConnections/Read",
                    "Microsoft.CloudPC/OnPremisesConnections/Update",
                    "Microsoft.CloudPC/OnPremisesConnections/RunHealthChecks",
                    "Microsoft.CloudPC/OnPremisesConnections/UpdateAdDomainPassword",
                    "Microsoft.CloudPC/ProvisioningPolicies/Assign",
                    "Microsoft.CloudPC/ProvisioningPolicies/Create",
                    "Microsoft.CloudPC/ProvisioningPolicies/Delete",
                    "Microsoft.CloudPC/ProvisioningPolicies/Read",
                    "Microsoft.CloudPC/ProvisioningPolicies/Update",
                    "Microsoft.CloudPC/RoleAssignments/Create",
                    "Microsoft.CloudPC/RoleAssignments/Update",
                    "Microsoft.CloudPC/RoleAssignments/Delete",
                    "Microsoft.CloudPC/Roles/Read",
                    "Microsoft.CloudPC/SelfServiceSettings/Read",
                    "Microsoft.CloudPC/SelfServiceSettings/Update"
                ],
                "condition": null
            }
        ]
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



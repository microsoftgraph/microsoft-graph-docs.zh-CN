---
title: 获取 unifiedRoleAssignmentMultiple
description: 检索 unifiedRoleAssignmentMultiple 对象的属性和关系。
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 6b1aeecdae5b36e4c10768ee37b1505aba25687b
ms.sourcegitcommit: ae83b2b372902268517fd17a8b10d6d9add422af
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/08/2021
ms.locfileid: "53334498"
---
# <a name="get-unifiedroleassignmentmultiple"></a><span data-ttu-id="96da4-103">获取 unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="96da4-103">Get unifiedRoleAssignmentMultiple</span></span>

<span data-ttu-id="96da4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="96da4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="96da4-105">获取 RBAC 提供程序 [的 unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="96da4-105">Get the properties and relationships of a [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) object of an RBAC provider.</span></span> 

<span data-ttu-id="96da4-106">目前支持以下 RBAC 提供程序：</span><span class="sxs-lookup"><span data-stu-id="96da4-106">The following RBAC providers are currently supported:</span></span>
- <span data-ttu-id="96da4-107">云电脑</span><span class="sxs-lookup"><span data-stu-id="96da4-107">cloud PC</span></span> 
- <span data-ttu-id="96da4-108">Intune (设备) </span><span class="sxs-lookup"><span data-stu-id="96da4-108">device management (Intune)</span></span>

<span data-ttu-id="96da4-109">For other Microsoft 365 applications (like Azure AD) ， use [unifiedRoleAssignment](../resources/unifiedroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="96da4-109">For other Microsoft 365 applications (like Azure AD), use [unifiedRoleAssignment](../resources/unifiedroleassignment.md).</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="96da4-110">权限</span><span class="sxs-lookup"><span data-stu-id="96da4-110">Permissions</span></span>

<span data-ttu-id="96da4-111">根据 RBAC 提供程序以及 (或应用程序) 的权限类型，从下表中选择调用此 API 所需的最低特权权限。</span><span class="sxs-lookup"><span data-stu-id="96da4-111">Depending on the RBAC provider and the permission type (delegated or application) that is needed, choose from the following table the least privileged permission required to call this API.</span></span> <span data-ttu-id="96da4-112">若要了解 [更多信息，包括在](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) 选择更多特权权限之前保持谨慎，请参阅 [权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="96da4-112">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, see [Permissions](/graph/permissions-reference).</span></span> 

### <a name="for-cloud-pc-provider"></a><span data-ttu-id="96da4-113">对于云电脑提供商</span><span class="sxs-lookup"><span data-stu-id="96da4-113">For Cloud PC provider</span></span>

|<span data-ttu-id="96da4-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="96da4-114">Permission type</span></span>      | <span data-ttu-id="96da4-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="96da4-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="96da4-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="96da4-116">Delegated (work or school account)</span></span> |  <span data-ttu-id="96da4-117">CloudPC.Read.All、CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96da4-117">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>   |
|<span data-ttu-id="96da4-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="96da4-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="96da4-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="96da4-119">Not supported.</span></span>    |
|<span data-ttu-id="96da4-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="96da4-120">Application</span></span> | <span data-ttu-id="96da4-121">CloudPC.Read.All、CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96da4-121">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>  |

### <a name="for-device-management-intune-provider"></a><span data-ttu-id="96da4-122">对于 Intune (提供程序的设备) 管理</span><span class="sxs-lookup"><span data-stu-id="96da4-122">For Device management (Intune) provider</span></span>

|<span data-ttu-id="96da4-123">权限类型</span><span class="sxs-lookup"><span data-stu-id="96da4-123">Permission type</span></span>      | <span data-ttu-id="96da4-124">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="96da4-124">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="96da4-125">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="96da4-125">Delegated (work or school account)</span></span> |  <span data-ttu-id="96da4-126">DeviceManagementRBAC.Read.All、DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96da4-126">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span></span>   |
|<span data-ttu-id="96da4-127">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="96da4-127">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="96da4-128">不支持。</span><span class="sxs-lookup"><span data-stu-id="96da4-128">Not supported.</span></span>    |
|<span data-ttu-id="96da4-129">应用程序</span><span class="sxs-lookup"><span data-stu-id="96da4-129">Application</span></span> | <span data-ttu-id="96da4-130">DeviceManagementRBAC.Read.All、DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96da4-130">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span></span> |



## <a name="http-request"></a><span data-ttu-id="96da4-131">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="96da4-131">HTTP request</span></span>

<span data-ttu-id="96da4-132">若要获取云电脑提供商的 unifiedRoleAssignmentMultiple 的属性和关系：</span><span class="sxs-lookup"><span data-stu-id="96da4-132">To get the properties and relationships of a unifiedRoleAssignmentMultiple for a cloud PC provider:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /roleManagement/cloudPC/roleAssignments/{id}
```

<span data-ttu-id="96da4-133">若要获取 Intune 提供程序的 unifiedRoleAssignmentMultiple 的属性和关系：</span><span class="sxs-lookup"><span data-stu-id="96da4-133">To get the properties and relationships of a unifiedRoleAssignmentMultiple for an Intune provider:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /roleManagement/deviceManagement/roleAssignments/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="96da4-134">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="96da4-134">Optional query parameters</span></span>

<span data-ttu-id="96da4-135">此方法支持 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="96da4-135">This method supports OData query parameters to help customize the response.</span></span> <span data-ttu-id="96da4-136">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="96da4-136">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="96da4-137">请求标头</span><span class="sxs-lookup"><span data-stu-id="96da4-137">Request headers</span></span>

| <span data-ttu-id="96da4-138">名称</span><span class="sxs-lookup"><span data-stu-id="96da4-138">Name</span></span>  | <span data-ttu-id="96da4-139">说明</span><span class="sxs-lookup"><span data-stu-id="96da4-139">Description</span></span> |
|:----- |:----------- |
| <span data-ttu-id="96da4-140">Authorization</span><span class="sxs-lookup"><span data-stu-id="96da4-140">Authorization</span></span> | <span data-ttu-id="96da4-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="96da4-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="96da4-143">请求正文</span><span class="sxs-lookup"><span data-stu-id="96da4-143">Request body</span></span>

<span data-ttu-id="96da4-144">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="96da4-144">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="96da4-145">响应</span><span class="sxs-lookup"><span data-stu-id="96da4-145">Response</span></span>

<span data-ttu-id="96da4-146">如果成功，此方法在响应正文中返回 响应代码和请求的 `200 OK` [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="96da4-146">If successful, this method returns a `200 OK` response code and the requested [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="96da4-147">示例</span><span class="sxs-lookup"><span data-stu-id="96da4-147">Examples</span></span>

### <a name="example-1-get-a-directory-scoped-roleassignmentmultiple-in-an-intune-provider"></a><span data-ttu-id="96da4-148">示例 1：获取 Intune 提供程序中的目录作用域角色AssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="96da4-148">Example 1: Get a directory-scoped roleAssignmentMultiple in an Intune provider</span></span>

#### <a name="request"></a><span data-ttu-id="96da4-149">请求</span><span class="sxs-lookup"><span data-stu-id="96da4-149">Request</span></span>

<span data-ttu-id="96da4-150">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="96da4-150">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="96da4-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="96da4-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_unifiedroleassignmentmultiple_1"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/deviceManagement/roleAssignments/lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1
```
# <a name="c"></a>[<span data-ttu-id="96da4-152">C#</span><span class="sxs-lookup"><span data-stu-id="96da4-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-unifiedroleassignmentmultiple-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="96da4-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="96da4-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-unifiedroleassignmentmultiple-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="96da4-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="96da4-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-unifiedroleassignmentmultiple-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="96da4-155">Java</span><span class="sxs-lookup"><span data-stu-id="96da4-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-unifiedroleassignmentmultiple-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="96da4-156">响应</span><span class="sxs-lookup"><span data-stu-id="96da4-156">Response</span></span>

<span data-ttu-id="96da4-157">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="96da4-157">The following is an example of the response.</span></span>
> <span data-ttu-id="96da4-158">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="96da4-158">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-2-get-a-roleassignmentmultiple-assigned-to-a-group-in-an-intune-provider"></a><span data-ttu-id="96da4-159">示例 2：获取分配给 Intune 提供程序中的组的 roleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="96da4-159">Example 2: Get a roleAssignmentMultiple assigned to a group in an Intune provider</span></span>

#### <a name="request"></a><span data-ttu-id="96da4-160">请求</span><span class="sxs-lookup"><span data-stu-id="96da4-160">Request</span></span>

<span data-ttu-id="96da4-161">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="96da4-161">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="96da4-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="96da4-162">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_unifiedroleassignmentmultiple_2"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/deviceManagement/roleAssignments?$filter = principalIds/any(x:x eq '564ae70c-73d9-476b-820b-fb61eb7384b9')
```
# <a name="c"></a>[<span data-ttu-id="96da4-163">C#</span><span class="sxs-lookup"><span data-stu-id="96da4-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-unifiedroleassignmentmultiple-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="96da4-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="96da4-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-unifiedroleassignmentmultiple-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="96da4-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="96da4-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-unifiedroleassignmentmultiple-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="96da4-166">Java</span><span class="sxs-lookup"><span data-stu-id="96da4-166">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-unifiedroleassignmentmultiple-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="96da4-167">响应</span><span class="sxs-lookup"><span data-stu-id="96da4-167">Response</span></span>

<span data-ttu-id="96da4-168">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="96da4-168">The following is an example of the response.</span></span>
> <span data-ttu-id="96da4-169">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="96da4-169">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-3-get-a-directory-scoped-roleassignmentmultiple-in-an-intune-provider-with-expand"></a><span data-ttu-id="96da4-170">示例 3：获取 Intune 提供程序中具有的目录作用域角色AssignmentMultiple `$expand`</span><span class="sxs-lookup"><span data-stu-id="96da4-170">Example 3: Get a directory-scoped roleAssignmentMultiple in an Intune provider with `$expand`</span></span>

#### <a name="request"></a><span data-ttu-id="96da4-171">请求</span><span class="sxs-lookup"><span data-stu-id="96da4-171">Request</span></span>

<span data-ttu-id="96da4-172">下面是一个包含查询参数 `$expand` 的请求示例。</span><span class="sxs-lookup"><span data-stu-id="96da4-172">The following is an example of the request with the `$expand` query parameter.</span></span>


# <a name="http"></a>[<span data-ttu-id="96da4-173">HTTP</span><span class="sxs-lookup"><span data-stu-id="96da4-173">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_unifiedroleassignment_3"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/deviceManagement/roleAssignments/lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1?$expand=roleDefinition,principals,directoryScopes
```
# <a name="c"></a>[<span data-ttu-id="96da4-174">C#</span><span class="sxs-lookup"><span data-stu-id="96da4-174">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-unifiedroleassignment-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="96da4-175">JavaScript</span><span class="sxs-lookup"><span data-stu-id="96da4-175">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-unifiedroleassignment-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="96da4-176">Objective-C</span><span class="sxs-lookup"><span data-stu-id="96da4-176">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-unifiedroleassignment-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="96da4-177">Java</span><span class="sxs-lookup"><span data-stu-id="96da4-177">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-unifiedroleassignment-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="96da4-178">响应</span><span class="sxs-lookup"><span data-stu-id="96da4-178">Response</span></span>

<span data-ttu-id="96da4-179">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="96da4-179">The following is an example of the response.</span></span>
> <span data-ttu-id="96da4-180">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="96da4-180">**Note:** The response object shown here might be shortened for readability.</span></span>

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
### <a name="example-4-get-a-roleassignmentmultiple-in-a-cloud-pc-provider"></a><span data-ttu-id="96da4-181">示例 4：获取云电脑提供商中的 roleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="96da4-181">Example 4: Get a roleAssignmentMultiple in a cloud PC provider</span></span>

#### <a name="request"></a><span data-ttu-id="96da4-182">请求</span><span class="sxs-lookup"><span data-stu-id="96da4-182">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="96da4-183">HTTP</span><span class="sxs-lookup"><span data-stu-id="96da4-183">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_unifiedroleassignmentmultiple_1"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/cloudPC/roleAssignments/dbe9d288-fd87-41f4-b33d-b498ed207096
```
# <a name="c"></a>[<span data-ttu-id="96da4-184">C#</span><span class="sxs-lookup"><span data-stu-id="96da4-184">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-unifiedroleassignmentmultiple-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="96da4-185">JavaScript</span><span class="sxs-lookup"><span data-stu-id="96da4-185">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-unifiedroleassignmentmultiple-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="96da4-186">Objective-C</span><span class="sxs-lookup"><span data-stu-id="96da4-186">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-unifiedroleassignmentmultiple-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="96da4-187">Java</span><span class="sxs-lookup"><span data-stu-id="96da4-187">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-unifiedroleassignmentmultiple-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="96da4-188">响应</span><span class="sxs-lookup"><span data-stu-id="96da4-188">Response</span></span>
> <span data-ttu-id="96da4-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="96da4-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-5-get-a-roleassignmentmultiple-in-a-cloud-pc-provider-with-expand"></a><span data-ttu-id="96da4-191">示例 5：在云电脑提供商获取 roleAssignmentMultiple `$expand`</span><span class="sxs-lookup"><span data-stu-id="96da4-191">Example 5: Get a roleAssignmentMultiple in a cloud PC provider with `$expand`</span></span>

#### <a name="request"></a><span data-ttu-id="96da4-192">请求</span><span class="sxs-lookup"><span data-stu-id="96da4-192">Request</span></span>

<span data-ttu-id="96da4-193">下面是一个包含查询参数 `$expand` 的请求示例。</span><span class="sxs-lookup"><span data-stu-id="96da4-193">The following is an example of the request with the `$expand` query parameter.</span></span>


# <a name="http"></a>[<span data-ttu-id="96da4-194">HTTP</span><span class="sxs-lookup"><span data-stu-id="96da4-194">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_unifiedroleassignment_3"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/cloudPC/roleAssignments/dbe9d288-fd87-41f4-b33d-b498ed207096?$expand=roleDefinition
```
# <a name="c"></a>[<span data-ttu-id="96da4-195">C#</span><span class="sxs-lookup"><span data-stu-id="96da4-195">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-unifiedroleassignment-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="96da4-196">JavaScript</span><span class="sxs-lookup"><span data-stu-id="96da4-196">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-unifiedroleassignment-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="96da4-197">Objective-C</span><span class="sxs-lookup"><span data-stu-id="96da4-197">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-unifiedroleassignment-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="96da4-198">Java</span><span class="sxs-lookup"><span data-stu-id="96da4-198">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-unifiedroleassignment-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="96da4-199">响应</span><span class="sxs-lookup"><span data-stu-id="96da4-199">Response</span></span>
> <span data-ttu-id="96da4-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="96da4-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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



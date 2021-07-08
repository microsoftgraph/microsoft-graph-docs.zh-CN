---
title: 列出 unifiedRoleAssignmentMultiple
description: 检索 unifiedRoleAssignmentMultiple 对象的属性和关系。
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 72c1c5f711148651b8faef38efb7d4d0d21cf432
ms.sourcegitcommit: ae83b2b372902268517fd17a8b10d6d9add422af
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/08/2021
ms.locfileid: "53334617"
---
# <a name="list-unifiedroleassignmentmultiple"></a><span data-ttu-id="e5c5e-103">列出 unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="e5c5e-103">List unifiedRoleAssignmentMultiple</span></span>

<span data-ttu-id="e5c5e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e5c5e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e5c5e-105">获取 RBAC [提供程序的 unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) 对象列表。</span><span class="sxs-lookup"><span data-stu-id="e5c5e-105">Get a list of [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) objects for an RBAC provider.</span></span>

<span data-ttu-id="e5c5e-106">目前支持以下 RBAC 提供程序：</span><span class="sxs-lookup"><span data-stu-id="e5c5e-106">The following RBAC providers are currently supported:</span></span>
- <span data-ttu-id="e5c5e-107">云电脑</span><span class="sxs-lookup"><span data-stu-id="e5c5e-107">cloud PC</span></span> 
- <span data-ttu-id="e5c5e-108">Intune (设备) </span><span class="sxs-lookup"><span data-stu-id="e5c5e-108">device management (Intune)</span></span>

<span data-ttu-id="e5c5e-109">For other Microsoft 365 applications (like Azure AD) ， use [unifiedRoleAssignment](../resources/unifiedroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="e5c5e-109">For other Microsoft 365 applications (like Azure AD), use [unifiedRoleAssignment](../resources/unifiedroleassignment.md).</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="e5c5e-110">权限</span><span class="sxs-lookup"><span data-stu-id="e5c5e-110">Permissions</span></span>

<span data-ttu-id="e5c5e-111">根据 RBAC 提供程序以及 (或应用程序) 的权限类型，从下表中选择调用此 API 所需的最低特权权限。</span><span class="sxs-lookup"><span data-stu-id="e5c5e-111">Depending on the RBAC provider and the permission type (delegated or application) that is needed, choose from the following table the least privileged permission required to call this API.</span></span> <span data-ttu-id="e5c5e-112">若要了解 [更多信息，包括在](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) 选择更多特权权限之前保持谨慎，请参阅 [权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e5c5e-112">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, see [Permissions](/graph/permissions-reference).</span></span> 

### <a name="for-cloud-pc-provider"></a><span data-ttu-id="e5c5e-113">对于云电脑提供商</span><span class="sxs-lookup"><span data-stu-id="e5c5e-113">For Cloud PC provider</span></span>

|<span data-ttu-id="e5c5e-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="e5c5e-114">Permission type</span></span>      | <span data-ttu-id="e5c5e-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e5c5e-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e5c5e-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e5c5e-116">Delegated (work or school account)</span></span> |  <span data-ttu-id="e5c5e-117">CloudPC.Read.All、CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5c5e-117">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>   |
|<span data-ttu-id="e5c5e-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e5c5e-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e5c5e-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="e5c5e-119">Not supported.</span></span>    |
|<span data-ttu-id="e5c5e-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="e5c5e-120">Application</span></span> | <span data-ttu-id="e5c5e-121">CloudPC.Read.All、CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5c5e-121">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>  |

### <a name="for-device-management-intune-provider"></a><span data-ttu-id="e5c5e-122">对于 Intune (提供程序的设备) 管理</span><span class="sxs-lookup"><span data-stu-id="e5c5e-122">For Device management (Intune) provider</span></span>

|<span data-ttu-id="e5c5e-123">权限类型</span><span class="sxs-lookup"><span data-stu-id="e5c5e-123">Permission type</span></span>      | <span data-ttu-id="e5c5e-124">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e5c5e-124">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e5c5e-125">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e5c5e-125">Delegated (work or school account)</span></span> |  <span data-ttu-id="e5c5e-126">DeviceManagementRBAC.Read.All、DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5c5e-126">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span></span>   |
|<span data-ttu-id="e5c5e-127">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e5c5e-127">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e5c5e-128">不支持。</span><span class="sxs-lookup"><span data-stu-id="e5c5e-128">Not supported.</span></span>    |
|<span data-ttu-id="e5c5e-129">应用程序</span><span class="sxs-lookup"><span data-stu-id="e5c5e-129">Application</span></span> | <span data-ttu-id="e5c5e-130">DeviceManagementRBAC.Read.All、DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5c5e-130">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span></span> |


## <a name="http-request"></a><span data-ttu-id="e5c5e-131">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e5c5e-131">HTTP request</span></span>

<span data-ttu-id="e5c5e-132">列出云电脑提供商的角色分配：</span><span class="sxs-lookup"><span data-stu-id="e5c5e-132">To list role assignments for a cloud PC provider:</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /roleManagement/cloudPc/roleAssignments
```

<span data-ttu-id="e5c5e-133">列出 Intune 提供程序的角色分配：</span><span class="sxs-lookup"><span data-stu-id="e5c5e-133">To list role assignments for an Intune provider:</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /roleManagement/deviceManagement/roleAssignments
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e5c5e-134">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="e5c5e-134">Optional query parameters</span></span>
<span data-ttu-id="e5c5e-135">可以筛选 或 `roleDefinitionId` `principalId` 属性。</span><span class="sxs-lookup"><span data-stu-id="e5c5e-135">You can filter on the `roleDefinitionId` or `principalId` properties.</span></span> <span data-ttu-id="e5c5e-136">属性 `roleDefinitionId` 可以是角色对象 ID 或角色模板对象 ID。</span><span class="sxs-lookup"><span data-stu-id="e5c5e-136">The `roleDefinitionId` property can be either a role object ID or a role template object ID.</span></span> <span data-ttu-id="e5c5e-137">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="e5c5e-137">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="e5c5e-138">请求标头</span><span class="sxs-lookup"><span data-stu-id="e5c5e-138">Request headers</span></span>

| <span data-ttu-id="e5c5e-139">名称</span><span class="sxs-lookup"><span data-stu-id="e5c5e-139">Name</span></span> | <span data-ttu-id="e5c5e-140">说明</span><span class="sxs-lookup"><span data-stu-id="e5c5e-140">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="e5c5e-141">Authorization</span><span class="sxs-lookup"><span data-stu-id="e5c5e-141">Authorization</span></span> | <span data-ttu-id="e5c5e-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e5c5e-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e5c5e-144">请求正文</span><span class="sxs-lookup"><span data-stu-id="e5c5e-144">Request body</span></span>

<span data-ttu-id="e5c5e-145">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e5c5e-145">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e5c5e-146">响应</span><span class="sxs-lookup"><span data-stu-id="e5c5e-146">Response</span></span>

<span data-ttu-id="e5c5e-147">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="e5c5e-147">If successful, this method returns a `200 OK` response code and a collection of [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e5c5e-148">示例</span><span class="sxs-lookup"><span data-stu-id="e5c5e-148">Example</span></span>

### <a name="example-1-list-the-role-assignments-for-a-specific-principal-for-an-intune-provider"></a><span data-ttu-id="e5c5e-149">示例 1：列出 Intune 提供程序的特定主体的角色分配</span><span class="sxs-lookup"><span data-stu-id="e5c5e-149">Example 1: List the role assignments for a specific principal for an Intune provider</span></span>

### <a name="request"></a><span data-ttu-id="e5c5e-150">请求</span><span class="sxs-lookup"><span data-stu-id="e5c5e-150">Request</span></span>

<span data-ttu-id="e5c5e-151">下面是一个请求示例：</span><span class="sxs-lookup"><span data-stu-id="e5c5e-151">The following is an example of the request:</span></span>

<!-- {
  "blockType": "request",
  "name": "list_unifiedroleassignmentmultiple"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/deviceManagement/roleAssignments/$filter=principalId eq '9e47fc6f-2d7a-464c-944e-d3dd0de522e4'
```

### <a name="response"></a><span data-ttu-id="e5c5e-152">响应</span><span class="sxs-lookup"><span data-stu-id="e5c5e-152">Response</span></span>

<span data-ttu-id="e5c5e-153">下面是一个响应示例：</span><span class="sxs-lookup"><span data-stu-id="e5c5e-153">The following is an example of the response:</span></span>
> <span data-ttu-id="e5c5e-154">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="e5c5e-154">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignmentMultiple"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/deviceManagement/roleAssignments/$entity",
    "value": [ 
       {
            "@odata.type": "#microsoft.graph.unifiedRoleAssignmentMultiple",
            "id": "lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1",
            "roleDefinitionId": "62e90394-69f5-4237-9190-012177145e10",
            "principalIds[]": ["9e47fc6f-2d7a-464c-944e-d3dd0de522e4", "f8ca5a85-489a-49a0-b555-0a6d81e56f0d"],
            "directoryScopeIds[]": ["28ca5a85-489a-49a0-b555-0a6d81e56f0", "8152656a-cf9a-4928-a457-1512d4cae295"]
       },
       {
            "@odata.type": "#microsoft.graph.unifiedRoleAssignmentMultiple",
            "id": "2BNpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SWRD-2",
            "roleDefinitionId": "9e47fc6f-2d7a-464c-944e-d3dd0de522e4",
            "principalIds[]": ["9e47fc6f-2d7a-464c-944e-d3dd0de522e4", "53a6c08d-0227-41bd-8bc6-2728df6be749", "a4991fe1-6d7c-427c-969b-bda6df78c458"],
            "appScopeIds[]": ["28ca5a85-489a-49a0-b555-0a6d81e56f0"]
       }
    ]
}
```
### <a name="example-2-list-role-assignments-for-a-cloud-pc-provider"></a><span data-ttu-id="e5c5e-155">示例 2：列出云电脑提供商的角色分配</span><span class="sxs-lookup"><span data-stu-id="e5c5e-155">Example 2: List role assignments for a cloud PC provider</span></span>

### <a name="request"></a><span data-ttu-id="e5c5e-156">请求</span><span class="sxs-lookup"><span data-stu-id="e5c5e-156">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="e5c5e-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="e5c5e-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_cloudpcunifiedroleassignmentmultiple_1"
}-->

```msgraph-interactive
GET  https://graph.microsoft.com/beta/roleManagement/cloudPC/roleAssignments
```
# <a name="c"></a>[<span data-ttu-id="e5c5e-158">C#</span><span class="sxs-lookup"><span data-stu-id="e5c5e-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-cloudpcunifiedroleassignmentmultiple-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e5c5e-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e5c5e-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-cloudpcunifiedroleassignmentmultiple-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e5c5e-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e5c5e-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-cloudpcunifiedroleassignmentmultiple-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e5c5e-161">Java</span><span class="sxs-lookup"><span data-stu-id="e5c5e-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-cloudpcunifiedroleassignmentmultiple-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e5c5e-162">响应</span><span class="sxs-lookup"><span data-stu-id="e5c5e-162">Response</span></span>

> <span data-ttu-id="e5c5e-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="e5c5e-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignmentMultiple"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/cloudPC/roleAssignments/$entity",
    "value": [
        {
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
        },
        {
            "id": "fad74173-3fe3-4e64-9a80-297bdad2b36e",
            "description": null,
            "displayName": "My test role assignment 2",
            "roleDefinitionId": "b5c08161-a7af-481c-ace2-a20a69a48fb1",
            "principalIds": [
                "8e811502-ebda-4782-8f81-071d17f0f892",
            ],
            "directoryScopeIds": [
                "/"
            ],
            "appScopeIds": []
        }
    ]
}
```

### <a name="example-3-list-role-assignments-for-specific-role-of-a-cloud-pc-provider"></a><span data-ttu-id="e5c5e-165">示例 3：列出云电脑提供商的特定角色的角色分配</span><span class="sxs-lookup"><span data-stu-id="e5c5e-165">Example 3: List role assignments for specific role of a cloud PC provider</span></span>

### <a name="request"></a><span data-ttu-id="e5c5e-166">请求</span><span class="sxs-lookup"><span data-stu-id="e5c5e-166">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="e5c5e-167">HTTP</span><span class="sxs-lookup"><span data-stu-id="e5c5e-167">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_cloudpcunifiedroleassignmentmultiple_2"
}-->

```msgraph-interactive
GET  https://graph.microsoft.com/beta/roleManagement/cloudPC/roleAssignments?$filter=roleDefinitionId eq 'b5c08161-a7af-481c-ace2-a20a69a48fb1'
```
# <a name="c"></a>[<span data-ttu-id="e5c5e-168">C#</span><span class="sxs-lookup"><span data-stu-id="e5c5e-168">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-cloudpcunifiedroleassignmentmultiple-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e5c5e-169">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e5c5e-169">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-cloudpcunifiedroleassignmentmultiple-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e5c5e-170">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e5c5e-170">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-cloudpcunifiedroleassignmentmultiple-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e5c5e-171">Java</span><span class="sxs-lookup"><span data-stu-id="e5c5e-171">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-cloudpcunifiedroleassignmentmultiple-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e5c5e-172">响应</span><span class="sxs-lookup"><span data-stu-id="e5c5e-172">Response</span></span>

> <span data-ttu-id="e5c5e-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="e5c5e-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignmentMultiple"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/cloudPC/roleAssignments",
    "value": [{
        "id": "ed9e247f-f23b-4d72-9e8c-97fa6f385246",
        "description": "",
        "displayName": "test",
        "roleDefinitionId": "b5c08161-a7af-481c-ace2-a20a69a48fb1",
        "principalIds": ["689c9051-77ff-4f14-9b39-3d22de07321a"],
        "directoryScopeIds": ["/"],
        "appScopeIds": []
    }, {
        "id": "3d8e564b-761a-4b32-8f50-63d555f7bc00",
        "description": "test1",
        "displayName": "AssignmentTest",
        "roleDefinitionId": "b5c08161-a7af-481c-ace2-a20a69a48fb1",
        "principalIds": ["0ec7855b-4057-4b7c-9217-09ee9bf4dfd7"],
        "directoryScopeIds": ["/"],
        "appScopeIds": []
    }, {
        "id": "f36a3269-d03d-4d33-81e7-190bded40ad2",
        "description": "",
        "displayName": "test3",
        "roleDefinitionId": "b5c08161-a7af-481c-ace2-a20a69a48fb1",
        "principalIds": ["e4ea53cf-cdd6-46b5-bf38-570033a0fba3"],
        "directoryScopeIds": ["/"],
        "appScopeIds": []
    }]
}
```
<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List roleAssignmentsMultiple",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->



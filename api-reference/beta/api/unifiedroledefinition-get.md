---
title: 获取 unifiedRoleDefinition
description: 检索 unifiedRoleDefinition 对象的属性和关系。
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 0ac38b1c6b131c22f8b3197500640cf36ef2f691
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50444810"
---
# <a name="get-unifiedroledefinition"></a><span data-ttu-id="0d2c8-103">获取 unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="0d2c8-103">Get unifiedRoleDefinition</span></span>

<span data-ttu-id="0d2c8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0d2c8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0d2c8-105">检索 [unifiedRoleDefinition](../resources/unifiedRoleDefinition.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0d2c8-105">Retrieve the properties and relationships of a [unifiedRoleDefinition](../resources/unifiedRoleDefinition.md) object.</span></span> <span data-ttu-id="0d2c8-106">目前，"目录"是唯一受支持的 RBAC 应用程序。</span><span class="sxs-lookup"><span data-stu-id="0d2c8-106">Currently "directory" is the only RBAC application supported.</span></span>

## <a name="permissions"></a><span data-ttu-id="0d2c8-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="0d2c8-107">Permissions</span></span>

<span data-ttu-id="0d2c8-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0d2c8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0d2c8-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="0d2c8-110">Permission type</span></span>      | <span data-ttu-id="0d2c8-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0d2c8-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0d2c8-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0d2c8-112">Delegated (work or school account)</span></span> | <span data-ttu-id="0d2c8-113">RoleManagement.Read.Directory、Directory.Read.All、RoleManagement.ReadWrite.Directory、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0d2c8-113">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="0d2c8-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0d2c8-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0d2c8-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="0d2c8-115">Not supported.</span></span>    |
|<span data-ttu-id="0d2c8-116">Application</span><span class="sxs-lookup"><span data-stu-id="0d2c8-116">Application</span></span> | <span data-ttu-id="0d2c8-117">RoleManagement.Read.Directory、Directory.Read.All、RoleManagement.ReadWrite.Directory、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0d2c8-117">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0d2c8-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0d2c8-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /roleManagement/directory/roleDefinitions/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0d2c8-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="0d2c8-119">Optional query parameters</span></span>

<span data-ttu-id="0d2c8-120">此方法支持 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="0d2c8-120">This method supports OData query parameters to help customize the response.</span></span> <span data-ttu-id="0d2c8-121">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="0d2c8-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="0d2c8-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="0d2c8-122">Request headers</span></span>

| <span data-ttu-id="0d2c8-123">名称</span><span class="sxs-lookup"><span data-stu-id="0d2c8-123">Name</span></span>      |<span data-ttu-id="0d2c8-124">说明</span><span class="sxs-lookup"><span data-stu-id="0d2c8-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="0d2c8-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="0d2c8-125">Authorization</span></span> | <span data-ttu-id="0d2c8-126">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="0d2c8-126">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="0d2c8-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="0d2c8-127">Request body</span></span>

<span data-ttu-id="0d2c8-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0d2c8-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0d2c8-129">响应</span><span class="sxs-lookup"><span data-stu-id="0d2c8-129">Response</span></span>

<span data-ttu-id="0d2c8-130">如果成功，此方法在响应正文中返回响应代码和请求的 `200 OK` [unifiedRoleDefinition](../resources/unifiedroledefinition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0d2c8-130">If successful, this method returns a `200 OK` response code and the requested [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0d2c8-131">示例</span><span class="sxs-lookup"><span data-stu-id="0d2c8-131">Examples</span></span>

### <a name="example-1-get-the-definition-of-a-custom-role"></a><span data-ttu-id="0d2c8-132">示例 1：获取自定义角色的定义</span><span class="sxs-lookup"><span data-stu-id="0d2c8-132">Example 1: Get the definition of a custom role</span></span>

#### <a name="request"></a><span data-ttu-id="0d2c8-133">请求</span><span class="sxs-lookup"><span data-stu-id="0d2c8-133">Request</span></span>

<span data-ttu-id="0d2c8-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="0d2c8-134">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="0d2c8-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="0d2c8-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_custom_role_unifiedroledefinition"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/directory/roleDefinitions/f189965f-f560-4c59-9101-933d4c87a91a
```
# <a name="c"></a>[<span data-ttu-id="0d2c8-136">C#</span><span class="sxs-lookup"><span data-stu-id="0d2c8-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-custom-role-unifiedroledefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0d2c8-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0d2c8-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-custom-role-unifiedroledefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0d2c8-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0d2c8-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-custom-role-unifiedroledefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0d2c8-139">Java</span><span class="sxs-lookup"><span data-stu-id="0d2c8-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-custom-role-unifiedroledefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="0d2c8-140">响应</span><span class="sxs-lookup"><span data-stu-id="0d2c8-140">Response</span></span>

<span data-ttu-id="0d2c8-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="0d2c8-141">The following is an example of the response.</span></span>

> <span data-ttu-id="0d2c8-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="0d2c8-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleDefinition"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json


{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleDefinitions/$entity",
    "id": "429c3819-053d-4250-9926-4c7dcb18ae17",
    "description": "Allows reading Application Registrations",
    "displayName": "Application Registration Reader",
    "isBuiltIn": false,
    "isEnabled": true,
    "templateId": "f189965f-f560-4c59-9101-933d4c87a91a",
    "version": null,
    "rolePermissions": [
        {
            "allowedResourceActions": [
                "microsoft.directory/applications/allProperties/read"
            ],
            "condition": null
        }
    ],
    "inheritsPermissionsFrom@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleDefinitions('f189965f-f560-4c59-9101-933d4c87a91a')/inheritsPermissionsFrom",
    "inheritsPermissionsFrom": []
}
```

### <a name="example-2-get-the-definition-of-a-built-in-role"></a><span data-ttu-id="0d2c8-144">示例 2：获取内置角色的定义</span><span class="sxs-lookup"><span data-stu-id="0d2c8-144">Example 2: Get the definition of a built-in role</span></span>

#### <a name="request"></a><span data-ttu-id="0d2c8-145">请求</span><span class="sxs-lookup"><span data-stu-id="0d2c8-145">Request</span></span>

<span data-ttu-id="0d2c8-146">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="0d2c8-146">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="0d2c8-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="0d2c8-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_built_in_role_unifiedroledefinition"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/directory/roleDefinitions/fdd7a751-b60b-444a-984c-02652fe8fa1c
```
# <a name="c"></a>[<span data-ttu-id="0d2c8-148">C#</span><span class="sxs-lookup"><span data-stu-id="0d2c8-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-built-in-role-unifiedroledefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0d2c8-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0d2c8-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-built-in-role-unifiedroledefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0d2c8-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0d2c8-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-built-in-role-unifiedroledefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0d2c8-151">Java</span><span class="sxs-lookup"><span data-stu-id="0d2c8-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-built-in-role-unifiedroledefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---


#### <a name="response"></a><span data-ttu-id="0d2c8-152">响应</span><span class="sxs-lookup"><span data-stu-id="0d2c8-152">Response</span></span>

<span data-ttu-id="0d2c8-153">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="0d2c8-153">The following is an example of the response.</span></span>

> <span data-ttu-id="0d2c8-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="0d2c8-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleDefinition"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleDefinitions/$entity",
    "id": "fdd7a751-b60b-444a-984c-02652fe8fa1c",
    "description": "Members of this role can create/manage groups, create/manage groups settings like naming and expiration policies, and view groups activity and audit reports.",
    "displayName": "Groups Administrator",
    "isBuiltIn": true,
    "isEnabled": true,
    "resourceScopes": [
        "/"
    ],
    "templateId": "fdd7a751-b60b-444a-984c-02652fe8fa1c",
    "version": "1",
    "rolePermissions": [
        {
            "allowedResourceActions": [
                "microsoft.directory/groups/assignLicense",
                "microsoft.directory/groups/create",
                "microsoft.directory/groups/delete",
                "microsoft.directory/groups/hiddenMembers/read",
                "microsoft.directory/groups/reprocessLicenseAssignment",
                "microsoft.directory/groups/restore",
                "microsoft.directory/groups/basic/update",
                "microsoft.directory/groups/classification/update",
                "microsoft.directory/groups/dynamicMembershipRule/update",
                "microsoft.directory/groups/groupType/update",
                "microsoft.directory/groups/members/update",
                "microsoft.directory/groups/owners/update",
                "microsoft.directory/groups/settings/update",
                "microsoft.directory/groups/visibility/update",
                "microsoft.azure.serviceHealth/allEntities/allTasks",
                "microsoft.azure.supportTickets/allEntities/allTasks",
                "microsoft.office365.serviceHealth/allEntities/allTasks",
                "microsoft.office365.supportTickets/allEntities/allTasks",
                "microsoft.office365.webPortal/allEntities/standard/read"
            ],
            "condition": null
        }
    ],
    "inheritsPermissionsFrom@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleDefinitions('fdd7a751-b60b-444a-984c-02652fe8fa1c')/inheritsPermissionsFrom",
    "inheritsPermissionsFrom": [
        {
            "id": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b"
        }
    ]
}
```
### <a name="example-3-get-the-definition-of-an-azure-ad-built-in-role-and-expand-on-the-role-it-inherits-from"></a><span data-ttu-id="0d2c8-156">示例 3：获取 Azure AD 内置角色的定义，$expand其继承的角色</span><span class="sxs-lookup"><span data-stu-id="0d2c8-156">Example 3: Get the definition of an Azure AD built-in role and $expand on the role it inherits from</span></span>

#### <a name="request"></a><span data-ttu-id="0d2c8-157">请求</span><span class="sxs-lookup"><span data-stu-id="0d2c8-157">Request</span></span>

<span data-ttu-id="0d2c8-158">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="0d2c8-158">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="0d2c8-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="0d2c8-159">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_inheritsFrom_unifiedroledefinition"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/directory/roleDefinitions/fdd7a751-b60b-444a-984c-02652fe8fa1c?$expand=inheritsPermissionsFrom
```
# <a name="c"></a>[<span data-ttu-id="0d2c8-160">C#</span><span class="sxs-lookup"><span data-stu-id="0d2c8-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-inheritsfrom-unifiedroledefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0d2c8-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0d2c8-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-inheritsfrom-unifiedroledefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0d2c8-162">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0d2c8-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-inheritsfrom-unifiedroledefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0d2c8-163">Java</span><span class="sxs-lookup"><span data-stu-id="0d2c8-163">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-inheritsfrom-unifiedroledefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---


#### <a name="response"></a><span data-ttu-id="0d2c8-164">响应</span><span class="sxs-lookup"><span data-stu-id="0d2c8-164">Response</span></span>

<span data-ttu-id="0d2c8-165">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="0d2c8-165">The following is an example of the response.</span></span>

> <span data-ttu-id="0d2c8-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="0d2c8-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleDefinition"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json


{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleDefinitions(inheritsPermissionsFrom())/$entity",
    "id": "fdd7a751-b60b-444a-984c-02652fe8fa1c",
    "description": "Members of this role can create/manage groups, create/manage groups settings like naming and expiration policies, and view groups activity and audit reports.",
    "displayName": "Groups Administrator",
    "isBuiltIn": true,
    "isEnabled": true,
    "resourceScopes": [
        "/"
    ],
    "templateId": "fdd7a751-b60b-444a-984c-02652fe8fa1c",
    "version": "1",
    "rolePermissions": [
        {
            "allowedResourceActions": [
                "microsoft.directory/groups/assignLicense",
                "microsoft.directory/groups/create",
                "microsoft.directory/groups/delete",
                "microsoft.directory/groups/hiddenMembers/read",
                "microsoft.directory/groups/reprocessLicenseAssignment",
                "microsoft.directory/groups/restore",
                "microsoft.directory/groups/basic/update",
                "microsoft.directory/groups/classification/update",
                "microsoft.directory/groups/dynamicMembershipRule/update",
                "microsoft.directory/groups/groupType/update",
                "microsoft.directory/groups/members/update",
                "microsoft.directory/groups/owners/update",
                "microsoft.directory/groups/settings/update",
                "microsoft.directory/groups/visibility/update",
                "microsoft.azure.serviceHealth/allEntities/allTasks",
                "microsoft.azure.supportTickets/allEntities/allTasks",
                "microsoft.office365.serviceHealth/allEntities/allTasks",
                "microsoft.office365.supportTickets/allEntities/allTasks",
                "microsoft.office365.webPortal/allEntities/standard/read"
            ],
            "condition": null
        }
    ],
    "inheritsPermissionsFrom@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleDefinitions('fdd7a751-b60b-444a-984c-02652fe8fa1c')/inheritsPermissionsFrom",
    "inheritsPermissionsFrom": [
        {
            "id": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b",
            "description": "Can read basic directory information. Commonly used to grant directory read access to applications and guests.",
            "displayName": "Directory Readers",
            "isBuiltIn": true,
            "isEnabled": true,
            "resourceScopes": [
                "/"
            ],
            "templateId": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b",
            "version": "1",
            "rolePermissions": [
                {
                    "allowedResourceActions": [
                        "microsoft.directory/administrativeUnits/standard/read",
                        "microsoft.directory/administrativeUnits/members/read",
                        "microsoft.directory/applications/standard/read",
                        "microsoft.directory/applications/owners/read",
                        "microsoft.directory/applications/policies/read",
                        "microsoft.directory/contacts/standard/read",
                        "microsoft.directory/contacts/memberOf/read",
                        "microsoft.directory/contracts/standard/read",
                        "microsoft.directory/devices/standard/read",
                        "microsoft.directory/devices/memberOf/read",
                        "microsoft.directory/devices/registeredOwners/read",
                        "microsoft.directory/devices/registeredUsers/read",
                        "microsoft.directory/directoryRoles/standard/read",
                        "microsoft.directory/directoryRoles/eligibleMembers/read",
                        "microsoft.directory/directoryRoles/members/read",
                        "microsoft.directory/domains/standard/read",
                        "microsoft.directory/groups/standard/read",
                        "microsoft.directory/groups/appRoleAssignments/read",
                        "microsoft.directory/groups/memberOf/read",
                        "microsoft.directory/groups/members/read",
                        "microsoft.directory/groups/owners/read",
                        "microsoft.directory/groups/settings/read",
                        "microsoft.directory/groupSettings/standard/read",
                        "microsoft.directory/groupSettingTemplates/standard/read",
                        "microsoft.directory/oAuth2PermissionGrants/standard/read",
                        "microsoft.directory/organization/standard/read",
                        "microsoft.directory/organization/trustedCAsForPasswordlessAuth/read",
                        "microsoft.directory/applicationPolicies/standard/read",
                        "microsoft.directory/roleAssignments/standard/read",
                        "microsoft.directory/roleDefinitions/standard/read",
                        "microsoft.directory/servicePrincipals/appRoleAssignedTo/read",
                        "microsoft.directory/servicePrincipals/appRoleAssignments/read",
                        "microsoft.directory/servicePrincipals/standard/read",
                        "microsoft.directory/servicePrincipals/memberOf/read",
                        "microsoft.directory/servicePrincipals/oAuth2PermissionGrants/read",
                        "microsoft.directory/servicePrincipals/owners/read",
                        "microsoft.directory/servicePrincipals/ownedObjects/read",
                        "microsoft.directory/servicePrincipals/policies/read",
                        "microsoft.directory/subscribedSkus/standard/read",
                        "microsoft.directory/users/standard/read",
                        "microsoft.directory/users/appRoleAssignments/read",
                        "microsoft.directory/users/directReports/read",
                        "microsoft.directory/users/manager/read",
                        "microsoft.directory/users/memberOf/read",
                        "microsoft.directory/users/oAuth2PermissionGrants/read",
                        "microsoft.directory/users/ownedDevices/read",
                        "microsoft.directory/users/ownedObjects/read",
                        "microsoft.directory/users/registeredDevices/read"
                    ],
                    "condition": null
                }
            ]
        }
    ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get unifiedRoleDefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->



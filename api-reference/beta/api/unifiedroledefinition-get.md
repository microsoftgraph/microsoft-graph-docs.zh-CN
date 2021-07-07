---
title: 获取 unifiedRoleDefinition
description: 检索 unifiedRoleDefinition 对象的属性和关系。
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 07b9aff276c46fbdcca56b365d11e7ac12066408
ms.sourcegitcommit: ada6eab637b9b318129aefb98edbe7316399d9ba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/07/2021
ms.locfileid: "53317075"
---
# <a name="get-unifiedroledefinition"></a><span data-ttu-id="0e87b-103">获取 unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="0e87b-103">Get unifiedRoleDefinition</span></span>

<span data-ttu-id="0e87b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0e87b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0e87b-105">获取 RBAC 提供程序 [的 unifiedRoleDefinition](../resources/unifiedRoleDefinition.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0e87b-105">Get the properties and relationships of a [unifiedRoleDefinition](../resources/unifiedRoleDefinition.md) object of an RBAC provider.</span></span> 

<span data-ttu-id="0e87b-106">目前支持以下 RBAC 提供程序：</span><span class="sxs-lookup"><span data-stu-id="0e87b-106">The following RBAC providers are currently supported:</span></span>
- <span data-ttu-id="0e87b-107">云电脑</span><span class="sxs-lookup"><span data-stu-id="0e87b-107">cloud PC</span></span> 
- <span data-ttu-id="0e87b-108">Intune (设备) </span><span class="sxs-lookup"><span data-stu-id="0e87b-108">device management (Intune)</span></span>
- <span data-ttu-id="0e87b-109">directory (Azure AD directory roles) </span><span class="sxs-lookup"><span data-stu-id="0e87b-109">directory (Azure AD directory roles)</span></span>
- <span data-ttu-id="0e87b-110">授权管理 (Azure AD 权利管理) </span><span class="sxs-lookup"><span data-stu-id="0e87b-110">entitlement management (Azure AD entitlement management)</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="0e87b-111">权限</span><span class="sxs-lookup"><span data-stu-id="0e87b-111">Permissions</span></span>

<span data-ttu-id="0e87b-112">根据 RBAC 提供程序以及 (或应用程序) 的权限类型，从下表中选择调用此 API 所需的最低特权权限。</span><span class="sxs-lookup"><span data-stu-id="0e87b-112">Depending on the RBAC provider and the permission type (delegated or application) that is needed, choose from the following table the least privileged permission required to call this API.</span></span> <span data-ttu-id="0e87b-113">若要了解其他信息， [在](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) 特权权限之前要特别小心，在"权限" [中搜索](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0e87b-113">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in [Permissions](/graph/permissions-reference).</span></span> 

|<span data-ttu-id="0e87b-114">支持的提供程序</span><span class="sxs-lookup"><span data-stu-id="0e87b-114">Supported provider</span></span>      | <span data-ttu-id="0e87b-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0e87b-115">Delegated (work or school account)</span></span>  | <span data-ttu-id="0e87b-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0e87b-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0e87b-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="0e87b-117">Application</span></span> |
|:-----------------------|:------------------------------------|:---------------------------------------|:------------|
| <span data-ttu-id="0e87b-118">云电脑</span><span class="sxs-lookup"><span data-stu-id="0e87b-118">Cloud PC</span></span> | <span data-ttu-id="0e87b-119">CloudPC.Read.All、CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e87b-119">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span> | <span data-ttu-id="0e87b-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="0e87b-120">Not supported.</span></span> | <span data-ttu-id="0e87b-121">CloudPC.Read.All、CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e87b-121">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span> |
| <span data-ttu-id="0e87b-122">设备管理</span><span class="sxs-lookup"><span data-stu-id="0e87b-122">Device management</span></span> | <span data-ttu-id="0e87b-123">DeviceManagementRBAC.Read.All、DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e87b-123">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span></span> | <span data-ttu-id="0e87b-124">不支持。</span><span class="sxs-lookup"><span data-stu-id="0e87b-124">Not supported.</span></span> | <span data-ttu-id="0e87b-125">DeviceManagementRBAC.Read.All、DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e87b-125">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span></span> |
| <span data-ttu-id="0e87b-126">目录</span><span class="sxs-lookup"><span data-stu-id="0e87b-126">Directory</span></span> | <span data-ttu-id="0e87b-127">RoleManagement.Read.Directory、Directory.Read.All、RoleManagement.ReadWrite.Directory、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0e87b-127">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> | <span data-ttu-id="0e87b-128">不支持。</span><span class="sxs-lookup"><span data-stu-id="0e87b-128">Not supported.</span></span>| <span data-ttu-id="0e87b-129">RoleManagement.Read.Directory、Directory.Read.All、RoleManagement.ReadWrite.Directory、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e87b-129">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="0e87b-130">权利管理</span><span class="sxs-lookup"><span data-stu-id="0e87b-130">Entitlement management</span></span> | <span data-ttu-id="0e87b-131">EntitlementManagement.Read.All、EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e87b-131">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> | <span data-ttu-id="0e87b-132">不支持。</span><span class="sxs-lookup"><span data-stu-id="0e87b-132">Not supported.</span></span> | <span data-ttu-id="0e87b-133">不支持。</span><span class="sxs-lookup"><span data-stu-id="0e87b-133">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0e87b-134">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0e87b-134">HTTP request</span></span>

<span data-ttu-id="0e87b-135">获取云电脑提供商的角色定义：</span><span class="sxs-lookup"><span data-stu-id="0e87b-135">Get a role definition for a cloud PC provider:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /roleManagement/cloudPC/roleDefinitions/{id}
```

<span data-ttu-id="0e87b-136">获取设备管理提供程序的角色定义：</span><span class="sxs-lookup"><span data-stu-id="0e87b-136">Get a role definition for a device management provider:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /roleManagement/deviceManagement/roleDefinitions/{id}
```

<span data-ttu-id="0e87b-137">获取目录提供程序的角色定义：</span><span class="sxs-lookup"><span data-stu-id="0e87b-137">Get a role definition for a directory provider:</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /roleManagement/directory/roleDefinitions/{id}
```

<span data-ttu-id="0e87b-138">获取权利管理提供程序的角色定义：</span><span class="sxs-lookup"><span data-stu-id="0e87b-138">Get a role definition for the entitlement management provider:</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /roleManagement/entitlementManagement/roleDefinitions/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0e87b-139">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="0e87b-139">Optional query parameters</span></span>

<span data-ttu-id="0e87b-140">此方法支持 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="0e87b-140">This method supports OData query parameters to help customize the response.</span></span> <span data-ttu-id="0e87b-141">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="0e87b-141">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="0e87b-142">请求标头</span><span class="sxs-lookup"><span data-stu-id="0e87b-142">Request headers</span></span>

| <span data-ttu-id="0e87b-143">名称</span><span class="sxs-lookup"><span data-stu-id="0e87b-143">Name</span></span>      |<span data-ttu-id="0e87b-144">说明</span><span class="sxs-lookup"><span data-stu-id="0e87b-144">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="0e87b-145">Authorization</span><span class="sxs-lookup"><span data-stu-id="0e87b-145">Authorization</span></span> | <span data-ttu-id="0e87b-146">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="0e87b-146">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="0e87b-147">请求正文</span><span class="sxs-lookup"><span data-stu-id="0e87b-147">Request body</span></span>

<span data-ttu-id="0e87b-148">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0e87b-148">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0e87b-149">响应</span><span class="sxs-lookup"><span data-stu-id="0e87b-149">Response</span></span>

<span data-ttu-id="0e87b-150">如果成功，此方法在响应正文中返回 响应代码和请求的 `200 OK` [unifiedRoleDefinition](../resources/unifiedroledefinition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0e87b-150">If successful, this method returns a `200 OK` response code and the requested [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0e87b-151">示例</span><span class="sxs-lookup"><span data-stu-id="0e87b-151">Examples</span></span>

### <a name="example-1-get-the-definition-of-a-custom-role-for-a-directory-provider"></a><span data-ttu-id="0e87b-152">示例 1：获取目录提供程序的自定义角色的定义</span><span class="sxs-lookup"><span data-stu-id="0e87b-152">Example 1: Get the definition of a custom role for a directory provider</span></span>

#### <a name="request"></a><span data-ttu-id="0e87b-153">请求</span><span class="sxs-lookup"><span data-stu-id="0e87b-153">Request</span></span>

<span data-ttu-id="0e87b-154">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="0e87b-154">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="0e87b-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="0e87b-155">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_custom_role_unifiedroledefinition"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/directory/roleDefinitions/f189965f-f560-4c59-9101-933d4c87a91a
```
# <a name="c"></a>[<span data-ttu-id="0e87b-156">C#</span><span class="sxs-lookup"><span data-stu-id="0e87b-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-custom-role-unifiedroledefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0e87b-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0e87b-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-custom-role-unifiedroledefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0e87b-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0e87b-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-custom-role-unifiedroledefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0e87b-159">Java</span><span class="sxs-lookup"><span data-stu-id="0e87b-159">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-custom-role-unifiedroledefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="0e87b-160">响应</span><span class="sxs-lookup"><span data-stu-id="0e87b-160">Response</span></span>

<span data-ttu-id="0e87b-161">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="0e87b-161">The following is an example of the response.</span></span>

> <span data-ttu-id="0e87b-162">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="0e87b-162">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-2-get-the-definition-of-a-built-in-role-for-a-directory-provider"></a><span data-ttu-id="0e87b-163">示例 2：获取目录提供程序的内置角色的定义</span><span class="sxs-lookup"><span data-stu-id="0e87b-163">Example 2: Get the definition of a built-in role for a directory provider</span></span>

#### <a name="request"></a><span data-ttu-id="0e87b-164">请求</span><span class="sxs-lookup"><span data-stu-id="0e87b-164">Request</span></span>

<span data-ttu-id="0e87b-165">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="0e87b-165">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="0e87b-166">HTTP</span><span class="sxs-lookup"><span data-stu-id="0e87b-166">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_built_in_role_unifiedroledefinition"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/directory/roleDefinitions/fdd7a751-b60b-444a-984c-02652fe8fa1c
```
# <a name="c"></a>[<span data-ttu-id="0e87b-167">C#</span><span class="sxs-lookup"><span data-stu-id="0e87b-167">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-built-in-role-unifiedroledefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0e87b-168">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0e87b-168">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-built-in-role-unifiedroledefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0e87b-169">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0e87b-169">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-built-in-role-unifiedroledefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0e87b-170">Java</span><span class="sxs-lookup"><span data-stu-id="0e87b-170">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-built-in-role-unifiedroledefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---


#### <a name="response"></a><span data-ttu-id="0e87b-171">响应</span><span class="sxs-lookup"><span data-stu-id="0e87b-171">Response</span></span>

<span data-ttu-id="0e87b-172">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="0e87b-172">The following is an example of the response.</span></span>

> <span data-ttu-id="0e87b-173">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="0e87b-173">**Note:** The response object shown here might be shortened for readability.</span></span>

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
### <a name="example-3-get-the-definition-of-an-azure-ad-built-in-role-and-expand-on-the-role-it-inherits-from"></a><span data-ttu-id="0e87b-174">示例 3：获取 Azure AD 内置角色的定义，$expand继承自的角色定义</span><span class="sxs-lookup"><span data-stu-id="0e87b-174">Example 3: Get the definition of an Azure AD built-in role and $expand on the role it inherits from</span></span>

#### <a name="request"></a><span data-ttu-id="0e87b-175">请求</span><span class="sxs-lookup"><span data-stu-id="0e87b-175">Request</span></span>

<span data-ttu-id="0e87b-176">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="0e87b-176">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="0e87b-177">HTTP</span><span class="sxs-lookup"><span data-stu-id="0e87b-177">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_inheritsFrom_unifiedroledefinition"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/directory/roleDefinitions/fdd7a751-b60b-444a-984c-02652fe8fa1c?$expand=inheritsPermissionsFrom
```
# <a name="c"></a>[<span data-ttu-id="0e87b-178">C#</span><span class="sxs-lookup"><span data-stu-id="0e87b-178">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-inheritsfrom-unifiedroledefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0e87b-179">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0e87b-179">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-inheritsfrom-unifiedroledefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0e87b-180">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0e87b-180">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-inheritsfrom-unifiedroledefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0e87b-181">Java</span><span class="sxs-lookup"><span data-stu-id="0e87b-181">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-inheritsfrom-unifiedroledefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---


#### <a name="response"></a><span data-ttu-id="0e87b-182">响应</span><span class="sxs-lookup"><span data-stu-id="0e87b-182">Response</span></span>

<span data-ttu-id="0e87b-183">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="0e87b-183">The following is an example of the response.</span></span>

> <span data-ttu-id="0e87b-184">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="0e87b-184">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-4-get-the-definition-of-a-built-in-role-for-a-cloud-pc-provider"></a><span data-ttu-id="0e87b-185">示例 4：获取云电脑提供商的内置角色的定义</span><span class="sxs-lookup"><span data-stu-id="0e87b-185">Example 4: Get the definition of a built-in role for a cloud PC provider</span></span>

#### <a name="request"></a><span data-ttu-id="0e87b-186">请求</span><span class="sxs-lookup"><span data-stu-id="0e87b-186">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="0e87b-187">HTTP</span><span class="sxs-lookup"><span data-stu-id="0e87b-187">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_built-in_cloudpc_role_unifiedroledefinition"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/cloudPC/roleDefinitions/d40368cb-fbf4-4965-bbc1-f17b3a78e510
```
# <a name="c"></a>[<span data-ttu-id="0e87b-188">C#</span><span class="sxs-lookup"><span data-stu-id="0e87b-188">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-built-in-cloudpc-role-unifiedroledefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0e87b-189">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0e87b-189">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-built-in-cloudpc-role-unifiedroledefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0e87b-190">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0e87b-190">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-built-in-cloudpc-role-unifiedroledefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0e87b-191">Java</span><span class="sxs-lookup"><span data-stu-id="0e87b-191">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-built-in-cloudpc-role-unifiedroledefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="0e87b-192">响应</span><span class="sxs-lookup"><span data-stu-id="0e87b-192">Response</span></span>
> <span data-ttu-id="0e87b-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="0e87b-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleDefinition"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/cloudPC/roleDefinitions/$entity",
    "id": "d40368cb-fbf4-4965-bbc1-f17b3a78e510",
    "description": "Have read-only access all Cloud PC features.",
    "displayName": "Cloud PC Reader",
    "isBuiltIn": true,
    "isEnabled": true,
    "resourceScopes": [
        "/"
    ],
    "templateId": "d40368cb-fbf4-4965-bbc1-f17b3a78e510",
    "version": null,
    "rolePermissions": [
        {
            "allowedResourceActions": [
                "Microsoft.CloudPC/CloudPCs/Read",
                "Microsoft.CloudPC/DeviceImages/Read",
                "Microsoft.CloudPC/OnPremisesConnections/Read",
                "Microsoft.CloudPC/ProvisioningPolicies/Read",
                "Microsoft.CloudPC/Roles/Read",
                "Microsoft.CloudPC/SelfServiceSettings/Read"
            ],
            "condition": null
        }
    ]
}
```

## <a name="example-5-get-the-definition-of-a-built-in-role-for-the-entitlement-management-provider"></a><span data-ttu-id="0e87b-195">示例 5：获取权利管理提供程序的内置角色的定义</span><span class="sxs-lookup"><span data-stu-id="0e87b-195">Example 5: Get the definition of a built-in role for the entitlement management provider</span></span>

#### <a name="request"></a><span data-ttu-id="0e87b-196">请求</span><span class="sxs-lookup"><span data-stu-id="0e87b-196">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_built-in_entitlementmanagement_role_unifiedroledefinition"
}-->

```http
GET https://graph.microsoft.com/beta/roleManagement/entitlementManagement/roleDefinitions/ba92d953-d8e0-4e39-a797-0cbedb0a89e8
```


#### <a name="response"></a><span data-ttu-id="0e87b-197">响应</span><span class="sxs-lookup"><span data-stu-id="0e87b-197">Response</span></span>
> <span data-ttu-id="0e87b-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="0e87b-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleDefinition"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/entitlementManagement/roleDefinitions/$entity",
    "id": "ba92d953-d8e0-4e39-a797-0cbedb0a89e8",
    "displayName": "Catalog creator",
    "description": "Catalog creator",
    "isBuiltIn": true,
    "isEnabled": true,
    "templateId": "ba92d953-d8e0-4e39-a797-0cbedb0a89e8",
    "version": "1.0",
    "rolePermissions": [
        {
            "allowedResourceActions": [
                "microsoft.entitlementManagement/AccessPackageCatalog/Create"
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



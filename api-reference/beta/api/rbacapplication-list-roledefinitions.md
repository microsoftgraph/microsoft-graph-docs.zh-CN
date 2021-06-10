---
title: 列出 unifiedRoleDefinitions
description: 获取 unifiedRoleDefinition 对象的列表。
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 04a34aec3c611e5cf178910b7a8513a048fb797e
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2021
ms.locfileid: "52869131"
---
# <a name="list-unifiedroledefinitions"></a><span data-ttu-id="832e2-103">列出 unifiedRoleDefinitions</span><span class="sxs-lookup"><span data-stu-id="832e2-103">List unifiedRoleDefinitions</span></span>

<span data-ttu-id="832e2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="832e2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="832e2-105">获取 RBAC [提供程序的 unifiedRoleDefinition](../resources/unifiedroledefinition.md) 对象列表。</span><span class="sxs-lookup"><span data-stu-id="832e2-105">Get a list of [unifiedRoleDefinition](../resources/unifiedroledefinition.md) objects for an RBAC provider.</span></span>

<span data-ttu-id="832e2-106">目前支持以下 RBAC 提供程序：</span><span class="sxs-lookup"><span data-stu-id="832e2-106">The following RBAC providers are currently supported:</span></span>
- <span data-ttu-id="832e2-107">云电脑</span><span class="sxs-lookup"><span data-stu-id="832e2-107">cloud PC</span></span> 
- <span data-ttu-id="832e2-108">Intune (设备) </span><span class="sxs-lookup"><span data-stu-id="832e2-108">device management (Intune)</span></span>
- <span data-ttu-id="832e2-109">Azure AD (目录) </span><span class="sxs-lookup"><span data-stu-id="832e2-109">directory (Azure AD)</span></span> 

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="832e2-110">权限</span><span class="sxs-lookup"><span data-stu-id="832e2-110">Permissions</span></span>

<span data-ttu-id="832e2-111">根据 RBAC 提供程序以及 (或应用程序) 的权限类型，从下表中选择调用此 API 所需的最低特权权限。</span><span class="sxs-lookup"><span data-stu-id="832e2-111">Depending on the RBAC provider and the permission type (delegated or application) that is needed, choose from the following table the least privileged permission required to call this API.</span></span> <span data-ttu-id="832e2-112">若要了解详细信息，包括在选择更多特权之前的[注意事项](/graph/auth/auth-concepts#best-practices-for-requesting-permissions)，请在“[权限](/graph/permissions-reference)”中搜索以下权限。</span><span class="sxs-lookup"><span data-stu-id="832e2-112">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in [Permissions](/graph/permissions-reference).</span></span> 

|<span data-ttu-id="832e2-113">支持的提供程序</span><span class="sxs-lookup"><span data-stu-id="832e2-113">Supported provider</span></span>      | <span data-ttu-id="832e2-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="832e2-114">Delegated (work or school account)</span></span>  | <span data-ttu-id="832e2-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="832e2-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="832e2-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="832e2-116">Application</span></span> |
|:-----------------------|:------------------------------------|:---------------------------------------|:------------|
| <span data-ttu-id="832e2-117">Cloud PC</span><span class="sxs-lookup"><span data-stu-id="832e2-117">Cloud PC</span></span> | <span data-ttu-id="832e2-118">CloudPC.Read.All、CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="832e2-118">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span> | <span data-ttu-id="832e2-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="832e2-119">Not supported.</span></span> | <span data-ttu-id="832e2-120">CloudPC.Read.All、CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="832e2-120">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span> |
| <span data-ttu-id="832e2-121">设备管理</span><span class="sxs-lookup"><span data-stu-id="832e2-121">Device management</span></span> | <span data-ttu-id="832e2-122">DeviceManagementRBAC.Read.All、DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="832e2-122">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span></span> | <span data-ttu-id="832e2-123">不支持。</span><span class="sxs-lookup"><span data-stu-id="832e2-123">Not supported.</span></span> | <span data-ttu-id="832e2-124">DeviceManagementRBAC.Read.All、DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="832e2-124">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span></span> |
| <span data-ttu-id="832e2-125">目录</span><span class="sxs-lookup"><span data-stu-id="832e2-125">Directory</span></span> | <span data-ttu-id="832e2-126">RoleManagement.Read.Directory、Directory.Read.All、RoleManagement.ReadWrite.Directory、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="832e2-126">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> | <span data-ttu-id="832e2-127">不支持。</span><span class="sxs-lookup"><span data-stu-id="832e2-127">Not supported.</span></span>| <span data-ttu-id="832e2-128">RoleManagement.Read.Directory、Directory.Read.All、RoleManagement.ReadWrite.Directory、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="832e2-128">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |


## <a name="http-request"></a><span data-ttu-id="832e2-129">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="832e2-129">HTTP request</span></span>

<span data-ttu-id="832e2-130">列出云电脑提供商的角色定义：</span><span class="sxs-lookup"><span data-stu-id="832e2-130">To list role definitions for a cloud PC provider:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /roleManagement/cloudPC/roleDefinitions
```

<span data-ttu-id="832e2-131">列出设备管理提供程序的角色定义：</span><span class="sxs-lookup"><span data-stu-id="832e2-131">To list role definitions for a device management provider:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /roleManagement/deviceManagement/roleDefinitions
```

<span data-ttu-id="832e2-132">列出目录提供程序的角色定义：</span><span class="sxs-lookup"><span data-stu-id="832e2-132">To list role definitions for a directory provider:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /roleManagement/directory/roleDefinitions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="832e2-133">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="832e2-133">Optional query parameters</span></span>
<span data-ttu-id="832e2-134">此方法支持 `$filter` 对 、 `id` 和 `displayName` 属性使用查询 `isBuiltIn` 参数。</span><span class="sxs-lookup"><span data-stu-id="832e2-134">This method supports `$filter` query parameter on `id`, `displayName`, and `isBuiltIn` properties.</span></span> <span data-ttu-id="832e2-135">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="832e2-135">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="832e2-136">请求标头</span><span class="sxs-lookup"><span data-stu-id="832e2-136">Request headers</span></span>

| <span data-ttu-id="832e2-137">名称</span><span class="sxs-lookup"><span data-stu-id="832e2-137">Name</span></span>      |<span data-ttu-id="832e2-138">说明</span><span class="sxs-lookup"><span data-stu-id="832e2-138">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="832e2-139">Authorization</span><span class="sxs-lookup"><span data-stu-id="832e2-139">Authorization</span></span> | <span data-ttu-id="832e2-140">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="832e2-140">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="832e2-141">请求正文</span><span class="sxs-lookup"><span data-stu-id="832e2-141">Request body</span></span>

<span data-ttu-id="832e2-142">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="832e2-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="832e2-143">响应</span><span class="sxs-lookup"><span data-stu-id="832e2-143">Response</span></span>

<span data-ttu-id="832e2-144">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [unifiedRoleDefinition](../resources/unifiedroledefinition.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="832e2-144">If successful, this method returns a `200 OK` response code and a collection of [unifiedRoleDefinition](../resources/unifiedroledefinition.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="832e2-145">示例</span><span class="sxs-lookup"><span data-stu-id="832e2-145">Examples</span></span>

### <a name="example-1-list-role-definitions-for-a-directory-provider"></a><span data-ttu-id="832e2-146">示例 1：列出目录提供程序的角色定义</span><span class="sxs-lookup"><span data-stu-id="832e2-146">Example 1: List role definitions for a directory provider</span></span>

#### <a name="request"></a><span data-ttu-id="832e2-147">请求</span><span class="sxs-lookup"><span data-stu-id="832e2-147">Request</span></span>

<span data-ttu-id="832e2-148">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="832e2-148">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="832e2-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="832e2-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_roledefinitions_directory"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/directory/roleDefinitions
```
# <a name="c"></a>[<span data-ttu-id="832e2-150">C#</span><span class="sxs-lookup"><span data-stu-id="832e2-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-roledefinitions-directory-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="832e2-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="832e2-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-roledefinitions-directory-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="832e2-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="832e2-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-roledefinitions-directory-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="832e2-153">Java</span><span class="sxs-lookup"><span data-stu-id="832e2-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-roledefinitions-directory-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="832e2-154">响应</span><span class="sxs-lookup"><span data-stu-id="832e2-154">Response</span></span>

<span data-ttu-id="832e2-155">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="832e2-155">The following is an example of the response.</span></span>

> <span data-ttu-id="832e2-156">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="832e2-156">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "name": "get_roledefinitions_directory",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleDefinition",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleDefinitions",
    "value": [
        {
            "id": "729827e3-9c14-49f7-bb1b-9608f156bbb8",
            "description": "Can reset passwords for non-administrators and Helpdesk Administrators.",
            "displayName": "Helpdesk Administrator",
            "isBuiltIn": true,
            "isEnabled": true,
            "templateId": "729827e3-9c14-49f7-bb1b-9608f156bbb8",
            "version": "1",
            "rolePermissions": [
                {
                    "allowedResourceActions": [
                        "microsoft.directory/users/invalidateAllRefreshTokens",
                        "microsoft.directory/users/bitLockerRecoveryKeys/read",
                        "microsoft.directory/users/password/update",
                        "microsoft.azure.serviceHealth/allEntities/allTasks",
                        "microsoft.azure.supportTickets/allEntities/allTasks",
                        "microsoft.office365.webPortal/allEntities/standard/read",
                        "microsoft.office365.serviceHealth/allEntities/allTasks",
                        "microsoft.office365.supportTickets/allEntities/allTasks"
                    ],
                    "condition": null
                }
            ],
            "inheritsPermissionsFrom@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleDefinitions('729827e3-9c14-49f7-bb1b-9608f156bbb8')/inheritsPermissionsFrom",
            "inheritsPermissionsFrom": [
                {
                    "id": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b"
                }
            ]
        },
        {
            "id": "f023fd81-a637-4b56-95fd-791ac0226033",
            "description": "Can read service health information and manage support tickets.",
            "displayName": "Service Support Administrator",
            "isBuiltIn": true,
            "isEnabled": true,
            "templateId": "f023fd81-a637-4b56-95fd-791ac0226033",
            "version": "1",
            "rolePermissions": [
                {
                    "allowedResourceActions": [
                        "microsoft.azure.serviceHealth/allEntities/allTasks",
                        "microsoft.azure.supportTickets/allEntities/allTasks",
                        "microsoft.office365.webPortal/allEntities/standard/read",
                        "microsoft.office365.serviceHealth/allEntities/allTasks",
                        "microsoft.office365.supportTickets/allEntities/allTasks"
                    ],
                    "condition": null
                }
            ],
            "inheritsPermissionsFrom@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleDefinitions('f023fd81-a637-4b56-95fd-791ac0226033')/inheritsPermissionsFrom",
            "inheritsPermissionsFrom": [
                {
                    "id": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b"
                }
            ]
        },
        {
            "id": "b0f54661-2d74-4c50-afa3-1ec803f12efe",
            "description": "Can perform common billing related tasks like updating payment information.",
            "displayName": "Billing Administrator",
            "isBuiltIn": true,
            "isEnabled": true,
            "templateId": "b0f54661-2d74-4c50-afa3-1ec803f12efe",
            "version": "1",
            "rolePermissions": [
                {
                    "allowedResourceActions": [
                        "microsoft.directory/organization/basic/update",
                        "microsoft.azure.serviceHealth/allEntities/allTasks",
                        "microsoft.azure.supportTickets/allEntities/allTasks",
                        "microsoft.commerce.billing/allEntities/allTasks",
                        "microsoft.office365.webPortal/allEntities/standard/read",
                        "microsoft.office365.serviceHealth/allEntities/allTasks",
                        "microsoft.office365.supportTickets/allEntities/allTasks"
                    ],
                    "condition": null
                }
            ],
            "inheritsPermissionsFrom@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleDefinitions('b0f54661-2d74-4c50-afa3-1ec803f12efe')/inheritsPermissionsFrom",
            "inheritsPermissionsFrom": [
                {
                    "id": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b"
                }
            ]
        }
    ]
}
```

### <a name="example-2-list-role-definitions-for-a-cloud-pc-provider"></a><span data-ttu-id="832e2-157">示例 2：列出云电脑提供商的角色定义</span><span class="sxs-lookup"><span data-stu-id="832e2-157">Example 2: List role definitions for a cloud PC provider</span></span>

#### <a name="request"></a><span data-ttu-id="832e2-158">请求</span><span class="sxs-lookup"><span data-stu-id="832e2-158">Request</span></span>

<span data-ttu-id="832e2-159">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="832e2-159">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="832e2-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="832e2-160">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_roledefinitions_cloudpc"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/cloudPC/roleDefinitions
```
# <a name="c"></a>[<span data-ttu-id="832e2-161">C#</span><span class="sxs-lookup"><span data-stu-id="832e2-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-roledefinitions-cloudpc-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="832e2-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="832e2-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-roledefinitions-cloudpc-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="832e2-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="832e2-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-roledefinitions-cloudpc-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="832e2-164">Java</span><span class="sxs-lookup"><span data-stu-id="832e2-164">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-roledefinitions-cloudpc-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="832e2-165">响应</span><span class="sxs-lookup"><span data-stu-id="832e2-165">Response</span></span>

<span data-ttu-id="832e2-166">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="832e2-166">The following is an example of the response.</span></span>

> <span data-ttu-id="832e2-167">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="832e2-167">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "name": "get_roledefinitions_cloudpc",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleDefinition",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/cloudPC/roleDefinitions",
    "value": [
        {
            "id": "b5c08161-a7af-481c-ace2-a20a69a48fb1",
            "description": "Cloud PC Administrator has read and write access to all Cloud PC features located within the Cloud PC blade.",
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
                        "Microsoft.CloudPC/Roles/Read"
                    ],
                    "condition": null
                }
            ]
        },
        {
            "id": "d40368cb-fbf4-4965-bbc1-f17b3a78e510",
            "description": "Cloud PC Reader has read access to all Cloud PC features located within the Cloud PC blade.",
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
                        "Microsoft.CloudPC/Roles/Read"
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
  "description": "List roleDefinitions",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->



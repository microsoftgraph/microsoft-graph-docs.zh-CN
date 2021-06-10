---
title: 获取 unifiedRoleDefinition
description: 检索 unifiedRoleDefinition 对象的属性和关系。
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 71948e099507bf081739dbef9f4e07d43f358af9
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2021
ms.locfileid: "52870316"
---
# <a name="get-unifiedroledefinition"></a><span data-ttu-id="d308e-103">获取 unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="d308e-103">Get unifiedRoleDefinition</span></span>

<span data-ttu-id="d308e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d308e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d308e-105">获取 RBAC 提供程序 [的 unifiedRoleDefinition](../resources/unifiedRoleDefinition.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d308e-105">Get the properties and relationships of a [unifiedRoleDefinition](../resources/unifiedRoleDefinition.md) object of an RBAC provider.</span></span> 

<span data-ttu-id="d308e-106">目前支持以下 RBAC 提供程序：</span><span class="sxs-lookup"><span data-stu-id="d308e-106">The following RBAC providers are currently supported:</span></span>
- <span data-ttu-id="d308e-107">云电脑</span><span class="sxs-lookup"><span data-stu-id="d308e-107">cloud PC</span></span> 
- <span data-ttu-id="d308e-108">Intune (设备) </span><span class="sxs-lookup"><span data-stu-id="d308e-108">device management (Intune)</span></span>
- <span data-ttu-id="d308e-109">Azure AD (目录) </span><span class="sxs-lookup"><span data-stu-id="d308e-109">directory (Azure AD)</span></span> 

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="d308e-110">权限</span><span class="sxs-lookup"><span data-stu-id="d308e-110">Permissions</span></span>

<span data-ttu-id="d308e-111">根据 RBAC 提供程序以及 (或应用程序) 的权限类型，从下表中选择调用此 API 所需的最低特权权限。</span><span class="sxs-lookup"><span data-stu-id="d308e-111">Depending on the RBAC provider and the permission type (delegated or application) that is needed, choose from the following table the least privileged permission required to call this API.</span></span> <span data-ttu-id="d308e-112">若要了解详细信息，包括在选择更多特权之前的[注意事项](/graph/auth/auth-concepts#best-practices-for-requesting-permissions)，请在“[权限](/graph/permissions-reference)”中搜索以下权限。</span><span class="sxs-lookup"><span data-stu-id="d308e-112">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in [Permissions](/graph/permissions-reference).</span></span> 

|<span data-ttu-id="d308e-113">支持的提供程序</span><span class="sxs-lookup"><span data-stu-id="d308e-113">Supported provider</span></span>      | <span data-ttu-id="d308e-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d308e-114">Delegated (work or school account)</span></span>  | <span data-ttu-id="d308e-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d308e-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d308e-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="d308e-116">Application</span></span> |
|:-----------------------|:------------------------------------|:---------------------------------------|:------------|
| <span data-ttu-id="d308e-117">Cloud PC</span><span class="sxs-lookup"><span data-stu-id="d308e-117">Cloud PC</span></span> | <span data-ttu-id="d308e-118">CloudPC.Read.All、CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d308e-118">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span> | <span data-ttu-id="d308e-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="d308e-119">Not supported.</span></span> | <span data-ttu-id="d308e-120">CloudPC.Read.All、CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d308e-120">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span> |
| <span data-ttu-id="d308e-121">设备管理</span><span class="sxs-lookup"><span data-stu-id="d308e-121">Device management</span></span> | <span data-ttu-id="d308e-122">DeviceManagementRBAC.Read.All、DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d308e-122">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span></span> | <span data-ttu-id="d308e-123">不支持。</span><span class="sxs-lookup"><span data-stu-id="d308e-123">Not supported.</span></span> | <span data-ttu-id="d308e-124">DeviceManagementRBAC.Read.All、DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d308e-124">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span></span> |
| <span data-ttu-id="d308e-125">目录</span><span class="sxs-lookup"><span data-stu-id="d308e-125">Directory</span></span> | <span data-ttu-id="d308e-126">RoleManagement.Read.Directory、Directory.Read.All、RoleManagement.ReadWrite.Directory、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d308e-126">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> | <span data-ttu-id="d308e-127">不支持。</span><span class="sxs-lookup"><span data-stu-id="d308e-127">Not supported.</span></span>| <span data-ttu-id="d308e-128">RoleManagement.Read.Directory、Directory.Read.All、RoleManagement.ReadWrite.Directory、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d308e-128">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d308e-129">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d308e-129">HTTP request</span></span>

<span data-ttu-id="d308e-130">获取云电脑提供商的角色定义：</span><span class="sxs-lookup"><span data-stu-id="d308e-130">Get a role definition for a cloud PC provider:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /roleManagement/cloudPC/roleDefinitions/{id}
```

<span data-ttu-id="d308e-131">获取设备管理提供程序的角色定义：</span><span class="sxs-lookup"><span data-stu-id="d308e-131">Get a role definition for a device management provider:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /roleManagement/deviceManagement/roleDefinitions/{id}
```

<span data-ttu-id="d308e-132">获取目录提供程序的角色定义：</span><span class="sxs-lookup"><span data-stu-id="d308e-132">Get a role definition for a directory provider:</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /roleManagement/directory/roleDefinitions/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d308e-133">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d308e-133">Optional query parameters</span></span>

<span data-ttu-id="d308e-134">此方法支持 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="d308e-134">This method supports OData query parameters to help customize the response.</span></span> <span data-ttu-id="d308e-135">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="d308e-135">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="d308e-136">请求标头</span><span class="sxs-lookup"><span data-stu-id="d308e-136">Request headers</span></span>

| <span data-ttu-id="d308e-137">名称</span><span class="sxs-lookup"><span data-stu-id="d308e-137">Name</span></span>      |<span data-ttu-id="d308e-138">说明</span><span class="sxs-lookup"><span data-stu-id="d308e-138">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d308e-139">Authorization</span><span class="sxs-lookup"><span data-stu-id="d308e-139">Authorization</span></span> | <span data-ttu-id="d308e-140">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="d308e-140">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="d308e-141">请求正文</span><span class="sxs-lookup"><span data-stu-id="d308e-141">Request body</span></span>

<span data-ttu-id="d308e-142">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d308e-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d308e-143">响应</span><span class="sxs-lookup"><span data-stu-id="d308e-143">Response</span></span>

<span data-ttu-id="d308e-144">如果成功，此方法在响应正文中返回 响应代码和请求的 `200 OK` [unifiedRoleDefinition](../resources/unifiedroledefinition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d308e-144">If successful, this method returns a `200 OK` response code and the requested [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d308e-145">示例</span><span class="sxs-lookup"><span data-stu-id="d308e-145">Examples</span></span>

### <a name="example-1-get-the-definition-of-a-custom-role-for-a-directory-provider"></a><span data-ttu-id="d308e-146">示例 1：获取目录提供程序的自定义角色的定义</span><span class="sxs-lookup"><span data-stu-id="d308e-146">Example 1: Get the definition of a custom role for a directory provider</span></span>

#### <a name="request"></a><span data-ttu-id="d308e-147">请求</span><span class="sxs-lookup"><span data-stu-id="d308e-147">Request</span></span>

<span data-ttu-id="d308e-148">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d308e-148">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="d308e-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="d308e-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_custom_role_unifiedroledefinition"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/directory/roleDefinitions/f189965f-f560-4c59-9101-933d4c87a91a
```
# <a name="c"></a>[<span data-ttu-id="d308e-150">C#</span><span class="sxs-lookup"><span data-stu-id="d308e-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-custom-role-unifiedroledefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d308e-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d308e-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-custom-role-unifiedroledefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d308e-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d308e-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-custom-role-unifiedroledefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d308e-153">Java</span><span class="sxs-lookup"><span data-stu-id="d308e-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-custom-role-unifiedroledefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="d308e-154">响应</span><span class="sxs-lookup"><span data-stu-id="d308e-154">Response</span></span>

<span data-ttu-id="d308e-155">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="d308e-155">The following is an example of the response.</span></span>

> <span data-ttu-id="d308e-156">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="d308e-156">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-2-get-the-definition-of-a-built-in-role-for-a-directory-provider"></a><span data-ttu-id="d308e-157">示例 2：获取目录提供程序的内置角色的定义</span><span class="sxs-lookup"><span data-stu-id="d308e-157">Example 2: Get the definition of a built-in role for a directory provider</span></span>

#### <a name="request"></a><span data-ttu-id="d308e-158">请求</span><span class="sxs-lookup"><span data-stu-id="d308e-158">Request</span></span>

<span data-ttu-id="d308e-159">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d308e-159">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="d308e-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="d308e-160">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_built_in_role_unifiedroledefinition"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/directory/roleDefinitions/fdd7a751-b60b-444a-984c-02652fe8fa1c
```
# <a name="c"></a>[<span data-ttu-id="d308e-161">C#</span><span class="sxs-lookup"><span data-stu-id="d308e-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-built-in-role-unifiedroledefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d308e-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d308e-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-built-in-role-unifiedroledefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d308e-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d308e-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-built-in-role-unifiedroledefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d308e-164">Java</span><span class="sxs-lookup"><span data-stu-id="d308e-164">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-built-in-role-unifiedroledefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---


#### <a name="response"></a><span data-ttu-id="d308e-165">响应</span><span class="sxs-lookup"><span data-stu-id="d308e-165">Response</span></span>

<span data-ttu-id="d308e-166">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="d308e-166">The following is an example of the response.</span></span>

> <span data-ttu-id="d308e-167">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="d308e-167">**Note:** The response object shown here might be shortened for readability.</span></span>

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
### <a name="example-3-get-the-definition-of-an-azure-ad-built-in-role-and-expand-on-the-role-it-inherits-from"></a><span data-ttu-id="d308e-168">示例 3：获取 Azure AD 内置角色的定义，$expand继承自的角色定义</span><span class="sxs-lookup"><span data-stu-id="d308e-168">Example 3: Get the definition of an Azure AD built-in role and $expand on the role it inherits from</span></span>

#### <a name="request"></a><span data-ttu-id="d308e-169">请求</span><span class="sxs-lookup"><span data-stu-id="d308e-169">Request</span></span>

<span data-ttu-id="d308e-170">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d308e-170">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="d308e-171">HTTP</span><span class="sxs-lookup"><span data-stu-id="d308e-171">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_inheritsFrom_unifiedroledefinition"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/directory/roleDefinitions/fdd7a751-b60b-444a-984c-02652fe8fa1c?$expand=inheritsPermissionsFrom
```
# <a name="c"></a>[<span data-ttu-id="d308e-172">C#</span><span class="sxs-lookup"><span data-stu-id="d308e-172">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-inheritsfrom-unifiedroledefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d308e-173">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d308e-173">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-inheritsfrom-unifiedroledefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d308e-174">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d308e-174">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-inheritsfrom-unifiedroledefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d308e-175">Java</span><span class="sxs-lookup"><span data-stu-id="d308e-175">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-inheritsfrom-unifiedroledefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---


#### <a name="response"></a><span data-ttu-id="d308e-176">响应</span><span class="sxs-lookup"><span data-stu-id="d308e-176">Response</span></span>

<span data-ttu-id="d308e-177">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="d308e-177">The following is an example of the response.</span></span>

> <span data-ttu-id="d308e-178">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="d308e-178">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-4-get-the-definition-of-a-built-in-role-for-a-cloud-pc-provider"></a><span data-ttu-id="d308e-179">示例 4：获取云电脑提供商的内置角色的定义</span><span class="sxs-lookup"><span data-stu-id="d308e-179">Example 4: Get the definition of a built-in role for a cloud PC provider</span></span>

#### <a name="request"></a><span data-ttu-id="d308e-180">请求</span><span class="sxs-lookup"><span data-stu-id="d308e-180">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="d308e-181">HTTP</span><span class="sxs-lookup"><span data-stu-id="d308e-181">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_built-in_cloudpc_role_unifiedroledefinition"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/cloudPC/roleDefinitions/d40368cb-fbf4-4965-bbc1-f17b3a78e510
```
# <a name="c"></a>[<span data-ttu-id="d308e-182">C#</span><span class="sxs-lookup"><span data-stu-id="d308e-182">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-built-in-cloudpc-role-unifiedroledefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d308e-183">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d308e-183">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-built-in-cloudpc-role-unifiedroledefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d308e-184">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d308e-184">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-built-in-cloudpc-role-unifiedroledefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d308e-185">Java</span><span class="sxs-lookup"><span data-stu-id="d308e-185">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-built-in-cloudpc-role-unifiedroledefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="d308e-186">响应</span><span class="sxs-lookup"><span data-stu-id="d308e-186">Response</span></span>
> <span data-ttu-id="d308e-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="d308e-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get unifiedRoleDefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->



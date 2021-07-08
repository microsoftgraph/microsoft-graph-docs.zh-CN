---
title: 创建 unifiedRoleDefinition
description: 创建新的 unifiedRoleDefinition 对象。
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 8b5fb362456b306b8f7887ad84fe80677e3262b1
ms.sourcegitcommit: ae83b2b372902268517fd17a8b10d6d9add422af
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/08/2021
ms.locfileid: "53334610"
---
# <a name="create-unifiedroledefinition"></a><span data-ttu-id="68687-103">创建 unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="68687-103">Create unifiedRoleDefinition</span></span>

<span data-ttu-id="68687-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="68687-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="68687-105">为 RBAC [提供程序创建新的 unifiedRoleDefinition](../resources/unifiedroledefinition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="68687-105">Create a new [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object for an RBAC provider.</span></span>

<span data-ttu-id="68687-106">目前支持以下 RBAC 提供程序：</span><span class="sxs-lookup"><span data-stu-id="68687-106">The following RBAC providers are currently supported:</span></span>
- <span data-ttu-id="68687-107">Intune (设备) </span><span class="sxs-lookup"><span data-stu-id="68687-107">device management (Intune)</span></span>
- <span data-ttu-id="68687-108">Azure AD (目录) </span><span class="sxs-lookup"><span data-stu-id="68687-108">directory (Azure AD)</span></span>

> [!NOTE]
> <span data-ttu-id="68687-109">云电脑 RBAC 提供商当前仅支持[列表和](rbacapplication-list-roledefinitions.md)[获取](unifiedroledefinition-get.md)操作。</span><span class="sxs-lookup"><span data-stu-id="68687-109">The cloud PC RBAC provider currently supports only the [list](rbacapplication-list-roledefinitions.md) and [get](unifiedroledefinition-get.md) operations.</span></span>

## <a name="permissions"></a><span data-ttu-id="68687-110">权限</span><span class="sxs-lookup"><span data-stu-id="68687-110">Permissions</span></span>

<span data-ttu-id="68687-111">根据 RBAC 提供程序以及 (或应用程序) 的权限类型，从下表中选择调用此 API 所需的最低特权权限。</span><span class="sxs-lookup"><span data-stu-id="68687-111">Depending on the RBAC provider and the permission type (delegated or application) that is needed, choose from the following table the least privileged permission required to call this API.</span></span> <span data-ttu-id="68687-112">若要了解 [更多信息，包括在](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) 选择更多特权权限之前保持谨慎，请参阅 [权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="68687-112">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, see [Permissions](/graph/permissions-reference).</span></span> 

### <a name="for-device-management-intune-provider"></a><span data-ttu-id="68687-113">对于 Intune (提供程序的设备) 管理</span><span class="sxs-lookup"><span data-stu-id="68687-113">For Device management (Intune) provider</span></span>

|<span data-ttu-id="68687-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="68687-114">Permission type</span></span>      | <span data-ttu-id="68687-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="68687-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="68687-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="68687-116">Delegated (work or school account)</span></span> |  <span data-ttu-id="68687-117">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="68687-117">DeviceManagementRBAC.ReadWrite.All</span></span>   |
|<span data-ttu-id="68687-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="68687-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="68687-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="68687-119">Not supported.</span></span>    |
|<span data-ttu-id="68687-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="68687-120">Application</span></span> | <span data-ttu-id="68687-121">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="68687-121">DeviceManagementRBAC.ReadWrite.All</span></span> |

### <a name="for-directory-azure-ad-provider"></a><span data-ttu-id="68687-122">对于 Azure AD (提供程序) 目录</span><span class="sxs-lookup"><span data-stu-id="68687-122">For Directory (Azure AD) provider</span></span>

|<span data-ttu-id="68687-123">权限类型</span><span class="sxs-lookup"><span data-stu-id="68687-123">Permission type</span></span>      | <span data-ttu-id="68687-124">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="68687-124">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="68687-125">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="68687-125">Delegated (work or school account)</span></span> |  <span data-ttu-id="68687-126">RoleManagement.ReadWrite.Directory、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="68687-126">RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>   |
|<span data-ttu-id="68687-127">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="68687-127">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="68687-128">不支持。</span><span class="sxs-lookup"><span data-stu-id="68687-128">Not supported.</span></span>    |
|<span data-ttu-id="68687-129">应用程序</span><span class="sxs-lookup"><span data-stu-id="68687-129">Application</span></span> | <span data-ttu-id="68687-130">RoleManagement.ReadWrite.Directory、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="68687-130">RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="68687-131">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="68687-131">HTTP request</span></span>

<span data-ttu-id="68687-132">若要为设备管理提供程序创建角色定义，请运行：</span><span class="sxs-lookup"><span data-stu-id="68687-132">To create a role definition for a device management provider:</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /roleManagement/deviceManagement/roleDefinitions
```

<span data-ttu-id="68687-133">为目录提供程序创建角色定义：</span><span class="sxs-lookup"><span data-stu-id="68687-133">To create a role definition for a directory provider:</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /roleManagement/directory/roleDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="68687-134">请求标头</span><span class="sxs-lookup"><span data-stu-id="68687-134">Request headers</span></span>

| <span data-ttu-id="68687-135">名称</span><span class="sxs-lookup"><span data-stu-id="68687-135">Name</span></span>          | <span data-ttu-id="68687-136">说明</span><span class="sxs-lookup"><span data-stu-id="68687-136">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="68687-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="68687-137">Authorization</span></span> | <span data-ttu-id="68687-138">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="68687-138">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="68687-139">请求正文</span><span class="sxs-lookup"><span data-stu-id="68687-139">Request body</span></span>

<span data-ttu-id="68687-140">在请求正文中，提供 [unifiedRoleDefinition](../resources/unifiedroledefinition.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="68687-140">In the request body, supply a JSON representation of [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object.</span></span>

<span data-ttu-id="68687-141">下表显示创建 roleDefinition 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="68687-141">The following table shows the properties that are required when you create a roleDefinition.</span></span>

| <span data-ttu-id="68687-142">参数</span><span class="sxs-lookup"><span data-stu-id="68687-142">Parameter</span></span> | <span data-ttu-id="68687-143">类型</span><span class="sxs-lookup"><span data-stu-id="68687-143">Type</span></span> | <span data-ttu-id="68687-144">说明</span><span class="sxs-lookup"><span data-stu-id="68687-144">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="68687-145">displayName</span><span class="sxs-lookup"><span data-stu-id="68687-145">displayName</span></span> |<span data-ttu-id="68687-146">string</span><span class="sxs-lookup"><span data-stu-id="68687-146">string</span></span> |<span data-ttu-id="68687-147">角色显示名称的角色定义。</span><span class="sxs-lookup"><span data-stu-id="68687-147">The display name for the role definition.</span></span>|
|<span data-ttu-id="68687-148">isEnabled</span><span class="sxs-lookup"><span data-stu-id="68687-148">isEnabled</span></span> |<span data-ttu-id="68687-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="68687-149">Boolean</span></span> |<span data-ttu-id="68687-150">指示角色是否已启用分配的标志。</span><span class="sxs-lookup"><span data-stu-id="68687-150">Flag indicating if the role is enabled for assignment.</span></span> <span data-ttu-id="68687-151">如果为 false，则角色不能用于分配。</span><span class="sxs-lookup"><span data-stu-id="68687-151">If false the role is not available for assignment.</span></span>|
|<span data-ttu-id="68687-152">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="68687-152">rolePermissions</span></span> |<span data-ttu-id="68687-153">[unifiedRolePermission](../resources/unifiedrolepermission.md) 集合</span><span class="sxs-lookup"><span data-stu-id="68687-153">[unifiedRolePermission](../resources/unifiedrolepermission.md) collection</span></span> |<span data-ttu-id="68687-154">角色中包含的权限列表。</span><span class="sxs-lookup"><span data-stu-id="68687-154">List of permissions included in the role.</span></span>|

## <a name="response"></a><span data-ttu-id="68687-155">响应</span><span class="sxs-lookup"><span data-stu-id="68687-155">Response</span></span>

<span data-ttu-id="68687-156">如果成功，此方法在 `201 Created` 响应正文中返回 响应代码和新的 [unifiedRoleDefinition](../resources/unifiedroledefinition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="68687-156">If successful, this method returns `201 Created` response code and a new [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="68687-157">示例</span><span class="sxs-lookup"><span data-stu-id="68687-157">Example</span></span>

### <a name="request"></a><span data-ttu-id="68687-158">请求</span><span class="sxs-lookup"><span data-stu-id="68687-158">Request</span></span>

<span data-ttu-id="68687-159">下面是为目录提供程序创建自定义角色的示例。</span><span class="sxs-lookup"><span data-stu-id="68687-159">The following is an example of creating a custom role for a directory provider.</span></span>


# <a name="http"></a>[<span data-ttu-id="68687-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="68687-160">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_unifiedroledefinition_from_rbacapplication"
}-->

```http
POST https://graph.microsoft.com/beta/roleManagement/directory/roleDefinitions
Content-type: application/json

{
  "description": "Update basic properties of application registrations",
  "displayName": "Application Registration Support Administrator",
  "rolePermissions":
    [
        {
            "allowedResourceActions": 
            [
                "microsoft.directory/applications/basic/read"
            ]
        }
    ],
    "isEnabled" : "true"
}
```
# <a name="c"></a>[<span data-ttu-id="68687-161">C#</span><span class="sxs-lookup"><span data-stu-id="68687-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-unifiedroledefinition-from-rbacapplication-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="68687-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="68687-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-unifiedroledefinition-from-rbacapplication-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="68687-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="68687-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-unifiedroledefinition-from-rbacapplication-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="68687-164">Java</span><span class="sxs-lookup"><span data-stu-id="68687-164">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-unifiedroledefinition-from-rbacapplication-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="68687-165">响应</span><span class="sxs-lookup"><span data-stu-id="68687-165">Response</span></span>

<span data-ttu-id="68687-166">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="68687-166">The following is an example of the response.</span></span>
> <span data-ttu-id="68687-167">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="68687-167">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleDefinition"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleDefinitions/$entity",
    "id": "d5eec5e0-6992-4c6b-b430-0f833f1a815a",
    "description": "Update basic properties of application registrations",
    "displayName": "Application Registration Support Administrator",
    "isBuiltIn": false,
    "isEnabled": true,
    "templateId": "c2cb59a3-2d01-4176-a458-95b0e674966f",
    "version": null,
    "rolePermissions": [
        {
            "allowedResourceActions": [
                "microsoft.directory/applications/standard/read",
                "microsoft.directory/applications/basic/update"
            ],
            "condition": null
        }
    ],
    "inheritsPermissionsFrom@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleDefinitions('c2cb59a3-2d01-4176-a458-95b0e674966f')/inheritsPermissionsFrom",
    "inheritsPermissionsFrom": []
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create unifiedRoleDefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->



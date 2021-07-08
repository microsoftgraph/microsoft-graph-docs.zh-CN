---
title: 更新 unifiedRoleDefinition
description: 更新 unifiedRoleDefinition 对象的属性。
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 9e5315a58adc5c6b4447b725ee7315d390d18904
ms.sourcegitcommit: ae83b2b372902268517fd17a8b10d6d9add422af
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/08/2021
ms.locfileid: "53334715"
---
# <a name="update-unifiedroledefinition"></a><span data-ttu-id="e636c-103">更新 unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="e636c-103">Update unifiedRoleDefinition</span></span>

<span data-ttu-id="e636c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e636c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e636c-105">更新 RBAC 提供程序 [的 unifiedRoleDefinition](../resources/unifiedroledefinition.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="e636c-105">Update the properties of a [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object for an RBAC provider.</span></span>

<span data-ttu-id="e636c-106">目前支持以下 RBAC 提供程序：</span><span class="sxs-lookup"><span data-stu-id="e636c-106">The following RBAC providers are currently supported:</span></span>
- <span data-ttu-id="e636c-107">Intune (设备) </span><span class="sxs-lookup"><span data-stu-id="e636c-107">device management (Intune)</span></span>
- <span data-ttu-id="e636c-108">Azure AD (目录) </span><span class="sxs-lookup"><span data-stu-id="e636c-108">directory (Azure AD)</span></span> 

> [!NOTE]
> <span data-ttu-id="e636c-109">云电脑 RBAC 提供商当前仅支持[列表和](rbacapplication-list-roledefinitions.md)[获取](unifiedroledefinition-get.md)操作。</span><span class="sxs-lookup"><span data-stu-id="e636c-109">The cloud PC RBAC provider currently supports only the [list](rbacapplication-list-roledefinitions.md) and [get](unifiedroledefinition-get.md) operations.</span></span>

## <a name="permissions"></a><span data-ttu-id="e636c-110">权限</span><span class="sxs-lookup"><span data-stu-id="e636c-110">Permissions</span></span>

<span data-ttu-id="e636c-111">根据 RBAC 提供程序以及 (或应用程序) 的权限类型，从下表中选择调用此 API 所需的最低特权权限。</span><span class="sxs-lookup"><span data-stu-id="e636c-111">Depending on the RBAC provider and the permission type (delegated or application) that is needed, choose from the following table the least privileged permission required to call this API.</span></span> <span data-ttu-id="e636c-112">若要了解 [更多信息（包括在](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) 选择更多特权权限之前要谨慎操作），请搜索权限参考 [中的以下权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e636c-112">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in the [Permissions reference](/graph/permissions-reference).</span></span> 

|<span data-ttu-id="e636c-113">支持的提供程序</span><span class="sxs-lookup"><span data-stu-id="e636c-113">Supported provider</span></span>      | <span data-ttu-id="e636c-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e636c-114">Delegated (work or school account)</span></span>  | <span data-ttu-id="e636c-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e636c-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e636c-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="e636c-116">Application</span></span> |
|:-----------------------|:------------------------------------|:---------------------------------------|:------------|
| <span data-ttu-id="e636c-117">设备管理</span><span class="sxs-lookup"><span data-stu-id="e636c-117">Device management</span></span> | <span data-ttu-id="e636c-118">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e636c-118">DeviceManagementRBAC.ReadWrite.All</span></span> | <span data-ttu-id="e636c-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="e636c-119">Not supported.</span></span> | <span data-ttu-id="e636c-120">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e636c-120">DeviceManagementRBAC.ReadWrite.All</span></span> |
| <span data-ttu-id="e636c-121">目录</span><span class="sxs-lookup"><span data-stu-id="e636c-121">Directory</span></span> | <span data-ttu-id="e636c-122">RoleManagement.ReadWrite.Directory、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e636c-122">RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> | <span data-ttu-id="e636c-123">不支持。</span><span class="sxs-lookup"><span data-stu-id="e636c-123">Not supported.</span></span>| <span data-ttu-id="e636c-124">RoleManagement.ReadWrite.Directory、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e636c-124">RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

### <a name="for-device-management-intune-provider"></a><span data-ttu-id="e636c-125">对于 Intune (提供程序的设备) 管理</span><span class="sxs-lookup"><span data-stu-id="e636c-125">For Device management (Intune) provider</span></span>

|<span data-ttu-id="e636c-126">权限类型</span><span class="sxs-lookup"><span data-stu-id="e636c-126">Permission type</span></span>      | <span data-ttu-id="e636c-127">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e636c-127">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e636c-128">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e636c-128">Delegated (work or school account)</span></span> |  <span data-ttu-id="e636c-129">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e636c-129">DeviceManagementRBAC.ReadWrite.All</span></span>   |
|<span data-ttu-id="e636c-130">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e636c-130">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e636c-131">不支持。</span><span class="sxs-lookup"><span data-stu-id="e636c-131">Not supported.</span></span>    |
|<span data-ttu-id="e636c-132">应用程序</span><span class="sxs-lookup"><span data-stu-id="e636c-132">Application</span></span> | <span data-ttu-id="e636c-133">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e636c-133">DeviceManagementRBAC.ReadWrite.All</span></span> |

### <a name="for-directory-azure-ad-provider"></a><span data-ttu-id="e636c-134">对于 Azure AD (提供程序) 目录</span><span class="sxs-lookup"><span data-stu-id="e636c-134">For Directory (Azure AD) provider</span></span>

|<span data-ttu-id="e636c-135">权限类型</span><span class="sxs-lookup"><span data-stu-id="e636c-135">Permission type</span></span>      | <span data-ttu-id="e636c-136">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e636c-136">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e636c-137">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e636c-137">Delegated (work or school account)</span></span> |  <span data-ttu-id="e636c-138">RoleManagement.ReadWrite.Directory、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e636c-138">RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>   |
|<span data-ttu-id="e636c-139">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e636c-139">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e636c-140">不支持。</span><span class="sxs-lookup"><span data-stu-id="e636c-140">Not supported.</span></span>    |
|<span data-ttu-id="e636c-141">应用程序</span><span class="sxs-lookup"><span data-stu-id="e636c-141">Application</span></span> | <span data-ttu-id="e636c-142">RoleManagement.ReadWrite.Directory、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e636c-142">RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e636c-143">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e636c-143">HTTP request</span></span>

<span data-ttu-id="e636c-144">若要更新设备管理提供程序的角色定义，请运行：</span><span class="sxs-lookup"><span data-stu-id="e636c-144">To update a role definition for a device management provider:</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /roleManagement/deviceManagement/roleDefinitions/{id}
```

<span data-ttu-id="e636c-145">更新目录提供程序的角色定义：</span><span class="sxs-lookup"><span data-stu-id="e636c-145">To update a role definition for a directory provider:</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /roleManagement/directory/roleDefinitions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="e636c-146">请求标头</span><span class="sxs-lookup"><span data-stu-id="e636c-146">Request headers</span></span>

| <span data-ttu-id="e636c-147">名称</span><span class="sxs-lookup"><span data-stu-id="e636c-147">Name</span></span>       | <span data-ttu-id="e636c-148">说明</span><span class="sxs-lookup"><span data-stu-id="e636c-148">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="e636c-149">Authorization</span><span class="sxs-lookup"><span data-stu-id="e636c-149">Authorization</span></span> | <span data-ttu-id="e636c-150">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="e636c-150">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="e636c-151">请求正文</span><span class="sxs-lookup"><span data-stu-id="e636c-151">Request body</span></span>

<span data-ttu-id="e636c-152">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="e636c-152">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="e636c-153">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="e636c-153">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="e636c-154">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="e636c-154">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="e636c-155">属性</span><span class="sxs-lookup"><span data-stu-id="e636c-155">Property</span></span>     | <span data-ttu-id="e636c-156">类型</span><span class="sxs-lookup"><span data-stu-id="e636c-156">Type</span></span>        | <span data-ttu-id="e636c-157">说明</span><span class="sxs-lookup"><span data-stu-id="e636c-157">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e636c-158">说明</span><span class="sxs-lookup"><span data-stu-id="e636c-158">description</span></span>|<span data-ttu-id="e636c-159">String</span><span class="sxs-lookup"><span data-stu-id="e636c-159">String</span></span>| <span data-ttu-id="e636c-160">角色定义的说明。</span><span class="sxs-lookup"><span data-stu-id="e636c-160">The description for the role definition.</span></span> <span data-ttu-id="e636c-161">isBuiltIn 为 true 时为只读。</span><span class="sxs-lookup"><span data-stu-id="e636c-161">Read-only when isBuiltIn is true.</span></span> |
|<span data-ttu-id="e636c-162">displayName</span><span class="sxs-lookup"><span data-stu-id="e636c-162">displayName</span></span>|<span data-ttu-id="e636c-163">String</span><span class="sxs-lookup"><span data-stu-id="e636c-163">String</span></span>| <span data-ttu-id="e636c-164">角色显示名称的角色定义。</span><span class="sxs-lookup"><span data-stu-id="e636c-164">The display name for the role definition.</span></span> <span data-ttu-id="e636c-165">isBuiltIn 为 true 时为只读。</span><span class="sxs-lookup"><span data-stu-id="e636c-165">Read-only when isBuiltIn is true.</span></span> <span data-ttu-id="e636c-166">必需。</span><span class="sxs-lookup"><span data-stu-id="e636c-166">Required.</span></span>|
|<span data-ttu-id="e636c-167">id</span><span class="sxs-lookup"><span data-stu-id="e636c-167">id</span></span>|<span data-ttu-id="e636c-168">String</span><span class="sxs-lookup"><span data-stu-id="e636c-168">String</span></span>| <span data-ttu-id="e636c-169">角色定义的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="e636c-169">The unique identifier for the role definition.</span></span> <span data-ttu-id="e636c-170">键，不可为 null，只读。</span><span class="sxs-lookup"><span data-stu-id="e636c-170">Key, not nullable, Read-only.</span></span> |
|<span data-ttu-id="e636c-171">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="e636c-171">isBuiltIn</span></span>|<span data-ttu-id="e636c-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="e636c-172">Boolean</span></span>| <span data-ttu-id="e636c-173">指示角色定义是否属于产品或自定义中包含的默认集的标志。</span><span class="sxs-lookup"><span data-stu-id="e636c-173">Flag indicating if the role definition is part of the default set included with the product or custom.</span></span> <span data-ttu-id="e636c-174">只读。</span><span class="sxs-lookup"><span data-stu-id="e636c-174">Read-only.</span></span> |
|<span data-ttu-id="e636c-175">isEnabled</span><span class="sxs-lookup"><span data-stu-id="e636c-175">isEnabled</span></span>|<span data-ttu-id="e636c-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="e636c-176">Boolean</span></span>| <span data-ttu-id="e636c-177">指示角色是否已启用分配的标志。</span><span class="sxs-lookup"><span data-stu-id="e636c-177">Flag indicating if the role is enabled for assignment.</span></span> <span data-ttu-id="e636c-178">如果为 false，则角色不能用于分配。</span><span class="sxs-lookup"><span data-stu-id="e636c-178">If false the role is not available for assignment.</span></span> <span data-ttu-id="e636c-179">isBuiltIn 为 true 时为只读。</span><span class="sxs-lookup"><span data-stu-id="e636c-179">Read-only when isBuiltIn is true.</span></span> |
|<span data-ttu-id="e636c-180">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="e636c-180">resourceScopes</span></span>|<span data-ttu-id="e636c-181">String collection</span><span class="sxs-lookup"><span data-stu-id="e636c-181">String collection</span></span>| <span data-ttu-id="e636c-182">角色定义授予的作用域权限列表适用。</span><span class="sxs-lookup"><span data-stu-id="e636c-182">List of scopes permissions granted by the role definition apply to.</span></span> <span data-ttu-id="e636c-183">目前仅支持"/"。</span><span class="sxs-lookup"><span data-stu-id="e636c-183">Currently only "/" is supported.</span></span> <span data-ttu-id="e636c-184">isBuiltIn 为 true 时为只读。</span><span class="sxs-lookup"><span data-stu-id="e636c-184">Read-only when isBuiltIn is true.</span></span> <span data-ttu-id="e636c-185">**请勿使用。此属性将很快弃用。将作用域附加到角色分配。**</span><span class="sxs-lookup"><span data-stu-id="e636c-185">**DO NOT USE. This property will be deprecated soon. Attach scope to role assignment.**</span></span>|
|<span data-ttu-id="e636c-186">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="e636c-186">rolePermissions</span></span>|<span data-ttu-id="e636c-187">[unifiedRolePermission](../resources/unifiedrolepermission.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e636c-187">[unifiedRolePermission](../resources/unifiedrolepermission.md) collection</span></span>| <span data-ttu-id="e636c-188">角色中包含的权限列表。</span><span class="sxs-lookup"><span data-stu-id="e636c-188">List of permissions included in the role.</span></span> <span data-ttu-id="e636c-189">isBuiltIn 为 true 时为只读。</span><span class="sxs-lookup"><span data-stu-id="e636c-189">Read-only when isBuiltIn is true.</span></span> <span data-ttu-id="e636c-190">必填。</span><span class="sxs-lookup"><span data-stu-id="e636c-190">Required.</span></span> |
|<span data-ttu-id="e636c-191">templateId</span><span class="sxs-lookup"><span data-stu-id="e636c-191">templateId</span></span>|<span data-ttu-id="e636c-192">String</span><span class="sxs-lookup"><span data-stu-id="e636c-192">String</span></span>| <span data-ttu-id="e636c-193">可以在 isBuiltIn 为 false 时设置的自定义模板标识符。</span><span class="sxs-lookup"><span data-stu-id="e636c-193">Custom template identifier that can be set when isBuiltIn is false.</span></span> <span data-ttu-id="e636c-194">如果一个标识符在不同目录之间需要相同，则通常使用此标识符。</span><span class="sxs-lookup"><span data-stu-id="e636c-194">This identifier is typically used if one needs an identifier to be the same across different directories.</span></span> <span data-ttu-id="e636c-195">isBuiltIn 为 true 时为只读。</span><span class="sxs-lookup"><span data-stu-id="e636c-195">Read-only when isBuiltIn is true.</span></span> |
|<span data-ttu-id="e636c-196">inheritsPermissionsFrom</span><span class="sxs-lookup"><span data-stu-id="e636c-196">inheritsPermissionsFrom</span></span>| <span data-ttu-id="e636c-197">[unifiedRoleDefinition](../resources/unifiedroledefinition.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e636c-197">[unifiedRoleDefinition](../resources/unifiedroledefinition.md) collection</span></span>| <span data-ttu-id="e636c-198">给定角色定义从其继承的角色定义的只读集合。</span><span class="sxs-lookup"><span data-stu-id="e636c-198">Read-only collection of role definitions that the given role definition inherits from.</span></span> <span data-ttu-id="e636c-199">仅 Azure AD 内置角色支持此属性。</span><span class="sxs-lookup"><span data-stu-id="e636c-199">Only Azure AD built-in roles support this attribute.</span></span> |
|<span data-ttu-id="e636c-200">version</span><span class="sxs-lookup"><span data-stu-id="e636c-200">version</span></span>|<span data-ttu-id="e636c-201">String</span><span class="sxs-lookup"><span data-stu-id="e636c-201">String</span></span>| <span data-ttu-id="e636c-202">指示角色定义的版本。</span><span class="sxs-lookup"><span data-stu-id="e636c-202">Indicates version of the role definition.</span></span> <span data-ttu-id="e636c-203">isBuiltIn 为 true 时为只读。</span><span class="sxs-lookup"><span data-stu-id="e636c-203">Read-only when isBuiltIn is true.</span></span>|

## <a name="response"></a><span data-ttu-id="e636c-204">响应</span><span class="sxs-lookup"><span data-stu-id="e636c-204">Response</span></span>

<span data-ttu-id="e636c-205">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [unifiedRoleDefinition](../resources/unifiedroledefinition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e636c-205">If successful, this method returns a `200 OK` response code and an updated [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e636c-206">示例</span><span class="sxs-lookup"><span data-stu-id="e636c-206">Example</span></span>

### <a name="request"></a><span data-ttu-id="e636c-207">请求</span><span class="sxs-lookup"><span data-stu-id="e636c-207">Request</span></span>

<span data-ttu-id="e636c-208">以下示例更新目录提供程序 **的 unifiedRoleDefinition。**</span><span class="sxs-lookup"><span data-stu-id="e636c-208">The following example updates a **unifiedRoleDefinition** for a directory provider.</span></span>


# <a name="http"></a>[<span data-ttu-id="e636c-209">HTTP</span><span class="sxs-lookup"><span data-stu-id="e636c-209">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_unifiedroledefinition"
}-->

```http
PATCH https://graph.microsoft.com/beta/roleManagement/directory/roleDefinitions/0d55728d-3e24-4309-9b1b-5ac09921475a
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
    ]
}
```
# <a name="c"></a>[<span data-ttu-id="e636c-210">C#</span><span class="sxs-lookup"><span data-stu-id="e636c-210">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-unifiedroledefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e636c-211">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e636c-211">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-unifiedroledefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e636c-212">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e636c-212">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-unifiedroledefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e636c-213">Java</span><span class="sxs-lookup"><span data-stu-id="e636c-213">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-unifiedroledefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e636c-214">响应</span><span class="sxs-lookup"><span data-stu-id="e636c-214">Response</span></span>

<span data-ttu-id="e636c-215">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="e636c-215">The following is an example of the response.</span></span>
> <span data-ttu-id="e636c-216">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="e636c-216">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 204 OK
Content-type: application/json

```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update unifiedroledefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->



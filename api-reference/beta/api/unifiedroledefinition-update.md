---
title: 更新 unifiedRoleDefinition
description: 更新 unifiedRoleDefinition 对象的属性。
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 4102ece8a559161e5813e175d81a62a4c7ce9843
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787413"
---
# <a name="update-unifiedroledefinition"></a><span data-ttu-id="e8b9d-103">更新 unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="e8b9d-103">Update unifiedRoleDefinition</span></span>

<span data-ttu-id="e8b9d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e8b9d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e8b9d-105">更新 RBAC 提供程序 [的 unifiedRoleDefinition](../resources/unifiedroledefinition.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="e8b9d-105">Update the properties of a [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object for an RBAC provider.</span></span>

<span data-ttu-id="e8b9d-106">目前支持以下 RBAC 提供程序：</span><span class="sxs-lookup"><span data-stu-id="e8b9d-106">The following RBAC providers are currently supported:</span></span>
- <span data-ttu-id="e8b9d-107">Intune (设备) </span><span class="sxs-lookup"><span data-stu-id="e8b9d-107">device management (Intune)</span></span>
- <span data-ttu-id="e8b9d-108">Azure AD (目录) </span><span class="sxs-lookup"><span data-stu-id="e8b9d-108">directory (Azure AD)</span></span> 

> [!NOTE]
> <span data-ttu-id="e8b9d-109">云电脑 RBAC 提供商当前仅支持[列表和](rbacapplication-list-roledefinitions.md)[获取](unifiedroledefinition-get.md)操作。</span><span class="sxs-lookup"><span data-stu-id="e8b9d-109">The cloud PC RBAC provider currently supports only the [list](rbacapplication-list-roledefinitions.md) and [get](unifiedroledefinition-get.md) operations.</span></span>

## <a name="permissions"></a><span data-ttu-id="e8b9d-110">权限</span><span class="sxs-lookup"><span data-stu-id="e8b9d-110">Permissions</span></span>

<span data-ttu-id="e8b9d-111">根据 RBAC 提供程序以及 (或应用程序) 的权限类型，从下表中选择调用此 API 所需的最低特权权限。</span><span class="sxs-lookup"><span data-stu-id="e8b9d-111">Depending on the RBAC provider and the permission type (delegated or application) that is needed, choose from the following table the least privileged permission required to call this API.</span></span> <span data-ttu-id="e8b9d-112">若要了解详细信息，包括在选择更多特权之前的[注意事项](/graph/auth/auth-concepts#best-practices-for-requesting-permissions)，请在“[权限](/graph/permissions-reference)”中搜索以下权限。</span><span class="sxs-lookup"><span data-stu-id="e8b9d-112">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in [Permissions](/graph/permissions-reference).</span></span> 

|<span data-ttu-id="e8b9d-113">支持的提供程序</span><span class="sxs-lookup"><span data-stu-id="e8b9d-113">Supported provider</span></span>      | <span data-ttu-id="e8b9d-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e8b9d-114">Delegated (work or school account)</span></span>  | <span data-ttu-id="e8b9d-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e8b9d-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e8b9d-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="e8b9d-116">Application</span></span> |
|:-----------------------|:------------------------------------|:---------------------------------------|:------------|
| <span data-ttu-id="e8b9d-117">设备管理</span><span class="sxs-lookup"><span data-stu-id="e8b9d-117">Device management</span></span> | <span data-ttu-id="e8b9d-118">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8b9d-118">DeviceManagementRBAC.ReadWrite.All</span></span> | <span data-ttu-id="e8b9d-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="e8b9d-119">Not supported.</span></span> | <span data-ttu-id="e8b9d-120">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8b9d-120">DeviceManagementRBAC.ReadWrite.All</span></span> |
| <span data-ttu-id="e8b9d-121">目录</span><span class="sxs-lookup"><span data-stu-id="e8b9d-121">Directory</span></span> | <span data-ttu-id="e8b9d-122">RoleManagement.ReadWrite.Directory、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e8b9d-122">RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> | <span data-ttu-id="e8b9d-123">不支持。</span><span class="sxs-lookup"><span data-stu-id="e8b9d-123">Not supported.</span></span>| <span data-ttu-id="e8b9d-124">RoleManagement.ReadWrite.Directory、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8b9d-124">RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e8b9d-125">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e8b9d-125">HTTP request</span></span>

<span data-ttu-id="e8b9d-126">若要更新设备管理提供程序的角色定义，请运行：</span><span class="sxs-lookup"><span data-stu-id="e8b9d-126">To update a role definition for a device management provider:</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /roleManagement/deviceManagement/roleDefinitions/{id}
```

<span data-ttu-id="e8b9d-127">更新目录提供程序的角色定义：</span><span class="sxs-lookup"><span data-stu-id="e8b9d-127">To update a role definition for a directory provider:</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /roleManagement/directory/roleDefinitions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="e8b9d-128">请求标头</span><span class="sxs-lookup"><span data-stu-id="e8b9d-128">Request headers</span></span>

| <span data-ttu-id="e8b9d-129">名称</span><span class="sxs-lookup"><span data-stu-id="e8b9d-129">Name</span></span>       | <span data-ttu-id="e8b9d-130">说明</span><span class="sxs-lookup"><span data-stu-id="e8b9d-130">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="e8b9d-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="e8b9d-131">Authorization</span></span> | <span data-ttu-id="e8b9d-132">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="e8b9d-132">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="e8b9d-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="e8b9d-133">Request body</span></span>

<span data-ttu-id="e8b9d-134">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="e8b9d-134">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="e8b9d-135">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="e8b9d-135">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="e8b9d-136">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="e8b9d-136">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="e8b9d-137">属性</span><span class="sxs-lookup"><span data-stu-id="e8b9d-137">Property</span></span>     | <span data-ttu-id="e8b9d-138">类型</span><span class="sxs-lookup"><span data-stu-id="e8b9d-138">Type</span></span>        | <span data-ttu-id="e8b9d-139">说明</span><span class="sxs-lookup"><span data-stu-id="e8b9d-139">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e8b9d-140">说明</span><span class="sxs-lookup"><span data-stu-id="e8b9d-140">description</span></span>|<span data-ttu-id="e8b9d-141">String</span><span class="sxs-lookup"><span data-stu-id="e8b9d-141">String</span></span>| <span data-ttu-id="e8b9d-142">角色定义的说明。</span><span class="sxs-lookup"><span data-stu-id="e8b9d-142">The description for the role definition.</span></span> <span data-ttu-id="e8b9d-143">isBuiltIn 为 true 时为只读。</span><span class="sxs-lookup"><span data-stu-id="e8b9d-143">Read-only when isBuiltIn is true.</span></span> |
|<span data-ttu-id="e8b9d-144">displayName</span><span class="sxs-lookup"><span data-stu-id="e8b9d-144">displayName</span></span>|<span data-ttu-id="e8b9d-145">String</span><span class="sxs-lookup"><span data-stu-id="e8b9d-145">String</span></span>| <span data-ttu-id="e8b9d-146">角色显示名称的角色定义。</span><span class="sxs-lookup"><span data-stu-id="e8b9d-146">The display name for the role definition.</span></span> <span data-ttu-id="e8b9d-147">isBuiltIn 为 true 时为只读。</span><span class="sxs-lookup"><span data-stu-id="e8b9d-147">Read-only when isBuiltIn is true.</span></span> <span data-ttu-id="e8b9d-148">必需。</span><span class="sxs-lookup"><span data-stu-id="e8b9d-148">Required.</span></span>|
|<span data-ttu-id="e8b9d-149">id</span><span class="sxs-lookup"><span data-stu-id="e8b9d-149">id</span></span>|<span data-ttu-id="e8b9d-150">String</span><span class="sxs-lookup"><span data-stu-id="e8b9d-150">String</span></span>| <span data-ttu-id="e8b9d-151">角色定义的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="e8b9d-151">The unique identifier for the role definition.</span></span> <span data-ttu-id="e8b9d-152">键，不可为 null，只读。</span><span class="sxs-lookup"><span data-stu-id="e8b9d-152">Key, not nullable, Read-only.</span></span> |
|<span data-ttu-id="e8b9d-153">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="e8b9d-153">isBuiltIn</span></span>|<span data-ttu-id="e8b9d-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8b9d-154">Boolean</span></span>| <span data-ttu-id="e8b9d-155">指示角色定义是否属于产品或自定义中包含的默认集的标志。</span><span class="sxs-lookup"><span data-stu-id="e8b9d-155">Flag indicating if the role definition is part of the default set included with the product or custom.</span></span> <span data-ttu-id="e8b9d-156">只读。</span><span class="sxs-lookup"><span data-stu-id="e8b9d-156">Read-only.</span></span> |
|<span data-ttu-id="e8b9d-157">isEnabled</span><span class="sxs-lookup"><span data-stu-id="e8b9d-157">isEnabled</span></span>|<span data-ttu-id="e8b9d-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8b9d-158">Boolean</span></span>| <span data-ttu-id="e8b9d-159">指示角色是否已启用分配的标志。</span><span class="sxs-lookup"><span data-stu-id="e8b9d-159">Flag indicating if the role is enabled for assignment.</span></span> <span data-ttu-id="e8b9d-160">如果为 false，则角色不能用于分配。</span><span class="sxs-lookup"><span data-stu-id="e8b9d-160">If false the role is not available for assignment.</span></span> <span data-ttu-id="e8b9d-161">isBuiltIn 为 true 时为只读。</span><span class="sxs-lookup"><span data-stu-id="e8b9d-161">Read-only when isBuiltIn is true.</span></span> |
|<span data-ttu-id="e8b9d-162">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="e8b9d-162">resourceScopes</span></span>|<span data-ttu-id="e8b9d-163">String collection</span><span class="sxs-lookup"><span data-stu-id="e8b9d-163">String collection</span></span>| <span data-ttu-id="e8b9d-164">角色定义授予的作用域权限列表适用。</span><span class="sxs-lookup"><span data-stu-id="e8b9d-164">List of scopes permissions granted by the role definition apply to.</span></span> <span data-ttu-id="e8b9d-165">目前仅支持"/"。</span><span class="sxs-lookup"><span data-stu-id="e8b9d-165">Currently only "/" is supported.</span></span> <span data-ttu-id="e8b9d-166">isBuiltIn 为 true 时为只读。</span><span class="sxs-lookup"><span data-stu-id="e8b9d-166">Read-only when isBuiltIn is true.</span></span> <span data-ttu-id="e8b9d-167">**请勿使用。此属性将很快弃用。将作用域附加到角色分配。**</span><span class="sxs-lookup"><span data-stu-id="e8b9d-167">**DO NOT USE. This property will be deprecated soon. Attach scope to role assignment.**</span></span>|
|<span data-ttu-id="e8b9d-168">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="e8b9d-168">rolePermissions</span></span>|<span data-ttu-id="e8b9d-169">[unifiedRolePermission](../resources/unifiedrolepermission.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e8b9d-169">[unifiedRolePermission](../resources/unifiedrolepermission.md) collection</span></span>| <span data-ttu-id="e8b9d-170">角色中包含的权限列表。</span><span class="sxs-lookup"><span data-stu-id="e8b9d-170">List of permissions included in the role.</span></span> <span data-ttu-id="e8b9d-171">isBuiltIn 为 true 时为只读。</span><span class="sxs-lookup"><span data-stu-id="e8b9d-171">Read-only when isBuiltIn is true.</span></span> <span data-ttu-id="e8b9d-172">必填。</span><span class="sxs-lookup"><span data-stu-id="e8b9d-172">Required.</span></span> |
|<span data-ttu-id="e8b9d-173">templateId</span><span class="sxs-lookup"><span data-stu-id="e8b9d-173">templateId</span></span>|<span data-ttu-id="e8b9d-174">String</span><span class="sxs-lookup"><span data-stu-id="e8b9d-174">String</span></span>| <span data-ttu-id="e8b9d-175">可以在 isBuiltIn 为 false 时设置的自定义模板标识符。</span><span class="sxs-lookup"><span data-stu-id="e8b9d-175">Custom template identifier that can be set when isBuiltIn is false.</span></span> <span data-ttu-id="e8b9d-176">如果一个标识符在不同目录之间需要相同，则通常使用此标识符。</span><span class="sxs-lookup"><span data-stu-id="e8b9d-176">This identifier is typically used if one needs an identifier to be the same across different directories.</span></span> <span data-ttu-id="e8b9d-177">isBuiltIn 为 true 时为只读。</span><span class="sxs-lookup"><span data-stu-id="e8b9d-177">Read-only when isBuiltIn is true.</span></span> |
|<span data-ttu-id="e8b9d-178">inheritsPermissionsFrom</span><span class="sxs-lookup"><span data-stu-id="e8b9d-178">inheritsPermissionsFrom</span></span>| <span data-ttu-id="e8b9d-179">[unifiedRoleDefinition](../resources/unifiedroledefinition.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e8b9d-179">[unifiedRoleDefinition](../resources/unifiedroledefinition.md) collection</span></span>| <span data-ttu-id="e8b9d-180">给定角色定义从其继承的角色定义的只读集合。</span><span class="sxs-lookup"><span data-stu-id="e8b9d-180">Read-only collection of role definitions that the given role definition inherits from.</span></span> <span data-ttu-id="e8b9d-181">仅 Azure AD 内置角色支持此属性。</span><span class="sxs-lookup"><span data-stu-id="e8b9d-181">Only Azure AD built-in roles support this attribute.</span></span> |
|<span data-ttu-id="e8b9d-182">version</span><span class="sxs-lookup"><span data-stu-id="e8b9d-182">version</span></span>|<span data-ttu-id="e8b9d-183">String</span><span class="sxs-lookup"><span data-stu-id="e8b9d-183">String</span></span>| <span data-ttu-id="e8b9d-184">指示角色定义的版本。</span><span class="sxs-lookup"><span data-stu-id="e8b9d-184">Indicates version of the role definition.</span></span> <span data-ttu-id="e8b9d-185">isBuiltIn 为 true 时为只读。</span><span class="sxs-lookup"><span data-stu-id="e8b9d-185">Read-only when isBuiltIn is true.</span></span>|

## <a name="response"></a><span data-ttu-id="e8b9d-186">响应</span><span class="sxs-lookup"><span data-stu-id="e8b9d-186">Response</span></span>

<span data-ttu-id="e8b9d-187">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [unifiedRoleDefinition](../resources/unifiedroledefinition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e8b9d-187">If successful, this method returns a `200 OK` response code and an updated [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e8b9d-188">示例</span><span class="sxs-lookup"><span data-stu-id="e8b9d-188">Example</span></span>

### <a name="request"></a><span data-ttu-id="e8b9d-189">请求</span><span class="sxs-lookup"><span data-stu-id="e8b9d-189">Request</span></span>

<span data-ttu-id="e8b9d-190">以下示例更新目录提供程序 **的 unifiedRoleDefinition。**</span><span class="sxs-lookup"><span data-stu-id="e8b9d-190">The following example updates a **unifiedRoleDefinition** for a directory provider.</span></span>


# <a name="http"></a>[<span data-ttu-id="e8b9d-191">HTTP</span><span class="sxs-lookup"><span data-stu-id="e8b9d-191">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="e8b9d-192">C#</span><span class="sxs-lookup"><span data-stu-id="e8b9d-192">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-unifiedroledefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e8b9d-193">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e8b9d-193">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-unifiedroledefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e8b9d-194">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e8b9d-194">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-unifiedroledefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e8b9d-195">Java</span><span class="sxs-lookup"><span data-stu-id="e8b9d-195">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-unifiedroledefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e8b9d-196">响应</span><span class="sxs-lookup"><span data-stu-id="e8b9d-196">Response</span></span>

<span data-ttu-id="e8b9d-197">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="e8b9d-197">The following is an example of the response.</span></span>
> <span data-ttu-id="e8b9d-198">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="e8b9d-198">**Note:** The response object shown here might be shortened for readability.</span></span>

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



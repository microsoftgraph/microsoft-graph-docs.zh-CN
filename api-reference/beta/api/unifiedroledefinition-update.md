---
title: 更新 unifiedRoleDefinition
description: 更新 unifiedRoleDefinition 对象的属性。
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: af8e75ca0364a269168c2c3b072c8c7ec6c087ae
ms.sourcegitcommit: 4888ac7504533344c4fc6828e2a06a002a1d72d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/09/2021
ms.locfileid: "53351074"
---
# <a name="update-unifiedroledefinition"></a><span data-ttu-id="85587-103">更新 unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="85587-103">Update unifiedRoleDefinition</span></span>

<span data-ttu-id="85587-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="85587-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="85587-105">更新 RBAC 提供程序 [的 unifiedRoleDefinition](../resources/unifiedroledefinition.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="85587-105">Update the properties of a [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object for an RBAC provider.</span></span>

<span data-ttu-id="85587-106">目前支持以下 RBAC 提供程序：</span><span class="sxs-lookup"><span data-stu-id="85587-106">The following RBAC providers are currently supported:</span></span>
- <span data-ttu-id="85587-107">Intune (设备) </span><span class="sxs-lookup"><span data-stu-id="85587-107">device management (Intune)</span></span>
- <span data-ttu-id="85587-108">Azure AD (目录) </span><span class="sxs-lookup"><span data-stu-id="85587-108">directory (Azure AD)</span></span> 

> [!NOTE]
> <span data-ttu-id="85587-109">云电脑 RBAC 提供商当前仅支持[列表和](rbacapplication-list-roledefinitions.md)[获取](unifiedroledefinition-get.md)操作。</span><span class="sxs-lookup"><span data-stu-id="85587-109">The cloud PC RBAC provider currently supports only the [list](rbacapplication-list-roledefinitions.md) and [get](unifiedroledefinition-get.md) operations.</span></span>

## <a name="permissions"></a><span data-ttu-id="85587-110">权限</span><span class="sxs-lookup"><span data-stu-id="85587-110">Permissions</span></span>

<span data-ttu-id="85587-111">根据 RBAC 提供程序以及 (或应用程序) 的权限类型，从下表中选择调用此 API 所需的最低特权权限。</span><span class="sxs-lookup"><span data-stu-id="85587-111">Depending on the RBAC provider and the permission type (delegated or application) that is needed, choose from the following table the least privileged permission required to call this API.</span></span> <span data-ttu-id="85587-112">若要了解 [更多信息（包括在](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) 选择更多特权权限之前要谨慎操作），请搜索权限参考 [中的以下权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="85587-112">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in the [Permissions reference](/graph/permissions-reference).</span></span> 

### <a name="for-device-management-intune-provider"></a><span data-ttu-id="85587-113">对于 Intune (提供程序的设备) 管理</span><span class="sxs-lookup"><span data-stu-id="85587-113">For Device management (Intune) provider</span></span>

|<span data-ttu-id="85587-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="85587-114">Permission type</span></span>      | <span data-ttu-id="85587-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="85587-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="85587-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="85587-116">Delegated (work or school account)</span></span> |  <span data-ttu-id="85587-117">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="85587-117">DeviceManagementRBAC.ReadWrite.All</span></span>   |
|<span data-ttu-id="85587-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="85587-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="85587-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="85587-119">Not supported.</span></span>    |
|<span data-ttu-id="85587-120">Application</span><span class="sxs-lookup"><span data-stu-id="85587-120">Application</span></span> | <span data-ttu-id="85587-121">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="85587-121">DeviceManagementRBAC.ReadWrite.All</span></span> |

### <a name="for-directory-azure-ad-provider"></a><span data-ttu-id="85587-122">对于 Azure AD (提供程序) 目录</span><span class="sxs-lookup"><span data-stu-id="85587-122">For Directory (Azure AD) provider</span></span>

|<span data-ttu-id="85587-123">权限类型</span><span class="sxs-lookup"><span data-stu-id="85587-123">Permission type</span></span>      | <span data-ttu-id="85587-124">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="85587-124">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="85587-125">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="85587-125">Delegated (work or school account)</span></span> |  <span data-ttu-id="85587-126">RoleManagement.ReadWrite.Directory、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="85587-126">RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>   |
|<span data-ttu-id="85587-127">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="85587-127">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="85587-128">不支持。</span><span class="sxs-lookup"><span data-stu-id="85587-128">Not supported.</span></span>    |
|<span data-ttu-id="85587-129">Application</span><span class="sxs-lookup"><span data-stu-id="85587-129">Application</span></span> | <span data-ttu-id="85587-130">RoleManagement.ReadWrite.Directory、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="85587-130">RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="85587-131">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="85587-131">HTTP request</span></span>

<span data-ttu-id="85587-132">若要更新设备管理提供程序的角色定义，请运行：</span><span class="sxs-lookup"><span data-stu-id="85587-132">To update a role definition for a device management provider:</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /roleManagement/deviceManagement/roleDefinitions/{id}
```

<span data-ttu-id="85587-133">更新目录提供程序的角色定义：</span><span class="sxs-lookup"><span data-stu-id="85587-133">To update a role definition for a directory provider:</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /roleManagement/directory/roleDefinitions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="85587-134">请求标头</span><span class="sxs-lookup"><span data-stu-id="85587-134">Request headers</span></span>

| <span data-ttu-id="85587-135">名称</span><span class="sxs-lookup"><span data-stu-id="85587-135">Name</span></span>       | <span data-ttu-id="85587-136">说明</span><span class="sxs-lookup"><span data-stu-id="85587-136">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="85587-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="85587-137">Authorization</span></span> | <span data-ttu-id="85587-138">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="85587-138">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="85587-139">请求正文</span><span class="sxs-lookup"><span data-stu-id="85587-139">Request body</span></span>

<span data-ttu-id="85587-140">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="85587-140">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="85587-141">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="85587-141">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="85587-142">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="85587-142">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="85587-143">属性</span><span class="sxs-lookup"><span data-stu-id="85587-143">Property</span></span>     | <span data-ttu-id="85587-144">类型</span><span class="sxs-lookup"><span data-stu-id="85587-144">Type</span></span>        | <span data-ttu-id="85587-145">说明</span><span class="sxs-lookup"><span data-stu-id="85587-145">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="85587-146">说明</span><span class="sxs-lookup"><span data-stu-id="85587-146">description</span></span>|<span data-ttu-id="85587-147">字符串</span><span class="sxs-lookup"><span data-stu-id="85587-147">String</span></span>| <span data-ttu-id="85587-148">角色定义的说明。</span><span class="sxs-lookup"><span data-stu-id="85587-148">The description for the role definition.</span></span> <span data-ttu-id="85587-149">isBuiltIn 为 true 时为只读。</span><span class="sxs-lookup"><span data-stu-id="85587-149">Read-only when isBuiltIn is true.</span></span> |
|<span data-ttu-id="85587-150">displayName</span><span class="sxs-lookup"><span data-stu-id="85587-150">displayName</span></span>|<span data-ttu-id="85587-151">字符串</span><span class="sxs-lookup"><span data-stu-id="85587-151">String</span></span>| <span data-ttu-id="85587-152">角色显示名称的角色定义。</span><span class="sxs-lookup"><span data-stu-id="85587-152">The display name for the role definition.</span></span> <span data-ttu-id="85587-153">isBuiltIn 为 true 时为只读。</span><span class="sxs-lookup"><span data-stu-id="85587-153">Read-only when isBuiltIn is true.</span></span> <span data-ttu-id="85587-154">必需。</span><span class="sxs-lookup"><span data-stu-id="85587-154">Required.</span></span>|
|<span data-ttu-id="85587-155">id</span><span class="sxs-lookup"><span data-stu-id="85587-155">id</span></span>|<span data-ttu-id="85587-156">字符串</span><span class="sxs-lookup"><span data-stu-id="85587-156">String</span></span>| <span data-ttu-id="85587-157">角色定义的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="85587-157">The unique identifier for the role definition.</span></span> <span data-ttu-id="85587-158">键，不可为 null，只读。</span><span class="sxs-lookup"><span data-stu-id="85587-158">Key, not nullable, Read-only.</span></span> |
|<span data-ttu-id="85587-159">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="85587-159">isBuiltIn</span></span>|<span data-ttu-id="85587-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="85587-160">Boolean</span></span>| <span data-ttu-id="85587-161">指示角色定义是否属于产品或自定义中包含的默认集的标志。</span><span class="sxs-lookup"><span data-stu-id="85587-161">Flag indicating if the role definition is part of the default set included with the product or custom.</span></span> <span data-ttu-id="85587-162">只读。</span><span class="sxs-lookup"><span data-stu-id="85587-162">Read-only.</span></span> |
|<span data-ttu-id="85587-163">isEnabled</span><span class="sxs-lookup"><span data-stu-id="85587-163">isEnabled</span></span>|<span data-ttu-id="85587-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="85587-164">Boolean</span></span>| <span data-ttu-id="85587-165">指示角色是否已启用分配的标志。</span><span class="sxs-lookup"><span data-stu-id="85587-165">Flag indicating if the role is enabled for assignment.</span></span> <span data-ttu-id="85587-166">如果为 false，则角色不能用于分配。</span><span class="sxs-lookup"><span data-stu-id="85587-166">If false the role is not available for assignment.</span></span> <span data-ttu-id="85587-167">isBuiltIn 为 true 时为只读。</span><span class="sxs-lookup"><span data-stu-id="85587-167">Read-only when isBuiltIn is true.</span></span> |
|<span data-ttu-id="85587-168">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="85587-168">resourceScopes</span></span>|<span data-ttu-id="85587-169">String collection</span><span class="sxs-lookup"><span data-stu-id="85587-169">String collection</span></span>| <span data-ttu-id="85587-170">角色定义授予的作用域权限列表适用。</span><span class="sxs-lookup"><span data-stu-id="85587-170">List of scopes permissions granted by the role definition apply to.</span></span> <span data-ttu-id="85587-171">目前仅支持"/"。</span><span class="sxs-lookup"><span data-stu-id="85587-171">Currently only "/" is supported.</span></span> <span data-ttu-id="85587-172">isBuiltIn 为 true 时为只读。</span><span class="sxs-lookup"><span data-stu-id="85587-172">Read-only when isBuiltIn is true.</span></span> <span data-ttu-id="85587-173">**请勿使用。此属性将很快弃用。将作用域附加到角色分配。**</span><span class="sxs-lookup"><span data-stu-id="85587-173">**DO NOT USE. This property will be deprecated soon. Attach scope to role assignment.**</span></span>|
|<span data-ttu-id="85587-174">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="85587-174">rolePermissions</span></span>|<span data-ttu-id="85587-175">[unifiedRolePermission](../resources/unifiedrolepermission.md) 集合</span><span class="sxs-lookup"><span data-stu-id="85587-175">[unifiedRolePermission](../resources/unifiedrolepermission.md) collection</span></span>| <span data-ttu-id="85587-176">角色中包含的权限列表。</span><span class="sxs-lookup"><span data-stu-id="85587-176">List of permissions included in the role.</span></span> <span data-ttu-id="85587-177">isBuiltIn 为 true 时为只读。</span><span class="sxs-lookup"><span data-stu-id="85587-177">Read-only when isBuiltIn is true.</span></span> <span data-ttu-id="85587-178">必填。</span><span class="sxs-lookup"><span data-stu-id="85587-178">Required.</span></span> |
|<span data-ttu-id="85587-179">templateId</span><span class="sxs-lookup"><span data-stu-id="85587-179">templateId</span></span>|<span data-ttu-id="85587-180">字符串</span><span class="sxs-lookup"><span data-stu-id="85587-180">String</span></span>| <span data-ttu-id="85587-181">可以在 isBuiltIn 为 false 时设置的自定义模板标识符。</span><span class="sxs-lookup"><span data-stu-id="85587-181">Custom template identifier that can be set when isBuiltIn is false.</span></span> <span data-ttu-id="85587-182">如果一个标识符在不同目录之间需要相同，则通常使用此标识符。</span><span class="sxs-lookup"><span data-stu-id="85587-182">This identifier is typically used if one needs an identifier to be the same across different directories.</span></span> <span data-ttu-id="85587-183">isBuiltIn 为 true 时为只读。</span><span class="sxs-lookup"><span data-stu-id="85587-183">Read-only when isBuiltIn is true.</span></span> |
|<span data-ttu-id="85587-184">inheritsPermissionsFrom</span><span class="sxs-lookup"><span data-stu-id="85587-184">inheritsPermissionsFrom</span></span>| <span data-ttu-id="85587-185">[unifiedRoleDefinition](../resources/unifiedroledefinition.md) 集合</span><span class="sxs-lookup"><span data-stu-id="85587-185">[unifiedRoleDefinition](../resources/unifiedroledefinition.md) collection</span></span>| <span data-ttu-id="85587-186">给定角色定义从其继承的角色定义的只读集合。</span><span class="sxs-lookup"><span data-stu-id="85587-186">Read-only collection of role definitions that the given role definition inherits from.</span></span> <span data-ttu-id="85587-187">仅 Azure AD 内置角色支持此属性。</span><span class="sxs-lookup"><span data-stu-id="85587-187">Only Azure AD built-in roles support this attribute.</span></span> |
|<span data-ttu-id="85587-188">version</span><span class="sxs-lookup"><span data-stu-id="85587-188">version</span></span>|<span data-ttu-id="85587-189">String</span><span class="sxs-lookup"><span data-stu-id="85587-189">String</span></span>| <span data-ttu-id="85587-190">指示角色定义的版本。</span><span class="sxs-lookup"><span data-stu-id="85587-190">Indicates version of the role definition.</span></span> <span data-ttu-id="85587-191">isBuiltIn 为 true 时为只读。</span><span class="sxs-lookup"><span data-stu-id="85587-191">Read-only when isBuiltIn is true.</span></span>|

## <a name="response"></a><span data-ttu-id="85587-192">响应</span><span class="sxs-lookup"><span data-stu-id="85587-192">Response</span></span>

<span data-ttu-id="85587-193">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [unifiedRoleDefinition](../resources/unifiedroledefinition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="85587-193">If successful, this method returns a `200 OK` response code and an updated [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="85587-194">示例</span><span class="sxs-lookup"><span data-stu-id="85587-194">Example</span></span>

### <a name="request"></a><span data-ttu-id="85587-195">请求</span><span class="sxs-lookup"><span data-stu-id="85587-195">Request</span></span>

<span data-ttu-id="85587-196">以下示例更新目录提供程序 **的 unifiedRoleDefinition。**</span><span class="sxs-lookup"><span data-stu-id="85587-196">The following example updates a **unifiedRoleDefinition** for a directory provider.</span></span>


# <a name="http"></a>[<span data-ttu-id="85587-197">HTTP</span><span class="sxs-lookup"><span data-stu-id="85587-197">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="85587-198">C#</span><span class="sxs-lookup"><span data-stu-id="85587-198">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-unifiedroledefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="85587-199">JavaScript</span><span class="sxs-lookup"><span data-stu-id="85587-199">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-unifiedroledefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="85587-200">Objective-C</span><span class="sxs-lookup"><span data-stu-id="85587-200">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-unifiedroledefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="85587-201">Java</span><span class="sxs-lookup"><span data-stu-id="85587-201">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-unifiedroledefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="85587-202">响应</span><span class="sxs-lookup"><span data-stu-id="85587-202">Response</span></span>

<span data-ttu-id="85587-203">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="85587-203">The following is an example of the response.</span></span>
> <span data-ttu-id="85587-204">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="85587-204">**Note:** The response object shown here might be shortened for readability.</span></span>

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



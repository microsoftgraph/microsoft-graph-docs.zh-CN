---
title: 更新 unifiedRoleDefinition
description: 更新 unifiedRoleDefinition 对象的属性。
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 38ab5c03693978cf62725b5d680f24a323f602d4
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50444761"
---
# <a name="update-unifiedroledefinition"></a><span data-ttu-id="09844-103">更新 unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="09844-103">Update unifiedRoleDefinition</span></span>

<span data-ttu-id="09844-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="09844-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="09844-105">更新 [unifiedRoleDefinition 对象](../resources/unifiedroledefinition.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="09844-105">Update the properties of a [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="09844-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="09844-106">Permissions</span></span>

<span data-ttu-id="09844-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="09844-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="09844-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="09844-109">Permission type</span></span>                        | <span data-ttu-id="09844-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="09844-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="09844-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="09844-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="09844-112">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="09844-112">RoleManagement.ReadWrite.Directory</span></span> |
| <span data-ttu-id="09844-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="09844-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="09844-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="09844-114">Not supported.</span></span> |
| <span data-ttu-id="09844-115">Application</span><span class="sxs-lookup"><span data-stu-id="09844-115">Application</span></span>                            | <span data-ttu-id="09844-116">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="09844-116">RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="09844-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="09844-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /roleManagement/directory/roleDefinitions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="09844-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="09844-118">Request headers</span></span>

| <span data-ttu-id="09844-119">名称</span><span class="sxs-lookup"><span data-stu-id="09844-119">Name</span></span>       | <span data-ttu-id="09844-120">说明</span><span class="sxs-lookup"><span data-stu-id="09844-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="09844-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="09844-121">Authorization</span></span> | <span data-ttu-id="09844-122">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="09844-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="09844-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="09844-123">Request body</span></span>

<span data-ttu-id="09844-124">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="09844-124">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="09844-125">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="09844-125">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="09844-126">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="09844-126">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="09844-127">属性</span><span class="sxs-lookup"><span data-stu-id="09844-127">Property</span></span>     | <span data-ttu-id="09844-128">类型</span><span class="sxs-lookup"><span data-stu-id="09844-128">Type</span></span>        | <span data-ttu-id="09844-129">说明</span><span class="sxs-lookup"><span data-stu-id="09844-129">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="09844-130">说明</span><span class="sxs-lookup"><span data-stu-id="09844-130">description</span></span>|<span data-ttu-id="09844-131">String</span><span class="sxs-lookup"><span data-stu-id="09844-131">String</span></span>| <span data-ttu-id="09844-132">角色定义的说明。</span><span class="sxs-lookup"><span data-stu-id="09844-132">The description for the role definition.</span></span> <span data-ttu-id="09844-133">isBuiltIn 为 true 时为只读。</span><span class="sxs-lookup"><span data-stu-id="09844-133">Read-only when isBuiltIn is true.</span></span> |
|<span data-ttu-id="09844-134">displayName</span><span class="sxs-lookup"><span data-stu-id="09844-134">displayName</span></span>|<span data-ttu-id="09844-135">String</span><span class="sxs-lookup"><span data-stu-id="09844-135">String</span></span>| <span data-ttu-id="09844-136">角色显示名称的定义。</span><span class="sxs-lookup"><span data-stu-id="09844-136">The display name for the role definition.</span></span> <span data-ttu-id="09844-137">isBuiltIn 为 true 时为只读。</span><span class="sxs-lookup"><span data-stu-id="09844-137">Read-only when isBuiltIn is true.</span></span> <span data-ttu-id="09844-138">必需。</span><span class="sxs-lookup"><span data-stu-id="09844-138">Required.</span></span>|
|<span data-ttu-id="09844-139">id</span><span class="sxs-lookup"><span data-stu-id="09844-139">id</span></span>|<span data-ttu-id="09844-140">String</span><span class="sxs-lookup"><span data-stu-id="09844-140">String</span></span>| <span data-ttu-id="09844-141">角色定义的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="09844-141">The unique identifier for the role definition.</span></span> <span data-ttu-id="09844-142">键，不可为 null，只读。</span><span class="sxs-lookup"><span data-stu-id="09844-142">Key, not nullable, Read-only.</span></span> |
|<span data-ttu-id="09844-143">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="09844-143">isBuiltIn</span></span>|<span data-ttu-id="09844-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="09844-144">Boolean</span></span>| <span data-ttu-id="09844-145">指示角色定义是产品或自定义中包含的默认集的一部分的标志。</span><span class="sxs-lookup"><span data-stu-id="09844-145">Flag indicating if the role definition is part of the default set included with the product or custom.</span></span> <span data-ttu-id="09844-146">只读。</span><span class="sxs-lookup"><span data-stu-id="09844-146">Read-only.</span></span> |
|<span data-ttu-id="09844-147">isEnabled</span><span class="sxs-lookup"><span data-stu-id="09844-147">isEnabled</span></span>|<span data-ttu-id="09844-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="09844-148">Boolean</span></span>| <span data-ttu-id="09844-149">指示是否已启用角色分配的标志。</span><span class="sxs-lookup"><span data-stu-id="09844-149">Flag indicating if the role is enabled for assignment.</span></span> <span data-ttu-id="09844-150">如果为 false，则角色不能用于分配。</span><span class="sxs-lookup"><span data-stu-id="09844-150">If false the role is not available for assignment.</span></span> <span data-ttu-id="09844-151">isBuiltIn 为 true 时为只读。</span><span class="sxs-lookup"><span data-stu-id="09844-151">Read-only when isBuiltIn is true.</span></span> |
|<span data-ttu-id="09844-152">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="09844-152">resourceScopes</span></span>|<span data-ttu-id="09844-153">String collection</span><span class="sxs-lookup"><span data-stu-id="09844-153">String collection</span></span>| <span data-ttu-id="09844-154">角色定义授予的范围权限列表适用。</span><span class="sxs-lookup"><span data-stu-id="09844-154">List of scopes permissions granted by the role definition apply to.</span></span> <span data-ttu-id="09844-155">当前仅支持"/"。</span><span class="sxs-lookup"><span data-stu-id="09844-155">Currently only "/" is supported.</span></span> <span data-ttu-id="09844-156">isBuiltIn 为 true 时为只读。</span><span class="sxs-lookup"><span data-stu-id="09844-156">Read-only when isBuiltIn is true.</span></span> <span data-ttu-id="09844-157">**请勿使用。此属性将很快弃用。将作用域附加到角色分配。**</span><span class="sxs-lookup"><span data-stu-id="09844-157">**DO NOT USE. This property will be deprecated soon. Attach scope to role assignment.**</span></span>|
|<span data-ttu-id="09844-158">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="09844-158">rolePermissions</span></span>|<span data-ttu-id="09844-159">[unifiedRolePermission](../resources/unifiedrolepermission.md) 集合</span><span class="sxs-lookup"><span data-stu-id="09844-159">[unifiedRolePermission](../resources/unifiedrolepermission.md) collection</span></span>| <span data-ttu-id="09844-160">角色中包含的权限列表。</span><span class="sxs-lookup"><span data-stu-id="09844-160">List of permissions included in the role.</span></span> <span data-ttu-id="09844-161">isBuiltIn 为 true 时为只读。</span><span class="sxs-lookup"><span data-stu-id="09844-161">Read-only when isBuiltIn is true.</span></span> <span data-ttu-id="09844-162">必需。</span><span class="sxs-lookup"><span data-stu-id="09844-162">Required.</span></span> |
|<span data-ttu-id="09844-163">templateId</span><span class="sxs-lookup"><span data-stu-id="09844-163">templateId</span></span>|<span data-ttu-id="09844-164">String</span><span class="sxs-lookup"><span data-stu-id="09844-164">String</span></span>| <span data-ttu-id="09844-165">IsBuiltIn 为 false 时可设置的自定义模板标识符。</span><span class="sxs-lookup"><span data-stu-id="09844-165">Custom template identifier that can be set when isBuiltIn is false.</span></span> <span data-ttu-id="09844-166">如果不同目录的标识符需要相同，则通常使用此标识符。</span><span class="sxs-lookup"><span data-stu-id="09844-166">This identifier is typically used if one needs an identifier to be the same across different directories.</span></span> <span data-ttu-id="09844-167">isBuiltIn 为 true 时为只读。</span><span class="sxs-lookup"><span data-stu-id="09844-167">Read-only when isBuiltIn is true.</span></span> |
|<span data-ttu-id="09844-168">inheritsPermissionsFrom</span><span class="sxs-lookup"><span data-stu-id="09844-168">inheritsPermissionsFrom</span></span>| <span data-ttu-id="09844-169">[unifiedRoleDefinition](../resources/unifiedroledefinition.md) 集合</span><span class="sxs-lookup"><span data-stu-id="09844-169">[unifiedRoleDefinition](../resources/unifiedroledefinition.md) collection</span></span>| <span data-ttu-id="09844-170">给定角色定义从其继承的角色定义的只读集合。</span><span class="sxs-lookup"><span data-stu-id="09844-170">Read-only collection of role definitions that the given role definition inherits from.</span></span> <span data-ttu-id="09844-171">只有 Azure AD 内置角色支持此属性。</span><span class="sxs-lookup"><span data-stu-id="09844-171">Only Azure AD built-in roles support this attribute.</span></span> |
|<span data-ttu-id="09844-172">version</span><span class="sxs-lookup"><span data-stu-id="09844-172">version</span></span>|<span data-ttu-id="09844-173">String</span><span class="sxs-lookup"><span data-stu-id="09844-173">String</span></span>| <span data-ttu-id="09844-174">指示角色定义的版本。</span><span class="sxs-lookup"><span data-stu-id="09844-174">Indicates version of the role definition.</span></span> <span data-ttu-id="09844-175">isBuiltIn 为 true 时为只读。</span><span class="sxs-lookup"><span data-stu-id="09844-175">Read-only when isBuiltIn is true.</span></span>|

## <a name="response"></a><span data-ttu-id="09844-176">响应</span><span class="sxs-lookup"><span data-stu-id="09844-176">Response</span></span>

<span data-ttu-id="09844-177">如果成功，此方法在响应正文中返回响应代码和更新的 `200 OK` [unifiedRoleDefinition](../resources/unifiedroledefinition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="09844-177">If successful, this method returns a `200 OK` response code and an updated [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="09844-178">示例</span><span class="sxs-lookup"><span data-stu-id="09844-178">Example</span></span>

### <a name="request"></a><span data-ttu-id="09844-179">请求</span><span class="sxs-lookup"><span data-stu-id="09844-179">Request</span></span>

<span data-ttu-id="09844-180">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="09844-180">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="09844-181">HTTP</span><span class="sxs-lookup"><span data-stu-id="09844-181">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="09844-182">C#</span><span class="sxs-lookup"><span data-stu-id="09844-182">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-unifiedroledefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="09844-183">JavaScript</span><span class="sxs-lookup"><span data-stu-id="09844-183">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-unifiedroledefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="09844-184">Objective-C</span><span class="sxs-lookup"><span data-stu-id="09844-184">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-unifiedroledefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="09844-185">Java</span><span class="sxs-lookup"><span data-stu-id="09844-185">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-unifiedroledefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="09844-186">响应</span><span class="sxs-lookup"><span data-stu-id="09844-186">Response</span></span>

<span data-ttu-id="09844-187">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="09844-187">The following is an example of the response.</span></span>
> <span data-ttu-id="09844-p113">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="09844-p113">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleDefinition"
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



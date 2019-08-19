---
title: 更新 unifiedRoleDefinition
description: 更新 unifiedRoleDefinition 对象的属性。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 3be16446147e3e0dd9d4c2a481b5fdae63312f6a
ms.sourcegitcommit: f50b1feff72182d1e19bfa346304beaf29558b68
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2019
ms.locfileid: "36461603"
---
# <a name="update-unifiedroledefinition"></a><span data-ttu-id="dd55f-103">更新 unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="dd55f-103">Update unifiedRoleDefinition</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dd55f-104">更新[unifiedRoleDefinition](../resources/unifiedroledefinition.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="dd55f-104">Update the properties of a [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="dd55f-105">权限</span><span class="sxs-lookup"><span data-stu-id="dd55f-105">Permissions</span></span>

<span data-ttu-id="dd55f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="dd55f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="dd55f-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="dd55f-108">Permission type</span></span>                        | <span data-ttu-id="dd55f-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="dd55f-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="dd55f-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dd55f-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="dd55f-111">RoleManagement、RoleManagement、目录</span><span class="sxs-lookup"><span data-stu-id="dd55f-111">RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span> |
| <span data-ttu-id="dd55f-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dd55f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dd55f-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="dd55f-113">Not supported.</span></span> |
| <span data-ttu-id="dd55f-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="dd55f-114">Application</span></span>                            | <span data-ttu-id="dd55f-115">RoleManagement、RoleManagement、目录</span><span class="sxs-lookup"><span data-stu-id="dd55f-115">RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="dd55f-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dd55f-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /roleManagement/directory/roleDefinitions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="dd55f-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="dd55f-117">Request headers</span></span>

| <span data-ttu-id="dd55f-118">名称</span><span class="sxs-lookup"><span data-stu-id="dd55f-118">Name</span></span>       | <span data-ttu-id="dd55f-119">说明</span><span class="sxs-lookup"><span data-stu-id="dd55f-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="dd55f-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="dd55f-120">Authorization</span></span> | <span data-ttu-id="dd55f-121">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="dd55f-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="dd55f-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="dd55f-122">Request body</span></span>

<span data-ttu-id="dd55f-123">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="dd55f-123">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="dd55f-124">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="dd55f-124">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="dd55f-125">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="dd55f-125">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="dd55f-126">属性</span><span class="sxs-lookup"><span data-stu-id="dd55f-126">Property</span></span>     | <span data-ttu-id="dd55f-127">类型</span><span class="sxs-lookup"><span data-stu-id="dd55f-127">Type</span></span>        | <span data-ttu-id="dd55f-128">说明</span><span class="sxs-lookup"><span data-stu-id="dd55f-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="dd55f-129">说明</span><span class="sxs-lookup"><span data-stu-id="dd55f-129">description</span></span>|<span data-ttu-id="dd55f-130">String</span><span class="sxs-lookup"><span data-stu-id="dd55f-130">String</span></span>| <span data-ttu-id="dd55f-131">角色定义的说明。</span><span class="sxs-lookup"><span data-stu-id="dd55f-131">The description for the role definition.</span></span> <span data-ttu-id="dd55f-132">当 isBuiltIn 为 true 时为只读。</span><span class="sxs-lookup"><span data-stu-id="dd55f-132">Read-only when isBuiltIn is true.</span></span> |
|<span data-ttu-id="dd55f-133">displayName</span><span class="sxs-lookup"><span data-stu-id="dd55f-133">displayName</span></span>|<span data-ttu-id="dd55f-134">字符串</span><span class="sxs-lookup"><span data-stu-id="dd55f-134">String</span></span>| <span data-ttu-id="dd55f-135">角色定义的显示名称。</span><span class="sxs-lookup"><span data-stu-id="dd55f-135">The display name for the role definition.</span></span> <span data-ttu-id="dd55f-136">当 isBuiltIn 为 true 时为只读。</span><span class="sxs-lookup"><span data-stu-id="dd55f-136">Read-only when isBuiltIn is true.</span></span> <span data-ttu-id="dd55f-137">必需。</span><span class="sxs-lookup"><span data-stu-id="dd55f-137">Required.</span></span>|
|<span data-ttu-id="dd55f-138">id</span><span class="sxs-lookup"><span data-stu-id="dd55f-138">id</span></span>|<span data-ttu-id="dd55f-139">字符串</span><span class="sxs-lookup"><span data-stu-id="dd55f-139">String</span></span>| <span data-ttu-id="dd55f-140">角色定义的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="dd55f-140">The unique identifier for the role definition.</span></span> <span data-ttu-id="dd55f-141">键, 不可为 null, 只读。</span><span class="sxs-lookup"><span data-stu-id="dd55f-141">Key, not nullable, Read-only.</span></span> |
|<span data-ttu-id="dd55f-142">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="dd55f-142">isBuiltIn</span></span>|<span data-ttu-id="dd55f-143">布尔值</span><span class="sxs-lookup"><span data-stu-id="dd55f-143">Boolean</span></span>| <span data-ttu-id="dd55f-144">指示角色定义是否是产品或自定义的默认设置的一部分的标志。</span><span class="sxs-lookup"><span data-stu-id="dd55f-144">Flag indicating if the role definition is part of the default set included with the product or custom.</span></span> <span data-ttu-id="dd55f-145">只读。</span><span class="sxs-lookup"><span data-stu-id="dd55f-145">Read-only.</span></span> |
|<span data-ttu-id="dd55f-146">isEnabled</span><span class="sxs-lookup"><span data-stu-id="dd55f-146">isEnabled</span></span>|<span data-ttu-id="dd55f-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="dd55f-147">Boolean</span></span>| <span data-ttu-id="dd55f-148">指示角色是否已启用分配的标志。</span><span class="sxs-lookup"><span data-stu-id="dd55f-148">Flag indicating if the role is enabled for assignment.</span></span> <span data-ttu-id="dd55f-149">如果为 false, 则该角色不可用于分配。</span><span class="sxs-lookup"><span data-stu-id="dd55f-149">If false the role is not available for assignment.</span></span> <span data-ttu-id="dd55f-150">当 isBuiltIn 为 true 时为只读。</span><span class="sxs-lookup"><span data-stu-id="dd55f-150">Read-only when isBuiltIn is true.</span></span> |
|<span data-ttu-id="dd55f-151">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="dd55f-151">resourceScopes</span></span>|<span data-ttu-id="dd55f-152">String collection</span><span class="sxs-lookup"><span data-stu-id="dd55f-152">String collection</span></span>| <span data-ttu-id="dd55f-153">由角色定义授予的范围权限列表应用于。</span><span class="sxs-lookup"><span data-stu-id="dd55f-153">List of scopes permissions granted by the role definition apply to.</span></span> <span data-ttu-id="dd55f-154">目前仅支持 "/"。</span><span class="sxs-lookup"><span data-stu-id="dd55f-154">Currently only "/" is supported.</span></span> <span data-ttu-id="dd55f-155">当 isBuiltIn 为 true 时为只读。</span><span class="sxs-lookup"><span data-stu-id="dd55f-155">Read-only when isBuiltIn is true.</span></span> |
|<span data-ttu-id="dd55f-156">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="dd55f-156">rolePermissions</span></span>|<span data-ttu-id="dd55f-157">[unifiedRolePermission](../resources/unifiedrolepermission.md)集合</span><span class="sxs-lookup"><span data-stu-id="dd55f-157">[unifiedRolePermission](../resources/unifiedrolepermission.md) collection</span></span>| <span data-ttu-id="dd55f-158">角色中包含的权限的列表。</span><span class="sxs-lookup"><span data-stu-id="dd55f-158">List of permissions included in the role.</span></span> <span data-ttu-id="dd55f-159">当 isBuiltIn 为 true 时为只读。</span><span class="sxs-lookup"><span data-stu-id="dd55f-159">Read-only when isBuiltIn is true.</span></span> <span data-ttu-id="dd55f-160">必需。</span><span class="sxs-lookup"><span data-stu-id="dd55f-160">Required.</span></span> |
|<span data-ttu-id="dd55f-161">templateId</span><span class="sxs-lookup"><span data-stu-id="dd55f-161">templateId</span></span>|<span data-ttu-id="dd55f-162">String</span><span class="sxs-lookup"><span data-stu-id="dd55f-162">String</span></span>| <span data-ttu-id="dd55f-163">当 isBuiltIn 为 false 时可设置的自定义模板标识符。</span><span class="sxs-lookup"><span data-stu-id="dd55f-163">Custom template identifier that can be set when isBuiltIn is false.</span></span> <span data-ttu-id="dd55f-164">如果一个要求标识符在不同目录中是相同的, 则通常使用此标识符。</span><span class="sxs-lookup"><span data-stu-id="dd55f-164">This identifier is typically used if one needs an identifier to be the same across different directories.</span></span> <span data-ttu-id="dd55f-165">当 isBuiltIn 为 true 时为只读。</span><span class="sxs-lookup"><span data-stu-id="dd55f-165">Read-only when isBuiltIn is true.</span></span> |
|<span data-ttu-id="dd55f-166">version</span><span class="sxs-lookup"><span data-stu-id="dd55f-166">version</span></span>|<span data-ttu-id="dd55f-167">String</span><span class="sxs-lookup"><span data-stu-id="dd55f-167">String</span></span>| <span data-ttu-id="dd55f-168">指示角色定义的版本。</span><span class="sxs-lookup"><span data-stu-id="dd55f-168">Indicates version of the role definition.</span></span> <span data-ttu-id="dd55f-169">当 isBuiltIn 为 true 时为只读。</span><span class="sxs-lookup"><span data-stu-id="dd55f-169">Read-only when isBuiltIn is true.</span></span>|

## <a name="response"></a><span data-ttu-id="dd55f-170">响应</span><span class="sxs-lookup"><span data-stu-id="dd55f-170">Response</span></span>

<span data-ttu-id="dd55f-171">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[unifiedRoleDefinition](../resources/unifiedroledefinition.md)对象。</span><span class="sxs-lookup"><span data-stu-id="dd55f-171">If successful, this method returns a `200 OK` response code and an updated [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dd55f-172">示例</span><span class="sxs-lookup"><span data-stu-id="dd55f-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="dd55f-173">请求</span><span class="sxs-lookup"><span data-stu-id="dd55f-173">Request</span></span>

<span data-ttu-id="dd55f-174">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="dd55f-174">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="dd55f-175">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="dd55f-175">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="dd55f-176">C#</span><span class="sxs-lookup"><span data-stu-id="dd55f-176">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-unifiedroledefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="dd55f-177">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dd55f-177">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-unifiedroledefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="dd55f-178">目标-C</span><span class="sxs-lookup"><span data-stu-id="dd55f-178">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-unifiedroledefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="dd55f-179">响应</span><span class="sxs-lookup"><span data-stu-id="dd55f-179">Response</span></span>

<span data-ttu-id="dd55f-180">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="dd55f-180">The following is an example of the response.</span></span>

> <span data-ttu-id="dd55f-p112">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="dd55f-p112">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

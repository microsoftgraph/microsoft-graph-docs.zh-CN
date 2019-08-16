---
title: 更新 unifiedRoleDefinition
description: 更新 unifiedRoleDefinition 对象的属性。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: bd76b6baa201315dc21ae5b8f610f6c58233b37f
ms.sourcegitcommit: 567d0420243765b4088bc8029306a517f92926fd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/16/2019
ms.locfileid: "36437753"
---
# <a name="update-unifiedroledefinition"></a><span data-ttu-id="0b179-103">更新 unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="0b179-103">Update unifiedRoleDefinition</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0b179-104">更新[unifiedRoleDefinition](../resources/unifiedroledefinition.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="0b179-104">Update the properties of a [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="0b179-105">权限</span><span class="sxs-lookup"><span data-stu-id="0b179-105">Permissions</span></span>

<span data-ttu-id="0b179-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0b179-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0b179-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="0b179-108">Permission type</span></span>                        | <span data-ttu-id="0b179-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0b179-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="0b179-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0b179-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="0b179-111">RoleManagement、RoleManagement、目录</span><span class="sxs-lookup"><span data-stu-id="0b179-111">RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span> |
| <span data-ttu-id="0b179-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0b179-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0b179-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="0b179-113">Not supported.</span></span> |
| <span data-ttu-id="0b179-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="0b179-114">Application</span></span>                            | <span data-ttu-id="0b179-115">RoleManagement、RoleManagement、目录</span><span class="sxs-lookup"><span data-stu-id="0b179-115">RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="0b179-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0b179-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /roleManagement/directory/roleDefinitions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="0b179-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="0b179-117">Request headers</span></span>

| <span data-ttu-id="0b179-118">名称</span><span class="sxs-lookup"><span data-stu-id="0b179-118">Name</span></span>       | <span data-ttu-id="0b179-119">说明</span><span class="sxs-lookup"><span data-stu-id="0b179-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="0b179-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="0b179-120">Authorization</span></span> | <span data-ttu-id="0b179-121">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="0b179-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="0b179-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="0b179-122">Request body</span></span>

<span data-ttu-id="0b179-123">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="0b179-123">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="0b179-124">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="0b179-124">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="0b179-125">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="0b179-125">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="0b179-126">属性</span><span class="sxs-lookup"><span data-stu-id="0b179-126">Property</span></span>     | <span data-ttu-id="0b179-127">类型</span><span class="sxs-lookup"><span data-stu-id="0b179-127">Type</span></span>        | <span data-ttu-id="0b179-128">说明</span><span class="sxs-lookup"><span data-stu-id="0b179-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0b179-129">说明</span><span class="sxs-lookup"><span data-stu-id="0b179-129">description</span></span>|<span data-ttu-id="0b179-130">String</span><span class="sxs-lookup"><span data-stu-id="0b179-130">String</span></span>| <span data-ttu-id="0b179-131">角色定义的说明。</span><span class="sxs-lookup"><span data-stu-id="0b179-131">The description for the role definition.</span></span> <span data-ttu-id="0b179-132">当 isBuiltIn 为 true 时为只读。</span><span class="sxs-lookup"><span data-stu-id="0b179-132">Read-only when isBuiltIn is true.</span></span> |
|<span data-ttu-id="0b179-133">displayName</span><span class="sxs-lookup"><span data-stu-id="0b179-133">displayName</span></span>|<span data-ttu-id="0b179-134">字符串</span><span class="sxs-lookup"><span data-stu-id="0b179-134">String</span></span>| <span data-ttu-id="0b179-135">角色定义的显示名称。</span><span class="sxs-lookup"><span data-stu-id="0b179-135">The display name for the role definition.</span></span> <span data-ttu-id="0b179-136">当 isBuiltIn 为 true 时为只读。</span><span class="sxs-lookup"><span data-stu-id="0b179-136">Read-only when isBuiltIn is true.</span></span> <span data-ttu-id="0b179-137">必需。</span><span class="sxs-lookup"><span data-stu-id="0b179-137">Required.</span></span>|
|<span data-ttu-id="0b179-138">id</span><span class="sxs-lookup"><span data-stu-id="0b179-138">id</span></span>|<span data-ttu-id="0b179-139">字符串</span><span class="sxs-lookup"><span data-stu-id="0b179-139">String</span></span>| <span data-ttu-id="0b179-140">角色定义的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="0b179-140">The unique identifier for the role definition.</span></span> <span data-ttu-id="0b179-141">键, 不可为 null, 只读。</span><span class="sxs-lookup"><span data-stu-id="0b179-141">Key, not nullable, Read-only.</span></span> |
|<span data-ttu-id="0b179-142">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="0b179-142">isBuiltIn</span></span>|<span data-ttu-id="0b179-143">布尔值</span><span class="sxs-lookup"><span data-stu-id="0b179-143">Boolean</span></span>| <span data-ttu-id="0b179-144">指示角色定义是否是产品或自定义的默认设置的一部分的标志。</span><span class="sxs-lookup"><span data-stu-id="0b179-144">Flag indicating if the role definition is part of the default set included with the product or custom.</span></span> <span data-ttu-id="0b179-145">只读。</span><span class="sxs-lookup"><span data-stu-id="0b179-145">Read-only.</span></span> |
|<span data-ttu-id="0b179-146">isEnabled</span><span class="sxs-lookup"><span data-stu-id="0b179-146">isEnabled</span></span>|<span data-ttu-id="0b179-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="0b179-147">Boolean</span></span>| <span data-ttu-id="0b179-148">指示角色是否已启用分配的标志。</span><span class="sxs-lookup"><span data-stu-id="0b179-148">Flag indicating if the role is enabled for assignment.</span></span> <span data-ttu-id="0b179-149">如果为 false, 则该角色不可用于分配。</span><span class="sxs-lookup"><span data-stu-id="0b179-149">If false the role is not available for assignment.</span></span> <span data-ttu-id="0b179-150">当 isBuiltIn 为 true 时为只读。</span><span class="sxs-lookup"><span data-stu-id="0b179-150">Read-only when isBuiltIn is true.</span></span> |
|<span data-ttu-id="0b179-151">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="0b179-151">resourceScopes</span></span>|<span data-ttu-id="0b179-152">String collection</span><span class="sxs-lookup"><span data-stu-id="0b179-152">String collection</span></span>| <span data-ttu-id="0b179-153">由角色定义授予的范围权限列表应用于。</span><span class="sxs-lookup"><span data-stu-id="0b179-153">List of scopes permissions granted by the role definition apply to.</span></span> <span data-ttu-id="0b179-154">目前仅支持 "/"。</span><span class="sxs-lookup"><span data-stu-id="0b179-154">Currently only "/" is supported.</span></span> <span data-ttu-id="0b179-155">当 isBuiltIn 为 true 时为只读。</span><span class="sxs-lookup"><span data-stu-id="0b179-155">Read-only when isBuiltIn is true.</span></span> |
|<span data-ttu-id="0b179-156">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="0b179-156">rolePermissions</span></span>|<span data-ttu-id="0b179-157">[unifiedRolePermission](../resources/unifiedrolepermission.md)集合</span><span class="sxs-lookup"><span data-stu-id="0b179-157">[unifiedRolePermission](../resources/unifiedrolepermission.md) collection</span></span>| <span data-ttu-id="0b179-158">角色中包含的权限的列表。</span><span class="sxs-lookup"><span data-stu-id="0b179-158">List of permissions included in the role.</span></span> <span data-ttu-id="0b179-159">当 isBuiltIn 为 true 时为只读。</span><span class="sxs-lookup"><span data-stu-id="0b179-159">Read-only when isBuiltIn is true.</span></span> <span data-ttu-id="0b179-160">必需。</span><span class="sxs-lookup"><span data-stu-id="0b179-160">Required.</span></span> |
|<span data-ttu-id="0b179-161">templateId</span><span class="sxs-lookup"><span data-stu-id="0b179-161">templateId</span></span>|<span data-ttu-id="0b179-162">String</span><span class="sxs-lookup"><span data-stu-id="0b179-162">String</span></span>| <span data-ttu-id="0b179-163">当 isBuiltIn 为 false 时可设置的自定义模板标识符。</span><span class="sxs-lookup"><span data-stu-id="0b179-163">Custom template identifier that can be set when isBuiltIn is false.</span></span> <span data-ttu-id="0b179-164">如果一个要求标识符在不同目录中是相同的, 则通常使用此标识符。</span><span class="sxs-lookup"><span data-stu-id="0b179-164">This identifier is typically used if one needs an identifier to be the same across different directories.</span></span> <span data-ttu-id="0b179-165">当 isBuiltIn 为 true 时为只读。</span><span class="sxs-lookup"><span data-stu-id="0b179-165">Read-only when isBuiltIn is true.</span></span> |
|<span data-ttu-id="0b179-166">version</span><span class="sxs-lookup"><span data-stu-id="0b179-166">version</span></span>|<span data-ttu-id="0b179-167">String</span><span class="sxs-lookup"><span data-stu-id="0b179-167">String</span></span>| <span data-ttu-id="0b179-168">指示角色定义的版本。</span><span class="sxs-lookup"><span data-stu-id="0b179-168">Indicates version of the role definition.</span></span> <span data-ttu-id="0b179-169">当 isBuiltIn 为 true 时为只读。</span><span class="sxs-lookup"><span data-stu-id="0b179-169">Read-only when isBuiltIn is true.</span></span>|

## <a name="response"></a><span data-ttu-id="0b179-170">响应</span><span class="sxs-lookup"><span data-stu-id="0b179-170">Response</span></span>

<span data-ttu-id="0b179-171">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[unifiedRoleDefinition](../resources/unifiedroledefinition.md)对象。</span><span class="sxs-lookup"><span data-stu-id="0b179-171">If successful, this method returns a `200 OK` response code and an updated [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0b179-172">示例</span><span class="sxs-lookup"><span data-stu-id="0b179-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="0b179-173">请求</span><span class="sxs-lookup"><span data-stu-id="0b179-173">Request</span></span>

<span data-ttu-id="0b179-174">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="0b179-174">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0b179-175">响应</span><span class="sxs-lookup"><span data-stu-id="0b179-175">Response</span></span>

<span data-ttu-id="0b179-176">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="0b179-176">The following is an example of the response.</span></span>

> <span data-ttu-id="0b179-p112">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="0b179-p112">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

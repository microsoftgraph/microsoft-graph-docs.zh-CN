---
title: 创建 unifiedRoleDefinition
description: 创建新的 unifiedRoleDefinition 对象。
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 2485652b97a015797ddd519d2009243a8a85902e
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50440869"
---
# <a name="create-unifiedroledefinition"></a><span data-ttu-id="f1b1c-103">创建 unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="f1b1c-103">Create unifiedRoleDefinition</span></span>

<span data-ttu-id="f1b1c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f1b1c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f1b1c-105">创建新的 [unifiedRoleDefinition](../resources/unifiedroledefinition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f1b1c-105">Create a new [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f1b1c-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="f1b1c-106">Permissions</span></span>

<span data-ttu-id="f1b1c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f1b1c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f1b1c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f1b1c-109">Permission type</span></span>                        | <span data-ttu-id="f1b1c-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f1b1c-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f1b1c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f1b1c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="f1b1c-112">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="f1b1c-112">RoleManagement.ReadWrite.Directory</span></span> |
| <span data-ttu-id="f1b1c-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f1b1c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f1b1c-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f1b1c-114">Not supported.</span></span> |
| <span data-ttu-id="f1b1c-115">Application</span><span class="sxs-lookup"><span data-stu-id="f1b1c-115">Application</span></span>                            | <span data-ttu-id="f1b1c-116">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="f1b1c-116">RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="f1b1c-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f1b1c-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /roleManagement/directory/roleDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="f1b1c-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="f1b1c-118">Request headers</span></span>

| <span data-ttu-id="f1b1c-119">名称</span><span class="sxs-lookup"><span data-stu-id="f1b1c-119">Name</span></span>          | <span data-ttu-id="f1b1c-120">说明</span><span class="sxs-lookup"><span data-stu-id="f1b1c-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="f1b1c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f1b1c-121">Authorization</span></span> | <span data-ttu-id="f1b1c-122">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="f1b1c-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="f1b1c-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="f1b1c-123">Request body</span></span>

<span data-ttu-id="f1b1c-124">在请求正文中，提供 [unifiedRoleDefinition](../resources/unifiedroledefinition.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f1b1c-124">In the request body, supply a JSON representation of [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object.</span></span>

<span data-ttu-id="f1b1c-125">下表显示创建 roleDefinition 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="f1b1c-125">The following table shows the properties that are required when you create a roleDefinition.</span></span>

| <span data-ttu-id="f1b1c-126">参数</span><span class="sxs-lookup"><span data-stu-id="f1b1c-126">Parameter</span></span> | <span data-ttu-id="f1b1c-127">类型</span><span class="sxs-lookup"><span data-stu-id="f1b1c-127">Type</span></span> | <span data-ttu-id="f1b1c-128">说明</span><span class="sxs-lookup"><span data-stu-id="f1b1c-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f1b1c-129">displayName</span><span class="sxs-lookup"><span data-stu-id="f1b1c-129">displayName</span></span> |<span data-ttu-id="f1b1c-130">string</span><span class="sxs-lookup"><span data-stu-id="f1b1c-130">string</span></span> |<span data-ttu-id="f1b1c-131">角色显示名称的定义。</span><span class="sxs-lookup"><span data-stu-id="f1b1c-131">The display name for the role definition.</span></span>|
|<span data-ttu-id="f1b1c-132">isEnabled</span><span class="sxs-lookup"><span data-stu-id="f1b1c-132">isEnabled</span></span> |<span data-ttu-id="f1b1c-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="f1b1c-133">Boolean</span></span> |<span data-ttu-id="f1b1c-134">指示是否已启用角色分配的标志。</span><span class="sxs-lookup"><span data-stu-id="f1b1c-134">Flag indicating if the role is enabled for assignment.</span></span> <span data-ttu-id="f1b1c-135">如果为 false，则角色不能用于分配。</span><span class="sxs-lookup"><span data-stu-id="f1b1c-135">If false the role is not available for assignment.</span></span>|
|<span data-ttu-id="f1b1c-136">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="f1b1c-136">rolePermissions</span></span> |<span data-ttu-id="f1b1c-137">[unifiedRolePermission](../resources/unifiedrolepermission.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f1b1c-137">[unifiedRolePermission](../resources/unifiedrolepermission.md) collection</span></span> |<span data-ttu-id="f1b1c-138">角色中包含的权限列表。</span><span class="sxs-lookup"><span data-stu-id="f1b1c-138">List of permissions included in the role.</span></span>|

## <a name="response"></a><span data-ttu-id="f1b1c-139">响应</span><span class="sxs-lookup"><span data-stu-id="f1b1c-139">Response</span></span>

<span data-ttu-id="f1b1c-140">如果成功，此方法在响应正文中返回响应代码和 `201 Created` 新的 [unifiedRoleDefinition](../resources/unifiedroledefinition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f1b1c-140">If successful, this method returns `201 Created` response code and a new [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f1b1c-141">示例</span><span class="sxs-lookup"><span data-stu-id="f1b1c-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="f1b1c-142">请求</span><span class="sxs-lookup"><span data-stu-id="f1b1c-142">Request</span></span>

<span data-ttu-id="f1b1c-143">下面是创建自定义角色的示例。</span><span class="sxs-lookup"><span data-stu-id="f1b1c-143">The following is an example of creating a custom role.</span></span>


# <a name="http"></a>[<span data-ttu-id="f1b1c-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="f1b1c-144">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="f1b1c-145">C#</span><span class="sxs-lookup"><span data-stu-id="f1b1c-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-unifiedroledefinition-from-rbacapplication-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f1b1c-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f1b1c-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-unifiedroledefinition-from-rbacapplication-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f1b1c-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f1b1c-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-unifiedroledefinition-from-rbacapplication-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f1b1c-148">Java</span><span class="sxs-lookup"><span data-stu-id="f1b1c-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-unifiedroledefinition-from-rbacapplication-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f1b1c-149">响应</span><span class="sxs-lookup"><span data-stu-id="f1b1c-149">Response</span></span>

<span data-ttu-id="f1b1c-150">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="f1b1c-150">The following is an example of the response.</span></span>
> <span data-ttu-id="f1b1c-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="f1b1c-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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



---
title: 添加目录角色成员
description: 创建新的目录角色成员。
author: abhijeetsinha
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 8425d978a48c2ab737577d2ed40a2d098daf275b
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2021
ms.locfileid: "52990767"
---
# <a name="add-directory-role-member"></a><span data-ttu-id="d8c97-103">添加目录角色成员</span><span class="sxs-lookup"><span data-stu-id="d8c97-103">Add directory role member</span></span>

<span data-ttu-id="d8c97-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d8c97-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d8c97-105">创建新的目录角色成员。</span><span class="sxs-lookup"><span data-stu-id="d8c97-105">Create a new directory role member.</span></span>

<span data-ttu-id="d8c97-106">你可以将 **directoryRole** 的对象 ID 和模板 ID 用于此 API。</span><span class="sxs-lookup"><span data-stu-id="d8c97-106">You can use both the object ID and template ID of the **directoryRole** with this API.</span></span> <span data-ttu-id="d8c97-107">内置角色的模板 ID 是不可可变的，可以在 Azure 门户的角色描述中查看。</span><span class="sxs-lookup"><span data-stu-id="d8c97-107">The template ID of a built-in role is immutable and can be seen in the role description on the Azure portal.</span></span> <span data-ttu-id="d8c97-108">有关详细信息，请参阅[角色模板的 ID。](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#role-template-ids)</span><span class="sxs-lookup"><span data-stu-id="d8c97-108">For details, see [Role template IDs](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#role-template-ids).</span></span>

## <a name="permissions"></a><span data-ttu-id="d8c97-109">权限</span><span class="sxs-lookup"><span data-stu-id="d8c97-109">Permissions</span></span>
<span data-ttu-id="d8c97-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d8c97-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d8c97-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="d8c97-112">Permission type</span></span>      | <span data-ttu-id="d8c97-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d8c97-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d8c97-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d8c97-114">Delegated (work or school account)</span></span> | <span data-ttu-id="d8c97-115">RoleManagement.ReadWrite.Directory、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d8c97-115">RoleManagement.ReadWrite.Directory, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d8c97-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d8c97-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d8c97-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="d8c97-117">Not supported.</span></span>    |
|<span data-ttu-id="d8c97-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="d8c97-118">Application</span></span> | <span data-ttu-id="d8c97-119">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="d8c97-119">RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="d8c97-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d8c97-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directoryRoles/{role-objectId}/members/$ref
POST /directoryRoles/roleTemplateId={role-templateId}/members/$ref
```
## <a name="request-headers"></a><span data-ttu-id="d8c97-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="d8c97-121">Request headers</span></span>
| <span data-ttu-id="d8c97-122">名称</span><span class="sxs-lookup"><span data-stu-id="d8c97-122">Name</span></span>       | <span data-ttu-id="d8c97-123">类型</span><span class="sxs-lookup"><span data-stu-id="d8c97-123">Type</span></span> | <span data-ttu-id="d8c97-124">说明</span><span class="sxs-lookup"><span data-stu-id="d8c97-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="d8c97-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="d8c97-125">Authorization</span></span>  | <span data-ttu-id="d8c97-126">string</span><span class="sxs-lookup"><span data-stu-id="d8c97-126">string</span></span>  | <span data-ttu-id="d8c97-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d8c97-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d8c97-129">Content-type</span><span class="sxs-lookup"><span data-stu-id="d8c97-129">Content-type</span></span> | <span data-ttu-id="d8c97-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="d8c97-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d8c97-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="d8c97-132">Request body</span></span>
<span data-ttu-id="d8c97-133">在请求正文中，提供 [directoryObject](../resources/directoryobject.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d8c97-133">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="d8c97-134">响应</span><span class="sxs-lookup"><span data-stu-id="d8c97-134">Response</span></span>

<span data-ttu-id="d8c97-135">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d8c97-135">If successful, this method returns a `201 Created` response code and a [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d8c97-136">示例</span><span class="sxs-lookup"><span data-stu-id="d8c97-136">Examples</span></span>

### <a name="example-1-assign-a-built-in-role-to-a-user"></a><span data-ttu-id="d8c97-137">示例 1：向用户分配内置角色</span><span class="sxs-lookup"><span data-stu-id="d8c97-137">Example 1: Assign a built-in role to a user</span></span>
#### <a name="request"></a><span data-ttu-id="d8c97-138">请求</span><span class="sxs-lookup"><span data-stu-id="d8c97-138">Request</span></span>
<span data-ttu-id="d8c97-139">以下示例将内置角色分配给用户。</span><span class="sxs-lookup"><span data-stu-id="d8c97-139">The following example assigns a built-in role to a user.</span></span>

# <a name="http"></a>[<span data-ttu-id="d8c97-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="d8c97-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_directoryrole_1"
}-->
```http
POST https://graph.microsoft.com/beta/directoryRoles/0afed502-2456-4fd4-988e-3c21924c28a7/members/$ref
Content-type: application/json
Content-length: 30

{
    "@odata.id":"https://graph.microsoft.com/beta/users/0f933635-5b77-4cf4-a577-f78a5eb090a2"
}
```
# <a name="javascript"></a>[<span data-ttu-id="d8c97-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d8c97-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-directoryrole-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="d8c97-142">C#</span><span class="sxs-lookup"><span data-stu-id="d8c97-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryobject-from-directoryrole-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d8c97-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d8c97-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryobject-from-directoryrole-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d8c97-144">Java</span><span class="sxs-lookup"><span data-stu-id="d8c97-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-directoryobject-from-directoryrole-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="d8c97-145">响应</span><span class="sxs-lookup"><span data-stu-id="d8c97-145">Response</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No content
```

### <a name="example-2-assign-a-built-in-role-to-a-group"></a><span data-ttu-id="d8c97-146">示例 2：向组分配内置角色</span><span class="sxs-lookup"><span data-stu-id="d8c97-146">Example 2: Assign a built-in role to a group</span></span>
#### <a name="request"></a><span data-ttu-id="d8c97-147">请求</span><span class="sxs-lookup"><span data-stu-id="d8c97-147">Request</span></span>
<span data-ttu-id="d8c97-148">可以在请求正文中使用特定资源集（如用户或组）或使用泛型 **directoryObjects**。</span><span class="sxs-lookup"><span data-stu-id="d8c97-148">You can use a specific resource set like users or groups in the request body, or you can use generic **directoryObjects**.</span></span> <span data-ttu-id="d8c97-149">此示例演示如何使用 **directoryObjects**。</span><span class="sxs-lookup"><span data-stu-id="d8c97-149">This example shows how you can use **directoryObjects**.</span></span>


# <a name="http"></a>[<span data-ttu-id="d8c97-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="d8c97-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_directoryrole_2"
}-->
```http
POST https://graph.microsoft.com/beta/directoryRoles/0afed502-2456-4fd4-988e-3c21924c28a7/members/$ref
Content-type: application/json
Content-length: 30

{
    "@odata.id":"https://graph.microsoft.com/beta/directoryObjects/2c891f12-928d-4da2-8d83-7d2434a0d8dc"
}
```
# <a name="c"></a>[<span data-ttu-id="d8c97-151">C#</span><span class="sxs-lookup"><span data-stu-id="d8c97-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryobject-from-directoryrole-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d8c97-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d8c97-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-directoryrole-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d8c97-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d8c97-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryobject-from-directoryrole-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d8c97-154">Java</span><span class="sxs-lookup"><span data-stu-id="d8c97-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-directoryobject-from-directoryrole-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="d8c97-155">响应</span><span class="sxs-lookup"><span data-stu-id="d8c97-155">Response</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No content
```

### <a name="example-3-add-a-new-member-to-a-directory-role-using-role-templateid"></a><span data-ttu-id="d8c97-156">示例 3：使用角色 templateId 向目录角色添加新成员</span><span class="sxs-lookup"><span data-stu-id="d8c97-156">Example 3: Add a new member to a directory role using role templateId</span></span>
#### <a name="request"></a><span data-ttu-id="d8c97-157">请求</span><span class="sxs-lookup"><span data-stu-id="d8c97-157">Request</span></span>
<span data-ttu-id="d8c97-158">在此请求中，将 替换为要分配给用户或目录对象的目录角色的 `88d8e3e3-8f55-4a1e-953a-9b9898b8876b` **roleTemplateId** 的值。</span><span class="sxs-lookup"><span data-stu-id="d8c97-158">In this request, replace `88d8e3e3-8f55-4a1e-953a-9b9898b8876b` with the value of the **roleTemplateId** for the directory role you wish to assign to the user or directory object.</span></span> <span data-ttu-id="d8c97-159">将 `bb165b45-151c-4cf6-9911-cd7188912848` 替换为 **用户** 或目录对象的 id 值。</span><span class="sxs-lookup"><span data-stu-id="d8c97-159">Replace `bb165b45-151c-4cf6-9911-cd7188912848` with the **id** value of your user or directory object.</span></span> 


# <a name="http"></a>[<span data-ttu-id="d8c97-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="d8c97-160">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_directoryrole_2_templateId"
}-->
```http
POST https://graph.microsoft.com/beta/directoryRoles/roleTemplateId=88d8e3e3-8f55-4a1e-953a-9b9898b8876b/members/$ref
Content-type: application/json
Content-length: 30

{
    "@odata.id": "https://graph.microsoft.com/beta/directoryObjects/bb165b45-151c-4cf6-9911-cd7188912848"
}
```
# <a name="c"></a>[<span data-ttu-id="d8c97-161">C#</span><span class="sxs-lookup"><span data-stu-id="d8c97-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryobject-from-directoryrole-2-templateid-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d8c97-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d8c97-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-directoryrole-2-templateid-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d8c97-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d8c97-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryobject-from-directoryrole-2-templateid-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d8c97-164">Java</span><span class="sxs-lookup"><span data-stu-id="d8c97-164">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-directoryobject-from-directoryrole-2-templateid-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="d8c97-165">响应</span><span class="sxs-lookup"><span data-stu-id="d8c97-165">Response</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No content
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create member",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->



---
title: 删除目录角色成员
description: 从 directoryRole 中删除成员。
author: abhijeetsinha
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: e03fb736cdd1dce8ca89335d87e9bd6bc65ddc4b
ms.sourcegitcommit: d0d2d17a31cbcb01b1ae18bd6a18c39d7077069a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/24/2021
ms.locfileid: "53118663"
---
# <a name="remove-directory-role-member"></a><span data-ttu-id="31788-103">删除目录角色成员</span><span class="sxs-lookup"><span data-stu-id="31788-103">Remove directory role member</span></span>

<span data-ttu-id="31788-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="31788-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="31788-105">从 [directoryRole 中删除成员](../resources/directoryrole.md)。</span><span class="sxs-lookup"><span data-stu-id="31788-105">Remove a member from a [directoryRole](../resources/directoryrole.md).</span></span>

<span data-ttu-id="31788-106">你可以将 **directoryRole** 的对象 ID 和模板 ID 用于此 API。</span><span class="sxs-lookup"><span data-stu-id="31788-106">You can use both the object ID and template ID of the **directoryRole** with this API.</span></span> <span data-ttu-id="31788-107">内置角色的模板 ID 是不可可变的，可以在 Azure 门户的角色描述中查看。</span><span class="sxs-lookup"><span data-stu-id="31788-107">The template ID of a built-in role is immutable and can be seen in the role description on the Azure portal.</span></span> <span data-ttu-id="31788-108">有关详细信息，请参阅[角色模板的 ID。](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#role-template-ids)</span><span class="sxs-lookup"><span data-stu-id="31788-108">For details, see [Role template IDs](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#role-template-ids).</span></span>

## <a name="permissions"></a><span data-ttu-id="31788-109">权限</span><span class="sxs-lookup"><span data-stu-id="31788-109">Permissions</span></span>

<span data-ttu-id="31788-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="31788-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="31788-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="31788-112">Permission type</span></span>      | <span data-ttu-id="31788-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="31788-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="31788-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="31788-114">Delegated (work or school account)</span></span> | <span data-ttu-id="31788-115">RoleManagement.ReadWrite.Directory、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="31788-115">RoleManagement.ReadWrite.Directory, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="31788-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="31788-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="31788-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="31788-117">Not supported.</span></span>    |
|<span data-ttu-id="31788-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="31788-118">Application</span></span> | <span data-ttu-id="31788-119">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="31788-119">RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="31788-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="31788-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /directoryRoles/{role-id}/members/{id}/$ref
DELETE /directoryRoles/roleTemplateId={roleTemplateId}/members/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="31788-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="31788-121">Request headers</span></span>

| <span data-ttu-id="31788-122">名称</span><span class="sxs-lookup"><span data-stu-id="31788-122">Name</span></span>       | <span data-ttu-id="31788-123">类型</span><span class="sxs-lookup"><span data-stu-id="31788-123">Type</span></span> | <span data-ttu-id="31788-124">说明</span><span class="sxs-lookup"><span data-stu-id="31788-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="31788-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="31788-125">Authorization</span></span>  | <span data-ttu-id="31788-126">string</span><span class="sxs-lookup"><span data-stu-id="31788-126">string</span></span>  | <span data-ttu-id="31788-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="31788-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="31788-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="31788-129">Request body</span></span>

<span data-ttu-id="31788-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="31788-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="31788-131">响应</span><span class="sxs-lookup"><span data-stu-id="31788-131">Response</span></span>

<span data-ttu-id="31788-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="31788-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="31788-134">示例</span><span class="sxs-lookup"><span data-stu-id="31788-134">Examples</span></span>

### <a name="example-1-remove-directory-role-member-using-role-id"></a><span data-ttu-id="31788-135">示例 1：使用角色 ID 删除目录角色成员</span><span class="sxs-lookup"><span data-stu-id="31788-135">Example 1: Remove directory role member using role id</span></span>

#### <a name="request"></a><span data-ttu-id="31788-136">请求</span><span class="sxs-lookup"><span data-stu-id="31788-136">Request</span></span>

<span data-ttu-id="31788-137">本示例中，将 替换为目录角色的 id 值和希望从目录角色中取消分配的用户或目录对象的 `f8e85ed8-f66f-4058-b170-3efae8b9c6e5`  `bb165b45-151c-4cf6-9911-cd7188912848` **id** 值。</span><span class="sxs-lookup"><span data-stu-id="31788-137">In this example, replace `f8e85ed8-f66f-4058-b170-3efae8b9c6e5` with the **id** value of the directory role and `bb165b45-151c-4cf6-9911-cd7188912848` with the **id** value of the user or directory object that you wish to unassign from the directory role.</span></span>

# <a name="http"></a>[<span data-ttu-id="31788-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="31788-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_directoryobject_from_directoryrole_objectId"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/directoryRoles/f8e85ed8-f66f-4058-b170-3efae8b9c6e5/members/bb165b45-151c-4cf6-9911-cd7188912848/$ref
```
# <a name="c"></a>[<span data-ttu-id="31788-139">C#</span><span class="sxs-lookup"><span data-stu-id="31788-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-directoryobject-from-directoryrole-objectid-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="31788-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="31788-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-directoryobject-from-directoryrole-objectid-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="31788-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="31788-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-directoryobject-from-directoryrole-objectid-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="31788-142">Java</span><span class="sxs-lookup"><span data-stu-id="31788-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-directoryobject-from-directoryrole-objectid-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="31788-143">响应</span><span class="sxs-lookup"><span data-stu-id="31788-143">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-remove-directory-role-member-using-roletemplateid"></a><span data-ttu-id="31788-144">示例 2：使用 roleTemplateId 删除目录角色成员</span><span class="sxs-lookup"><span data-stu-id="31788-144">Example 2: Remove directory role member using roleTemplateId</span></span>

#### <a name="request"></a><span data-ttu-id="31788-145">请求</span><span class="sxs-lookup"><span data-stu-id="31788-145">Request</span></span>

<span data-ttu-id="31788-146">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="31788-146">The following is an example of the request.</span></span> <span data-ttu-id="31788-147">将 `9f06204d-73c1-4d4c-880a-6edb90606fd8` 替换为 roleTemplateId 的值和 `bb165b45-151c-4cf6-9911-cd7188912848` directory 对象的用户的 **id** 值。</span><span class="sxs-lookup"><span data-stu-id="31788-147">Replace `9f06204d-73c1-4d4c-880a-6edb90606fd8` with the value of your roleTemplateId and `bb165b45-151c-4cf6-9911-cd7188912848` with the **id** value of your user of directory object.</span></span>

# <a name="http"></a>[<span data-ttu-id="31788-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="31788-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_directoryobject_from_directoryrole_templateId"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/directoryRoles/roleTemplateId=9f06204d-73c1-4d4c-880a-6edb90606fd8/members/bb165b45-151c-4cf6-9911-cd7188912848/$ref
```
# <a name="c"></a>[<span data-ttu-id="31788-149">C#</span><span class="sxs-lookup"><span data-stu-id="31788-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-directoryobject-from-directoryrole-templateid-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="31788-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="31788-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-directoryobject-from-directoryrole-templateid-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="31788-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="31788-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-directoryobject-from-directoryrole-templateid-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="31788-152">Java</span><span class="sxs-lookup"><span data-stu-id="31788-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-directoryobject-from-directoryrole-templateid-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="31788-153">响应</span><span class="sxs-lookup"><span data-stu-id="31788-153">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete a member",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->


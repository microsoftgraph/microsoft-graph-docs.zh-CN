---
title: 删除目录角色成员
description: 从 directoryRole 中删除成员。
author: abhijeetsinha
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: aec2f698c947a74f2814c4e91f350b612fa0600c
ms.sourcegitcommit: d0d2d17a31cbcb01b1ae18bd6a18c39d7077069a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/24/2021
ms.locfileid: "53118582"
---
# <a name="remove-directory-role-member"></a><span data-ttu-id="6ae46-103">删除目录角色成员</span><span class="sxs-lookup"><span data-stu-id="6ae46-103">Remove directory role member</span></span>

<span data-ttu-id="6ae46-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6ae46-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6ae46-105">从 directoryRole 中删除成员。</span><span class="sxs-lookup"><span data-stu-id="6ae46-105">Remove a member from a directoryRole.</span></span>

<span data-ttu-id="6ae46-106">你可以将 **directoryRole** 的对象 ID 和模板 ID 用于此 API。</span><span class="sxs-lookup"><span data-stu-id="6ae46-106">You can use both the object ID and template ID of the **directoryRole** with this API.</span></span> <span data-ttu-id="6ae46-107">内置角色的模板 ID 是不可可变的，可以在 Azure 门户的角色描述中查看。</span><span class="sxs-lookup"><span data-stu-id="6ae46-107">The template ID of a built-in role is immutable and can be seen in the role description on the Azure portal.</span></span> <span data-ttu-id="6ae46-108">有关详细信息，请参阅[角色模板的 ID。](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#role-template-ids)</span><span class="sxs-lookup"><span data-stu-id="6ae46-108">For details, see [Role template IDs](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#role-template-ids).</span></span>

## <a name="permissions"></a><span data-ttu-id="6ae46-109">权限</span><span class="sxs-lookup"><span data-stu-id="6ae46-109">Permissions</span></span>

<span data-ttu-id="6ae46-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6ae46-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="6ae46-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="6ae46-112">Permission type</span></span>      | <span data-ttu-id="6ae46-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6ae46-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6ae46-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6ae46-114">Delegated (work or school account)</span></span> | <span data-ttu-id="6ae46-115">RoleManagement.ReadWrite.Directory、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6ae46-115">RoleManagement.ReadWrite.Directory, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6ae46-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6ae46-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6ae46-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="6ae46-117">Not supported.</span></span>    |
|<span data-ttu-id="6ae46-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="6ae46-118">Application</span></span> | <span data-ttu-id="6ae46-119">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="6ae46-119">RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="6ae46-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6ae46-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /directoryRoles/{role-id}/members/{id}/$ref
DELETE /directoryRoles/roleTemplateId={roleTemplateId}/members/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="6ae46-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="6ae46-121">Request headers</span></span>

| <span data-ttu-id="6ae46-122">名称</span><span class="sxs-lookup"><span data-stu-id="6ae46-122">Name</span></span>       | <span data-ttu-id="6ae46-123">类型</span><span class="sxs-lookup"><span data-stu-id="6ae46-123">Type</span></span> | <span data-ttu-id="6ae46-124">说明</span><span class="sxs-lookup"><span data-stu-id="6ae46-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="6ae46-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="6ae46-125">Authorization</span></span>  | <span data-ttu-id="6ae46-126">string</span><span class="sxs-lookup"><span data-stu-id="6ae46-126">string</span></span>  | <span data-ttu-id="6ae46-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6ae46-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6ae46-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="6ae46-129">Request body</span></span>

<span data-ttu-id="6ae46-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6ae46-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6ae46-131">响应</span><span class="sxs-lookup"><span data-stu-id="6ae46-131">Response</span></span>

<span data-ttu-id="6ae46-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="6ae46-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6ae46-134">示例</span><span class="sxs-lookup"><span data-stu-id="6ae46-134">Examples</span></span>

### <a name="example-1-remove-directory-role-member-using-role-objectid"></a><span data-ttu-id="6ae46-135">示例 1：使用 role objectId 删除目录角色成员</span><span class="sxs-lookup"><span data-stu-id="6ae46-135">Example 1: Remove directory role member using role objectId</span></span>

#### <a name="request"></a><span data-ttu-id="6ae46-136">请求</span><span class="sxs-lookup"><span data-stu-id="6ae46-136">Request</span></span>

<span data-ttu-id="6ae46-137">本示例中，将 替换为目录角色的 id 值和希望从目录角色中取消分配的用户或目录对象的 `f8e85ed8-f66f-4058-b170-3efae8b9c6e5`  `bb165b45-151c-4cf6-9911-cd7188912848` **id** 值。</span><span class="sxs-lookup"><span data-stu-id="6ae46-137">In this example, replace `f8e85ed8-f66f-4058-b170-3efae8b9c6e5` with the **id** value of the directory role and `bb165b45-151c-4cf6-9911-cd7188912848` with the **id** value of the user or directory object that you wish to unassign from the directory role.</span></span>

# <a name="http"></a>[<span data-ttu-id="6ae46-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="6ae46-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_directoryobject_from_directoryrole"
}-->

```http
DELETE https://graph.microsoft.com/beta/directoryRoles/f8e85ed8-f66f-4058-b170-3efae8b9c6e5/members/bb165b45-151c-4cf6-9911-cd7188912848/$ref
```
# <a name="c"></a>[<span data-ttu-id="6ae46-139">C#</span><span class="sxs-lookup"><span data-stu-id="6ae46-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-directoryobject-from-directoryrole-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6ae46-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6ae46-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-directoryobject-from-directoryrole-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6ae46-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6ae46-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-directoryobject-from-directoryrole-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6ae46-142">Java</span><span class="sxs-lookup"><span data-stu-id="6ae46-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-directoryobject-from-directoryrole-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="6ae46-143">响应</span><span class="sxs-lookup"><span data-stu-id="6ae46-143">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-remove-directory-role-member-using-roletemplateid"></a><span data-ttu-id="6ae46-144">示例 2：使用 roleTemplateId 删除目录角色成员</span><span class="sxs-lookup"><span data-stu-id="6ae46-144">Example 2: Remove directory role member using roleTemplateId</span></span>

#### <a name="request"></a><span data-ttu-id="6ae46-145">请求</span><span class="sxs-lookup"><span data-stu-id="6ae46-145">Request</span></span>

<span data-ttu-id="6ae46-146">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="6ae46-146">The following is an example of the request.</span></span> <span data-ttu-id="6ae46-147">将 `9f06204d-73c1-4d4c-880a-6edb90606fd8` 替换为 roleTemplateId 的值和 `bb165b45-151c-4cf6-9911-cd7188912848` directory 对象的用户的 **id** 值。</span><span class="sxs-lookup"><span data-stu-id="6ae46-147">Replace `9f06204d-73c1-4d4c-880a-6edb90606fd8` with the value of your roleTemplateId and `bb165b45-151c-4cf6-9911-cd7188912848` with the **id** value of your user of directory object.</span></span>


# <a name="http"></a>[<span data-ttu-id="6ae46-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="6ae46-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_directoryobject_from_directoryrole_templateId"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/directoryRoles/roleTemplateId=9f06204d-73c1-4d4c-880a-6edb90606fd8/members/bb165b45-151c-4cf6-9911-cd7188912848/$ref
```
# <a name="c"></a>[<span data-ttu-id="6ae46-149">C#</span><span class="sxs-lookup"><span data-stu-id="6ae46-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-directoryobject-from-directoryrole-templateid-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6ae46-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6ae46-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-directoryobject-from-directoryrole-templateid-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6ae46-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6ae46-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-directoryobject-from-directoryrole-templateid-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6ae46-152">Java</span><span class="sxs-lookup"><span data-stu-id="6ae46-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-directoryobject-from-directoryrole-templateid-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="6ae46-153">响应</span><span class="sxs-lookup"><span data-stu-id="6ae46-153">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete a member",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->



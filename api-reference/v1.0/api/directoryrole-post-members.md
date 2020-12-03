---
title: 添加目录角色成员
description: 使用此 API 创建新的目录角色成员。
author: abhijeetsinha
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 9478f08f404967f8a95acf57eb6905ecbb2932fd
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/01/2020
ms.locfileid: "49522658"
---
# <a name="add-directory-role-member"></a><span data-ttu-id="25182-103">添加目录角色成员</span><span class="sxs-lookup"><span data-stu-id="25182-103">Add directory role member</span></span>

<span data-ttu-id="25182-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="25182-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="25182-105">使用此 API 创建新的目录角色成员。</span><span class="sxs-lookup"><span data-stu-id="25182-105">Use this API to create a new directory role member.</span></span>

> [!Note]
> <span data-ttu-id="25182-106">您可以将 **directoryRole** 的对象 id 和模板 ID 与此 API 一起使用。</span><span class="sxs-lookup"><span data-stu-id="25182-106">You can use both the object ID and template ID of the **directoryRole** with this API.</span></span> <span data-ttu-id="25182-107">内置角色的模板 ID 是不可变的，可在 Azure 门户上的角色说明中查看。</span><span class="sxs-lookup"><span data-stu-id="25182-107">The template ID of a built-in role is immutable and can be seen in the role description on the Azure portal.</span></span> <span data-ttu-id="25182-108">有关详细信息，请参阅 [角色模板 id](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#role-template-ids)。</span><span class="sxs-lookup"><span data-stu-id="25182-108">For details, see [Role template IDs](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#role-template-ids).</span></span>

## <a name="permissions"></a><span data-ttu-id="25182-109">权限</span><span class="sxs-lookup"><span data-stu-id="25182-109">Permissions</span></span>
<span data-ttu-id="25182-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="25182-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="25182-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="25182-112">Permission type</span></span>      | <span data-ttu-id="25182-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="25182-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="25182-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="25182-114">Delegated (work or school account)</span></span> | <span data-ttu-id="25182-115">RoleManagement、Directory.accessasuser.all 和所有子目录。</span><span class="sxs-lookup"><span data-stu-id="25182-115">RoleManagement.ReadWrite.Directory, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="25182-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="25182-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="25182-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="25182-117">Not supported.</span></span>    |
|<span data-ttu-id="25182-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="25182-118">Application</span></span> | <span data-ttu-id="25182-119">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="25182-119">RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="25182-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="25182-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directoryRoles/{id}/members/$ref
```
## <a name="request-headers"></a><span data-ttu-id="25182-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="25182-121">Request headers</span></span>
| <span data-ttu-id="25182-122">名称</span><span class="sxs-lookup"><span data-stu-id="25182-122">Name</span></span>       | <span data-ttu-id="25182-123">类型</span><span class="sxs-lookup"><span data-stu-id="25182-123">Type</span></span> | <span data-ttu-id="25182-124">说明</span><span class="sxs-lookup"><span data-stu-id="25182-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="25182-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="25182-125">Authorization</span></span>  | <span data-ttu-id="25182-126">string</span><span class="sxs-lookup"><span data-stu-id="25182-126">string</span></span>  | <span data-ttu-id="25182-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="25182-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="25182-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="25182-129">Content-Type</span></span>  | <span data-ttu-id="25182-130">string</span><span class="sxs-lookup"><span data-stu-id="25182-130">string</span></span>  | <span data-ttu-id="25182-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="25182-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="25182-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="25182-133">Request body</span></span>
<span data-ttu-id="25182-134">在请求正文中，提供要添加的 [directoryObject](../resources/directoryobject.md) 或 [user](../resources/user.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="25182-134">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md) or [user](../resources/user.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="25182-135">响应</span><span class="sxs-lookup"><span data-stu-id="25182-135">Response</span></span>

<span data-ttu-id="25182-136">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="25182-136">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="25182-137">示例</span><span class="sxs-lookup"><span data-stu-id="25182-137">Examples</span></span>

### <a name="example-1-add-a-new-member-to-a-directory-role-using-role-objectid"></a><span data-ttu-id="25182-138">示例1：使用角色 objectId 将新成员添加到目录角色</span><span class="sxs-lookup"><span data-stu-id="25182-138">Example 1: Add a new member to a directory role using role objectId</span></span>

##### <a name="request"></a><span data-ttu-id="25182-139">请求</span><span class="sxs-lookup"><span data-stu-id="25182-139">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="25182-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="25182-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_directoryrole_objectId"
}-->
```http
POST https://graph.microsoft.com/v1.0/directoryRoles/{role-objectId}/members/$ref
Content-type: application/json

{
  "@odata.id": "https://graph.microsoft.com/v1.0/directoryObjects/{user-id}"
}
```
# <a name="javascript"></a>[<span data-ttu-id="25182-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="25182-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-directoryrole-objectid-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="25182-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="25182-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryobject-from-directoryrole-objectid-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="25182-143">C#</span><span class="sxs-lookup"><span data-stu-id="25182-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryobject-from-directoryrole-objectid-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="25182-144">Java</span><span class="sxs-lookup"><span data-stu-id="25182-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-directoryobject-from-directoryrole-objectid-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="25182-145">响应</span><span class="sxs-lookup"><span data-stu-id="25182-145">Response</span></span>
><span data-ttu-id="25182-146">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="25182-146">**Note:** The response object shown here might be shortened for readability.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No Content
Content-type: text/plain

```

### <a name="example-2-add-a-new-member-to-a-directory-role-using-role-templateid"></a><span data-ttu-id="25182-147">示例2：使用角色 templateId 将新成员添加到目录角色</span><span class="sxs-lookup"><span data-stu-id="25182-147">Example 2: Add a new member to a directory role using role templateId</span></span>

##### <a name="request"></a><span data-ttu-id="25182-148">请求</span><span class="sxs-lookup"><span data-stu-id="25182-148">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="25182-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="25182-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_directoryrole_templateId"
}-->
```http
POST https://graph.microsoft.com/v1.0/directoryRoles/roleTemplateId={role-templateId}/members/$ref
Content-type: application/json

{
  "@odata.id": "https://graph.microsoft.com/v1.0/directoryObjects/{user-id}"
}
```
# <a name="javascript"></a>[<span data-ttu-id="25182-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="25182-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-directoryrole-templateid-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="25182-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="25182-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryobject-from-directoryrole-templateid-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="25182-152">C#</span><span class="sxs-lookup"><span data-stu-id="25182-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryobject-from-directoryrole-templateid-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="25182-153">Java</span><span class="sxs-lookup"><span data-stu-id="25182-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-directoryobject-from-directoryrole-templateid-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="25182-154">响应</span><span class="sxs-lookup"><span data-stu-id="25182-154">Response</span></span>
><span data-ttu-id="25182-155">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="25182-155">**Note:** The response object shown here might be shortened for readability.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create member",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->


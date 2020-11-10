---
title: 添加目录角色成员
description: 创建新的目录角色成员。
author: abhijeetsinha
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: dd7554c41816e54240e081fd1265861f24fa7d56
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48956294"
---
# <a name="add-directory-role-member"></a><span data-ttu-id="2743f-103">添加目录角色成员</span><span class="sxs-lookup"><span data-stu-id="2743f-103">Add directory role member</span></span>

<span data-ttu-id="2743f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2743f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2743f-105">创建新的目录角色成员。</span><span class="sxs-lookup"><span data-stu-id="2743f-105">Create a new directory role member.</span></span>
## <a name="permissions"></a><span data-ttu-id="2743f-106">权限</span><span class="sxs-lookup"><span data-stu-id="2743f-106">Permissions</span></span>
<span data-ttu-id="2743f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2743f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2743f-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="2743f-109">Permission type</span></span>      | <span data-ttu-id="2743f-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2743f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2743f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2743f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="2743f-112">RoleManagement、Directory.accessasuser.all 和所有子目录。</span><span class="sxs-lookup"><span data-stu-id="2743f-112">RoleManagement.ReadWrite.Directory, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="2743f-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2743f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2743f-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="2743f-114">Not supported.</span></span>    |
|<span data-ttu-id="2743f-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="2743f-115">Application</span></span> | <span data-ttu-id="2743f-116">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="2743f-116">RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="2743f-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2743f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directoryRoles/{id}/members/$ref
```
## <a name="request-headers"></a><span data-ttu-id="2743f-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="2743f-118">Request headers</span></span>
| <span data-ttu-id="2743f-119">名称</span><span class="sxs-lookup"><span data-stu-id="2743f-119">Name</span></span>       | <span data-ttu-id="2743f-120">类型</span><span class="sxs-lookup"><span data-stu-id="2743f-120">Type</span></span> | <span data-ttu-id="2743f-121">说明</span><span class="sxs-lookup"><span data-stu-id="2743f-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="2743f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2743f-122">Authorization</span></span>  | <span data-ttu-id="2743f-123">string</span><span class="sxs-lookup"><span data-stu-id="2743f-123">string</span></span>  | <span data-ttu-id="2743f-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2743f-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2743f-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="2743f-126">Content-type</span></span> | <span data-ttu-id="2743f-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="2743f-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2743f-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="2743f-129">Request body</span></span>
<span data-ttu-id="2743f-130">在请求正文中，提供 [directoryObject](../resources/directoryobject.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2743f-130">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="2743f-131">响应</span><span class="sxs-lookup"><span data-stu-id="2743f-131">Response</span></span>

<span data-ttu-id="2743f-132">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2743f-132">If successful, this method returns a `201 Created` response code and a [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2743f-133">示例</span><span class="sxs-lookup"><span data-stu-id="2743f-133">Examples</span></span>

### <a name="example-1-assign-a-built-in-role-to-a-user"></a><span data-ttu-id="2743f-134">示例1：向用户分配内置角色</span><span class="sxs-lookup"><span data-stu-id="2743f-134">Example 1: Assign a built-in role to a user</span></span>
#### <a name="request"></a><span data-ttu-id="2743f-135">请求</span><span class="sxs-lookup"><span data-stu-id="2743f-135">Request</span></span>
<span data-ttu-id="2743f-136">下面的示例将一个内置角色分配给用户。</span><span class="sxs-lookup"><span data-stu-id="2743f-136">The following example assigns a built-in role to a user.</span></span>

# <a name="http"></a>[<span data-ttu-id="2743f-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="2743f-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_directoryrole"
}-->
```http
POST https://graph.microsoft.com/beta/directoryRoles/0afed502-2456-4fd4-988e-3c21924c28a7/members/$ref
Content-type: application/json
Content-length: 30

{
    "@odata.id":"https://graph.microsoft.com/beta/users/0f933635-5b77-4cf4-a577-f78a5eb090a2"
}
```
# <a name="javascript"></a>[<span data-ttu-id="2743f-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2743f-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-directoryrole-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="2743f-139">C#</span><span class="sxs-lookup"><span data-stu-id="2743f-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryobject-from-directoryrole-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2743f-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2743f-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryobject-from-directoryrole-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2743f-141">Java</span><span class="sxs-lookup"><span data-stu-id="2743f-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-directoryobject-from-directoryrole-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="2743f-142">响应</span><span class="sxs-lookup"><span data-stu-id="2743f-142">Response</span></span>
<span data-ttu-id="2743f-143">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="2743f-143">The following example shows the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No content
```

### <a name="example-2-assign-a-built-in-role-to-a-group"></a><span data-ttu-id="2743f-144">示例2：向组分配内置角色</span><span class="sxs-lookup"><span data-stu-id="2743f-144">Example 2: Assign a built-in role to a group</span></span>
#### <a name="request"></a><span data-ttu-id="2743f-145">请求</span><span class="sxs-lookup"><span data-stu-id="2743f-145">Request</span></span>
<span data-ttu-id="2743f-146">您可以使用请求正文中的用户或组等特定资源集，也可以使用泛型 **directoryObjects** 。</span><span class="sxs-lookup"><span data-stu-id="2743f-146">You can use a specific resource set like users or groups in the request body, or you can use generic **directoryObjects**.</span></span> <span data-ttu-id="2743f-147">本示例演示如何使用 **directoryObjects** 。</span><span class="sxs-lookup"><span data-stu-id="2743f-147">This example shows how you can use **directoryObjects**.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_directoryrole"
}-->
```http
POST https://graph.microsoft.com/beta/directoryRoles/0afed502-2456-4fd4-988e-3c21924c28a7/members/$ref
Content-type: application/json
Content-length: 30

{
    "@odata.id":"https://graph.microsoft.com/beta/directoryObjects/2c891f12-928d-4da2-8d83-7d2434a0d8dc"
}
```

#### <a name="response"></a><span data-ttu-id="2743f-148">响应</span><span class="sxs-lookup"><span data-stu-id="2743f-148">Response</span></span>
<span data-ttu-id="2743f-149">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="2743f-149">The following example shows the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
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



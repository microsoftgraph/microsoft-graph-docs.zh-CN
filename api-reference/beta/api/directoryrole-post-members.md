---
title: 添加目录角色成员
description: 创建新的目录角色成员。
author: abhijeetsinha
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 0a62013b0a424e83eb2ad30bb554a6aba33b6d63
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/20/2020
ms.locfileid: "46819362"
---
# <a name="add-directory-role-member"></a><span data-ttu-id="2c592-103">添加目录角色成员</span><span class="sxs-lookup"><span data-stu-id="2c592-103">Add directory role member</span></span>

<span data-ttu-id="2c592-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2c592-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2c592-105">创建新的目录角色成员。</span><span class="sxs-lookup"><span data-stu-id="2c592-105">Create a new directory role member.</span></span>
## <a name="permissions"></a><span data-ttu-id="2c592-106">权限</span><span class="sxs-lookup"><span data-stu-id="2c592-106">Permissions</span></span>
<span data-ttu-id="2c592-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2c592-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2c592-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="2c592-109">Permission type</span></span>      | <span data-ttu-id="2c592-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2c592-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2c592-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2c592-111">Delegated (work or school account)</span></span> | <span data-ttu-id="2c592-112">RoleManagement.ReadWrite.Directory、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2c592-112">RoleManagement.ReadWrite.Directory, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="2c592-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2c592-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2c592-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="2c592-114">Not supported.</span></span>    |
|<span data-ttu-id="2c592-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="2c592-115">Application</span></span> | <span data-ttu-id="2c592-116">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="2c592-116">RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="2c592-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2c592-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directoryRoles/{id}/members/$ref

```
## <a name="request-headers"></a><span data-ttu-id="2c592-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="2c592-118">Request headers</span></span>
| <span data-ttu-id="2c592-119">名称</span><span class="sxs-lookup"><span data-stu-id="2c592-119">Name</span></span>       | <span data-ttu-id="2c592-120">类型</span><span class="sxs-lookup"><span data-stu-id="2c592-120">Type</span></span> | <span data-ttu-id="2c592-121">说明</span><span class="sxs-lookup"><span data-stu-id="2c592-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="2c592-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2c592-122">Authorization</span></span>  | <span data-ttu-id="2c592-123">string</span><span class="sxs-lookup"><span data-stu-id="2c592-123">string</span></span>  | <span data-ttu-id="2c592-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2c592-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2c592-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="2c592-126">Content-type</span></span> | <span data-ttu-id="2c592-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="2c592-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2c592-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="2c592-129">Request body</span></span>
<span data-ttu-id="2c592-130">在请求正文中，提供 [directoryObject](../resources/directoryobject.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2c592-130">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="2c592-131">响应</span><span class="sxs-lookup"><span data-stu-id="2c592-131">Response</span></span>

<span data-ttu-id="2c592-132">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2c592-132">If successful, this method returns a `201 Created` response code and a [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2c592-133">示例</span><span class="sxs-lookup"><span data-stu-id="2c592-133">Examples</span></span>

### <a name="example-1-assign-a-built-in-role-to-a-user"></a><span data-ttu-id="2c592-134">示例 1：向用户分配内置角色</span><span class="sxs-lookup"><span data-stu-id="2c592-134">Example 1: Assign a built-in role to a user</span></span>
#### <a name="request"></a><span data-ttu-id="2c592-135">请求</span><span class="sxs-lookup"><span data-stu-id="2c592-135">Request</span></span>
<span data-ttu-id="2c592-136">以下示例向用户分配内置角色。</span><span class="sxs-lookup"><span data-stu-id="2c592-136">The following example assigns a built-in role to a user.</span></span>

# <a name="http"></a>[<span data-ttu-id="2c592-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="2c592-137">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="2c592-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2c592-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-directoryrole-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="2c592-139">C#</span><span class="sxs-lookup"><span data-stu-id="2c592-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryobject-from-directoryrole-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="2c592-140">响应</span><span class="sxs-lookup"><span data-stu-id="2c592-140">Response</span></span>
<span data-ttu-id="2c592-141">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="2c592-141">The following example shows the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No content
```

### <a name="example-2-assign-a-built-in-role-to-a-group"></a><span data-ttu-id="2c592-142">示例 2：对组分配内置角色</span><span class="sxs-lookup"><span data-stu-id="2c592-142">Example 2: Assign a built-in role to a group</span></span>
#### <a name="request"></a><span data-ttu-id="2c592-143">请求</span><span class="sxs-lookup"><span data-stu-id="2c592-143">Request</span></span>
<span data-ttu-id="2c592-144">你可以使用特定资源集（如请求正文中的用户或组）或者可以使用泛型**directoryObjects。**</span><span class="sxs-lookup"><span data-stu-id="2c592-144">You can use a specific resource set like users or groups in the request body, or you can use generic **directoryObjects**.</span></span> <span data-ttu-id="2c592-145">此示例演示如何使用 **directoryObjects**。</span><span class="sxs-lookup"><span data-stu-id="2c592-145">This example shows how you can use **directoryObjects**.</span></span>

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

#### <a name="response"></a><span data-ttu-id="2c592-146">响应</span><span class="sxs-lookup"><span data-stu-id="2c592-146">Response</span></span>
<span data-ttu-id="2c592-147">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="2c592-147">The following example shows the response.</span></span> 

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

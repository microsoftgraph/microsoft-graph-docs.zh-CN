---
title: 添加成员
description: 通过**members**导航属性将成员添加到 Microsoft 365 组、安全组或启用邮件的安全组。
localization_priority: Priority
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 0388d13d0e50c6ffcc415503a75afb8af56fa14f
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2020
ms.locfileid: "44897146"
---
# <a name="add-member"></a><span data-ttu-id="db916-103">添加成员</span><span class="sxs-lookup"><span data-stu-id="db916-103">Add member</span></span>

<span data-ttu-id="db916-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="db916-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="db916-105">通过**members**导航属性将成员添加到 Microsoft 365 组或安全组。</span><span class="sxs-lookup"><span data-stu-id="db916-105">Add a member to a Microsoft 365 group or a security group through the **members** navigation property.</span></span>

<span data-ttu-id="db916-106">您可以添加用户、组织联系人、服务主体或其他组。</span><span class="sxs-lookup"><span data-stu-id="db916-106">You can add users, organizational contacts, service principals or other groups.</span></span> 

> [!IMPORTANT]
> <span data-ttu-id="db916-107">只能向通过云管理的安全和 Microsoft 365 组添加用户。</span><span class="sxs-lookup"><span data-stu-id="db916-107">You can only add users to security and Microsoft 365 groups managed through the cloud.</span></span>

## <a name="permissions"></a><span data-ttu-id="db916-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="db916-108">Permissions</span></span>
<span data-ttu-id="db916-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="db916-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="db916-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="db916-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="db916-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="db916-111">Permission type</span></span>      | <span data-ttu-id="db916-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="db916-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="db916-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="db916-113">Delegated (work or school account)</span></span> | <span data-ttu-id="db916-114">GroupMember.ReadWrite.All、Group.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="db916-114">GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="db916-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="db916-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="db916-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="db916-116">Not supported.</span></span>    |
|<span data-ttu-id="db916-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="db916-117">Application</span></span> | <span data-ttu-id="db916-118">GroupMember.ReadWrite.All、Group.ReadWrite.All 和 Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db916-118">GroupMember.ReadWrite.All, Group.ReadWrite.All and Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="db916-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="db916-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/members/$ref
```

## <a name="request-headers"></a><span data-ttu-id="db916-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="db916-120">Request headers</span></span>
| <span data-ttu-id="db916-121">标头</span><span class="sxs-lookup"><span data-stu-id="db916-121">Header</span></span>       | <span data-ttu-id="db916-122">值</span><span class="sxs-lookup"><span data-stu-id="db916-122">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="db916-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="db916-123">Authorization</span></span>  | <span data-ttu-id="db916-124">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="db916-124">Bearer {token}.</span></span> <span data-ttu-id="db916-125">Required.</span><span class="sxs-lookup"><span data-stu-id="db916-125">Required.</span></span> |
| <span data-ttu-id="db916-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="db916-126">Content-type</span></span>   | <span data-ttu-id="db916-127">application/json.</span><span class="sxs-lookup"><span data-stu-id="db916-127">application/json.</span></span> <span data-ttu-id="db916-128">Required.</span><span class="sxs-lookup"><span data-stu-id="db916-128">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="db916-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="db916-129">Request body</span></span>
<span data-ttu-id="db916-130">在请求正文中，提供要添加的 [directoryObject](../resources/directoryobject.md)、[user](../resources/user.md)、[group](../resources/group.md) 或 [organizational contact](../resources/orgcontact.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="db916-130">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md), [user](../resources/user.md), [group](../resources/group.md), or [organizational contact](../resources/orgcontact.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="db916-131">响应</span><span class="sxs-lookup"><span data-stu-id="db916-131">Response</span></span>
<span data-ttu-id="db916-132">If successful, this method returns a `204 No Content` response code.</span><span class="sxs-lookup"><span data-stu-id="db916-132">If successful, this method returns a `204 No Content` response code.</span></span> <span data-ttu-id="db916-133">It does not return anything in the response body.</span><span class="sxs-lookup"><span data-stu-id="db916-133">It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="db916-134">示例</span><span class="sxs-lookup"><span data-stu-id="db916-134">Examples</span></span>
### <a name="example-1-add-a-member-to-a-group"></a><span data-ttu-id="db916-135">示例1：向组中添加成员</span><span class="sxs-lookup"><span data-stu-id="db916-135">Example 1: Add a member to a group</span></span>
#### <a name="request"></a><span data-ttu-id="db916-136">请求</span><span class="sxs-lookup"><span data-stu-id="db916-136">Request</span></span>
<span data-ttu-id="db916-137">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="db916-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="db916-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="db916-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_member_from_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/members/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id": "https://graph.microsoft.com/v1.0/directoryObjects/{id}"
}
```
# <a name="javascript"></a>[<span data-ttu-id="db916-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="db916-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-member-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="db916-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="db916-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-member-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="db916-141">C#</span><span class="sxs-lookup"><span data-stu-id="db916-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-member-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="db916-142">Java</span><span class="sxs-lookup"><span data-stu-id="db916-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-member-from-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="db916-143">响应</span><span class="sxs-lookup"><span data-stu-id="db916-143">Response</span></span>
<span data-ttu-id="db916-144">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="db916-144">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-2-add-multiple-members-to-a-group-in-a-single-request"></a><span data-ttu-id="db916-145">示例2：将多个成员添加到单个请求中的组</span><span class="sxs-lookup"><span data-stu-id="db916-145">Example 2: Add multiple members to a group in a single request</span></span>
<span data-ttu-id="db916-146">本示例演示如何在修补程序操作中将多个成员添加到具有 OData 绑定支持的组中。</span><span class="sxs-lookup"><span data-stu-id="db916-146">This example shows how to add multiple members to a group with OData bind support in a PATCH operation.</span></span> <span data-ttu-id="db916-147">请注意，单个请求中最长可添加20个成员。</span><span class="sxs-lookup"><span data-stu-id="db916-147">Note that up to 20 members can be added in a single request.</span></span> <span data-ttu-id="db916-148">不支持 POST 操作。</span><span class="sxs-lookup"><span data-stu-id="db916-148">The POST operation is not supported.</span></span>
#### <a name="request"></a><span data-ttu-id="db916-149">请求</span><span class="sxs-lookup"><span data-stu-id="db916-149">Request</span></span>
<span data-ttu-id="db916-150">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="db916-150">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="db916-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="db916-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_member_from_group"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/groups/{id}
Content-type: application/json
Content-length: 30

{
  "members@odata.bind": [
    "https://graph.microsoft.com/v1.0/directoryObjects/{id}",
    "https://graph.microsoft.com/v1.0/directoryObjects/{id}",
    "https://graph.microsoft.com/v1.0/directoryObjects/{id}"
    ]
}
```
# <a name="javascript"></a>[<span data-ttu-id="db916-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="db916-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-member-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="db916-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="db916-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-member-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="db916-154">C#</span><span class="sxs-lookup"><span data-stu-id="db916-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-member-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="db916-155">Java</span><span class="sxs-lookup"><span data-stu-id="db916-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-member-from-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="db916-156">响应</span><span class="sxs-lookup"><span data-stu-id="db916-156">Response</span></span>
<span data-ttu-id="db916-157">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="db916-157">The following is an example of the response.</span></span>

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

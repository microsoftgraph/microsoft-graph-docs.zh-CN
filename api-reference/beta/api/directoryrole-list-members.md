---
title: 列出成员
description: 检索分配给目录角色的用户列表。只能将用户分配给目录角色。
author: abhijeetsinha
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: d90baace95b3698a84ef55f74cca327ab95b5081
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2021
ms.locfileid: "52990872"
---
# <a name="list-members"></a><span data-ttu-id="e9317-104">列出成员</span><span class="sxs-lookup"><span data-stu-id="e9317-104">List members</span></span>

<span data-ttu-id="e9317-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e9317-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e9317-p102">检索分配给目录角色的用户列表。只能将用户分配给目录角色。</span><span class="sxs-lookup"><span data-stu-id="e9317-p102">Retrieve a list of the users that are assigned to the directory role.  Only users can be assigned to a directory role.</span></span>

<span data-ttu-id="e9317-108">你可以将 **directoryRole** 的对象 ID 和模板 ID 用于此 API。</span><span class="sxs-lookup"><span data-stu-id="e9317-108">You can use both the object ID and template ID of the **directoryRole** with this API.</span></span> <span data-ttu-id="e9317-109">内置角色的模板 ID 是不可可变的，可以在 Azure 门户的角色描述中查看。</span><span class="sxs-lookup"><span data-stu-id="e9317-109">The template ID of a built-in role is immutable and can be seen in the role description on the Azure portal.</span></span> <span data-ttu-id="e9317-110">有关详细信息，请参阅[角色模板的 ID。](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#role-template-ids)</span><span class="sxs-lookup"><span data-stu-id="e9317-110">For details, see [Role template IDs](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#role-template-ids).</span></span>

## <a name="permissions"></a><span data-ttu-id="e9317-111">权限</span><span class="sxs-lookup"><span data-stu-id="e9317-111">Permissions</span></span>
<span data-ttu-id="e9317-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e9317-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="e9317-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="e9317-114">Permission type</span></span>      | <span data-ttu-id="e9317-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e9317-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e9317-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e9317-116">Delegated (work or school account)</span></span> | <span data-ttu-id="e9317-117">RoleManagement.Read.Directory、Directory.Read.All、RoleManagement.ReadWrite.Directory、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e9317-117">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e9317-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e9317-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e9317-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="e9317-119">Not supported.</span></span>    |
|<span data-ttu-id="e9317-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="e9317-120">Application</span></span> | <span data-ttu-id="e9317-121">RoleManagement.Read.Directory、Directory.Read.All、RoleManagement.ReadWrite.Directory、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e9317-121">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="e9317-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e9317-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoles/{role-objectId}/members
GET /directoryRoles/roleTemplateId={role-templateId}/members
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e9317-123">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="e9317-123">Optional query parameters</span></span>
<span data-ttu-id="e9317-124">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="e9317-124">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="e9317-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="e9317-125">Request headers</span></span>
| <span data-ttu-id="e9317-126">名称</span><span class="sxs-lookup"><span data-stu-id="e9317-126">Name</span></span>       | <span data-ttu-id="e9317-127">类型</span><span class="sxs-lookup"><span data-stu-id="e9317-127">Type</span></span> | <span data-ttu-id="e9317-128">说明</span><span class="sxs-lookup"><span data-stu-id="e9317-128">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="e9317-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="e9317-129">Authorization</span></span>  | <span data-ttu-id="e9317-130">string</span><span class="sxs-lookup"><span data-stu-id="e9317-130">string</span></span>  | <span data-ttu-id="e9317-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e9317-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e9317-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="e9317-133">Request body</span></span>
<span data-ttu-id="e9317-134">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e9317-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e9317-135">响应</span><span class="sxs-lookup"><span data-stu-id="e9317-135">Response</span></span>

<span data-ttu-id="e9317-136">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="e9317-136">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="e9317-137">示例</span><span class="sxs-lookup"><span data-stu-id="e9317-137">Examples</span></span>

### <a name="example-1-get-the-members-of-a-directory-role-using-role-objectid"></a><span data-ttu-id="e9317-138">示例 1：使用 role objectId 获取目录角色的成员</span><span class="sxs-lookup"><span data-stu-id="e9317-138">Example 1: Get the members of a directory role using role objectId</span></span>

#### <a name="request"></a><span data-ttu-id="e9317-139">请求</span><span class="sxs-lookup"><span data-stu-id="e9317-139">Request</span></span>
<span data-ttu-id="e9317-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e9317-140">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e9317-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="e9317-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directoryrole_members"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/directoryRoles/23f3b4b4-8a29-4420-8052-e4950273bbda/members
```
# <a name="c"></a>[<span data-ttu-id="e9317-142">C#</span><span class="sxs-lookup"><span data-stu-id="e9317-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directoryrole-members-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e9317-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e9317-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directoryrole-members-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e9317-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e9317-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directoryrole-members-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e9317-145">Java</span><span class="sxs-lookup"><span data-stu-id="e9317-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-directoryrole-members-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="e9317-146">响应</span><span class="sxs-lookup"><span data-stu-id="e9317-146">Response</span></span>
> <span data-ttu-id="e9317-147">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="e9317-147">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "businessPhones":["000-000-0000"],
      "displayName":"Adele Vance",
      "givenName":"Adele",
      "jobTitle":null,
      "mail":"AdeleV@contoso.com",
      "officeLocation":null,
      "preferredLanguage":"en-US",
      "surname":"Vance",
      "userPrincipalName":"AdeleV@contoso.com"
    }
  ]
}
```

### <a name="example-2-get-the-members-of-a-directory-role-using-role-templateid"></a><span data-ttu-id="e9317-148">示例 2：使用角色 templateId 获取目录角色的成员</span><span class="sxs-lookup"><span data-stu-id="e9317-148">Example 2: Get the members of a directory role using role templateId</span></span>

#### <a name="request"></a><span data-ttu-id="e9317-149">请求</span><span class="sxs-lookup"><span data-stu-id="e9317-149">Request</span></span>
<span data-ttu-id="e9317-150">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e9317-150">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="e9317-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="e9317-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directoryrole_members_templateId"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/directoryRoles/roleTemplateId=4a5d8f65-41da-4de4-8968-e035b65339cf/members
```
# <a name="c"></a>[<span data-ttu-id="e9317-152">C#</span><span class="sxs-lookup"><span data-stu-id="e9317-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directoryrole-members-templateid-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e9317-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e9317-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directoryrole-members-templateid-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e9317-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e9317-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directoryrole-members-templateid-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e9317-155">Java</span><span class="sxs-lookup"><span data-stu-id="e9317-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-directoryrole-members-templateid-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e9317-156">响应</span><span class="sxs-lookup"><span data-stu-id="e9317-156">Response</span></span>
><span data-ttu-id="e9317-157">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="e9317-157">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "businessPhones":["000-000-0000"],
      "displayName":"Adele Vance",
      "givenName":"Adele",
      "jobTitle":null,
      "mail":"AdeleV@contoso.com",
      "officeLocation":null,
      "preferredLanguage":"en-US",
      "surname":"Vance",
      "userPrincipalName":"AdeleV@contoso.com"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List members",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

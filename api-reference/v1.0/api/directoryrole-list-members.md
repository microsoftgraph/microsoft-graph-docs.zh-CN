---
title: 列出目录角色的成员
description: 检索分配给目录角色的主体列表。
author: abhijeetsinha
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 51e9a1fec22df0abf326a21f1cd7309e343fc152
ms.sourcegitcommit: d0d2d17a31cbcb01b1ae18bd6a18c39d7077069a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/24/2021
ms.locfileid: "53118635"
---
# <a name="list-members-of-a-directory-role"></a><span data-ttu-id="aea01-103">列出目录角色的成员</span><span class="sxs-lookup"><span data-stu-id="aea01-103">List members of a directory role</span></span>

<span data-ttu-id="aea01-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aea01-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="aea01-105">检索分配给目录角色的主体列表。</span><span class="sxs-lookup"><span data-stu-id="aea01-105">Retrieve the list of principals that are assigned to the directory role.</span></span> 

<span data-ttu-id="aea01-106">你可以将 **directoryRole** 的对象 ID 和模板 ID 用于此 API。</span><span class="sxs-lookup"><span data-stu-id="aea01-106">You can use both the object ID and template ID of the **directoryRole** with this API.</span></span> <span data-ttu-id="aea01-107">内置角色的模板 ID 是不可可变的，可以在 Azure 门户的角色描述中查看。</span><span class="sxs-lookup"><span data-stu-id="aea01-107">The template ID of a built-in role is immutable and can be seen in the role description on the Azure portal.</span></span> <span data-ttu-id="aea01-108">有关详细信息，请参阅[角色模板的 ID。](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#role-template-ids)</span><span class="sxs-lookup"><span data-stu-id="aea01-108">For details, see [Role template IDs](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#role-template-ids).</span></span>

## <a name="permissions"></a><span data-ttu-id="aea01-109">权限</span><span class="sxs-lookup"><span data-stu-id="aea01-109">Permissions</span></span>
<span data-ttu-id="aea01-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="aea01-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="aea01-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="aea01-112">Permission type</span></span>      | <span data-ttu-id="aea01-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="aea01-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aea01-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="aea01-114">Delegated (work or school account)</span></span> | <span data-ttu-id="aea01-115">RoleManagement.Read.Directory、Directory.Read.All、RoleManagement.ReadWrite.Directory、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="aea01-115">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="aea01-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="aea01-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aea01-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="aea01-117">Not supported.</span></span>    |
|<span data-ttu-id="aea01-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="aea01-118">Application</span></span> | <span data-ttu-id="aea01-119">RoleManagement.Read.Directory、Directory.Read.All、RoleManagement.ReadWrite.Directory、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aea01-119">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="aea01-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="aea01-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoles/{role-id}/members
GET /directoryRoles/roleTemplateId={roleTemplateId}/members
```
## <a name="optional-query-parameters"></a><span data-ttu-id="aea01-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="aea01-121">Optional query parameters</span></span>
<span data-ttu-id="aea01-122">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="aea01-122">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="aea01-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="aea01-123">Request headers</span></span>
| <span data-ttu-id="aea01-124">名称</span><span class="sxs-lookup"><span data-stu-id="aea01-124">Name</span></span>       | <span data-ttu-id="aea01-125">类型</span><span class="sxs-lookup"><span data-stu-id="aea01-125">Type</span></span> | <span data-ttu-id="aea01-126">说明</span><span class="sxs-lookup"><span data-stu-id="aea01-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="aea01-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="aea01-127">Authorization</span></span>  | <span data-ttu-id="aea01-128">string</span><span class="sxs-lookup"><span data-stu-id="aea01-128">string</span></span>  | <span data-ttu-id="aea01-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="aea01-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="aea01-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="aea01-131">Request body</span></span>
<span data-ttu-id="aea01-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="aea01-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="aea01-133">响应</span><span class="sxs-lookup"><span data-stu-id="aea01-133">Response</span></span>

<span data-ttu-id="aea01-134">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="aea01-134">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="aea01-135">示例</span><span class="sxs-lookup"><span data-stu-id="aea01-135">Examples</span></span>

### <a name="example-1-get-the-members-of-a-directory-role-using-role-id"></a><span data-ttu-id="aea01-136">示例 1：使用角色 ID 获取目录角色的成员</span><span class="sxs-lookup"><span data-stu-id="aea01-136">Example 1: Get the members of a directory role using role id</span></span>

#### <a name="request"></a><span data-ttu-id="aea01-137">请求</span><span class="sxs-lookup"><span data-stu-id="aea01-137">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="aea01-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="aea01-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directoryrole_members_objectid"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/directoryRoles/23f3b4b4-8a29-4420-8052-e4950273bbda/members
```
# <a name="c"></a>[<span data-ttu-id="aea01-139">C#</span><span class="sxs-lookup"><span data-stu-id="aea01-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directoryrole-members-objectid-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="aea01-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="aea01-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directoryrole-members-objectid-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="aea01-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="aea01-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directoryrole-members-objectid-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="aea01-142">Java</span><span class="sxs-lookup"><span data-stu-id="aea01-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-directoryrole-members-objectid-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="aea01-143">响应</span><span class="sxs-lookup"><span data-stu-id="aea01-143">Response</span></span>
> <span data-ttu-id="aea01-144">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="aea01-144">**Note:** The response object shown here might be shortened for readability.</span></span>
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
### <a name="example-2-get-the-members-of-a-directory-role-using-roletemplateid"></a><span data-ttu-id="aea01-145">示例 2：使用 roleTemplateId 获取目录角色的成员</span><span class="sxs-lookup"><span data-stu-id="aea01-145">Example 2: Get the members of a directory role using roleTemplateId</span></span>

##### <a name="request"></a><span data-ttu-id="aea01-146">请求</span><span class="sxs-lookup"><span data-stu-id="aea01-146">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="aea01-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="aea01-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directoryrole_members_templateId"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/directoryRoles/roleTemplateId=4a5d8f65-41da-4de4-8968-e035b65339cf/members
```
# <a name="c"></a>[<span data-ttu-id="aea01-148">C#</span><span class="sxs-lookup"><span data-stu-id="aea01-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directoryrole-members-templateid-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="aea01-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="aea01-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directoryrole-members-templateid-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="aea01-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="aea01-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directoryrole-members-templateid-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="aea01-151">Java</span><span class="sxs-lookup"><span data-stu-id="aea01-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-directoryrole-members-templateid-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="aea01-152">响应</span><span class="sxs-lookup"><span data-stu-id="aea01-152">Response</span></span>
><span data-ttu-id="aea01-153">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="aea01-153">**Note:** The response object shown here might be shortened for readability.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List members",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

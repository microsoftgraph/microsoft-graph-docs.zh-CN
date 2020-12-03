---
title: 列出目录角色的成员
description: 检索分配给目录角色的主体列表。
author: abhijeetsinha
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 357333bb1f15828e8dd4ee0d37233539ce47edbd
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/01/2020
ms.locfileid: "49524571"
---
# <a name="list-members-of-a-directory-role"></a><span data-ttu-id="e3505-103">列出目录角色的成员</span><span class="sxs-lookup"><span data-stu-id="e3505-103">List members of a directory role</span></span>

<span data-ttu-id="e3505-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e3505-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e3505-105">检索分配给目录角色的主体列表。</span><span class="sxs-lookup"><span data-stu-id="e3505-105">Retrieve the list of principals that are assigned to the directory role.</span></span> 

> [!Note]
> <span data-ttu-id="e3505-106">您可以将 **directoryRole** 的对象 id 和模板 ID 与此 API 一起使用。</span><span class="sxs-lookup"><span data-stu-id="e3505-106">You can use both the object ID and template ID of the **directoryRole** with this API.</span></span> <span data-ttu-id="e3505-107">内置角色的模板 ID 是不可变的，可在 Azure 门户上的角色说明中查看。</span><span class="sxs-lookup"><span data-stu-id="e3505-107">The template ID of a built-in role is immutable and can be seen in the role description on the Azure portal.</span></span> <span data-ttu-id="e3505-108">有关详细信息，请参阅 [角色模板 id](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#role-template-ids)。</span><span class="sxs-lookup"><span data-stu-id="e3505-108">For details, see [Role template IDs](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#role-template-ids).</span></span>

## <a name="permissions"></a><span data-ttu-id="e3505-109">权限</span><span class="sxs-lookup"><span data-stu-id="e3505-109">Permissions</span></span>
<span data-ttu-id="e3505-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e3505-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="e3505-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="e3505-112">Permission type</span></span>      | <span data-ttu-id="e3505-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e3505-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e3505-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e3505-114">Delegated (work or school account)</span></span> | <span data-ttu-id="e3505-115">RoleManagement、RoleManagement、Directory.accessasuser.all、all、、all、all 和的所有子目录。</span><span class="sxs-lookup"><span data-stu-id="e3505-115">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e3505-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e3505-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e3505-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="e3505-117">Not supported.</span></span>    |
|<span data-ttu-id="e3505-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="e3505-118">Application</span></span> | <span data-ttu-id="e3505-119">RoleManagement、RoleManagement、目录和所有读写的所有子目录。所有</span><span class="sxs-lookup"><span data-stu-id="e3505-119">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="e3505-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e3505-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoles/{id}/members
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e3505-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="e3505-121">Optional query parameters</span></span>
<span data-ttu-id="e3505-122">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="e3505-122">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="e3505-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="e3505-123">Request headers</span></span>
| <span data-ttu-id="e3505-124">名称</span><span class="sxs-lookup"><span data-stu-id="e3505-124">Name</span></span>       | <span data-ttu-id="e3505-125">类型</span><span class="sxs-lookup"><span data-stu-id="e3505-125">Type</span></span> | <span data-ttu-id="e3505-126">说明</span><span class="sxs-lookup"><span data-stu-id="e3505-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="e3505-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="e3505-127">Authorization</span></span>  | <span data-ttu-id="e3505-128">string</span><span class="sxs-lookup"><span data-stu-id="e3505-128">string</span></span>  | <span data-ttu-id="e3505-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e3505-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e3505-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="e3505-131">Request body</span></span>
<span data-ttu-id="e3505-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e3505-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e3505-133">响应</span><span class="sxs-lookup"><span data-stu-id="e3505-133">Response</span></span>

<span data-ttu-id="e3505-134">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="e3505-134">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="e3505-135">示例</span><span class="sxs-lookup"><span data-stu-id="e3505-135">Examples</span></span>

### <a name="example-1-get-the-members-of-a-directory-role-using-objectid"></a><span data-ttu-id="e3505-136">示例1：使用 objectId 获取目录角色的成员</span><span class="sxs-lookup"><span data-stu-id="e3505-136">Example 1: Get the members of a directory role using objectId</span></span>

##### <a name="request"></a><span data-ttu-id="e3505-137">请求</span><span class="sxs-lookup"><span data-stu-id="e3505-137">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="e3505-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="e3505-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directoryrole_members_objectid"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/directoryRoles/23f3b4b4-8a29-4420-8052-e4950273bbda/members
```
# <a name="c"></a>[<span data-ttu-id="e3505-139">C#</span><span class="sxs-lookup"><span data-stu-id="e3505-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directoryrole-members-objectid-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e3505-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e3505-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directoryrole-members-objectid-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e3505-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e3505-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directoryrole-members-objectid-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e3505-142">Java</span><span class="sxs-lookup"><span data-stu-id="e3505-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-directoryrole-members-objectid-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="e3505-143">响应</span><span class="sxs-lookup"><span data-stu-id="e3505-143">Response</span></span>
> <span data-ttu-id="e3505-144">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="e3505-144">**Note:** The response object shown here might be shortened for readability.</span></span>
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
      "displayName":"First Last",
      "givenName":"First",
      "jobTitle":null,
      "mail":"first@example.com",
      "officeLocation":null,
      "preferredLanguage":"en-US",
      "surname":"Last",
      "userPrincipalName":"first@example.com"
    }
  ]
}
```
### <a name="example-2-get-the-members-of-a-directory-role-using-templateid"></a><span data-ttu-id="e3505-145">示例2：使用 templateId 获取目录角色的成员</span><span class="sxs-lookup"><span data-stu-id="e3505-145">Example 2: Get the members of a directory role using templateId</span></span>

##### <a name="request"></a><span data-ttu-id="e3505-146">请求</span><span class="sxs-lookup"><span data-stu-id="e3505-146">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="e3505-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="e3505-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directoryrole_members_templateId"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/directoryRoles/roleTemplateId=4a5d8f65-41da-4de4-8968-e035b65339cf/members
```
# <a name="c"></a>[<span data-ttu-id="e3505-148">C#</span><span class="sxs-lookup"><span data-stu-id="e3505-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directoryrole-members-templateid-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e3505-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e3505-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directoryrole-members-templateid-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e3505-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e3505-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directoryrole-members-templateid-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e3505-151">Java</span><span class="sxs-lookup"><span data-stu-id="e3505-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-directoryrole-members-templateid-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="e3505-152">响应</span><span class="sxs-lookup"><span data-stu-id="e3505-152">Response</span></span>
><span data-ttu-id="e3505-153">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="e3505-153">**Note:** The response object shown here might be shortened for readability.</span></span>
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
      "displayName":"First Last",
      "givenName":"First",
      "jobTitle":null,
      "mail":"first@example.com",
      "officeLocation":null,
      "preferredLanguage":"en-US",
      "surname":"Last",
      "userPrincipalName":"first@example.com"
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

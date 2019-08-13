---
title: 列出成员
description: 检索分配给目录角色的用户列表。  只能将用户分配给目录角色。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e69d2ec79ffc82867df52519c0fa7a5ec7711edd
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36375350"
---
# <a name="list-members"></a><span data-ttu-id="db704-104">列出成员</span><span class="sxs-lookup"><span data-stu-id="db704-104">List members</span></span>

<span data-ttu-id="db704-105">检索分配给目录角色的用户列表。</span><span class="sxs-lookup"><span data-stu-id="db704-105">Retrieve a list of the users that are assigned to the directory role.</span></span>  <span data-ttu-id="db704-106">只能将用户分配给目录角色。</span><span class="sxs-lookup"><span data-stu-id="db704-106">Only users can be assigned to a directory role.</span></span>
## <a name="permissions"></a><span data-ttu-id="db704-107">权限</span><span class="sxs-lookup"><span data-stu-id="db704-107">Permissions</span></span>
<span data-ttu-id="db704-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="db704-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="db704-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="db704-110">Permission type</span></span>      | <span data-ttu-id="db704-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="db704-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="db704-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="db704-112">Delegated (work or school account)</span></span> | <span data-ttu-id="db704-113">RoleManagement、RoleManagement、Directory.accessasuser.all、all、、all、all 和的所有子目录。</span><span class="sxs-lookup"><span data-stu-id="db704-113">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="db704-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="db704-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="db704-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="db704-115">Not supported.</span></span>    |
|<span data-ttu-id="db704-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="db704-116">Application</span></span> | <span data-ttu-id="db704-117">RoleManagement、RoleManagement、目录和所有读写的所有子目录。所有</span><span class="sxs-lookup"><span data-stu-id="db704-117">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="db704-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="db704-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoles/{id}/members
```
## <a name="optional-query-parameters"></a><span data-ttu-id="db704-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="db704-119">Optional query parameters</span></span>
<span data-ttu-id="db704-120">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="db704-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="db704-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="db704-121">Request headers</span></span>
| <span data-ttu-id="db704-122">名称</span><span class="sxs-lookup"><span data-stu-id="db704-122">Name</span></span>       | <span data-ttu-id="db704-123">类型</span><span class="sxs-lookup"><span data-stu-id="db704-123">Type</span></span> | <span data-ttu-id="db704-124">说明</span><span class="sxs-lookup"><span data-stu-id="db704-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="db704-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="db704-125">Authorization</span></span>  | <span data-ttu-id="db704-126">string</span><span class="sxs-lookup"><span data-stu-id="db704-126">string</span></span>  | <span data-ttu-id="db704-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="db704-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="db704-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="db704-129">Request body</span></span>
<span data-ttu-id="db704-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="db704-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="db704-131">响应</span><span class="sxs-lookup"><span data-stu-id="db704-131">Response</span></span>

<span data-ttu-id="db704-132">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="db704-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="db704-133">示例</span><span class="sxs-lookup"><span data-stu-id="db704-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="db704-134">请求</span><span class="sxs-lookup"><span data-stu-id="db704-134">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="db704-135">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="db704-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_members"
}-->
```http
GET https://graph.microsoft.com/v1.0/directoryRoles/{id}/members
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="db704-136">C#</span><span class="sxs-lookup"><span data-stu-id="db704-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-members-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="db704-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="db704-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-members-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="db704-138">目标-C</span><span class="sxs-lookup"><span data-stu-id="db704-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-members-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="db704-139">Java</span><span class="sxs-lookup"><span data-stu-id="db704-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-members-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="db704-140">响应</span><span class="sxs-lookup"><span data-stu-id="db704-140">Response</span></span>
<span data-ttu-id="db704-p105">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="db704-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

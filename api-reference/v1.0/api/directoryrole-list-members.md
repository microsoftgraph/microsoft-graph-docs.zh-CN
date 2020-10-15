---
title: 列出成员
description: 检索分配给目录角色的用户列表。  只能将用户分配给目录角色。
author: abhijeetsinha
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 4041d4b94e873ab81c61986cb604664f2c268f0d
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/14/2020
ms.locfileid: "48460794"
---
# <a name="list-members"></a><span data-ttu-id="96933-104">列出成员</span><span class="sxs-lookup"><span data-stu-id="96933-104">List members</span></span>

<span data-ttu-id="96933-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="96933-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="96933-106">检索分配给目录角色的用户列表。</span><span class="sxs-lookup"><span data-stu-id="96933-106">Retrieve a list of the users that are assigned to the directory role.</span></span>  <span data-ttu-id="96933-107">只能将用户分配给目录角色。</span><span class="sxs-lookup"><span data-stu-id="96933-107">Only users can be assigned to a directory role.</span></span>
## <a name="permissions"></a><span data-ttu-id="96933-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="96933-108">Permissions</span></span>
<span data-ttu-id="96933-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="96933-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="96933-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="96933-111">Permission type</span></span>      | <span data-ttu-id="96933-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="96933-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="96933-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="96933-113">Delegated (work or school account)</span></span> | <span data-ttu-id="96933-114">RoleManagement、RoleManagement、Directory.accessasuser.all、all、、all、all 和的所有子目录。</span><span class="sxs-lookup"><span data-stu-id="96933-114">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="96933-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="96933-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="96933-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="96933-116">Not supported.</span></span>    |
|<span data-ttu-id="96933-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="96933-117">Application</span></span> | <span data-ttu-id="96933-118">RoleManagement、RoleManagement、目录和所有读写的所有子目录。所有</span><span class="sxs-lookup"><span data-stu-id="96933-118">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="96933-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="96933-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoles/{id}/members
```
## <a name="optional-query-parameters"></a><span data-ttu-id="96933-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="96933-120">Optional query parameters</span></span>
<span data-ttu-id="96933-121">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="96933-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="96933-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="96933-122">Request headers</span></span>
| <span data-ttu-id="96933-123">名称</span><span class="sxs-lookup"><span data-stu-id="96933-123">Name</span></span>       | <span data-ttu-id="96933-124">类型</span><span class="sxs-lookup"><span data-stu-id="96933-124">Type</span></span> | <span data-ttu-id="96933-125">说明</span><span class="sxs-lookup"><span data-stu-id="96933-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="96933-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="96933-126">Authorization</span></span>  | <span data-ttu-id="96933-127">string</span><span class="sxs-lookup"><span data-stu-id="96933-127">string</span></span>  | <span data-ttu-id="96933-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="96933-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="96933-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="96933-130">Request body</span></span>
<span data-ttu-id="96933-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="96933-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="96933-132">响应</span><span class="sxs-lookup"><span data-stu-id="96933-132">Response</span></span>

<span data-ttu-id="96933-133">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="96933-133">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="96933-134">示例</span><span class="sxs-lookup"><span data-stu-id="96933-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="96933-135">请求</span><span class="sxs-lookup"><span data-stu-id="96933-135">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="96933-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="96933-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directoryrole_members"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/directoryRoles/{id}/members
```
# <a name="c"></a>[<span data-ttu-id="96933-137">C#</span><span class="sxs-lookup"><span data-stu-id="96933-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directoryrole-members-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="96933-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="96933-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directoryrole-members-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="96933-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="96933-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directoryrole-members-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="96933-140">Java</span><span class="sxs-lookup"><span data-stu-id="96933-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-directoryrole-members-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="96933-141">响应</span><span class="sxs-lookup"><span data-stu-id="96933-141">Response</span></span>
<span data-ttu-id="96933-p105">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="96933-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

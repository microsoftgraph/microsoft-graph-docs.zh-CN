---
title: 列出成员
description: 检索分配给目录角色的用户列表。  只能将用户分配给目录角色。
author: abhijeetsinha
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: fe21dbeac9134ea0ae799d3504d0d43ed10bb965
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48956358"
---
# <a name="list-members"></a><span data-ttu-id="1c6a1-104">列出成员</span><span class="sxs-lookup"><span data-stu-id="1c6a1-104">List members</span></span>

<span data-ttu-id="1c6a1-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1c6a1-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1c6a1-106">检索分配给目录角色的用户列表。</span><span class="sxs-lookup"><span data-stu-id="1c6a1-106">Retrieve a list of the users that are assigned to the directory role.</span></span>  <span data-ttu-id="1c6a1-107">只能将用户分配给目录角色。</span><span class="sxs-lookup"><span data-stu-id="1c6a1-107">Only users can be assigned to a directory role.</span></span>
## <a name="permissions"></a><span data-ttu-id="1c6a1-108">权限</span><span class="sxs-lookup"><span data-stu-id="1c6a1-108">Permissions</span></span>
<span data-ttu-id="1c6a1-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1c6a1-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="1c6a1-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="1c6a1-111">Permission type</span></span>      | <span data-ttu-id="1c6a1-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1c6a1-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1c6a1-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1c6a1-113">Delegated (work or school account)</span></span> | <span data-ttu-id="1c6a1-114">RoleManagement、RoleManagement、Directory.accessasuser.all、all、、all、all 和的所有子目录。</span><span class="sxs-lookup"><span data-stu-id="1c6a1-114">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="1c6a1-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1c6a1-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1c6a1-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="1c6a1-116">Not supported.</span></span>    |
|<span data-ttu-id="1c6a1-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="1c6a1-117">Application</span></span> | <span data-ttu-id="1c6a1-118">RoleManagement、RoleManagement、目录和所有读写的所有子目录。所有</span><span class="sxs-lookup"><span data-stu-id="1c6a1-118">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="1c6a1-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1c6a1-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoles/{id}/members
```
## <a name="optional-query-parameters"></a><span data-ttu-id="1c6a1-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="1c6a1-120">Optional query parameters</span></span>
<span data-ttu-id="1c6a1-121">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="1c6a1-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="1c6a1-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="1c6a1-122">Request headers</span></span>
| <span data-ttu-id="1c6a1-123">名称</span><span class="sxs-lookup"><span data-stu-id="1c6a1-123">Name</span></span>       | <span data-ttu-id="1c6a1-124">类型</span><span class="sxs-lookup"><span data-stu-id="1c6a1-124">Type</span></span> | <span data-ttu-id="1c6a1-125">说明</span><span class="sxs-lookup"><span data-stu-id="1c6a1-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="1c6a1-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="1c6a1-126">Authorization</span></span>  | <span data-ttu-id="1c6a1-127">string</span><span class="sxs-lookup"><span data-stu-id="1c6a1-127">string</span></span>  | <span data-ttu-id="1c6a1-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1c6a1-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1c6a1-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="1c6a1-130">Request body</span></span>
<span data-ttu-id="1c6a1-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1c6a1-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1c6a1-132">响应</span><span class="sxs-lookup"><span data-stu-id="1c6a1-132">Response</span></span>

<span data-ttu-id="1c6a1-133">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="1c6a1-133">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1c6a1-134">示例</span><span class="sxs-lookup"><span data-stu-id="1c6a1-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1c6a1-135">请求</span><span class="sxs-lookup"><span data-stu-id="1c6a1-135">Request</span></span>
<span data-ttu-id="1c6a1-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1c6a1-136">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1c6a1-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="1c6a1-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directoryrole_members"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/directoryRoles/{id}/members
```
# <a name="c"></a>[<span data-ttu-id="1c6a1-138">C#</span><span class="sxs-lookup"><span data-stu-id="1c6a1-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directoryrole-members-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1c6a1-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1c6a1-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directoryrole-members-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1c6a1-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1c6a1-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directoryrole-members-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1c6a1-141">Java</span><span class="sxs-lookup"><span data-stu-id="1c6a1-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-directoryrole-members-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="1c6a1-142">响应</span><span class="sxs-lookup"><span data-stu-id="1c6a1-142">Response</span></span>
<span data-ttu-id="1c6a1-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1c6a1-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
      "id": "id-value"
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

---
title: 列出所有者
description: '检索组的所有者列表。所有者是一组具有 group 对象修改权限的非管理员用户。 '
localization_priority: Priority
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 4b447e9f24fecfd2ab89e6d70aec36f17f47907c
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048706"
---
# <a name="list-owners"></a><span data-ttu-id="ddef3-104">列出所有者</span><span class="sxs-lookup"><span data-stu-id="ddef3-104">List owners</span></span>

<span data-ttu-id="ddef3-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ddef3-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ddef3-106">检索组的所有者列表。</span><span class="sxs-lookup"><span data-stu-id="ddef3-106">Retrieve a list of the group's owners.</span></span> <span data-ttu-id="ddef3-107">所有者是一组可修改组对象的用户或服务主体。</span><span class="sxs-lookup"><span data-stu-id="ddef3-107">The owners are a set of users or service principals who are allowed to modify the group object.</span></span> <span data-ttu-id="ddef3-108">对于已在 Exchange 中创建的组，或者已从本地环境中同步的组，Microsoft Graph 目前未提供所有者角色。</span><span class="sxs-lookup"><span data-stu-id="ddef3-108">Owners are currently not available in Microsoft Graph for groups that were created in Exchange or groups that are synchronized from an on-premises environment.</span></span>

><span data-ttu-id="ddef3-109">**注意：** 当前，由于向 Microsoft Graph v1.0 终结点分阶段部署服务主体，服务主体未被列为组所有者。</span><span class="sxs-lookup"><span data-stu-id="ddef3-109">**Note:** Currently, service principals are not listed as group owners due to the staged rollout of service principals to the Microsoft Graph v1.0 endpoint.</span></span>

## <a name="permissions"></a><span data-ttu-id="ddef3-110">权限</span><span class="sxs-lookup"><span data-stu-id="ddef3-110">Permissions</span></span>
<span data-ttu-id="ddef3-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ddef3-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ddef3-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="ddef3-113">Permission type</span></span>      | <span data-ttu-id="ddef3-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ddef3-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ddef3-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ddef3-115">Delegated (work or school account)</span></span> | <span data-ttu-id="ddef3-116">GroupMember.Read.All，Group.Read.All，GroupMember.ReadWrite.All，Group.ReadWrite.All，Directory.Read.All，Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ddef3-116">GroupMember.Read.All, Group.Read.All, GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ddef3-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ddef3-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ddef3-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="ddef3-118">Not supported.</span></span>    |
|<span data-ttu-id="ddef3-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="ddef3-119">Application</span></span> | <span data-ttu-id="ddef3-120">GroupMember.Read.All，Group.Read.All，GroupMember.ReadWrite.All，Group.ReadWrite.All，Directory.Read.All，Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ddef3-120">GroupMember.Read.All, Group.Read.All, GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span></span>  |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="ddef3-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ddef3-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/owners
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ddef3-122">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="ddef3-122">Optional query parameters</span></span>
<span data-ttu-id="ddef3-123">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="ddef3-123">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ddef3-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="ddef3-124">Request headers</span></span>
| <span data-ttu-id="ddef3-125">名称</span><span class="sxs-lookup"><span data-stu-id="ddef3-125">Name</span></span>       | <span data-ttu-id="ddef3-126">类型</span><span class="sxs-lookup"><span data-stu-id="ddef3-126">Type</span></span> | <span data-ttu-id="ddef3-127">说明</span><span class="sxs-lookup"><span data-stu-id="ddef3-127">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="ddef3-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="ddef3-128">Authorization</span></span>  | <span data-ttu-id="ddef3-129">string</span><span class="sxs-lookup"><span data-stu-id="ddef3-129">string</span></span>  | <span data-ttu-id="ddef3-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ddef3-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ddef3-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="ddef3-132">Request body</span></span>
<span data-ttu-id="ddef3-133">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ddef3-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ddef3-134">响应</span><span class="sxs-lookup"><span data-stu-id="ddef3-134">Response</span></span>
<span data-ttu-id="ddef3-135">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [user](../resources/user.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="ddef3-135">If successful, this method returns a `200 OK` response code and collection of [user](../resources/user.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ddef3-136">示例</span><span class="sxs-lookup"><span data-stu-id="ddef3-136">Example</span></span>
#### <a name="request"></a><span data-ttu-id="ddef3-137">请求</span><span class="sxs-lookup"><span data-stu-id="ddef3-137">Request</span></span>
<span data-ttu-id="ddef3-138">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ddef3-138">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ddef3-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="ddef3-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_get_owners"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/owners
```
# <a name="c"></a>[<span data-ttu-id="ddef3-140">C#</span><span class="sxs-lookup"><span data-stu-id="ddef3-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-get-owners-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ddef3-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ddef3-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-get-owners-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ddef3-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ddef3-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-get-owners-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ddef3-143">Java</span><span class="sxs-lookup"><span data-stu-id="ddef3-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-get-owners-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ddef3-144">响应</span><span class="sxs-lookup"><span data-stu-id="ddef3-144">Response</span></span>
<span data-ttu-id="ddef3-145">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ddef3-145">The following is an example of the response.</span></span>
><span data-ttu-id="ddef3-146">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="ddef3-146">**Note:** The response object shown here might be shortened for readability.</span></span>
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
      "@odata.type": "#microsoft.graph.user"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List owners",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->


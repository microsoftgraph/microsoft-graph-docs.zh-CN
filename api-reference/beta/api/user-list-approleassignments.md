---
title: 列出向用户授予的 appRoleAssignment
description: 检索授予用户的应用角色分配的列表。
localization_priority: Priority
doc_type: apiPageType
ms.prod: users
author: psignoret
ms.openlocfilehash: 6fa31fd31c8c898b508b9b0d02c602047eea58c5
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50136211"
---
# <a name="list-approleassignments-granted-to-a-user"></a><span data-ttu-id="0478a-103">列出向用户授予的 appRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="0478a-103">List appRoleAssignments granted to a user</span></span>

<span data-ttu-id="0478a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0478a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0478a-105">检索授予用户的 [appRoleAssignment](../resources/approleassignment.md) 的列表。</span><span class="sxs-lookup"><span data-stu-id="0478a-105">Retrieve the list of [appRoleAssignment](../resources/approleassignment.md) that a user has been granted.</span></span> <span data-ttu-id="0478a-106">此操作也会返回分配给用户是其直接成员的组的应用角色。</span><span class="sxs-lookup"><span data-stu-id="0478a-106">This operation also returns app roles assigned to groups that the user is a direct member of.</span></span>

## <a name="permissions"></a><span data-ttu-id="0478a-107">权限</span><span class="sxs-lookup"><span data-stu-id="0478a-107">Permissions</span></span>

<span data-ttu-id="0478a-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0478a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0478a-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="0478a-110">Permission type</span></span>      | <span data-ttu-id="0478a-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0478a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0478a-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0478a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="0478a-113">Directory.Read.All、AppRoleAssignment.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0478a-113">Directory.Read.All, AppRoleAssignment.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="0478a-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0478a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0478a-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="0478a-115">Not supported.</span></span>    |
|<span data-ttu-id="0478a-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="0478a-116">Application</span></span> | <span data-ttu-id="0478a-117">Directory.Read.All、AppRoleAssignment.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0478a-117">Directory.Read.All, AppRoleAssignment.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0478a-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0478a-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/appRoleAssignments
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0478a-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="0478a-119">Optional query parameters</span></span>

<span data-ttu-id="0478a-120">此方法支持使用 [OData 查询参数](/graph/query_parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="0478a-120">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0478a-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="0478a-121">Request headers</span></span>

| <span data-ttu-id="0478a-122">名称</span><span class="sxs-lookup"><span data-stu-id="0478a-122">Name</span></span>           | <span data-ttu-id="0478a-123">说明</span><span class="sxs-lookup"><span data-stu-id="0478a-123">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="0478a-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="0478a-124">Authorization</span></span>  | <span data-ttu-id="0478a-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0478a-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0478a-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="0478a-127">Request body</span></span>

<span data-ttu-id="0478a-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0478a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0478a-129">响应</span><span class="sxs-lookup"><span data-stu-id="0478a-129">Response</span></span>

<span data-ttu-id="0478a-130">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和 [appRoleAssignment](../resources/approleassignment.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="0478a-130">If successful, this method returns a `200 OK` response code and a collection of [appRoleAssignment](../resources/approleassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0478a-131">示例</span><span class="sxs-lookup"><span data-stu-id="0478a-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="0478a-132">请求</span><span class="sxs-lookup"><span data-stu-id="0478a-132">Request</span></span>

<span data-ttu-id="0478a-133">下面的示例展示了检索已分配给用户的应用角色的请求。</span><span class="sxs-lookup"><span data-stu-id="0478a-133">Here is an example of the request to retrieve the app roles that have been assigned to a user.</span></span>


# <a name="http"></a>[<span data-ttu-id="0478a-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="0478a-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_get_approleassignments"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/appRoleAssignments
```
# <a name="c"></a>[<span data-ttu-id="0478a-135">C#</span><span class="sxs-lookup"><span data-stu-id="0478a-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-get-approleassignments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0478a-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0478a-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-get-approleassignments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0478a-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0478a-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-get-approleassignments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0478a-138">Java</span><span class="sxs-lookup"><span data-stu-id="0478a-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-get-approleassignments-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0478a-139">响应</span><span class="sxs-lookup"><span data-stu-id="0478a-139">Response</span></span>

<span data-ttu-id="0478a-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="0478a-140">The following is an example of the response.</span></span> 

> <span data-ttu-id="0478a-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="0478a-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.appRoleAssignment",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 306

{
  "value": [
    {
      "creationTimestamp": "2016-10-19T10:37:00Z",
      "id": "id-value",
      "principalDisplayName": "principalDisplayName-value",
      "principalId": "principalId-value",
      "principalType": "principalType-value",
      "resourceDisplayName": "resourceDisplayName-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List appRoleAssignments",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->



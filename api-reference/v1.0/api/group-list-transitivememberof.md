---
title: 列表组可传递的 memberOf
description: 获取组所属的组。  此操作是可传递的，还将包括此组嵌套成员的所有组。 与获取用户的 Office 365 组不同，这将返回所有类型的组，而不只是 Office 365 组。
author: anchanda
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: a02dd7e4ae4c65132decc6f9f2887bfd91c6d9e7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42517031"
---
# <a name="list-group-transitive-memberof"></a><span data-ttu-id="2a4ee-105">列表组可传递的 memberOf</span><span class="sxs-lookup"><span data-stu-id="2a4ee-105">List group transitive memberOf</span></span>

<span data-ttu-id="2a4ee-106">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2a4ee-106">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2a4ee-107">获取组所属的组。</span><span class="sxs-lookup"><span data-stu-id="2a4ee-107">Get groups that the group is a member of.</span></span>  <span data-ttu-id="2a4ee-108">此操作是可传递的，还将包括此组嵌套成员的所有组。</span><span class="sxs-lookup"><span data-stu-id="2a4ee-108">This operation is transitive and will also include all groups that this groups is a nested member of.</span></span> <span data-ttu-id="2a4ee-109">与获取用户的 Office 365 组不同，这将返回所有类型的组，而不只是 Office 365 组。</span><span class="sxs-lookup"><span data-stu-id="2a4ee-109">Unlike getting a user's Office 365 Groups, this returns all types of groups, not just Office 365 Groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="2a4ee-110">权限</span><span class="sxs-lookup"><span data-stu-id="2a4ee-110">Permissions</span></span>

<span data-ttu-id="2a4ee-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2a4ee-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2a4ee-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="2a4ee-113">Permission type</span></span>      | <span data-ttu-id="2a4ee-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2a4ee-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2a4ee-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2a4ee-115">Delegated (work or school account)</span></span> | <span data-ttu-id="2a4ee-116">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2a4ee-116">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="2a4ee-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2a4ee-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2a4ee-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="2a4ee-118">Not supported.</span></span>    |
|<span data-ttu-id="2a4ee-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="2a4ee-119">Application</span></span> | <span data-ttu-id="2a4ee-120">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a4ee-120">Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="2a4ee-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2a4ee-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/transitiveMemberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2a4ee-122">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="2a4ee-122">Optional query parameters</span></span>
<span data-ttu-id="2a4ee-123">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="2a4ee-123">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2a4ee-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="2a4ee-124">Request headers</span></span>
| <span data-ttu-id="2a4ee-125">名称</span><span class="sxs-lookup"><span data-stu-id="2a4ee-125">Name</span></span>       | <span data-ttu-id="2a4ee-126">类型</span><span class="sxs-lookup"><span data-stu-id="2a4ee-126">Type</span></span> | <span data-ttu-id="2a4ee-127">说明</span><span class="sxs-lookup"><span data-stu-id="2a4ee-127">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="2a4ee-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="2a4ee-128">Authorization</span></span>  | <span data-ttu-id="2a4ee-129">string</span><span class="sxs-lookup"><span data-stu-id="2a4ee-129">string</span></span>  | <span data-ttu-id="2a4ee-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2a4ee-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2a4ee-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="2a4ee-132">Request body</span></span>
<span data-ttu-id="2a4ee-133">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2a4ee-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2a4ee-134">响应</span><span class="sxs-lookup"><span data-stu-id="2a4ee-134">Response</span></span>
<span data-ttu-id="2a4ee-135">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="2a4ee-135">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2a4ee-136">示例</span><span class="sxs-lookup"><span data-stu-id="2a4ee-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="2a4ee-137">请求</span><span class="sxs-lookup"><span data-stu-id="2a4ee-137">Request</span></span>
<span data-ttu-id="2a4ee-138">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="2a4ee-138">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2a4ee-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="2a4ee-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_transitivememberof"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/transitiveMemberOf
```
# <a name="c"></a>[<span data-ttu-id="2a4ee-140">C#</span><span class="sxs-lookup"><span data-stu-id="2a4ee-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-transitivememberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2a4ee-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2a4ee-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-transitivememberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2a4ee-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2a4ee-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-transitivememberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2a4ee-143">Java</span><span class="sxs-lookup"><span data-stu-id="2a4ee-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-transitivememberof-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="2a4ee-144">响应</span><span class="sxs-lookup"><span data-stu-id="2a4ee-144">Response</span></span>

<span data-ttu-id="2a4ee-145">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="2a4ee-145">The following is an example of the response.</span></span>
><span data-ttu-id="2a4ee-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="2a4ee-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
      "@odata.type": "#microsoft.graph.group",
      "id": "id-value",
      "createdDateTime": null,
      "description": "All users at the company",
      "displayName": "All Users",
      "groupTypes": [],
      "mailEnabled": false,
      "securityEnabled": true,
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List group transitive memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

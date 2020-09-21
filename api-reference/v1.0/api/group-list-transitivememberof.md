---
title: List group transitive memberOf
description: 获取组所属的组。  此操作是可传递的，还将包括此组嵌套成员的所有组。 与获取用户的 Microsoft 365 组不同，这将返回所有类型的组，而不仅仅是 Microsoft 365 组。
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: c3f698329ba11f0c8d4d68711176318fae62debf
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48057547"
---
# <a name="list-group-transitive-memberof"></a><span data-ttu-id="42ef9-105">List group transitive memberOf</span><span class="sxs-lookup"><span data-stu-id="42ef9-105">List group transitive memberOf</span></span>

<span data-ttu-id="42ef9-106">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="42ef9-106">Namespace: microsoft.graph</span></span>

<span data-ttu-id="42ef9-107">获取组所属的组。</span><span class="sxs-lookup"><span data-stu-id="42ef9-107">Get groups that the group is a member of.</span></span>  <span data-ttu-id="42ef9-108">此操作是可传递的，还将包括此组嵌套成员的所有组。</span><span class="sxs-lookup"><span data-stu-id="42ef9-108">This operation is transitive and will also include all groups that this groups is a nested member of.</span></span> <span data-ttu-id="42ef9-109">与获取用户的 Microsoft 365 组不同，这将返回所有类型的组，而不仅仅是 Microsoft 365 组。</span><span class="sxs-lookup"><span data-stu-id="42ef9-109">Unlike getting a user's Microsoft 365 groups, this returns all types of groups, not just Microsoft 365 groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="42ef9-110">权限</span><span class="sxs-lookup"><span data-stu-id="42ef9-110">Permissions</span></span>

<span data-ttu-id="42ef9-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="42ef9-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="42ef9-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="42ef9-113">Permission type</span></span>      | <span data-ttu-id="42ef9-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="42ef9-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="42ef9-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="42ef9-115">Delegated (work or school account)</span></span> | <span data-ttu-id="42ef9-116">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="42ef9-116">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="42ef9-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="42ef9-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="42ef9-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="42ef9-118">Not supported.</span></span>    |
|<span data-ttu-id="42ef9-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="42ef9-119">Application</span></span> | <span data-ttu-id="42ef9-120">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42ef9-120">Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="42ef9-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="42ef9-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/transitiveMemberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="42ef9-122">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="42ef9-122">Optional query parameters</span></span>
<span data-ttu-id="42ef9-123">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="42ef9-123">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="42ef9-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="42ef9-124">Request headers</span></span>
| <span data-ttu-id="42ef9-125">名称</span><span class="sxs-lookup"><span data-stu-id="42ef9-125">Name</span></span>       | <span data-ttu-id="42ef9-126">类型</span><span class="sxs-lookup"><span data-stu-id="42ef9-126">Type</span></span> | <span data-ttu-id="42ef9-127">说明</span><span class="sxs-lookup"><span data-stu-id="42ef9-127">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="42ef9-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="42ef9-128">Authorization</span></span>  | <span data-ttu-id="42ef9-129">string</span><span class="sxs-lookup"><span data-stu-id="42ef9-129">string</span></span>  | <span data-ttu-id="42ef9-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="42ef9-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="42ef9-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="42ef9-132">Request body</span></span>
<span data-ttu-id="42ef9-133">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="42ef9-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="42ef9-134">响应</span><span class="sxs-lookup"><span data-stu-id="42ef9-134">Response</span></span>
<span data-ttu-id="42ef9-135">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="42ef9-135">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="42ef9-136">示例</span><span class="sxs-lookup"><span data-stu-id="42ef9-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="42ef9-137">请求</span><span class="sxs-lookup"><span data-stu-id="42ef9-137">Request</span></span>
<span data-ttu-id="42ef9-138">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="42ef9-138">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="42ef9-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="42ef9-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_transitivememberof"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/transitiveMemberOf
```
# <a name="c"></a>[<span data-ttu-id="42ef9-140">C#</span><span class="sxs-lookup"><span data-stu-id="42ef9-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-transitivememberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="42ef9-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="42ef9-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-transitivememberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="42ef9-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="42ef9-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-transitivememberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="42ef9-143">Java</span><span class="sxs-lookup"><span data-stu-id="42ef9-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-transitivememberof-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="42ef9-144">响应</span><span class="sxs-lookup"><span data-stu-id="42ef9-144">Response</span></span>

<span data-ttu-id="42ef9-145">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="42ef9-145">The following is an example of the response.</span></span>
><span data-ttu-id="42ef9-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="42ef9-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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


---
title: 列表组可传递的 memberOf
description: 获取组所属的组。  此操作是可传递的, 还将包括此组嵌套成员的所有组。 与获取用户的 Office 365 组不同, 这将返回所有类型的组, 而不只是 Office 365 组。
author: anchanda
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: dedc86619253cebceb772c62206fbb9cd9bdfa87
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33613794"
---
# <a name="list-group-transitive-memberof"></a><span data-ttu-id="d4aaa-105">列表组可传递的 memberOf</span><span class="sxs-lookup"><span data-stu-id="d4aaa-105">List group transitive memberOf</span></span>

<span data-ttu-id="d4aaa-106">获取组所属的组。</span><span class="sxs-lookup"><span data-stu-id="d4aaa-106">Get groups that the group is a member of.</span></span>  <span data-ttu-id="d4aaa-107">此操作是可传递的, 还将包括此组嵌套成员的所有组。</span><span class="sxs-lookup"><span data-stu-id="d4aaa-107">This operation is transitive and will also include all groups that this groups is a nested member of.</span></span> <span data-ttu-id="d4aaa-108">与获取用户的 Office 365 组不同, 这将返回所有类型的组, 而不只是 Office 365 组。</span><span class="sxs-lookup"><span data-stu-id="d4aaa-108">Unlike getting a user's Office 365 Groups, this returns all types of groups, not just Office 365 Groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="d4aaa-109">权限</span><span class="sxs-lookup"><span data-stu-id="d4aaa-109">Permissions</span></span>

<span data-ttu-id="d4aaa-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d4aaa-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d4aaa-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="d4aaa-112">Permission type</span></span>      | <span data-ttu-id="d4aaa-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d4aaa-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d4aaa-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d4aaa-114">Delegated (work or school account)</span></span> | <span data-ttu-id="d4aaa-115">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d4aaa-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d4aaa-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d4aaa-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d4aaa-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="d4aaa-117">Not supported.</span></span>    |
|<span data-ttu-id="d4aaa-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="d4aaa-118">Application</span></span> | <span data-ttu-id="d4aaa-119">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4aaa-119">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d4aaa-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d4aaa-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/transitiveMemberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d4aaa-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d4aaa-121">Optional query parameters</span></span>
<span data-ttu-id="d4aaa-122">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="d4aaa-122">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d4aaa-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="d4aaa-123">Request headers</span></span>
| <span data-ttu-id="d4aaa-124">名称</span><span class="sxs-lookup"><span data-stu-id="d4aaa-124">Name</span></span>       | <span data-ttu-id="d4aaa-125">类型</span><span class="sxs-lookup"><span data-stu-id="d4aaa-125">Type</span></span> | <span data-ttu-id="d4aaa-126">说明</span><span class="sxs-lookup"><span data-stu-id="d4aaa-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="d4aaa-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="d4aaa-127">Authorization</span></span>  | <span data-ttu-id="d4aaa-128">string</span><span class="sxs-lookup"><span data-stu-id="d4aaa-128">string</span></span>  | <span data-ttu-id="d4aaa-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d4aaa-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d4aaa-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="d4aaa-131">Request body</span></span>
<span data-ttu-id="d4aaa-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d4aaa-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d4aaa-133">响应</span><span class="sxs-lookup"><span data-stu-id="d4aaa-133">Response</span></span>
<span data-ttu-id="d4aaa-134">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="d4aaa-134">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d4aaa-135">示例</span><span class="sxs-lookup"><span data-stu-id="d4aaa-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="d4aaa-136">请求</span><span class="sxs-lookup"><span data-stu-id="d4aaa-136">Request</span></span>
<span data-ttu-id="d4aaa-137">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d4aaa-137">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_group_transitivememberof"
}-->

```http
GET https://graph.microsoft.com/v1.0/groups/{id}/transitiveMemberOf
```

### <a name="response"></a><span data-ttu-id="d4aaa-138">响应</span><span class="sxs-lookup"><span data-stu-id="d4aaa-138">Response</span></span>

<span data-ttu-id="d4aaa-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="d4aaa-139">The following is an example of the response.</span></span>
><span data-ttu-id="d4aaa-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="d4aaa-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="d4aaa-142">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="d4aaa-142">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="d4aaa-143">语言</span><span class="sxs-lookup"><span data-stu-id="d4aaa-143">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_group_transitivememberof-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d4aaa-144">Javascript</span><span class="sxs-lookup"><span data-stu-id="d4aaa-144">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_group_transitivememberof-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List group transitive memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/group-list-transitivememberof.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/group-list-transitivememberof.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->

---
title: 列表组可传递的 memberOf
description: 获取组所属的组和管理单元。  此操作是可传递的, 还将包括此组嵌套成员的所有组。 与获取用户的 Office 365 组不同, 这将返回所有类型的组, 而不只是 Office 365 组。
localization_priority: Normal
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: f93d4e812dc4673a72d8e4aa6ed324710819a510
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35953645"
---
# <a name="list-group-transitive-memberof"></a><span data-ttu-id="bb9ea-105">列表组可传递的 memberOf</span><span class="sxs-lookup"><span data-stu-id="bb9ea-105">List group transitive memberOf</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bb9ea-106">获取组所属的组和管理单元。</span><span class="sxs-lookup"><span data-stu-id="bb9ea-106">Get groups and administrative units that the group is a member of.</span></span>  <span data-ttu-id="bb9ea-107">此操作是可传递的, 还将包括此组嵌套成员的所有组。</span><span class="sxs-lookup"><span data-stu-id="bb9ea-107">This operation is transitive and will also include all groups that this groups is a nested member of.</span></span> <span data-ttu-id="bb9ea-108">与获取用户的 Office 365 组不同, 这将返回所有类型的组, 而不只是 Office 365 组。</span><span class="sxs-lookup"><span data-stu-id="bb9ea-108">Unlike getting a user's Office 365 Groups, this returns all types of groups, not just Office 365 Groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="bb9ea-109">权限</span><span class="sxs-lookup"><span data-stu-id="bb9ea-109">Permissions</span></span>

<span data-ttu-id="bb9ea-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bb9ea-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bb9ea-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="bb9ea-112">Permission type</span></span>      | <span data-ttu-id="bb9ea-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bb9ea-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bb9ea-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bb9ea-114">Delegated (work or school account)</span></span> | <span data-ttu-id="bb9ea-115">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="bb9ea-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="bb9ea-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bb9ea-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bb9ea-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="bb9ea-117">Not supported.</span></span>    |
|<span data-ttu-id="bb9ea-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="bb9ea-118">Application</span></span> | <span data-ttu-id="bb9ea-119">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb9ea-119">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bb9ea-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bb9ea-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/transitiveMemberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bb9ea-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="bb9ea-121">Optional query parameters</span></span>
<span data-ttu-id="bb9ea-122">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="bb9ea-122">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bb9ea-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="bb9ea-123">Request headers</span></span>
| <span data-ttu-id="bb9ea-124">名称</span><span class="sxs-lookup"><span data-stu-id="bb9ea-124">Name</span></span>       | <span data-ttu-id="bb9ea-125">类型</span><span class="sxs-lookup"><span data-stu-id="bb9ea-125">Type</span></span> | <span data-ttu-id="bb9ea-126">说明</span><span class="sxs-lookup"><span data-stu-id="bb9ea-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="bb9ea-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="bb9ea-127">Authorization</span></span>  | <span data-ttu-id="bb9ea-128">string</span><span class="sxs-lookup"><span data-stu-id="bb9ea-128">string</span></span>  | <span data-ttu-id="bb9ea-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="bb9ea-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bb9ea-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="bb9ea-131">Request body</span></span>
<span data-ttu-id="bb9ea-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="bb9ea-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bb9ea-133">响应</span><span class="sxs-lookup"><span data-stu-id="bb9ea-133">Response</span></span>
<span data-ttu-id="bb9ea-134">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="bb9ea-134">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bb9ea-135">示例</span><span class="sxs-lookup"><span data-stu-id="bb9ea-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="bb9ea-136">请求</span><span class="sxs-lookup"><span data-stu-id="bb9ea-136">Request</span></span>
<span data-ttu-id="bb9ea-137">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="bb9ea-137">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="bb9ea-138">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="bb9ea-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_transitivememberof"
}-->

```http
GET https://graph.microsoft.com/beta/groups/{id}/transitiveMemberOf
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="bb9ea-139">C#</span><span class="sxs-lookup"><span data-stu-id="bb9ea-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-transitivememberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bb9ea-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="bb9ea-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-transitivememberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="bb9ea-141">目标-C</span><span class="sxs-lookup"><span data-stu-id="bb9ea-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-transitivememberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="bb9ea-142">Java</span><span class="sxs-lookup"><span data-stu-id="bb9ea-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-transitivememberof-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="bb9ea-143">响应</span><span class="sxs-lookup"><span data-stu-id="bb9ea-143">Response</span></span>

<span data-ttu-id="bb9ea-144">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="bb9ea-144">The following is an example of the response.</span></span>
><span data-ttu-id="bb9ea-145">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="bb9ea-145">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="bb9ea-146">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="bb9ea-146">All the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "List group transitive memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

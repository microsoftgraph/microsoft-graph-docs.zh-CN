---
title: 列表组可传递的 memberOf
description: 获取组所属的组和管理单元。
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 6d8907752b2350e018df879e825d38a944de3da8
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43396822"
---
# <a name="list-group-transitive-memberof"></a><span data-ttu-id="109ea-103">列表组可传递的 memberOf</span><span class="sxs-lookup"><span data-stu-id="109ea-103">List group transitive memberOf</span></span>

<span data-ttu-id="109ea-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="109ea-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="109ea-105">获取组所属的组和管理单元。</span><span class="sxs-lookup"><span data-stu-id="109ea-105">Get groups and administrative units that the group is a member of.</span></span>  <span data-ttu-id="109ea-106">此操作是可传递的，还将包括此组嵌套成员的所有组。</span><span class="sxs-lookup"><span data-stu-id="109ea-106">This operation is transitive and will also include all groups that this groups is a nested member of.</span></span> <span data-ttu-id="109ea-107">与获取用户的 Office 365 组不同，这将返回所有类型的组，而不只是 Office 365 组。</span><span class="sxs-lookup"><span data-stu-id="109ea-107">Unlike getting a user's Office 365 Groups, this returns all types of groups, not just Office 365 Groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="109ea-108">权限</span><span class="sxs-lookup"><span data-stu-id="109ea-108">Permissions</span></span>

<span data-ttu-id="109ea-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="109ea-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="109ea-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="109ea-111">Permission type</span></span>      | <span data-ttu-id="109ea-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="109ea-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="109ea-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="109ea-113">Delegated (work or school account)</span></span> | <span data-ttu-id="109ea-114">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="109ea-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="109ea-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="109ea-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="109ea-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="109ea-116">Not supported.</span></span>    |
|<span data-ttu-id="109ea-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="109ea-117">Application</span></span> | <span data-ttu-id="109ea-118">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="109ea-118">Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="109ea-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="109ea-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/transitiveMemberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="109ea-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="109ea-120">Optional query parameters</span></span>
<span data-ttu-id="109ea-121">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="109ea-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="109ea-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="109ea-122">Request headers</span></span>
| <span data-ttu-id="109ea-123">名称</span><span class="sxs-lookup"><span data-stu-id="109ea-123">Name</span></span>       | <span data-ttu-id="109ea-124">类型</span><span class="sxs-lookup"><span data-stu-id="109ea-124">Type</span></span> | <span data-ttu-id="109ea-125">说明</span><span class="sxs-lookup"><span data-stu-id="109ea-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="109ea-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="109ea-126">Authorization</span></span>  | <span data-ttu-id="109ea-127">string</span><span class="sxs-lookup"><span data-stu-id="109ea-127">string</span></span>  | <span data-ttu-id="109ea-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="109ea-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="109ea-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="109ea-130">Request body</span></span>
<span data-ttu-id="109ea-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="109ea-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="109ea-132">响应</span><span class="sxs-lookup"><span data-stu-id="109ea-132">Response</span></span>
<span data-ttu-id="109ea-133">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="109ea-133">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="109ea-134">示例</span><span class="sxs-lookup"><span data-stu-id="109ea-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="109ea-135">请求</span><span class="sxs-lookup"><span data-stu-id="109ea-135">Request</span></span>
<span data-ttu-id="109ea-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="109ea-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="109ea-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="109ea-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_transitivememberof"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/transitiveMemberOf
```
# <a name="c"></a>[<span data-ttu-id="109ea-138">C#</span><span class="sxs-lookup"><span data-stu-id="109ea-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-transitivememberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="109ea-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="109ea-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-transitivememberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="109ea-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="109ea-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-transitivememberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="109ea-141">响应</span><span class="sxs-lookup"><span data-stu-id="109ea-141">Response</span></span>

<span data-ttu-id="109ea-142">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="109ea-142">The following is an example of the response.</span></span>
><span data-ttu-id="109ea-143">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="109ea-143">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="109ea-144">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="109ea-144">All the properties will be returned from an actual call.</span></span>
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

---
title: 列出用户可传递的 memberOf
description: 获取用户所属的组和目录角色。 此 API 请求是可传递的, 并且还将返回用户是其嵌套成员的所有组。
author: anchanda
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: ac0819c970fa1e2c5e17fda29fd68bb35105f01b
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35274002"
---
# <a name="list-user-transitive-memberof"></a><span data-ttu-id="802ef-104">列出用户可传递的 memberOf</span><span class="sxs-lookup"><span data-stu-id="802ef-104">List user transitive memberOf</span></span>

<span data-ttu-id="802ef-105">获取用户所属的组和目录角色。</span><span class="sxs-lookup"><span data-stu-id="802ef-105">Get groups, directory roles that the user is a member of.</span></span> <span data-ttu-id="802ef-106">此 API 请求是可传递的, 并且还将返回用户是其嵌套成员的所有组。</span><span class="sxs-lookup"><span data-stu-id="802ef-106">This API request is transitive, and will also return all groups the user is a nested member of.</span></span>

## <a name="permissions"></a><span data-ttu-id="802ef-107">权限</span><span class="sxs-lookup"><span data-stu-id="802ef-107">Permissions</span></span>

<span data-ttu-id="802ef-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="802ef-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="802ef-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="802ef-110">Permission type</span></span>      | <span data-ttu-id="802ef-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="802ef-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="802ef-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="802ef-112">Delegated (work or school account)</span></span> | <span data-ttu-id="802ef-113">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="802ef-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="802ef-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="802ef-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="802ef-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="802ef-115">Not supported.</span></span>    |
|<span data-ttu-id="802ef-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="802ef-116">Application</span></span> | <span data-ttu-id="802ef-117">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="802ef-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="802ef-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="802ef-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /users/{id | userPrincipalName}/transitiveMemberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="802ef-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="802ef-119">Optional query parameters</span></span>

<span data-ttu-id="802ef-120">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="802ef-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="802ef-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="802ef-121">Request headers</span></span>

| <span data-ttu-id="802ef-122">标头</span><span class="sxs-lookup"><span data-stu-id="802ef-122">Header</span></span>       | <span data-ttu-id="802ef-123">值</span><span class="sxs-lookup"><span data-stu-id="802ef-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="802ef-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="802ef-124">Authorization</span></span>  | <span data-ttu-id="802ef-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="802ef-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="802ef-127">接受</span><span class="sxs-lookup"><span data-stu-id="802ef-127">Accept</span></span>  | <span data-ttu-id="802ef-128">application/json</span><span class="sxs-lookup"><span data-stu-id="802ef-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="802ef-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="802ef-129">Request body</span></span>

<span data-ttu-id="802ef-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="802ef-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="802ef-131">响应</span><span class="sxs-lookup"><span data-stu-id="802ef-131">Response</span></span>

<span data-ttu-id="802ef-132">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="802ef-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="802ef-133">示例</span><span class="sxs-lookup"><span data-stu-id="802ef-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="802ef-134">请求</span><span class="sxs-lookup"><span data-stu-id="802ef-134">Request</span></span>

<span data-ttu-id="802ef-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="802ef-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_transitivememberof"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/transitiveMemberOf
```

### <a name="response"></a><span data-ttu-id="802ef-136">响应</span><span class="sxs-lookup"><span data-stu-id="802ef-136">Response</span></span>

<span data-ttu-id="802ef-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="802ef-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="802ef-140">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="802ef-140">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="802ef-141">C#</span><span class="sxs-lookup"><span data-stu-id="802ef-141">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_transitivememberof-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="802ef-142">Javascript</span><span class="sxs-lookup"><span data-stu-id="802ef-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_transitivememberof-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="802ef-143">目标-C</span><span class="sxs-lookup"><span data-stu-id="802ef-143">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_transitivememberof-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List transitiveMsemberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/user-list-transitivememberof.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/user-list-transitivememberof.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/user-list-transitivememberof.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->

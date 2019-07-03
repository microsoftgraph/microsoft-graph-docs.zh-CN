---
title: 列出用户可传递的 memberOf
description: 获取用户所属的组和目录角色。 此 API 请求是可传递的, 并且还将返回用户是其嵌套成员的所有组。
author: anchanda
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: f0ef5e9dc32d3109095bee58b95a19eba46d83c8
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35460180"
---
# <a name="list-user-transitive-memberof"></a><span data-ttu-id="14d40-104">列出用户可传递的 memberOf</span><span class="sxs-lookup"><span data-stu-id="14d40-104">List user transitive memberOf</span></span>

<span data-ttu-id="14d40-105">获取用户所属的组和目录角色。</span><span class="sxs-lookup"><span data-stu-id="14d40-105">Get groups, directory roles that the user is a member of.</span></span> <span data-ttu-id="14d40-106">此 API 请求是可传递的, 并且还将返回用户是其嵌套成员的所有组。</span><span class="sxs-lookup"><span data-stu-id="14d40-106">This API request is transitive, and will also return all groups the user is a nested member of.</span></span>

## <a name="permissions"></a><span data-ttu-id="14d40-107">权限</span><span class="sxs-lookup"><span data-stu-id="14d40-107">Permissions</span></span>

<span data-ttu-id="14d40-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="14d40-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="14d40-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="14d40-110">Permission type</span></span>      | <span data-ttu-id="14d40-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="14d40-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="14d40-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="14d40-112">Delegated (work or school account)</span></span> | <span data-ttu-id="14d40-113">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="14d40-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="14d40-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="14d40-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="14d40-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="14d40-115">Not supported.</span></span>    |
|<span data-ttu-id="14d40-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="14d40-116">Application</span></span> | <span data-ttu-id="14d40-117">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14d40-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="14d40-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="14d40-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /users/{id | userPrincipalName}/transitiveMemberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="14d40-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="14d40-119">Optional query parameters</span></span>

<span data-ttu-id="14d40-120">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="14d40-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="14d40-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="14d40-121">Request headers</span></span>

| <span data-ttu-id="14d40-122">标头</span><span class="sxs-lookup"><span data-stu-id="14d40-122">Header</span></span>       | <span data-ttu-id="14d40-123">值</span><span class="sxs-lookup"><span data-stu-id="14d40-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="14d40-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="14d40-124">Authorization</span></span>  | <span data-ttu-id="14d40-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="14d40-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="14d40-127">接受</span><span class="sxs-lookup"><span data-stu-id="14d40-127">Accept</span></span>  | <span data-ttu-id="14d40-128">application/json</span><span class="sxs-lookup"><span data-stu-id="14d40-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="14d40-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="14d40-129">Request body</span></span>

<span data-ttu-id="14d40-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="14d40-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="14d40-131">响应</span><span class="sxs-lookup"><span data-stu-id="14d40-131">Response</span></span>

<span data-ttu-id="14d40-132">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="14d40-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="14d40-133">示例</span><span class="sxs-lookup"><span data-stu-id="14d40-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="14d40-134">请求</span><span class="sxs-lookup"><span data-stu-id="14d40-134">Request</span></span>

<span data-ttu-id="14d40-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="14d40-135">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="14d40-136">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="14d40-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_transitivememberof"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/transitiveMemberOf
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="14d40-137">C#</span><span class="sxs-lookup"><span data-stu-id="14d40-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-transitivememberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="14d40-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="14d40-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-transitivememberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="14d40-139">目标-C</span><span class="sxs-lookup"><span data-stu-id="14d40-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-transitivememberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="14d40-140">响应</span><span class="sxs-lookup"><span data-stu-id="14d40-140">Response</span></span>

<span data-ttu-id="14d40-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="14d40-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
  "description": "List transitiveMsemberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

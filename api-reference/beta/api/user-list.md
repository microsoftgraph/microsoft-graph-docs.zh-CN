---
title: 列出用户
description: 检索用户对象列表。
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0a49e86b8aaccbf87e8c80f69659b648b3186405
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35456783"
---
# <a name="list-users"></a><span data-ttu-id="06a55-103">列出用户</span><span class="sxs-lookup"><span data-stu-id="06a55-103">List users</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="06a55-104">检索 user 对象列表。</span><span class="sxs-lookup"><span data-stu-id="06a55-104">Retrieve a list of user objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="06a55-105">权限</span><span class="sxs-lookup"><span data-stu-id="06a55-105">Permissions</span></span>

<span data-ttu-id="06a55-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="06a55-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="06a55-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="06a55-108">Permission type</span></span>      | <span data-ttu-id="06a55-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="06a55-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="06a55-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="06a55-110">Delegated (work or school account)</span></span> | <span data-ttu-id="06a55-111">User.ReadBasic.All、User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="06a55-111">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="06a55-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="06a55-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="06a55-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="06a55-113">Not supported.</span></span>    |
|<span data-ttu-id="06a55-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="06a55-114">Application</span></span> | <span data-ttu-id="06a55-115">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06a55-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="06a55-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="06a55-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users
```

## <a name="optional-query-parameters"></a><span data-ttu-id="06a55-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="06a55-117">Optional query parameters</span></span>

<span data-ttu-id="06a55-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="06a55-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="06a55-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="06a55-119">Request headers</span></span>
| <span data-ttu-id="06a55-120">标头</span><span class="sxs-lookup"><span data-stu-id="06a55-120">Header</span></span>        | <span data-ttu-id="06a55-121">值</span><span class="sxs-lookup"><span data-stu-id="06a55-121">Value</span></span>                      |
|:--------------|:---------------------------|
| <span data-ttu-id="06a55-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="06a55-122">Authorization</span></span> | <span data-ttu-id="06a55-123">Bearer {token}（必需）</span><span class="sxs-lookup"><span data-stu-id="06a55-123">Bearer {token} (required)</span></span>  |
| <span data-ttu-id="06a55-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="06a55-124">Content-Type</span></span>  | <span data-ttu-id="06a55-125">application/json</span><span class="sxs-lookup"><span data-stu-id="06a55-125">application/json</span></span>           |

## <a name="request-body"></a><span data-ttu-id="06a55-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="06a55-126">Request body</span></span>

<span data-ttu-id="06a55-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="06a55-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="06a55-128">响应</span><span class="sxs-lookup"><span data-stu-id="06a55-128">Response</span></span>

<span data-ttu-id="06a55-129">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [user](../resources/user.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="06a55-129">If successful, this method returns a `200 OK` response code and collection of [user](../resources/user.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="06a55-130">示例</span><span class="sxs-lookup"><span data-stu-id="06a55-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="06a55-131">请求</span><span class="sxs-lookup"><span data-stu-id="06a55-131">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="06a55-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="06a55-132">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_users"
}-->
```http
GET https://graph.microsoft.com/beta/users
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="06a55-133">C#</span><span class="sxs-lookup"><span data-stu-id="06a55-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="06a55-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="06a55-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="06a55-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="06a55-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="06a55-136">响应</span><span class="sxs-lookup"><span data-stu-id="06a55-136">Response</span></span>

<span data-ttu-id="06a55-137">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="06a55-137">Here is an example of the response.</span></span> <span data-ttu-id="06a55-138">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="06a55-138">Note: The response object shown here may be truncated for brevity.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 608

{
  "value": [
    {
      "businessPhones": [
        "businessPhones-value"
      ],
      "displayName": "displayName-value",
      "givenName": "givenName-value",
      "jobTitle": "jobTitle-value",
      "mail": "mail-value",
      "mobilePhone": "mobilePhone-value",
      "officeLocation": "officeLocation-value",
      "preferredLanguage": "preferredLanguage-value",
      "surname": "surname-value",
      "userPrincipalName": "userPrincipalName-value",
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
  "description": "List users",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

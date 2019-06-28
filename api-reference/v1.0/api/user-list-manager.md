---
title: 列出经理
description: 获取用户的经理。 返回指定为用户经理的用户或联系人。
localization_priority: Priority
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 12d20a0738e09841b997a332028d0c8dda283aff
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35269564"
---
# <a name="list-manager"></a><span data-ttu-id="e6a1b-104">列出经理</span><span class="sxs-lookup"><span data-stu-id="e6a1b-104">List manager</span></span>

<span data-ttu-id="e6a1b-105">获取用户的经理。</span><span class="sxs-lookup"><span data-stu-id="e6a1b-105">Get user's manager.</span></span> <span data-ttu-id="e6a1b-106">返回指定为用户经理的用户或联系人。</span><span class="sxs-lookup"><span data-stu-id="e6a1b-106">Returns the user or contact assigned as the user's manager.</span></span>
## <a name="permissions"></a><span data-ttu-id="e6a1b-107">权限</span><span class="sxs-lookup"><span data-stu-id="e6a1b-107">Permissions</span></span>
<span data-ttu-id="e6a1b-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e6a1b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e6a1b-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="e6a1b-110">Permission type</span></span>      | <span data-ttu-id="e6a1b-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e6a1b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e6a1b-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e6a1b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e6a1b-113">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e6a1b-113">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e6a1b-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e6a1b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e6a1b-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="e6a1b-115">Not supported.</span></span>    |
|<span data-ttu-id="e6a1b-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="e6a1b-116">Application</span></span> | <span data-ttu-id="e6a1b-117">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e6a1b-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e6a1b-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e6a1b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/manager
GET /users/{id | userPrincipalName}/manager
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e6a1b-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="e6a1b-119">Optional query parameters</span></span>
<span data-ttu-id="e6a1b-120">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="e6a1b-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="e6a1b-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="e6a1b-121">Request headers</span></span>
| <span data-ttu-id="e6a1b-122">标头</span><span class="sxs-lookup"><span data-stu-id="e6a1b-122">Header</span></span>       | <span data-ttu-id="e6a1b-123">值</span><span class="sxs-lookup"><span data-stu-id="e6a1b-123">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="e6a1b-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="e6a1b-124">Authorization</span></span>  | <span data-ttu-id="e6a1b-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e6a1b-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e6a1b-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e6a1b-127">Content-Type</span></span>   | <span data-ttu-id="e6a1b-128">application/json</span><span class="sxs-lookup"><span data-stu-id="e6a1b-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e6a1b-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="e6a1b-129">Request body</span></span>
<span data-ttu-id="e6a1b-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e6a1b-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e6a1b-131">响应</span><span class="sxs-lookup"><span data-stu-id="e6a1b-131">Response</span></span>

<span data-ttu-id="e6a1b-132">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e6a1b-132">If successful, this method returns a `200 OK` response code and a [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e6a1b-133">示例</span><span class="sxs-lookup"><span data-stu-id="e6a1b-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e6a1b-134">请求</span><span class="sxs-lookup"><span data-stu-id="e6a1b-134">Request</span></span>
<span data-ttu-id="e6a1b-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e6a1b-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_manager"
}-->
```http
GET https://graph.microsoft.com/v1.0/users/{id|userPrincipalName}/manager
```
##### <a name="response"></a><span data-ttu-id="e6a1b-136">响应</span><span class="sxs-lookup"><span data-stu-id="e6a1b-136">Response</span></span>
<span data-ttu-id="e6a1b-137">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="e6a1b-137">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": false
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "objectType": "User",
  "id": "111048d2-2761-4347-b978-07354283363b",
  "accountEnabled": true,
  "city": "San Diego",
  "country": "United States",
  "department": "Sales & Marketing",
  "displayName": "Sara Davis",
  "givenName": "Sara",
  "jobTitle": "Finance VP",
  "mail": "SaraD@contoso.onmicrosoft.com",
  "mailNickname": "SaraD",
  "state": "CA",
  "streetAddress": "9256 Towne Center Dr., Suite 400",
  "surname": "Davis",
  "usageLocation": "US",
  "userPrincipalName": "SaraD@contoso.onmicrosoft.com"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="e6a1b-138">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="e6a1b-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="e6a1b-139">C#</span><span class="sxs-lookup"><span data-stu-id="e6a1b-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_manager-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e6a1b-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="e6a1b-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_manager-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="e6a1b-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e6a1b-141">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_manager-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List directReports",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/user-list-manager.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/user-list-manager.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/user-list-manager.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->

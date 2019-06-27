---
title: 列出 directReports
description: 获取用户的直接下属。 返回指定此用户作为经理的用户和联系人。
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 143c92f1b30eef96569b8fa3b9d669d90b3ebd2d
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35270180"
---
# <a name="list-directreports"></a><span data-ttu-id="be961-104">列出 directReports</span><span class="sxs-lookup"><span data-stu-id="be961-104">List directReports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="be961-105">获取用户的直接下属。</span><span class="sxs-lookup"><span data-stu-id="be961-105">Get user's direct reports.</span></span> <span data-ttu-id="be961-106">返回指定此用户作为经理的用户和联系人。</span><span class="sxs-lookup"><span data-stu-id="be961-106">Returns the users and contacts for whom this user is assigned as manager.</span></span>
## <a name="permissions"></a><span data-ttu-id="be961-107">权限</span><span class="sxs-lookup"><span data-stu-id="be961-107">Permissions</span></span>
<span data-ttu-id="be961-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="be961-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="be961-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="be961-110">Permission type</span></span>      | <span data-ttu-id="be961-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="be961-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="be961-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="be961-112">Delegated (work or school account)</span></span> | <span data-ttu-id="be961-113">User.Read、User.ReadWrite、User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="be961-113">User.Read, User.ReadWrite, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="be961-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="be961-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="be961-115">User.Read、User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="be961-115">User.Read, User.ReadWrite</span></span>    |
|<span data-ttu-id="be961-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="be961-116">Application</span></span> | <span data-ttu-id="be961-117">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be961-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="be961-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="be961-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/directReports
GET /users/{id | userPrincipalName}/directReports
```
## <a name="optional-query-parameters"></a><span data-ttu-id="be961-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="be961-119">Optional query parameters</span></span>
<span data-ttu-id="be961-120">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="be961-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="be961-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="be961-121">Request headers</span></span>
| <span data-ttu-id="be961-122">标头</span><span class="sxs-lookup"><span data-stu-id="be961-122">Header</span></span>       | <span data-ttu-id="be961-123">值</span><span class="sxs-lookup"><span data-stu-id="be961-123">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="be961-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="be961-124">Authorization</span></span>  | <span data-ttu-id="be961-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="be961-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="be961-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="be961-127">Content-Type</span></span>   | <span data-ttu-id="be961-128">application/json</span><span class="sxs-lookup"><span data-stu-id="be961-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="be961-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="be961-129">Request body</span></span>
<span data-ttu-id="be961-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="be961-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="be961-131">响应</span><span class="sxs-lookup"><span data-stu-id="be961-131">Response</span></span>

<span data-ttu-id="be961-132">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="be961-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="be961-133">示例</span><span class="sxs-lookup"><span data-stu-id="be961-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="be961-134">请求</span><span class="sxs-lookup"><span data-stu-id="be961-134">Request</span></span>
<span data-ttu-id="be961-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="be961-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_directreports"
}-->
```http
GET https://graph.microsoft.com/beta/me/directReports
```
##### <a name="response"></a><span data-ttu-id="be961-136">响应</span><span class="sxs-lookup"><span data-stu-id="be961-136">Response</span></span>
<span data-ttu-id="be961-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="be961-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="be961-140">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="be961-140">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="be961-141">C#</span><span class="sxs-lookup"><span data-stu-id="be961-141">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_directreports-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="be961-142">Javascript</span><span class="sxs-lookup"><span data-stu-id="be961-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_directreports-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="be961-143">目标-C</span><span class="sxs-lookup"><span data-stu-id="be961-143">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_directreports-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List directReports",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/user-list-directreports.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/user-list-directreports.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/user-list-directreports.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->

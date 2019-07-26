---
title: 列出 directReports
description: 获取用户的直接下属。 返回指定此用户作为经理的用户和联系人。
localization_priority: Priority
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 7c9549fe4dfc5c91ec4cdc8278ffbeb8165a3b3a
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35888894"
---
# <a name="list-directreports"></a><span data-ttu-id="33824-104">列出 directReports</span><span class="sxs-lookup"><span data-stu-id="33824-104">List directReports</span></span>

<span data-ttu-id="33824-105">获取用户的直接下属。</span><span class="sxs-lookup"><span data-stu-id="33824-105">Get user's direct reports.</span></span> <span data-ttu-id="33824-106">返回指定此用户作为经理的用户和联系人。</span><span class="sxs-lookup"><span data-stu-id="33824-106">Returns the users and contacts for whom this user is assigned as manager.</span></span>
## <a name="permissions"></a><span data-ttu-id="33824-107">权限</span><span class="sxs-lookup"><span data-stu-id="33824-107">Permissions</span></span>
<span data-ttu-id="33824-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="33824-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="33824-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="33824-110">Permission type</span></span>      | <span data-ttu-id="33824-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="33824-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="33824-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="33824-112">Delegated (work or school account)</span></span> | <span data-ttu-id="33824-113">User.Read、User.ReadWrite、User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="33824-113">User.Read, User.ReadWrite, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="33824-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="33824-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="33824-115">User.Read、User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="33824-115">User.Read, User.ReadWrite</span></span>    |
|<span data-ttu-id="33824-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="33824-116">Application</span></span> | <span data-ttu-id="33824-117">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="33824-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="33824-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="33824-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/directReports
GET /users/{id | userPrincipalName}/directReports
```
## <a name="optional-query-parameters"></a><span data-ttu-id="33824-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="33824-119">Optional query parameters</span></span>
<span data-ttu-id="33824-120">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="33824-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="33824-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="33824-121">Request headers</span></span>
| <span data-ttu-id="33824-122">标头</span><span class="sxs-lookup"><span data-stu-id="33824-122">Header</span></span>       | <span data-ttu-id="33824-123">值</span><span class="sxs-lookup"><span data-stu-id="33824-123">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="33824-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="33824-124">Authorization</span></span>  | <span data-ttu-id="33824-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="33824-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="33824-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="33824-127">Content-Type</span></span>   | <span data-ttu-id="33824-128">application/json</span><span class="sxs-lookup"><span data-stu-id="33824-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="33824-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="33824-129">Request body</span></span>
<span data-ttu-id="33824-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="33824-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="33824-131">响应</span><span class="sxs-lookup"><span data-stu-id="33824-131">Response</span></span>

<span data-ttu-id="33824-132">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="33824-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="33824-133">示例</span><span class="sxs-lookup"><span data-stu-id="33824-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="33824-134">请求</span><span class="sxs-lookup"><span data-stu-id="33824-134">Request</span></span>
<span data-ttu-id="33824-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="33824-135">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="33824-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="33824-136">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directreports"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/directReports
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="33824-137">C#</span><span class="sxs-lookup"><span data-stu-id="33824-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directreports-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="33824-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="33824-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directreports-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="33824-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="33824-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directreports-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="33824-140">Java</span><span class="sxs-lookup"><span data-stu-id="33824-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-directreports-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="33824-141">响应</span><span class="sxs-lookup"><span data-stu-id="33824-141">Response</span></span>
<span data-ttu-id="33824-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="33824-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List directReports",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

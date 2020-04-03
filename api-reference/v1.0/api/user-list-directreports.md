---
title: 列出 directReports
description: 获取用户的直接下属。
localization_priority: Priority
author: krbain
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 90ea3bad86307f1172869f72a311238c4ee43eaa
ms.sourcegitcommit: d6386c5d4bb8917132c3f6c4de945487939b7fb7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2020
ms.locfileid: "43108842"
---
# <a name="list-directreports"></a><span data-ttu-id="696da-103">列出 directReports</span><span class="sxs-lookup"><span data-stu-id="696da-103">List directReports</span></span>

<span data-ttu-id="696da-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="696da-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="696da-105">获取用户的直接下属。</span><span class="sxs-lookup"><span data-stu-id="696da-105">Get a user's direct reports.</span></span>

## <a name="permissions"></a><span data-ttu-id="696da-106">权限</span><span class="sxs-lookup"><span data-stu-id="696da-106">Permissions</span></span>
<span data-ttu-id="696da-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="696da-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="696da-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="696da-109">Permission type</span></span>      | <span data-ttu-id="696da-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="696da-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="696da-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="696da-111">Delegated (work or school account)</span></span> | <span data-ttu-id="696da-112">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="696da-112">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="696da-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="696da-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="696da-114">不支持</span><span class="sxs-lookup"><span data-stu-id="696da-114">Not supported</span></span> |
|<span data-ttu-id="696da-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="696da-115">Application</span></span> | <span data-ttu-id="696da-116">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="696da-116">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="696da-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="696da-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/directReports
GET /users/{id | userPrincipalName}/directReports
```
## <a name="optional-query-parameters"></a><span data-ttu-id="696da-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="696da-118">Optional query parameters</span></span>
<span data-ttu-id="696da-119">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="696da-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="696da-120">请求头</span><span class="sxs-lookup"><span data-stu-id="696da-120">Request headers</span></span>
| <span data-ttu-id="696da-121">标头</span><span class="sxs-lookup"><span data-stu-id="696da-121">Header</span></span>       | <span data-ttu-id="696da-122">值</span><span class="sxs-lookup"><span data-stu-id="696da-122">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="696da-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="696da-123">Authorization</span></span>  | <span data-ttu-id="696da-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="696da-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="696da-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="696da-126">Content-Type</span></span>   | <span data-ttu-id="696da-127">application/json</span><span class="sxs-lookup"><span data-stu-id="696da-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="696da-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="696da-128">Request body</span></span>
<span data-ttu-id="696da-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="696da-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="696da-130">响应</span><span class="sxs-lookup"><span data-stu-id="696da-130">Response</span></span>

<span data-ttu-id="696da-131">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="696da-131">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="696da-132">示例</span><span class="sxs-lookup"><span data-stu-id="696da-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="696da-133">请求</span><span class="sxs-lookup"><span data-stu-id="696da-133">Request</span></span>
<span data-ttu-id="696da-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="696da-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="696da-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="696da-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directreports"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/directReports
```
# <a name="c"></a>[<span data-ttu-id="696da-136">C#</span><span class="sxs-lookup"><span data-stu-id="696da-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directreports-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="696da-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="696da-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directreports-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="696da-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="696da-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directreports-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="696da-139">Java</span><span class="sxs-lookup"><span data-stu-id="696da-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-directreports-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="696da-140">响应</span><span class="sxs-lookup"><span data-stu-id="696da-140">Response</span></span>
<span data-ttu-id="696da-141">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="696da-141">Here is an example of the response.</span></span> 

><span data-ttu-id="696da-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="696da-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

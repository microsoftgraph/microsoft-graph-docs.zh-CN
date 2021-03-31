---
title: 列出 directReports
description: 获取用户的直接下属。
localization_priority: Priority
author: jpettere
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 17e2dd9396da3ae572e883250514b26fd3ba7c21
ms.sourcegitcommit: 17f1c9cff2e59049b894db32435af02e4ae32a70
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2021
ms.locfileid: "51472077"
---
# <a name="list-directreports"></a><span data-ttu-id="0810e-103">列出 directReports</span><span class="sxs-lookup"><span data-stu-id="0810e-103">List directReports</span></span>

<span data-ttu-id="0810e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0810e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0810e-105">获取用户的直接下属。</span><span class="sxs-lookup"><span data-stu-id="0810e-105">Get a user's direct reports.</span></span>

## <a name="permissions"></a><span data-ttu-id="0810e-106">权限</span><span class="sxs-lookup"><span data-stu-id="0810e-106">Permissions</span></span>
<span data-ttu-id="0810e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0810e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0810e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="0810e-109">Permission type</span></span>      | <span data-ttu-id="0810e-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0810e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0810e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0810e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0810e-112">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0810e-112">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="0810e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0810e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0810e-114">不支持</span><span class="sxs-lookup"><span data-stu-id="0810e-114">Not supported</span></span> |
|<span data-ttu-id="0810e-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="0810e-115">Application</span></span> | <span data-ttu-id="0810e-116">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0810e-116">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="0810e-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0810e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/directReports
GET /users/{id | userPrincipalName}/directReports
```
## <a name="optional-query-parameters"></a><span data-ttu-id="0810e-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="0810e-118">Optional query parameters</span></span>
<span data-ttu-id="0810e-119">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="0810e-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0810e-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="0810e-120">Request headers</span></span>
| <span data-ttu-id="0810e-121">标头</span><span class="sxs-lookup"><span data-stu-id="0810e-121">Header</span></span>       | <span data-ttu-id="0810e-122">值</span><span class="sxs-lookup"><span data-stu-id="0810e-122">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="0810e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0810e-123">Authorization</span></span>  | <span data-ttu-id="0810e-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0810e-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="0810e-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0810e-126">Content-Type</span></span>   | <span data-ttu-id="0810e-127">application/json</span><span class="sxs-lookup"><span data-stu-id="0810e-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0810e-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="0810e-128">Request body</span></span>
<span data-ttu-id="0810e-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0810e-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0810e-130">响应</span><span class="sxs-lookup"><span data-stu-id="0810e-130">Response</span></span>

<span data-ttu-id="0810e-131">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="0810e-131">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0810e-132">示例</span><span class="sxs-lookup"><span data-stu-id="0810e-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="0810e-133">请求</span><span class="sxs-lookup"><span data-stu-id="0810e-133">Request</span></span>
<span data-ttu-id="0810e-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0810e-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0810e-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="0810e-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directreports"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/directReports
```
# <a name="c"></a>[<span data-ttu-id="0810e-136">C#</span><span class="sxs-lookup"><span data-stu-id="0810e-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directreports-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0810e-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0810e-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directreports-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0810e-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0810e-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directreports-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0810e-139">Java</span><span class="sxs-lookup"><span data-stu-id="0810e-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-directreports-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="0810e-140">响应</span><span class="sxs-lookup"><span data-stu-id="0810e-140">Response</span></span>
<span data-ttu-id="0810e-141">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="0810e-141">Here is an example of the response.</span></span> 

><span data-ttu-id="0810e-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="0810e-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
      "id": "a97733ce-92a4-4e7e-8d45-8e1f3e6a69d8"
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


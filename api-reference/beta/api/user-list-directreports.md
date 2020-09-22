---
title: 列出 directReports
description: 获取用户的直接下属。
localization_priority: Normal
author: krbain
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: c0d72cc416d7487330e6309931e5e5a3863f94e6
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48016945"
---
# <a name="list-directreports"></a><span data-ttu-id="e96f3-103">列出 directReports</span><span class="sxs-lookup"><span data-stu-id="e96f3-103">List directReports</span></span>

<span data-ttu-id="e96f3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e96f3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e96f3-105">获取用户的直接下属。</span><span class="sxs-lookup"><span data-stu-id="e96f3-105">Get a user's direct reports.</span></span> <span data-ttu-id="e96f3-106">返回指定此用户作为经理的用户和联系人。</span><span class="sxs-lookup"><span data-stu-id="e96f3-106">Returns the users and contacts for whom this user is assigned as manager.</span></span>

## <a name="permissions"></a><span data-ttu-id="e96f3-107">权限</span><span class="sxs-lookup"><span data-stu-id="e96f3-107">Permissions</span></span>
<span data-ttu-id="e96f3-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e96f3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e96f3-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="e96f3-110">Permission type</span></span>      | <span data-ttu-id="e96f3-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e96f3-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e96f3-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e96f3-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e96f3-113">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e96f3-113">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="e96f3-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e96f3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e96f3-115">不支持</span><span class="sxs-lookup"><span data-stu-id="e96f3-115">Not supported</span></span> |
|<span data-ttu-id="e96f3-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="e96f3-116">Application</span></span> | <span data-ttu-id="e96f3-117">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e96f3-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="e96f3-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e96f3-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/directReports
GET /users/{id | userPrincipalName}/directReports
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e96f3-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="e96f3-119">Optional query parameters</span></span>
<span data-ttu-id="e96f3-120">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="e96f3-120">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="e96f3-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="e96f3-121">Request headers</span></span>
| <span data-ttu-id="e96f3-122">标头</span><span class="sxs-lookup"><span data-stu-id="e96f3-122">Header</span></span>       | <span data-ttu-id="e96f3-123">值</span><span class="sxs-lookup"><span data-stu-id="e96f3-123">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="e96f3-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="e96f3-124">Authorization</span></span>  | <span data-ttu-id="e96f3-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e96f3-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e96f3-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e96f3-127">Content-Type</span></span>   | <span data-ttu-id="e96f3-128">application/json</span><span class="sxs-lookup"><span data-stu-id="e96f3-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e96f3-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="e96f3-129">Request body</span></span>
<span data-ttu-id="e96f3-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e96f3-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e96f3-131">响应</span><span class="sxs-lookup"><span data-stu-id="e96f3-131">Response</span></span>

<span data-ttu-id="e96f3-132">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="e96f3-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e96f3-133">示例</span><span class="sxs-lookup"><span data-stu-id="e96f3-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e96f3-134">请求</span><span class="sxs-lookup"><span data-stu-id="e96f3-134">Request</span></span>
<span data-ttu-id="e96f3-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e96f3-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e96f3-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="e96f3-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directreports"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/directReports
```
# <a name="c"></a>[<span data-ttu-id="e96f3-137">C#</span><span class="sxs-lookup"><span data-stu-id="e96f3-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directreports-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e96f3-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e96f3-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directreports-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e96f3-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e96f3-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directreports-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="e96f3-140">响应</span><span class="sxs-lookup"><span data-stu-id="e96f3-140">Response</span></span>
<span data-ttu-id="e96f3-141">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="e96f3-141">Here is an example of the response.</span></span> 

><span data-ttu-id="e96f3-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="e96f3-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "List directReports",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->



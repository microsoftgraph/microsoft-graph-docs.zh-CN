---
title: 列出 rejectedSender
description: '获取此组的“遭拒的发件人”列表中的用户或组列表。 '
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: b4794c7b2d16f51584ff0a5e8b60c75bfe979df6
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052311"
---
# <a name="list-rejectedsenders"></a><span data-ttu-id="0706e-103">列出 rejectedSender</span><span class="sxs-lookup"><span data-stu-id="0706e-103">List rejectedSenders</span></span>

<span data-ttu-id="0706e-104">命名空间：microsoft.graph 获取此组的拒绝发件人列表中的用户或组列表。</span><span class="sxs-lookup"><span data-stu-id="0706e-104">Namespace: microsoft.graph Get a list of users or groups that are in the rejected-senders list for this group.</span></span> 

<span data-ttu-id="0706e-p101">已拒绝的发件人列表中的用户无法发布到组对话（在 GET 请求 URL 中标识）。确保未在拒绝的发件人和接受的发件人列表中指定同一用户或组，否则会发生错误。</span><span class="sxs-lookup"><span data-stu-id="0706e-p101">Users in the rejected senders list cannot post to conversations of the group (identified in the GET request URL). Make sure you do not specify the same user or group in the rejected senders and accepted senders lists, otherwise you will get an error.</span></span>

## <a name="permissions"></a><span data-ttu-id="0706e-107">权限</span><span class="sxs-lookup"><span data-stu-id="0706e-107">Permissions</span></span>
<span data-ttu-id="0706e-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0706e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0706e-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="0706e-110">Permission type</span></span>      | <span data-ttu-id="0706e-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0706e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0706e-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0706e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="0706e-113">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0706e-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="0706e-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0706e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0706e-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="0706e-115">Not supported.</span></span>    |
|<span data-ttu-id="0706e-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="0706e-116">Application</span></span> | <span data-ttu-id="0706e-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="0706e-117">Not supported.</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="0706e-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0706e-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/rejectedSenders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="0706e-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="0706e-119">Optional query parameters</span></span>
<span data-ttu-id="0706e-120">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="0706e-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0706e-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="0706e-121">Request headers</span></span>
| <span data-ttu-id="0706e-122">标头</span><span class="sxs-lookup"><span data-stu-id="0706e-122">Header</span></span>       | <span data-ttu-id="0706e-123">值</span><span class="sxs-lookup"><span data-stu-id="0706e-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0706e-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="0706e-124">Authorization</span></span>  | <span data-ttu-id="0706e-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0706e-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0706e-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="0706e-127">Request body</span></span>
<span data-ttu-id="0706e-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0706e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0706e-129">响应</span><span class="sxs-lookup"><span data-stu-id="0706e-129">Response</span></span>
<span data-ttu-id="0706e-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="0706e-130">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0706e-131">示例</span><span class="sxs-lookup"><span data-stu-id="0706e-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="0706e-132">请求</span><span class="sxs-lookup"><span data-stu-id="0706e-132">Request</span></span>
<span data-ttu-id="0706e-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="0706e-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0706e-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="0706e-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_rejectedsenders"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/rejectedSenders
```
# <a name="c"></a>[<span data-ttu-id="0706e-135">C#</span><span class="sxs-lookup"><span data-stu-id="0706e-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-rejectedsenders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0706e-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0706e-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-rejectedsenders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0706e-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0706e-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-rejectedsenders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0706e-138">Java</span><span class="sxs-lookup"><span data-stu-id="0706e-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-rejectedsenders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="0706e-139">响应</span><span class="sxs-lookup"><span data-stu-id="0706e-139">Response</span></span>
<span data-ttu-id="0706e-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="0706e-140">The following is an example of the response.</span></span>
><span data-ttu-id="0706e-141">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="0706e-141">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "description": "List rejectedSenders",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->


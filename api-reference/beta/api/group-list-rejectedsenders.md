---
title: 列出 rejectedSender
description: '获取此组的“遭拒的发件人”列表中的用户或组列表。 '
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 657f6a847d8d00b8543a2d560e5a6eac955243c5
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52041454"
---
# <a name="list-rejectedsenders"></a><span data-ttu-id="a0c86-103">列出 rejectedSender</span><span class="sxs-lookup"><span data-stu-id="a0c86-103">List rejectedSenders</span></span>

<span data-ttu-id="a0c86-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a0c86-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a0c86-105">获取此组的“遭拒的发件人”列表中的用户或组列表。</span><span class="sxs-lookup"><span data-stu-id="a0c86-105">Get a list of users or groups that are in the rejected-senders list for this group.</span></span> 

<span data-ttu-id="a0c86-p101">已拒绝的发件人列表中的用户无法发布到组对话（在 GET 请求 URL 中标识）。确保未在拒绝的发件人和接受的发件人列表中指定同一用户或组，否则会发生错误。</span><span class="sxs-lookup"><span data-stu-id="a0c86-p101">Users in the rejected senders list cannot post to conversations of the group (identified in the GET request URL). Make sure you do not specify the same user or group in the rejected senders and accepted senders lists, otherwise you will get an error.</span></span>

## <a name="permissions"></a><span data-ttu-id="a0c86-108">权限</span><span class="sxs-lookup"><span data-stu-id="a0c86-108">Permissions</span></span>
<span data-ttu-id="a0c86-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a0c86-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a0c86-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="a0c86-111">Permission type</span></span>      | <span data-ttu-id="a0c86-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a0c86-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a0c86-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a0c86-113">Delegated (work or school account)</span></span> | <span data-ttu-id="a0c86-114">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0c86-114">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="a0c86-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a0c86-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a0c86-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a0c86-116">Not supported.</span></span>    |
|<span data-ttu-id="a0c86-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="a0c86-117">Application</span></span> | <span data-ttu-id="a0c86-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="a0c86-118">Not supported.</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="a0c86-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a0c86-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/rejectedSenders
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a0c86-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="a0c86-120">Optional query parameters</span></span>
<span data-ttu-id="a0c86-121">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="a0c86-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a0c86-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="a0c86-122">Request headers</span></span>
| <span data-ttu-id="a0c86-123">标头</span><span class="sxs-lookup"><span data-stu-id="a0c86-123">Header</span></span>       | <span data-ttu-id="a0c86-124">值</span><span class="sxs-lookup"><span data-stu-id="a0c86-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a0c86-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="a0c86-125">Authorization</span></span>  | <span data-ttu-id="a0c86-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a0c86-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a0c86-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="a0c86-128">Request body</span></span>
<span data-ttu-id="a0c86-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a0c86-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a0c86-130">响应</span><span class="sxs-lookup"><span data-stu-id="a0c86-130">Response</span></span>
<span data-ttu-id="a0c86-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="a0c86-131">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a0c86-132">示例</span><span class="sxs-lookup"><span data-stu-id="a0c86-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="a0c86-133">请求</span><span class="sxs-lookup"><span data-stu-id="a0c86-133">Request</span></span>
<span data-ttu-id="a0c86-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a0c86-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a0c86-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="a0c86-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_rejectedsenders"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/rejectedSenders
```
# <a name="c"></a>[<span data-ttu-id="a0c86-136">C#</span><span class="sxs-lookup"><span data-stu-id="a0c86-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-rejectedsenders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a0c86-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a0c86-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-rejectedsenders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a0c86-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a0c86-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-rejectedsenders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a0c86-139">Java</span><span class="sxs-lookup"><span data-stu-id="a0c86-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-rejectedsenders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a0c86-140">响应</span><span class="sxs-lookup"><span data-stu-id="a0c86-140">Response</span></span>
<span data-ttu-id="a0c86-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="a0c86-141">The following is an example of the response.</span></span>
><span data-ttu-id="a0c86-142">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="a0c86-142">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "description": "List rejectedSenders",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->



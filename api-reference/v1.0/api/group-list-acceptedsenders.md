---
title: 列出 acceptedSender
description: 获取此组的“接受的发件人”列表中的用户或组列表。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: b61ad82aed14ed8bafea1c4092f956a2b2da36c4
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36337333"
---
# <a name="list-acceptedsenders"></a><span data-ttu-id="301ba-103">列出 acceptedSender</span><span class="sxs-lookup"><span data-stu-id="301ba-103">List acceptedSenders</span></span>
<span data-ttu-id="301ba-104">获取此组的“接受的发件人”列表中的用户或组列表。</span><span class="sxs-lookup"><span data-stu-id="301ba-104">Get a list of users or groups that are in the accepted-senders list for this group.</span></span>

<span data-ttu-id="301ba-p101">接受的发件人列表中的用户可以发布到组对话（在 GET 请求 URL 中标识）。确保未在接受的发件人和拒绝的发件人列表中指定同一用户或组，否则会发生错误。</span><span class="sxs-lookup"><span data-stu-id="301ba-p101">Users in the accepted senders list can post to conversations of the group (identified in the GET request URL). Make sure you do not specify the same user or group in the accepted senders and rejected senders lists, otherwise you will get an error.</span></span>

## <a name="permissions"></a><span data-ttu-id="301ba-107">权限</span><span class="sxs-lookup"><span data-stu-id="301ba-107">Permissions</span></span>
<span data-ttu-id="301ba-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="301ba-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="301ba-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="301ba-110">Permission type</span></span>      | <span data-ttu-id="301ba-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="301ba-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="301ba-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="301ba-112">Delegated (work or school account)</span></span> | <span data-ttu-id="301ba-113">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="301ba-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="301ba-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="301ba-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="301ba-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="301ba-115">Not supported.</span></span>    |
|<span data-ttu-id="301ba-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="301ba-116">Application</span></span> | <span data-ttu-id="301ba-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="301ba-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="301ba-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="301ba-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/acceptedSenders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="301ba-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="301ba-119">Optional query parameters</span></span>
<span data-ttu-id="301ba-120">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="301ba-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="301ba-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="301ba-121">Request headers</span></span>
| <span data-ttu-id="301ba-122">标头</span><span class="sxs-lookup"><span data-stu-id="301ba-122">Header</span></span>       | <span data-ttu-id="301ba-123">值</span><span class="sxs-lookup"><span data-stu-id="301ba-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="301ba-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="301ba-124">Authorization</span></span>  | <span data-ttu-id="301ba-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="301ba-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="301ba-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="301ba-127">Request body</span></span>
<span data-ttu-id="301ba-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="301ba-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="301ba-129">响应</span><span class="sxs-lookup"><span data-stu-id="301ba-129">Response</span></span>
<span data-ttu-id="301ba-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="301ba-130">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="301ba-131">示例</span><span class="sxs-lookup"><span data-stu-id="301ba-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="301ba-132">请求</span><span class="sxs-lookup"><span data-stu-id="301ba-132">Request</span></span>
<span data-ttu-id="301ba-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="301ba-133">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="301ba-134">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="301ba-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_acceptedsenders"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/acceptedSenders
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="301ba-135">C#</span><span class="sxs-lookup"><span data-stu-id="301ba-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-acceptedsenders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="301ba-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="301ba-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-acceptedsenders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="301ba-137">目标-C</span><span class="sxs-lookup"><span data-stu-id="301ba-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-acceptedsenders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="301ba-138">Java</span><span class="sxs-lookup"><span data-stu-id="301ba-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-acceptedsenders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="301ba-139">响应</span><span class="sxs-lookup"><span data-stu-id="301ba-139">Response</span></span>
<span data-ttu-id="301ba-140">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="301ba-140">The following is an example of the response.</span></span>
><span data-ttu-id="301ba-141">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="301ba-141">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="301ba-142">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="301ba-142">All the properties will be returned from an actual call.</span></span>
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
  "description": "List acceptedSenders",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

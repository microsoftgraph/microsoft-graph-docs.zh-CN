---
title: 列出 rejectedSender
description: '获取此组的“遭拒的发件人”列表中的用户或组列表。 '
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: b4a45bba59d71d262e0d3591021a4b8de5466098
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42419301"
---
# <a name="list-rejectedsenders"></a><span data-ttu-id="1085d-103">列出 rejectedSender</span><span class="sxs-lookup"><span data-stu-id="1085d-103">List rejectedSenders</span></span>

<span data-ttu-id="1085d-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="1085d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1085d-105">获取此组的“遭拒的发件人”列表中的用户或组列表。</span><span class="sxs-lookup"><span data-stu-id="1085d-105">Get a list of users or groups that are in the rejected-senders list for this group.</span></span> 

<span data-ttu-id="1085d-p101">已拒绝的发件人列表中的用户无法发布到组对话（在 GET 请求 URL 中标识）。确保未在拒绝的发件人和接受的发件人列表中指定同一用户或组，否则会发生错误。</span><span class="sxs-lookup"><span data-stu-id="1085d-p101">Users in the rejected senders list cannot post to conversations of the group (identified in the GET request URL). Make sure you do not specify the same user or group in the rejected senders and accepted senders lists, otherwise you will get an error.</span></span>

## <a name="permissions"></a><span data-ttu-id="1085d-108">权限</span><span class="sxs-lookup"><span data-stu-id="1085d-108">Permissions</span></span>
<span data-ttu-id="1085d-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1085d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1085d-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="1085d-111">Permission type</span></span>      | <span data-ttu-id="1085d-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1085d-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1085d-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1085d-113">Delegated (work or school account)</span></span> | <span data-ttu-id="1085d-114">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1085d-114">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="1085d-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1085d-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1085d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="1085d-116">Not supported.</span></span>    |
|<span data-ttu-id="1085d-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="1085d-117">Application</span></span> | <span data-ttu-id="1085d-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="1085d-118">Not supported.</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="1085d-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1085d-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/rejectedSenders
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1085d-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="1085d-120">Optional query parameters</span></span>
<span data-ttu-id="1085d-121">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="1085d-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1085d-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="1085d-122">Request headers</span></span>
| <span data-ttu-id="1085d-123">标头</span><span class="sxs-lookup"><span data-stu-id="1085d-123">Header</span></span>       | <span data-ttu-id="1085d-124">值</span><span class="sxs-lookup"><span data-stu-id="1085d-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1085d-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="1085d-125">Authorization</span></span>  | <span data-ttu-id="1085d-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1085d-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1085d-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="1085d-128">Request body</span></span>
<span data-ttu-id="1085d-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1085d-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1085d-130">响应</span><span class="sxs-lookup"><span data-stu-id="1085d-130">Response</span></span>
<span data-ttu-id="1085d-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="1085d-131">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1085d-132">示例</span><span class="sxs-lookup"><span data-stu-id="1085d-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="1085d-133">请求</span><span class="sxs-lookup"><span data-stu-id="1085d-133">Request</span></span>
<span data-ttu-id="1085d-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="1085d-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1085d-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="1085d-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_rejectedsenders"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/rejectedSenders
```
# <a name="c"></a>[<span data-ttu-id="1085d-136">C#</span><span class="sxs-lookup"><span data-stu-id="1085d-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-rejectedsenders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1085d-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1085d-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-rejectedsenders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1085d-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1085d-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-rejectedsenders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="1085d-139">响应</span><span class="sxs-lookup"><span data-stu-id="1085d-139">Response</span></span>
<span data-ttu-id="1085d-140">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="1085d-140">The following is an example of the response.</span></span>
><span data-ttu-id="1085d-141">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="1085d-141">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="1085d-142">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="1085d-142">All the properties will be returned from an actual call.</span></span>
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

---
title: 列出 acceptedSender
description: 获取此组的“接受的发件人”列表中的用户或组列表。
author: Jordanndahl
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: a60225965c0da6657a6d7476dd46499a75c19b73
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/27/2021
ms.locfileid: "52681660"
---
# <a name="list-acceptedsenders"></a><span data-ttu-id="39bb6-103">列出 acceptedSender</span><span class="sxs-lookup"><span data-stu-id="39bb6-103">List acceptedSenders</span></span>

<span data-ttu-id="39bb6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="39bb6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="39bb6-105">获取此组的“接受的发件人”列表中的用户或组列表。</span><span class="sxs-lookup"><span data-stu-id="39bb6-105">Get a list of users or groups that are in the accepted-senders list for this group.</span></span>

<span data-ttu-id="39bb6-p101">接受的发件人列表中的用户可以发布到组对话（在 GET 请求 URL 中标识）。确保未在接受的发件人和拒绝的发件人列表中指定同一用户或组，否则会发生错误。</span><span class="sxs-lookup"><span data-stu-id="39bb6-p101">Users in the accepted senders list can post to conversations of the group (identified in the GET request URL). Make sure you do not specify the same user or group in the accepted senders and rejected senders lists, otherwise you will get an error.</span></span>

## <a name="permissions"></a><span data-ttu-id="39bb6-108">权限</span><span class="sxs-lookup"><span data-stu-id="39bb6-108">Permissions</span></span>
<span data-ttu-id="39bb6-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="39bb6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="39bb6-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="39bb6-111">Permission type</span></span>      | <span data-ttu-id="39bb6-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="39bb6-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="39bb6-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="39bb6-113">Delegated (work or school account)</span></span> | <span data-ttu-id="39bb6-114">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="39bb6-114">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="39bb6-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="39bb6-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="39bb6-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="39bb6-116">Not supported.</span></span>    |
|<span data-ttu-id="39bb6-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="39bb6-117">Application</span></span> | <span data-ttu-id="39bb6-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="39bb6-118">Not supported.</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="39bb6-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="39bb6-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/acceptedSenders
```

## <a name="optional-query-parameters"></a><span data-ttu-id="39bb6-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="39bb6-120">Optional query parameters</span></span>
<span data-ttu-id="39bb6-121">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="39bb6-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="39bb6-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="39bb6-122">Request headers</span></span>
| <span data-ttu-id="39bb6-123">标头</span><span class="sxs-lookup"><span data-stu-id="39bb6-123">Header</span></span>       | <span data-ttu-id="39bb6-124">值</span><span class="sxs-lookup"><span data-stu-id="39bb6-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="39bb6-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="39bb6-125">Authorization</span></span>  | <span data-ttu-id="39bb6-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="39bb6-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="39bb6-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="39bb6-128">Request body</span></span>
<span data-ttu-id="39bb6-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="39bb6-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="39bb6-130">响应</span><span class="sxs-lookup"><span data-stu-id="39bb6-130">Response</span></span>
<span data-ttu-id="39bb6-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="39bb6-131">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="39bb6-132">示例</span><span class="sxs-lookup"><span data-stu-id="39bb6-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="39bb6-133">请求</span><span class="sxs-lookup"><span data-stu-id="39bb6-133">Request</span></span>
<span data-ttu-id="39bb6-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="39bb6-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="39bb6-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="39bb6-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_acceptedsenders"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/acceptedSenders
```
# <a name="c"></a>[<span data-ttu-id="39bb6-136">C#</span><span class="sxs-lookup"><span data-stu-id="39bb6-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-acceptedsenders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="39bb6-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="39bb6-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-acceptedsenders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="39bb6-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="39bb6-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-acceptedsenders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="39bb6-139">Java</span><span class="sxs-lookup"><span data-stu-id="39bb6-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-acceptedsenders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="39bb6-140">响应</span><span class="sxs-lookup"><span data-stu-id="39bb6-140">Response</span></span>
<span data-ttu-id="39bb6-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="39bb6-141">The following is an example of the response.</span></span>
><span data-ttu-id="39bb6-142">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="39bb6-142">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "description": "List acceptedSenders",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->



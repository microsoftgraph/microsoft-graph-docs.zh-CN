---
title: 列出 allowedUsers
description: 检索已授予访问权限以将打印作业提交到关联的打印机共享的用户列表。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: eaa1c5fc9a7e006ff8e0a0d6bd4869e1d16022df
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/02/2020
ms.locfileid: "44216831"
---
# <a name="list-allowedusers"></a><span data-ttu-id="584ed-103">列出 allowedUsers</span><span class="sxs-lookup"><span data-stu-id="584ed-103">List allowedUsers</span></span>

<span data-ttu-id="584ed-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="584ed-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="584ed-105">检索已授予访问权限以将打印作业提交到相关[printerShare](../resources/printershare.md)的用户的列表。</span><span class="sxs-lookup"><span data-stu-id="584ed-105">Retrieve a list of users who have been granted access to submit print jobs to the associated [printerShare](../resources/printershare.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="584ed-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="584ed-106">Permissions</span></span>
<span data-ttu-id="584ed-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="584ed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="584ed-109">除了以下权限之外，用户的租户还必须具有活动的通用打印订阅。</span><span class="sxs-lookup"><span data-stu-id="584ed-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="584ed-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="584ed-110">Permission type</span></span> | <span data-ttu-id="584ed-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="584ed-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="584ed-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="584ed-112">Delegated (work or school account)</span></span>| <span data-ttu-id="584ed-113">已阅读的用户。所有</span><span class="sxs-lookup"><span data-stu-id="584ed-113">Users.Read.All</span></span> |
|<span data-ttu-id="584ed-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="584ed-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="584ed-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="584ed-115">Not Supported.</span></span>|
|<span data-ttu-id="584ed-116">Application</span><span class="sxs-lookup"><span data-stu-id="584ed-116">Application</span></span>|<span data-ttu-id="584ed-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="584ed-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="584ed-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="584ed-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/shares/{id}/allowedUsers
```

## <a name="request-headers"></a><span data-ttu-id="584ed-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="584ed-119">Request headers</span></span>
| <span data-ttu-id="584ed-120">名称</span><span class="sxs-lookup"><span data-stu-id="584ed-120">Name</span></span>      |<span data-ttu-id="584ed-121">说明</span><span class="sxs-lookup"><span data-stu-id="584ed-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="584ed-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="584ed-122">Authorization</span></span> | <span data-ttu-id="584ed-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="584ed-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="584ed-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="584ed-125">Request body</span></span>
<span data-ttu-id="584ed-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="584ed-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="584ed-127">响应</span><span class="sxs-lookup"><span data-stu-id="584ed-127">Response</span></span>
<span data-ttu-id="584ed-128">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和[printUserIdentity](../resources/printuseridentity.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="584ed-128">If successful, this method returns a `200 OK` response code and a collection of [printUserIdentity](../resources/printuseridentity.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="584ed-129">示例</span><span class="sxs-lookup"><span data-stu-id="584ed-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="584ed-130">请求</span><span class="sxs-lookup"><span data-stu-id="584ed-130">Request</span></span>
<span data-ttu-id="584ed-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="584ed-131">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="584ed-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="584ed-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_allowedUsers"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/shares/{id}/allowedUsers
```
# <a name="c"></a>[<span data-ttu-id="584ed-133">C#</span><span class="sxs-lookup"><span data-stu-id="584ed-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-allowedusers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="584ed-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="584ed-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-allowedusers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="584ed-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="584ed-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-allowedusers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="584ed-136">响应</span><span class="sxs-lookup"><span data-stu-id="584ed-136">Response</span></span>
<span data-ttu-id="584ed-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="584ed-137">The following is an example of the response.</span></span>
><span data-ttu-id="584ed-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="584ed-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printUserIdentity",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 286

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.printUserIdentity)",
  "value": [
    {
      "id": "016b5565-3bbf-4067-b9ff-4d68167eb1a6",
      "displayName": "UserName",
      "userPrincipalName": "username@microsoft.com"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List allowedUsers",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

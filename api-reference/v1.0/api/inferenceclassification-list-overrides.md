---
title: 列出替代
description: 获取用户设置为始终以特定方式对来自特定发件人的邮件进行分类的替代。
localization_priority: Normal
author: abheek-das
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: fb6cd4c87c5ee06e0d9849bdaa13e62b616c7d3c
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52051373"
---
# <a name="list-overrides"></a><span data-ttu-id="6faf7-103">列出替代</span><span class="sxs-lookup"><span data-stu-id="6faf7-103">List overrides</span></span>

<span data-ttu-id="6faf7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6faf7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6faf7-105">获取用户设置为始终以特定方式对来自特定发件人的邮件进行分类的替代。</span><span class="sxs-lookup"><span data-stu-id="6faf7-105">Get the overrides that a user has set up to always classify messages from certain senders in specific ways.</span></span>

<span data-ttu-id="6faf7-p101">每个替代均对应一个发件人的 SMTP 地址。最初，用户没有任何替代。</span><span class="sxs-lookup"><span data-stu-id="6faf7-p101">Each override corresponds to an SMTP address of a sender. Initially, a user does not have any overrides.</span></span>
## <a name="permissions"></a><span data-ttu-id="6faf7-108">权限</span><span class="sxs-lookup"><span data-stu-id="6faf7-108">Permissions</span></span>
<span data-ttu-id="6faf7-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6faf7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6faf7-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="6faf7-111">Permission type</span></span>      | <span data-ttu-id="6faf7-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6faf7-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6faf7-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6faf7-113">Delegated (work or school account)</span></span> | <span data-ttu-id="6faf7-114">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="6faf7-114">Mail.Read</span></span>    |
|<span data-ttu-id="6faf7-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6faf7-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6faf7-116">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="6faf7-116">Mail.Read</span></span>    |
|<span data-ttu-id="6faf7-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="6faf7-117">Application</span></span> | <span data-ttu-id="6faf7-118">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="6faf7-118">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="6faf7-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6faf7-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/inferenceClassification/overrides
GET /users/{id}/inferenceClassification/overrides
```

## <a name="request-headers"></a><span data-ttu-id="6faf7-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="6faf7-120">Request headers</span></span>
| <span data-ttu-id="6faf7-121">名称</span><span class="sxs-lookup"><span data-stu-id="6faf7-121">Name</span></span>       | <span data-ttu-id="6faf7-122">类型</span><span class="sxs-lookup"><span data-stu-id="6faf7-122">Type</span></span> | <span data-ttu-id="6faf7-123">说明</span><span class="sxs-lookup"><span data-stu-id="6faf7-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="6faf7-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="6faf7-124">Authorization</span></span>  | <span data-ttu-id="6faf7-125">string</span><span class="sxs-lookup"><span data-stu-id="6faf7-125">string</span></span>  | <span data-ttu-id="6faf7-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6faf7-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6faf7-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="6faf7-128">Request body</span></span>
<span data-ttu-id="6faf7-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6faf7-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6faf7-130">响应</span><span class="sxs-lookup"><span data-stu-id="6faf7-130">Response</span></span>

<span data-ttu-id="6faf7-p104">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) 对象集合。如果用户未设置任何替代，则返回空集合。</span><span class="sxs-lookup"><span data-stu-id="6faf7-p104">If successful, this method returns a `200 OK` response code and a collection of [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) objects in the response body. An empty collection is returned if the user doesn't have any overrides set up.</span></span>
## <a name="example"></a><span data-ttu-id="6faf7-133">示例</span><span class="sxs-lookup"><span data-stu-id="6faf7-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6faf7-134">请求</span><span class="sxs-lookup"><span data-stu-id="6faf7-134">Request</span></span>
<span data-ttu-id="6faf7-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6faf7-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6faf7-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="6faf7-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_overrides"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/inferenceClassification/overrides
```
# <a name="c"></a>[<span data-ttu-id="6faf7-137">C#</span><span class="sxs-lookup"><span data-stu-id="6faf7-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-overrides-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6faf7-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6faf7-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-overrides-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6faf7-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6faf7-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-overrides-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6faf7-140">Java</span><span class="sxs-lookup"><span data-stu-id="6faf7-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-overrides-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="6faf7-141">响应</span><span class="sxs-lookup"><span data-stu-id="6faf7-141">Response</span></span>
<span data-ttu-id="6faf7-142">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="6faf7-142">Here is an example of the response.</span></span> <span data-ttu-id="6faf7-143">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="6faf7-143">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.inferenceClassificationOverride",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "classifyAs": "focused",
      "senderEmailAddress": {
        "name": "Samantha Booth",
        "address": "samanthab@adatum.onmicrosoft.com"
      },
      "id": "98f5bdef-576a-404d-a2ea-07a3cf11a9b9"
    },
    {
      "classifyAs": "other",
      "senderEmailAddress": {
        "name": "Randi Welch",
        "address": "randiw@adatum.onmicrosoft.com"
      },
      "id": "98f5bdef-576a-404d-a2ea-07a3cf34af4r"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List overrides",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->


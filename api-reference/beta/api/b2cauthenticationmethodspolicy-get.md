---
title: 获取 b2cAuthenticationMethodsPolicy
description: 阅读 b2cAuthenticationMethodsPolicy 对象的属性。
localization_priority: Priority
author: namkedia
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 840d3be6471391e4c4128421dbf69da6efa6a985
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50438398"
---
# <a name="get-b2cauthenticationmethodspolicy"></a><span data-ttu-id="8e3a4-103">获取 b2cAuthenticationMethodsPolicy</span><span class="sxs-lookup"><span data-stu-id="8e3a4-103">Get b2cAuthenticationMethodsPolicy</span></span>

<span data-ttu-id="8e3a4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8e3a4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8e3a4-105">阅读 [b2cAuthenticationMethodsPolicy](../resources/b2cauthenticationmethodspolicy.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="8e3a4-105">Read the properties of a [b2cAuthenticationMethodsPolicy](../resources/b2cauthenticationmethodspolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="8e3a4-106">权限</span><span class="sxs-lookup"><span data-stu-id="8e3a4-106">Permissions</span></span>

<span data-ttu-id="8e3a4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8e3a4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8e3a4-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="8e3a4-109">Permission type</span></span>                        | <span data-ttu-id="8e3a4-110">权限</span><span class="sxs-lookup"><span data-stu-id="8e3a4-110">Permissions</span></span>|
|:---------------------------------------|:---------------|
| <span data-ttu-id="8e3a4-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8e3a4-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="8e3a4-112">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="8e3a4-112">Policy.Read.All</span></span>|
| <span data-ttu-id="8e3a4-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8e3a4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8e3a4-114">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="8e3a4-114">Policy.Read.All</span></span>|
| <span data-ttu-id="8e3a4-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="8e3a4-115">Application</span></span>                            | <span data-ttu-id="8e3a4-116">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="8e3a4-116">Policy.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8e3a4-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8e3a4-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/b2cAuthenticationMethodsPolicy
```

## <a name="request-headers"></a><span data-ttu-id="8e3a4-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="8e3a4-118">Request headers</span></span>

| <span data-ttu-id="8e3a4-119">名称</span><span class="sxs-lookup"><span data-stu-id="8e3a4-119">Name</span></span>      |<span data-ttu-id="8e3a4-120">说明</span><span class="sxs-lookup"><span data-stu-id="8e3a4-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8e3a4-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="8e3a4-121">Authorization</span></span> | <span data-ttu-id="8e3a4-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8e3a4-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8e3a4-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="8e3a4-124">Request body</span></span>

<span data-ttu-id="8e3a4-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8e3a4-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8e3a4-126">响应</span><span class="sxs-lookup"><span data-stu-id="8e3a4-126">Response</span></span>

<span data-ttu-id="8e3a4-127">如果成功，此方法在响应正文中返回`200 OK`响应代码和请求的 [b2cAuthenticationMethodsPolicy](../resources/b2cauthenticationmethodspolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8e3a4-127">If successful, this method returns a `200 OK` response code and the requested [b2cAuthenticationMethodsPolicy](../resources/b2cauthenticationmethodspolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8e3a4-128">示例</span><span class="sxs-lookup"><span data-stu-id="8e3a4-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8e3a4-129">请求</span><span class="sxs-lookup"><span data-stu-id="8e3a4-129">Request</span></span>

<span data-ttu-id="8e3a4-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="8e3a4-130">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="8e3a4-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="8e3a4-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_b2cauthenticationmethodspolicy"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/policies/b2cAuthenticationMethodsPolicy
```
# <a name="c"></a>[<span data-ttu-id="8e3a4-132">C#</span><span class="sxs-lookup"><span data-stu-id="8e3a4-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-b2cauthenticationmethodspolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8e3a4-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8e3a4-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-b2cauthenticationmethodspolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8e3a4-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8e3a4-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-b2cauthenticationmethodspolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8e3a4-135">Java</span><span class="sxs-lookup"><span data-stu-id="8e3a4-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-b2cauthenticationmethodspolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8e3a4-136">响应</span><span class="sxs-lookup"><span data-stu-id="8e3a4-136">Response</span></span>

<span data-ttu-id="8e3a4-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="8e3a4-137">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.b2cAuthenticationMethodsPolicy"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#b2cAuthenticationMethodsPolicy",
    "id": "b2CAuthenticationMethodsPolicy",
    "isEmailPasswordAuthenticationEnabled": true,
    "isUserNameAuthenticationEnabled": false
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get b2cAuthenticationMethodsPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

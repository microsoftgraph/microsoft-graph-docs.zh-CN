---
title: 获取 b2cAuthenticationMethodsPolicy
description: 阅读 b2cAuthenticationMethodsPolicy 对象的属性。
localization_priority: Priority
author: namkedia
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 5b2fc42c3a2d65dd06dce6e3e39e1cae090023bb
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/09/2020
ms.locfileid: "48406283"
---
# <a name="get-b2cauthenticationmethodspolicy"></a><span data-ttu-id="142d3-103">获取 b2cAuthenticationMethodsPolicy</span><span class="sxs-lookup"><span data-stu-id="142d3-103">Get b2cAuthenticationMethodsPolicy</span></span>

<span data-ttu-id="142d3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="142d3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="142d3-105">阅读 [b2cAuthenticationMethodsPolicy](../resources/b2cauthenticationmethodspolicy.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="142d3-105">Read the properties of a [b2cAuthenticationMethodsPolicy](../resources/b2cauthenticationmethodspolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="142d3-106">权限</span><span class="sxs-lookup"><span data-stu-id="142d3-106">Permissions</span></span>

<span data-ttu-id="142d3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="142d3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="142d3-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="142d3-109">Permission type</span></span>                        | <span data-ttu-id="142d3-110">权限</span><span class="sxs-lookup"><span data-stu-id="142d3-110">Permissions</span></span>|
|:---------------------------------------|:---------------|
| <span data-ttu-id="142d3-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="142d3-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="142d3-112">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="142d3-112">Policy.Read.All</span></span>|
| <span data-ttu-id="142d3-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="142d3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="142d3-114">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="142d3-114">Policy.Read.All</span></span>|
| <span data-ttu-id="142d3-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="142d3-115">Application</span></span>                            | <span data-ttu-id="142d3-116">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="142d3-116">Policy.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="142d3-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="142d3-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/b2cAuthenticationMethodsPolicy
```

## <a name="request-headers"></a><span data-ttu-id="142d3-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="142d3-118">Request headers</span></span>

| <span data-ttu-id="142d3-119">名称</span><span class="sxs-lookup"><span data-stu-id="142d3-119">Name</span></span>      |<span data-ttu-id="142d3-120">说明</span><span class="sxs-lookup"><span data-stu-id="142d3-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="142d3-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="142d3-121">Authorization</span></span> | <span data-ttu-id="142d3-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="142d3-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="142d3-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="142d3-124">Request body</span></span>

<span data-ttu-id="142d3-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="142d3-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="142d3-126">响应</span><span class="sxs-lookup"><span data-stu-id="142d3-126">Response</span></span>

<span data-ttu-id="142d3-127">如果成功，此方法在响应正文中返回`200 OK`响应代码和请求的 [b2cAuthenticationMethodsPolicy](../resources/b2cauthenticationmethodspolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="142d3-127">If successful, this method returns a `200 OK` response code and the requested [b2cAuthenticationMethodsPolicy](../resources/b2cauthenticationmethodspolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="142d3-128">示例</span><span class="sxs-lookup"><span data-stu-id="142d3-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="142d3-129">请求</span><span class="sxs-lookup"><span data-stu-id="142d3-129">Request</span></span>

<span data-ttu-id="142d3-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="142d3-130">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_b2cauthenticationmethodspolicy"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/policies/b2cAuthenticationMethodsPolicy
```

### <a name="response"></a><span data-ttu-id="142d3-131">响应</span><span class="sxs-lookup"><span data-stu-id="142d3-131">Response</span></span>

<span data-ttu-id="142d3-132">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="142d3-132">The following is an example of the response.</span></span>

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

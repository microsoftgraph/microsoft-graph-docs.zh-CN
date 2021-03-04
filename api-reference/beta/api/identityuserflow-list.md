---
title: 列出 userFlows
description: 检索 userFlow 对象的列表。
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 7c60d86c6baa2b18b3957872f81b2069683ea237
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50435306"
---
# <a name="list-userflows"></a><span data-ttu-id="ea98d-103">列出 userFlows</span><span class="sxs-lookup"><span data-stu-id="ea98d-103">List userFlows</span></span>

<span data-ttu-id="ea98d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ea98d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ea98d-105">检索用户 [流列表](../resources/identityuserflow.md)。</span><span class="sxs-lookup"><span data-stu-id="ea98d-105">Retrieve a list of [userflows](../resources/identityuserflow.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ea98d-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="ea98d-106">Permissions</span></span>

<span data-ttu-id="ea98d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ea98d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ea98d-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="ea98d-109">Permission type</span></span>                        | <span data-ttu-id="ea98d-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ea98d-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ea98d-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ea98d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ea98d-112">IdentityUserFlow.Read.All、IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ea98d-112">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>  |
| <span data-ttu-id="ea98d-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ea98d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ea98d-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="ea98d-114">Not supported.</span></span> |
| <span data-ttu-id="ea98d-115">Application</span><span class="sxs-lookup"><span data-stu-id="ea98d-115">Application</span></span>                            | <span data-ttu-id="ea98d-116">IdentityUserFlow.Read.All、IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ea98d-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ea98d-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ea98d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/userFlows
```

## <a name="request-headers"></a><span data-ttu-id="ea98d-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="ea98d-118">Request headers</span></span>

| <span data-ttu-id="ea98d-119">名称</span><span class="sxs-lookup"><span data-stu-id="ea98d-119">Name</span></span>      |<span data-ttu-id="ea98d-120">说明</span><span class="sxs-lookup"><span data-stu-id="ea98d-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ea98d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="ea98d-121">Authorization</span></span> | <span data-ttu-id="ea98d-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ea98d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ea98d-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="ea98d-124">Request body</span></span>

<span data-ttu-id="ea98d-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ea98d-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ea98d-126">响应</span><span class="sxs-lookup"><span data-stu-id="ea98d-126">Response</span></span>

<span data-ttu-id="ea98d-127">如果成功，此方法在响应正文中返回响应代码和 `200 OK` [userFlow](../resources/identityuserflow.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="ea98d-127">If successful, this method returns a `200 OK` response code and a collection of [userFlow](../resources/identityuserflow.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ea98d-128">示例</span><span class="sxs-lookup"><span data-stu-id="ea98d-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ea98d-129">请求</span><span class="sxs-lookup"><span data-stu-id="ea98d-129">Request</span></span>

<span data-ttu-id="ea98d-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ea98d-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ea98d-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="ea98d-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_userflows"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identity/userFlows
```
# <a name="c"></a>[<span data-ttu-id="ea98d-132">C#</span><span class="sxs-lookup"><span data-stu-id="ea98d-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-userflows-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ea98d-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ea98d-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-userflows-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ea98d-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ea98d-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-userflows-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ea98d-135">Java</span><span class="sxs-lookup"><span data-stu-id="ea98d-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-userflows-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ea98d-136">响应</span><span class="sxs-lookup"><span data-stu-id="ea98d-136">Response</span></span>

<span data-ttu-id="ea98d-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ea98d-137">The following is an example of the response.</span></span>

> <span data-ttu-id="ea98d-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="ea98d-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.UserFlow",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "B2C_1_UserFlow1",
      "userFlowType": "signUpOrSignIn",
      "userFlowTypeVersion": 1
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List userFlows",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: get_userflows/container/userFlowTypeVersion:\r\n      Expected type Single but actual was Int64. Property: userFlowTypeVersion, actual value: '1'"
  ]
}-->



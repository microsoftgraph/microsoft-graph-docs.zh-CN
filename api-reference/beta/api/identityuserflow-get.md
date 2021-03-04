---
title: 获取 userFlow
description: 检索 userflow 对象的属性和关系。
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 143b86109eb0f7cfd14d3366a66fd712f6406262
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50435313"
---
# <a name="get-userflow"></a><span data-ttu-id="cfaeb-103">获取 userFlow</span><span class="sxs-lookup"><span data-stu-id="cfaeb-103">Get userFlow</span></span>

<span data-ttu-id="cfaeb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cfaeb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cfaeb-105">检索 [userFlow](../resources/identityuserflow.md) 对象的属性和关联。</span><span class="sxs-lookup"><span data-stu-id="cfaeb-105">Retrieve the properties and associations for an [userFlow](../resources/identityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="cfaeb-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="cfaeb-106">Permissions</span></span>

<span data-ttu-id="cfaeb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cfaeb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cfaeb-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="cfaeb-109">Permission type</span></span>                        | <span data-ttu-id="cfaeb-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cfaeb-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="cfaeb-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cfaeb-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="cfaeb-112">IdentityUserFlow.Read.All、IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cfaeb-112">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span> |
| <span data-ttu-id="cfaeb-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cfaeb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cfaeb-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="cfaeb-114">Not supported.</span></span> |
| <span data-ttu-id="cfaeb-115">Application</span><span class="sxs-lookup"><span data-stu-id="cfaeb-115">Application</span></span>                            | <span data-ttu-id="cfaeb-116">IdentityUserFlow.Read.All、IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cfaeb-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cfaeb-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cfaeb-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/userFlows/{id}
```

## <a name="request-headers"></a><span data-ttu-id="cfaeb-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="cfaeb-118">Request headers</span></span>

| <span data-ttu-id="cfaeb-119">名称</span><span class="sxs-lookup"><span data-stu-id="cfaeb-119">Name</span></span>      |<span data-ttu-id="cfaeb-120">说明</span><span class="sxs-lookup"><span data-stu-id="cfaeb-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="cfaeb-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="cfaeb-121">Authorization</span></span> | <span data-ttu-id="cfaeb-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="cfaeb-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="cfaeb-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="cfaeb-124">Content-type</span></span> | <span data-ttu-id="cfaeb-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="cfaeb-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cfaeb-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="cfaeb-127">Request body</span></span>

<span data-ttu-id="cfaeb-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="cfaeb-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cfaeb-129">响应</span><span class="sxs-lookup"><span data-stu-id="cfaeb-129">Response</span></span>

<span data-ttu-id="cfaeb-130">如果成功，此方法在响应正文中返回响应代码和请求的 `200 OK` [userFlow](../resources/identityuserflow.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="cfaeb-130">If successful, this method returns a `200 OK` response code and the requested [userFlow](../resources/identityuserflow.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cfaeb-131">示例</span><span class="sxs-lookup"><span data-stu-id="cfaeb-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="cfaeb-132">请求</span><span class="sxs-lookup"><span data-stu-id="cfaeb-132">Request</span></span>

<span data-ttu-id="cfaeb-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="cfaeb-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="cfaeb-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="cfaeb-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_identityuserflow"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identity/userFlows/B2C_1_Pol1
```
# <a name="c"></a>[<span data-ttu-id="cfaeb-135">C#</span><span class="sxs-lookup"><span data-stu-id="cfaeb-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-identityuserflow-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cfaeb-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cfaeb-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-identityuserflow-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cfaeb-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cfaeb-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-identityuserflow-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cfaeb-138">Java</span><span class="sxs-lookup"><span data-stu-id="cfaeb-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-identityuserflow-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="cfaeb-139">响应</span><span class="sxs-lookup"><span data-stu-id="cfaeb-139">Response</span></span>

<span data-ttu-id="cfaeb-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="cfaeb-140">The following is an example of the response.</span></span>

> <span data-ttu-id="cfaeb-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="cfaeb-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.UserFlow"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "B2C_1_Pol1",
    "userFlowType": "signUpOrSignIn",
    "userFlowTypeVersion": 1
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get UserFlow",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
   "suppressions": [
    "Error: get_identityuserflow/userFlowTypeVersion:\r\n      Expected type Single but actual was Int64. Property: userFlowTypeVersion, actual value: '1'"
  ]
}-->



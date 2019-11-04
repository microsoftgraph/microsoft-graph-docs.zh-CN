---
title: 列出 userFlows
description: 检索 userFlow 对象的列表。
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 585353891219f47666b980a532cd8a7d3dea3918
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938584"
---
# <a name="list-userflows"></a><span data-ttu-id="8001e-103">列出 userFlows</span><span class="sxs-lookup"><span data-stu-id="8001e-103">List userFlows</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8001e-104">检索[userflows](../resources/identityuserflow.md)的列表。</span><span class="sxs-lookup"><span data-stu-id="8001e-104">Retrieve a list of [userflows](../resources/identityuserflow.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="8001e-105">权限</span><span class="sxs-lookup"><span data-stu-id="8001e-105">Permissions</span></span>

<span data-ttu-id="8001e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8001e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8001e-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="8001e-108">Permission type</span></span>                        | <span data-ttu-id="8001e-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8001e-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="8001e-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8001e-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="8001e-111">IdentityUserFlow、IdentityUserFlow 和所有</span><span class="sxs-lookup"><span data-stu-id="8001e-111">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>  |
| <span data-ttu-id="8001e-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8001e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8001e-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="8001e-113">Not supported.</span></span> |
| <span data-ttu-id="8001e-114">Application</span><span class="sxs-lookup"><span data-stu-id="8001e-114">Application</span></span>                            | <span data-ttu-id="8001e-115">IdentityUserFlow、IdentityUserFlow 和所有</span><span class="sxs-lookup"><span data-stu-id="8001e-115">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8001e-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8001e-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/userFlows
```

## <a name="request-headers"></a><span data-ttu-id="8001e-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="8001e-117">Request headers</span></span>

| <span data-ttu-id="8001e-118">名称</span><span class="sxs-lookup"><span data-stu-id="8001e-118">Name</span></span>      |<span data-ttu-id="8001e-119">说明</span><span class="sxs-lookup"><span data-stu-id="8001e-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8001e-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="8001e-120">Authorization</span></span> | <span data-ttu-id="8001e-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8001e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8001e-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="8001e-123">Request body</span></span>

<span data-ttu-id="8001e-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8001e-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8001e-125">响应</span><span class="sxs-lookup"><span data-stu-id="8001e-125">Response</span></span>

<span data-ttu-id="8001e-126">如果成功，此方法在响应`200 OK`正文中返回响应代码和[userFlow](../resources/identityuserflow.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="8001e-126">If successful, this method returns a `200 OK` response code and a collection of [userFlow](../resources/identityuserflow.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8001e-127">示例</span><span class="sxs-lookup"><span data-stu-id="8001e-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8001e-128">请求</span><span class="sxs-lookup"><span data-stu-id="8001e-128">Request</span></span>

<span data-ttu-id="8001e-129">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="8001e-129">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="8001e-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="8001e-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_userflows"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identity/userFlows
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="8001e-131">C#</span><span class="sxs-lookup"><span data-stu-id="8001e-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-userflows-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8001e-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8001e-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-userflows-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8001e-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8001e-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-userflows-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8001e-134">响应</span><span class="sxs-lookup"><span data-stu-id="8001e-134">Response</span></span>

<span data-ttu-id="8001e-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="8001e-135">The following is an example of the response.</span></span>

> <span data-ttu-id="8001e-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="8001e-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

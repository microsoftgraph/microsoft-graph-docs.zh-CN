---
title: 获取 userFlow
description: 检索 userflow 对象的属性和关系。
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 6f671cc351675dfb2f62bfe3ad992facd8def402
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52040768"
---
# <a name="get-userflow"></a><span data-ttu-id="1fa13-103">获取 userFlow</span><span class="sxs-lookup"><span data-stu-id="1fa13-103">Get userFlow</span></span>

<span data-ttu-id="1fa13-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1fa13-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1fa13-105">检索 [userFlow](../resources/identityuserflow.md) 对象的属性和关联。</span><span class="sxs-lookup"><span data-stu-id="1fa13-105">Retrieve the properties and associations for an [userFlow](../resources/identityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="1fa13-106">权限</span><span class="sxs-lookup"><span data-stu-id="1fa13-106">Permissions</span></span>

<span data-ttu-id="1fa13-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1fa13-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1fa13-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="1fa13-109">Permission type</span></span>                        | <span data-ttu-id="1fa13-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1fa13-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="1fa13-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1fa13-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="1fa13-112">IdentityUserFlow.Read.All、IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1fa13-112">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span> |
| <span data-ttu-id="1fa13-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1fa13-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1fa13-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="1fa13-114">Not supported.</span></span> |
| <span data-ttu-id="1fa13-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="1fa13-115">Application</span></span>                            | <span data-ttu-id="1fa13-116">IdentityUserFlow.Read.All、IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1fa13-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1fa13-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1fa13-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/userFlows/{id}
```

## <a name="request-headers"></a><span data-ttu-id="1fa13-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="1fa13-118">Request headers</span></span>

| <span data-ttu-id="1fa13-119">名称</span><span class="sxs-lookup"><span data-stu-id="1fa13-119">Name</span></span>      |<span data-ttu-id="1fa13-120">说明</span><span class="sxs-lookup"><span data-stu-id="1fa13-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1fa13-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="1fa13-121">Authorization</span></span> | <span data-ttu-id="1fa13-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1fa13-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1fa13-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="1fa13-124">Content-type</span></span> | <span data-ttu-id="1fa13-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="1fa13-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1fa13-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="1fa13-127">Request body</span></span>

<span data-ttu-id="1fa13-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1fa13-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1fa13-129">响应</span><span class="sxs-lookup"><span data-stu-id="1fa13-129">Response</span></span>

<span data-ttu-id="1fa13-130">如果成功，此方法在响应正文中返回 响应代码和请求的 `200 OK` [userFlow](../resources/identityuserflow.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1fa13-130">If successful, this method returns a `200 OK` response code and the requested [userFlow](../resources/identityuserflow.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1fa13-131">示例</span><span class="sxs-lookup"><span data-stu-id="1fa13-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1fa13-132">请求</span><span class="sxs-lookup"><span data-stu-id="1fa13-132">Request</span></span>

<span data-ttu-id="1fa13-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="1fa13-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1fa13-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="1fa13-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_identityuserflow"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identity/userFlows/B2C_1_Pol1
```
# <a name="c"></a>[<span data-ttu-id="1fa13-135">C#</span><span class="sxs-lookup"><span data-stu-id="1fa13-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-identityuserflow-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1fa13-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1fa13-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-identityuserflow-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1fa13-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1fa13-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-identityuserflow-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1fa13-138">Java</span><span class="sxs-lookup"><span data-stu-id="1fa13-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-identityuserflow-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1fa13-139">响应</span><span class="sxs-lookup"><span data-stu-id="1fa13-139">Response</span></span>

<span data-ttu-id="1fa13-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="1fa13-140">The following is an example of the response.</span></span>

> <span data-ttu-id="1fa13-141">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="1fa13-141">**Note:** The response object shown here might be shortened for readability.</span></span>

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



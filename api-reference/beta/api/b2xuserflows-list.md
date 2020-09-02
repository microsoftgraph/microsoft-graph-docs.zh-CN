---
title: 列出 b2xUserFlows
description: 检索 b2xUserFlow 对象的列表。
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 135ce0d335be077e5673c39979f1fa198f97b440
ms.sourcegitcommit: 726f20403323be7d267b67c2764ed7c244e02ee1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/02/2020
ms.locfileid: "47329426"
---
# <a name="list-b2xuserflows"></a><span data-ttu-id="2a529-103">列出 b2xUserFlows</span><span class="sxs-lookup"><span data-stu-id="2a529-103">List b2xUserFlows</span></span>

<span data-ttu-id="2a529-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2a529-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2a529-105">检索 [b2xUserFlow](../resources/b2xuserflows.md) 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="2a529-105">Retrieve a list of [b2xUserFlow](../resources/b2xuserflows.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="2a529-106">权限</span><span class="sxs-lookup"><span data-stu-id="2a529-106">Permissions</span></span>

<span data-ttu-id="2a529-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2a529-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2a529-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="2a529-109">Permission type</span></span>      | <span data-ttu-id="2a529-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2a529-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2a529-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2a529-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2a529-112">IdentityUserFlow、IdentityUserFlow 和所有</span><span class="sxs-lookup"><span data-stu-id="2a529-112">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="2a529-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2a529-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="2a529-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="2a529-114">Not supported.</span></span>|
|<span data-ttu-id="2a529-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="2a529-115">Application</span></span>|<span data-ttu-id="2a529-116">IdentityUserFlow、IdentityUserFlow 和所有</span><span class="sxs-lookup"><span data-stu-id="2a529-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="2a529-117">工作或学校帐户需要属于下列角色之一：</span><span class="sxs-lookup"><span data-stu-id="2a529-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="2a529-118">全局管理员</span><span class="sxs-lookup"><span data-stu-id="2a529-118">Global administrator</span></span>
* <span data-ttu-id="2a529-119">外部标识用户流管理员</span><span class="sxs-lookup"><span data-stu-id="2a529-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="2a529-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2a529-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/b2xUserFlows
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2a529-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="2a529-121">Optional query parameters</span></span>

<span data-ttu-id="2a529-122">您可以使用 `$expand` 展开默认情况下不展开的特定用户流属性。</span><span class="sxs-lookup"><span data-stu-id="2a529-122">You can use `$expand` to expand specific user flow properties that are not expanded by default.</span></span>

<span data-ttu-id="2a529-123">有关详细信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="2a529-123">For more information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="2a529-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="2a529-124">Request headers</span></span>

|<span data-ttu-id="2a529-125">名称</span><span class="sxs-lookup"><span data-stu-id="2a529-125">Name</span></span>|<span data-ttu-id="2a529-126">说明</span><span class="sxs-lookup"><span data-stu-id="2a529-126">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="2a529-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="2a529-127">Authorization</span></span>|<span data-ttu-id="2a529-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2a529-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2a529-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="2a529-130">Request body</span></span>

<span data-ttu-id="2a529-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2a529-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2a529-132">响应</span><span class="sxs-lookup"><span data-stu-id="2a529-132">Response</span></span>

<span data-ttu-id="2a529-133">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [b2xUserFlow](../resources/b2xuserflows.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="2a529-133">If successful, this method returns a `200 OK` response code and a collection of [b2xUserFlow](../resources/b2xuserflows.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2a529-134">示例</span><span class="sxs-lookup"><span data-stu-id="2a529-134">Examples</span></span>

### <a name="example-1-list-all-b2xuserflows"></a><span data-ttu-id="2a529-135">示例1：列出所有 b2xUserFlows</span><span class="sxs-lookup"><span data-stu-id="2a529-135">Example 1: List all b2xUserFlows</span></span>

#### <a name="request"></a><span data-ttu-id="2a529-136">请求</span><span class="sxs-lookup"><span data-stu-id="2a529-136">Request</span></span>

<span data-ttu-id="2a529-137">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="2a529-137">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="2a529-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="2a529-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_b2xUserFlows"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2xUserFlows
```
# <a name="c"></a>[<span data-ttu-id="2a529-139">C#</span><span class="sxs-lookup"><span data-stu-id="2a529-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-b2xuserflows-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2a529-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2a529-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-b2xuserflows-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2a529-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2a529-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-b2xuserflows-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="2a529-142">响应</span><span class="sxs-lookup"><span data-stu-id="2a529-142">Response</span></span>

<span data-ttu-id="2a529-143">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="2a529-143">The following is an example of the response.</span></span>

<span data-ttu-id="2a529-144">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="2a529-144">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.b2xIdentityUserFlow",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identity/b2xUserFlows",
    "value": [
      {
          "id": "B2X_1_PartnerSignUp",
          "userFlowType": "signUpOrSignIn",
          "userFlowTypeVersion": 1
      },
      {
          "id": "B2X_1_ContosoSignUp",
          "userFlowType": "signUpOrSignIn",
          "userFlowTypeVersion": 1
      },
    ]
}
```

### <a name="example-2-list-all-b2xuserflows-and-expand-identityproviders"></a><span data-ttu-id="2a529-145">示例2：列出所有 b2xUserFlows 并展开 identityProviders</span><span class="sxs-lookup"><span data-stu-id="2a529-145">Example 2: List all b2xUserFlows and expand identityProviders</span></span>

#### <a name="request"></a><span data-ttu-id="2a529-146">请求</span><span class="sxs-lookup"><span data-stu-id="2a529-146">Request</span></span>

<span data-ttu-id="2a529-147">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="2a529-147">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="2a529-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="2a529-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_b2xUserFlows_expand"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2xUserFlows?$expand=identityProviders
```
# <a name="c"></a>[<span data-ttu-id="2a529-149">C#</span><span class="sxs-lookup"><span data-stu-id="2a529-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-b2xuserflows-expand-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2a529-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2a529-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-b2xuserflows-expand-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2a529-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2a529-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-b2xuserflows-expand-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="2a529-152">响应</span><span class="sxs-lookup"><span data-stu-id="2a529-152">Response</span></span>

<span data-ttu-id="2a529-153">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="2a529-153">The following is an example of the response.</span></span>

<span data-ttu-id="2a529-154">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="2a529-154">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.b2xIdentityUserFlow",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identity/b2xUserFlows(identityProviders)",
    "value": [
      {
          "id": "B2X_1_PartnerSignUp",
          "userFlowType": "signUpOrSignIn",
          "userFlowTypeVersion": 1,
          "identityProviders": [
              {
                "id": "Facebook-OAuth",
                "type": "Facebook",
                "name": "Facebook",
                "clientId": "clientIdFromFacebook",
                "clientSecret": "*******"
              }  
          ]
      },
      {
          "id": "B2X_1_ContosoSignUp",
          "userFlowType": "signUpOrSignIn",
          "userFlowTypeVersion": 1,
          "identityProviders": [
              {
                "id": "Facebook-OAuth",
                "type": "Facebook",
                "name": "Facebook",
                "clientId": "clientIdFromFacebook",
                "clientSecret": "*******"
              }  
          ]
      }
   ]
}
```

<!-- {
  "type": "#page.annotation",
  "description": "List b2xUserFlows",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: list_b2xUserFlows/container/userFlowTypeVersion:\r\n      Expected type Single but actual was Int64. Property: userFlowTypeVersion, actual value: '1'",
    "Error: list_b2xUserFlows_expand/container/userFlowTypeVersion:\r\n    Expected type Single but actual was Int64. Property: userFlowTypeVersion, actual value: '1'"
  ]
}-->

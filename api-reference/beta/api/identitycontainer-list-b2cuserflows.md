---
title: 列出 b2cIdentityUserFlows
description: 检索 b2cIdentityUserFlow 对象的列表。
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: identity-and-sign-in
ms.openlocfilehash: 6dfcdb67de89b298d98268b20c68b4d10dbef7b3
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50435551"
---
# <a name="list-b2cidentityuserflows"></a><span data-ttu-id="f0f8e-103">列出 b2cIdentityUserFlows</span><span class="sxs-lookup"><span data-stu-id="f0f8e-103">List b2cIdentityUserFlows</span></span>

<span data-ttu-id="f0f8e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f0f8e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f0f8e-105">检索 [b2cIdentityUserFlow 对象](../resources/b2cidentityuserflow.md) 的列表。</span><span class="sxs-lookup"><span data-stu-id="f0f8e-105">Retrieve a list of [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="f0f8e-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="f0f8e-106">Permissions</span></span>

<span data-ttu-id="f0f8e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f0f8e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f0f8e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f0f8e-109">Permission type</span></span>      | <span data-ttu-id="f0f8e-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f0f8e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f0f8e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f0f8e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f0f8e-112">IdentityUserFlow.Read.All、IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f0f8e-112">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="f0f8e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f0f8e-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="f0f8e-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f0f8e-114">Not supported.</span></span>|
|<span data-ttu-id="f0f8e-115">Application</span><span class="sxs-lookup"><span data-stu-id="f0f8e-115">Application</span></span>|<span data-ttu-id="f0f8e-116">IdentityUserFlow.Read.All、IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f0f8e-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="f0f8e-117">工作或学校帐户需要属于以下角色之一：</span><span class="sxs-lookup"><span data-stu-id="f0f8e-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="f0f8e-118">全局管理员</span><span class="sxs-lookup"><span data-stu-id="f0f8e-118">Global administrator</span></span>
* <span data-ttu-id="f0f8e-119">外部标识用户流管理员</span><span class="sxs-lookup"><span data-stu-id="f0f8e-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="f0f8e-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f0f8e-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/b2cUserFlows
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f0f8e-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="f0f8e-121">Optional query parameters</span></span>

<span data-ttu-id="f0f8e-122">可用于展开默认情况下未扩展 `$expand` 的特定用户流属性。</span><span class="sxs-lookup"><span data-stu-id="f0f8e-122">You can use `$expand` to expand specific user flow properties that are not expanded by default.</span></span>

<span data-ttu-id="f0f8e-123">有关详细信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="f0f8e-123">For more information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="f0f8e-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="f0f8e-124">Request headers</span></span>

|<span data-ttu-id="f0f8e-125">名称</span><span class="sxs-lookup"><span data-stu-id="f0f8e-125">Name</span></span>|<span data-ttu-id="f0f8e-126">说明</span><span class="sxs-lookup"><span data-stu-id="f0f8e-126">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="f0f8e-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="f0f8e-127">Authorization</span></span>|<span data-ttu-id="f0f8e-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f0f8e-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f0f8e-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="f0f8e-130">Request body</span></span>

<span data-ttu-id="f0f8e-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f0f8e-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f0f8e-132">响应</span><span class="sxs-lookup"><span data-stu-id="f0f8e-132">Response</span></span>

<span data-ttu-id="f0f8e-133">如果成功，此方法在响应正文中返回响应代码 `200 OK` 和 [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md)  对象集合。</span><span class="sxs-lookup"><span data-stu-id="f0f8e-133">If successful, this method returns a `200 OK` response code and a collection of [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md)  objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f0f8e-134">示例</span><span class="sxs-lookup"><span data-stu-id="f0f8e-134">Examples</span></span>

### <a name="example-1-list-all-b2cidentityuserflow-objects"></a><span data-ttu-id="f0f8e-135">示例 1：列出所有 b2cIdentityUserFlow 对象</span><span class="sxs-lookup"><span data-stu-id="f0f8e-135">Example 1: List all b2cIdentityUserFlow objects</span></span>

#### <a name="request"></a><span data-ttu-id="f0f8e-136">请求</span><span class="sxs-lookup"><span data-stu-id="f0f8e-136">Request</span></span>

<span data-ttu-id="f0f8e-137">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f0f8e-137">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="f0f8e-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="f0f8e-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_b2cUserFlows"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2cUserFlows
```
# <a name="c"></a>[<span data-ttu-id="f0f8e-139">C#</span><span class="sxs-lookup"><span data-stu-id="f0f8e-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-b2cuserflows-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f0f8e-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f0f8e-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-b2cuserflows-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f0f8e-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f0f8e-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-b2cuserflows-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f0f8e-142">Java</span><span class="sxs-lookup"><span data-stu-id="f0f8e-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-b2cuserflows-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="f0f8e-143">响应</span><span class="sxs-lookup"><span data-stu-id="f0f8e-143">Response</span></span>

<span data-ttu-id="f0f8e-144">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="f0f8e-144">The following is an example of the response.</span></span>

<span data-ttu-id="f0f8e-145">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="f0f8e-145">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.b2cIdentityUserFlow",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identity/b2cUserFlows",
    "value": [
      {
          "id": "B2C_1_CustomerSignUp",
          "userFlowType": "signUp",
          "userFlowTypeVersion": 1,
          "isLanguageCustomizationEnabled": false,
          "defaultLanguageTag": null
      },
      {
          "id": "B2C_1_CustomerSignIn",
          "userFlowType": "signIn",
          "userFlowTypeVersion": 1,
          "isLanguageCustomizationEnabled": true,
          "defaultLanguageTag": "en"
      },
    ]
}
```

### <a name="example-2-list-all-b2cidentityuserflow-objects-and-expand-identityproviders"></a><span data-ttu-id="f0f8e-146">示例 2：列出所有 b2cIdentityUserFlow 对象并展开 identityProviders</span><span class="sxs-lookup"><span data-stu-id="f0f8e-146">Example 2: List all b2cIdentityUserFlow objects and expand identityProviders</span></span>

#### <a name="request"></a><span data-ttu-id="f0f8e-147">请求</span><span class="sxs-lookup"><span data-stu-id="f0f8e-147">Request</span></span>

<span data-ttu-id="f0f8e-148">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f0f8e-148">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="f0f8e-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="f0f8e-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_b2cUserFlows_expand"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2cUserFlows?$expand=identityProviders
```
# <a name="c"></a>[<span data-ttu-id="f0f8e-150">C#</span><span class="sxs-lookup"><span data-stu-id="f0f8e-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-b2cuserflows-expand-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f0f8e-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f0f8e-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-b2cuserflows-expand-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f0f8e-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f0f8e-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-b2cuserflows-expand-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f0f8e-153">Java</span><span class="sxs-lookup"><span data-stu-id="f0f8e-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-b2cuserflows-expand-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="f0f8e-154">响应</span><span class="sxs-lookup"><span data-stu-id="f0f8e-154">Response</span></span>

<span data-ttu-id="f0f8e-155">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="f0f8e-155">The following is an example of the response.</span></span>

<span data-ttu-id="f0f8e-156">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="f0f8e-156">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.b2cIdentityUserFlow",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identity/b2cUserFlows",
    "value": [
      {
          "id": "B2C_1_CustomerSignUp",
          "userFlowType": "signUp",
          "userFlowTypeVersion": 1,
          "isLanguageCustomizationEnabled": false,
          "defaultLanguageTag": null,
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
          "id": "B2C_1_CustomerSignIn",
          "userFlowType": "signIn",
          "userFlowTypeVersion": 1,
          "isLanguageCustomizationEnabled": true,
          "defaultLanguageTag": "en",
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
  "description": "List b2cUserFlows",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: list_b2cUserFlows/container/userFlowTypeVersion:\r\n      Expected type Single but actual was Int64. Property: userFlowTypeVersion, actual value: '1'",
    "Error: list_b2cUserFlows_expand/container/userFlowTypeVersion:\r\n    Expected type Single but actual was Int64. Property: userFlowTypeVersion, actual value: '1'"
  ]
}-->



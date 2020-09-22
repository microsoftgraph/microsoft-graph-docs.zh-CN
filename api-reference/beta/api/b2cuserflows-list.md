---
title: 列出 b2cUserFlows
description: 检索 b2cUserFlow 对象的列表。
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 333dc0872e228ab1f2bd66570c780488ba4ee1a6
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47991458"
---
# <a name="list-b2cuserflows"></a><span data-ttu-id="e97c7-103">列出 b2cUserFlows</span><span class="sxs-lookup"><span data-stu-id="e97c7-103">List b2cUserFlows</span></span>

<span data-ttu-id="e97c7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e97c7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e97c7-105">检索 [b2cUserFlow](../resources/b2cuserflows.md) 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="e97c7-105">Retrieve a list of [b2cUserFlow](../resources/b2cuserflows.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="e97c7-106">权限</span><span class="sxs-lookup"><span data-stu-id="e97c7-106">Permissions</span></span>

<span data-ttu-id="e97c7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e97c7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e97c7-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="e97c7-109">Permission type</span></span>      | <span data-ttu-id="e97c7-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e97c7-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e97c7-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e97c7-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e97c7-112">IdentityUserFlow、IdentityUserFlow 和所有</span><span class="sxs-lookup"><span data-stu-id="e97c7-112">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="e97c7-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e97c7-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="e97c7-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="e97c7-114">Not supported.</span></span>|
|<span data-ttu-id="e97c7-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="e97c7-115">Application</span></span>|<span data-ttu-id="e97c7-116">IdentityUserFlow、IdentityUserFlow 和所有</span><span class="sxs-lookup"><span data-stu-id="e97c7-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="e97c7-117">工作或学校帐户需要属于下列角色之一：</span><span class="sxs-lookup"><span data-stu-id="e97c7-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="e97c7-118">全局管理员</span><span class="sxs-lookup"><span data-stu-id="e97c7-118">Global administrator</span></span>
* <span data-ttu-id="e97c7-119">外部标识用户流管理员</span><span class="sxs-lookup"><span data-stu-id="e97c7-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="e97c7-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e97c7-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/b2cUserFlows
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e97c7-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="e97c7-121">Optional query parameters</span></span>

<span data-ttu-id="e97c7-122">您可以使用 `$expand` 展开默认情况下不展开的特定用户流属性。</span><span class="sxs-lookup"><span data-stu-id="e97c7-122">You can use `$expand` to expand specific user flow properties that are not expanded by default.</span></span>

<span data-ttu-id="e97c7-123">有关详细信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="e97c7-123">For more information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="e97c7-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="e97c7-124">Request headers</span></span>

|<span data-ttu-id="e97c7-125">名称</span><span class="sxs-lookup"><span data-stu-id="e97c7-125">Name</span></span>|<span data-ttu-id="e97c7-126">说明</span><span class="sxs-lookup"><span data-stu-id="e97c7-126">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="e97c7-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="e97c7-127">Authorization</span></span>|<span data-ttu-id="e97c7-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e97c7-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e97c7-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="e97c7-130">Request body</span></span>

<span data-ttu-id="e97c7-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e97c7-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e97c7-132">响应</span><span class="sxs-lookup"><span data-stu-id="e97c7-132">Response</span></span>

<span data-ttu-id="e97c7-133">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [b2cUserFlow](../resources/b2cuserflows.md)  对象集合。</span><span class="sxs-lookup"><span data-stu-id="e97c7-133">If successful, this method returns a `200 OK` response code and a collection of [b2cUserFlow](../resources/b2cuserflows.md)  objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e97c7-134">示例</span><span class="sxs-lookup"><span data-stu-id="e97c7-134">Examples</span></span>

### <a name="example-1-list-all-b2cuserflows"></a><span data-ttu-id="e97c7-135">示例1：列出所有 b2cUserFlows</span><span class="sxs-lookup"><span data-stu-id="e97c7-135">Example 1: List all b2cUserFlows</span></span>

#### <a name="request"></a><span data-ttu-id="e97c7-136">请求</span><span class="sxs-lookup"><span data-stu-id="e97c7-136">Request</span></span>

<span data-ttu-id="e97c7-137">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e97c7-137">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="e97c7-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="e97c7-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_b2cUserFlows"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2cUserFlows
```
# <a name="c"></a>[<span data-ttu-id="e97c7-139">C#</span><span class="sxs-lookup"><span data-stu-id="e97c7-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-b2cuserflows-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e97c7-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e97c7-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-b2cuserflows-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e97c7-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e97c7-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-b2cuserflows-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e97c7-142">响应</span><span class="sxs-lookup"><span data-stu-id="e97c7-142">Response</span></span>

<span data-ttu-id="e97c7-143">下面介绍响应示例。</span><span class="sxs-lookup"><span data-stu-id="e97c7-143">The following is an example of the response.</span></span>

<span data-ttu-id="e97c7-144">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="e97c7-144">**Note:** The response object shown here might be shortened for readability.</span></span>

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
          "userFlowTypeVersion": 1
      },
      {
          "id": "B2C_1_CustomerSignIn",
          "userFlowType": "signIn",
          "userFlowTypeVersion": 1
      },
    ]
}
```

### <a name="example-2-list-all-b2cuserflows-and-expand-identityproviders"></a><span data-ttu-id="e97c7-145">示例2：列出所有 b2cUserFlows 并展开 identityProviders</span><span class="sxs-lookup"><span data-stu-id="e97c7-145">Example 2: List all b2cUserFlows and expand identityProviders</span></span>

#### <a name="request"></a><span data-ttu-id="e97c7-146">请求</span><span class="sxs-lookup"><span data-stu-id="e97c7-146">Request</span></span>

<span data-ttu-id="e97c7-147">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e97c7-147">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="e97c7-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="e97c7-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_b2cUserFlows_expand"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2cUserFlows?$expand=identityProviders
```
# <a name="c"></a>[<span data-ttu-id="e97c7-149">C#</span><span class="sxs-lookup"><span data-stu-id="e97c7-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-b2cuserflows-expand-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e97c7-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e97c7-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-b2cuserflows-expand-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e97c7-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e97c7-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-b2cuserflows-expand-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e97c7-152">响应</span><span class="sxs-lookup"><span data-stu-id="e97c7-152">Response</span></span>

<span data-ttu-id="e97c7-153">下面介绍响应示例。</span><span class="sxs-lookup"><span data-stu-id="e97c7-153">The following is an example of the response.</span></span>

<span data-ttu-id="e97c7-154">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="e97c7-154">**Note:** The response object shown here might be shortened for readability.</span></span>

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



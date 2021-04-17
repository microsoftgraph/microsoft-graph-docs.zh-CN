---
title: 列出 b2xIdentityUserFlows
description: 检索 b2xIdentityUserFlow 对象的列表。
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: identity-and-sign-in
ms.openlocfilehash: 36b0399c7fd45a90b5bbfb95084f46a15ff65296
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882817"
---
# <a name="list-b2xidentityuserflows"></a><span data-ttu-id="9159d-103">列出 b2xIdentityUserFlows</span><span class="sxs-lookup"><span data-stu-id="9159d-103">List b2xIdentityUserFlows</span></span>

<span data-ttu-id="9159d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9159d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9159d-105">检索 [b2xIdentityUserFlow 对象](../resources/b2xidentityuserflow.md) 的列表。</span><span class="sxs-lookup"><span data-stu-id="9159d-105">Retrieve a list of [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="9159d-106">权限</span><span class="sxs-lookup"><span data-stu-id="9159d-106">Permissions</span></span>

<span data-ttu-id="9159d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9159d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9159d-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="9159d-109">Permission type</span></span>      | <span data-ttu-id="9159d-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9159d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9159d-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9159d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9159d-112">IdentityUserFlow.Read.All、IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9159d-112">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="9159d-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9159d-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="9159d-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="9159d-114">Not supported.</span></span>|
|<span data-ttu-id="9159d-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="9159d-115">Application</span></span>|<span data-ttu-id="9159d-116">IdentityUserFlow.Read.All、IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9159d-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="9159d-117">工作或学校帐户需要属于以下角色之一：</span><span class="sxs-lookup"><span data-stu-id="9159d-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="9159d-118">全局管理员</span><span class="sxs-lookup"><span data-stu-id="9159d-118">Global administrator</span></span>
* <span data-ttu-id="9159d-119">外部标识用户流管理员</span><span class="sxs-lookup"><span data-stu-id="9159d-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="9159d-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9159d-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/b2xUserFlows
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9159d-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="9159d-121">Optional query parameters</span></span>

<span data-ttu-id="9159d-122">可以使用 展开 `$expand` 默认不展开的特定用户流属性。</span><span class="sxs-lookup"><span data-stu-id="9159d-122">You can use `$expand` to expand specific user flow properties that are not expanded by default.</span></span> <span data-ttu-id="9159d-123">有关详细信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="9159d-123">For more information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="9159d-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="9159d-124">Request headers</span></span>

|<span data-ttu-id="9159d-125">名称</span><span class="sxs-lookup"><span data-stu-id="9159d-125">Name</span></span>|<span data-ttu-id="9159d-126">说明</span><span class="sxs-lookup"><span data-stu-id="9159d-126">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="9159d-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="9159d-127">Authorization</span></span>|<span data-ttu-id="9159d-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9159d-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9159d-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="9159d-130">Request body</span></span>

<span data-ttu-id="9159d-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9159d-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9159d-132">响应</span><span class="sxs-lookup"><span data-stu-id="9159d-132">Response</span></span>

<span data-ttu-id="9159d-133">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="9159d-133">If successful, this method returns a `200 OK` response code and a collection of [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9159d-134">示例</span><span class="sxs-lookup"><span data-stu-id="9159d-134">Examples</span></span>

### <a name="example-1-list-all-b2xidentityuserflow-objects"></a><span data-ttu-id="9159d-135">示例 1：列出所有 b2xIdentityUserFlow 对象</span><span class="sxs-lookup"><span data-stu-id="9159d-135">Example 1: List all b2xIdentityUserFlow objects</span></span>

#### <a name="request"></a><span data-ttu-id="9159d-136">请求</span><span class="sxs-lookup"><span data-stu-id="9159d-136">Request</span></span>

<span data-ttu-id="9159d-137">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="9159d-137">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "list_b2xUserFlows"
}
-->

``` http
GET https://graph.microsoft.com/v1.0/identity/b2xUserFlows
```

#### <a name="response"></a><span data-ttu-id="9159d-138">响应</span><span class="sxs-lookup"><span data-stu-id="9159d-138">Response</span></span>

<span data-ttu-id="9159d-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="9159d-139">The following is an example of the response.</span></span>

<span data-ttu-id="9159d-140">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="9159d-140">**Note:** The response object shown here might be shortened for readability.</span></span>

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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identity/b2xUserFlows",
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

### <a name="example-2-list-all-b2xidentityuserflow-objects-and-expand-identityproviders"></a><span data-ttu-id="9159d-141">示例 2：列出所有 b2xIdentityUserFlow 对象并展开 identityProviders</span><span class="sxs-lookup"><span data-stu-id="9159d-141">Example 2: List all b2xIdentityUserFlow objects and expand identityProviders</span></span>

#### <a name="request"></a><span data-ttu-id="9159d-142">请求</span><span class="sxs-lookup"><span data-stu-id="9159d-142">Request</span></span>

<span data-ttu-id="9159d-143">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="9159d-143">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "list_b2xUserFlows_expand"
}
-->

``` http
GET https://graph.microsoft.com/v1.0/identity/b2xUserFlows?$expand=identityProviders
```

#### <a name="response"></a><span data-ttu-id="9159d-144">响应</span><span class="sxs-lookup"><span data-stu-id="9159d-144">Response</span></span>

<span data-ttu-id="9159d-145">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="9159d-145">The following is an example of the response.</span></span>

<span data-ttu-id="9159d-146">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="9159d-146">**Note:** The response object shown here might be shortened for readability.</span></span>

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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identity/b2xUserFlows(identityProviders)",
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

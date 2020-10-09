---
title: 获取 b2cIdentityUserFlow
description: 检索 b2cIdentityUserFlow 对象的属性和关系。
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: microsoft-identity-platform
ms.openlocfilehash: f95a79ec31b08649db541eb00505a24effe90e40
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/09/2020
ms.locfileid: "48406278"
---
# <a name="get-b2cidentityuserflow"></a><span data-ttu-id="fbd51-103">获取 b2cIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="fbd51-103">Get b2cIdentityUserFlow</span></span>

<span data-ttu-id="fbd51-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fbd51-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fbd51-105">检索 [b2cUserFlow](../resources/b2cidentityuserflow.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="fbd51-105">Retrieve the properties and relationships of a [b2cUserFlow](../resources/b2cidentityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="fbd51-106">权限</span><span class="sxs-lookup"><span data-stu-id="fbd51-106">Permissions</span></span>

<span data-ttu-id="fbd51-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fbd51-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fbd51-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="fbd51-109">Permission type</span></span>      | <span data-ttu-id="fbd51-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fbd51-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fbd51-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fbd51-111">Delegated (work or school account)</span></span>|<span data-ttu-id="fbd51-112">IdentityUserFlow、IdentityUserFlow 和所有</span><span class="sxs-lookup"><span data-stu-id="fbd51-112">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="fbd51-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fbd51-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="fbd51-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="fbd51-114">Not supported.</span></span>|
|<span data-ttu-id="fbd51-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="fbd51-115">Application</span></span>|<span data-ttu-id="fbd51-116">IdentityUserFlow、IdentityUserFlow 和所有</span><span class="sxs-lookup"><span data-stu-id="fbd51-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="fbd51-117">工作或学校帐户需要属于下列角色之一：</span><span class="sxs-lookup"><span data-stu-id="fbd51-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="fbd51-118">全局管理员</span><span class="sxs-lookup"><span data-stu-id="fbd51-118">Global administrator</span></span>
* <span data-ttu-id="fbd51-119">外部标识用户流管理员</span><span class="sxs-lookup"><span data-stu-id="fbd51-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="fbd51-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fbd51-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/b2cUserFlows/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fbd51-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="fbd51-121">Optional query parameters</span></span>

<span data-ttu-id="fbd51-122">您可以使用 `$expand` 展开默认情况下不展开的特定用户流属性。</span><span class="sxs-lookup"><span data-stu-id="fbd51-122">You can use `$expand` to expand specific user flow properties that are not expanded by default.</span></span>

<span data-ttu-id="fbd51-123">有关详细信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="fbd51-123">For more information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="fbd51-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="fbd51-124">Request headers</span></span>

|<span data-ttu-id="fbd51-125">名称</span><span class="sxs-lookup"><span data-stu-id="fbd51-125">Name</span></span>|<span data-ttu-id="fbd51-126">说明</span><span class="sxs-lookup"><span data-stu-id="fbd51-126">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="fbd51-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="fbd51-127">Authorization</span></span>|<span data-ttu-id="fbd51-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="fbd51-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fbd51-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="fbd51-130">Request body</span></span>

<span data-ttu-id="fbd51-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="fbd51-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fbd51-132">响应</span><span class="sxs-lookup"><span data-stu-id="fbd51-132">Response</span></span>

<span data-ttu-id="fbd51-133">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [B2CIDENTITYUSERFLOW](../resources/b2cidentityuserflow.md) 的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fbd51-133">If successful, this method returns a `200 OK` response code and a JSON representation of the [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fbd51-134">示例</span><span class="sxs-lookup"><span data-stu-id="fbd51-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="fbd51-135">请求</span><span class="sxs-lookup"><span data-stu-id="fbd51-135">Request</span></span>

<span data-ttu-id="fbd51-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="fbd51-136">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="fbd51-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="fbd51-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_b2cUserFlows"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2cUserFlows/{id}
```
# <a name="c"></a>[<span data-ttu-id="fbd51-138">C#</span><span class="sxs-lookup"><span data-stu-id="fbd51-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-b2cuserflows-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fbd51-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fbd51-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-b2cuserflows-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fbd51-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fbd51-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-b2cuserflows-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="fbd51-141">响应</span><span class="sxs-lookup"><span data-stu-id="fbd51-141">Response</span></span>

<span data-ttu-id="fbd51-142">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="fbd51-142">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.b2cIdentityUserFlow"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "B2C_1_CustomerSignUp",
    "userFlowType": "signUpOrSignIn",
    "userFlowTypeVersion": 1
}
```

<!-- {
  "type": "#page.annotation",
  "description": "Get b2cUserFlow",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: get_b2cUserFlows/userFlowTypeVersion:\r\n      Expected type Single but actual was Int64. Property: userFlowTypeVersion, actual value: '1'"
  ]
}-->



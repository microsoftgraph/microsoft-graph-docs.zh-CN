---
title: 获取 b2xIdentityUserFlow
description: 检索 b2xIdentityUserFlow 对象的属性和关系。
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: identity-and-sign-in
ms.openlocfilehash: fa7897b2e98da58b0280f09ebb70f320baaf6007
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/21/2021
ms.locfileid: "51919969"
---
# <a name="get-b2xidentityuserflow"></a><span data-ttu-id="1a33e-103">获取 b2xIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="1a33e-103">Get b2xIdentityUserFlow</span></span>

<span data-ttu-id="1a33e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1a33e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1a33e-105">检索 [b2xIdentityUserFlow 对象的属性和](../resources/b2xidentityuserflow.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="1a33e-105">Retrieve the properties and relationships of a [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="1a33e-106">权限</span><span class="sxs-lookup"><span data-stu-id="1a33e-106">Permissions</span></span>

<span data-ttu-id="1a33e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1a33e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1a33e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="1a33e-109">Permission type</span></span>      | <span data-ttu-id="1a33e-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1a33e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1a33e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1a33e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1a33e-112">IdentityUserFlow.Read.All、IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a33e-112">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="1a33e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1a33e-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="1a33e-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="1a33e-114">Not supported.</span></span>|
|<span data-ttu-id="1a33e-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="1a33e-115">Application</span></span>|<span data-ttu-id="1a33e-116">IdentityUserFlow.Read.All、IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a33e-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="1a33e-117">工作或学校帐户需要属于以下角色之一：</span><span class="sxs-lookup"><span data-stu-id="1a33e-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="1a33e-118">全局管理员</span><span class="sxs-lookup"><span data-stu-id="1a33e-118">Global administrator</span></span>
* <span data-ttu-id="1a33e-119">外部标识用户流管理员</span><span class="sxs-lookup"><span data-stu-id="1a33e-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="1a33e-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1a33e-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/b2xUserFlows/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1a33e-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="1a33e-121">Optional query parameters</span></span>

<span data-ttu-id="1a33e-122">可以使用 展开 `$expand` 默认不展开的特定用户流属性。</span><span class="sxs-lookup"><span data-stu-id="1a33e-122">You can use `$expand` to expand specific user flow properties that are not expanded by default.</span></span> <span data-ttu-id="1a33e-123">有关详细信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="1a33e-123">For more information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="1a33e-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="1a33e-124">Request headers</span></span>

|<span data-ttu-id="1a33e-125">名称</span><span class="sxs-lookup"><span data-stu-id="1a33e-125">Name</span></span>|<span data-ttu-id="1a33e-126">说明</span><span class="sxs-lookup"><span data-stu-id="1a33e-126">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="1a33e-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="1a33e-127">Authorization</span></span>|<span data-ttu-id="1a33e-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1a33e-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1a33e-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="1a33e-130">Request body</span></span>

<span data-ttu-id="1a33e-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1a33e-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1a33e-132">响应</span><span class="sxs-lookup"><span data-stu-id="1a33e-132">Response</span></span>

<span data-ttu-id="1a33e-133">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) 的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1a33e-133">If successful, this method returns a `200 OK` response code and a JSON representation of the [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1a33e-134">示例</span><span class="sxs-lookup"><span data-stu-id="1a33e-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="1a33e-135">请求</span><span class="sxs-lookup"><span data-stu-id="1a33e-135">Request</span></span>

<span data-ttu-id="1a33e-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="1a33e-136">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="1a33e-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="1a33e-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_b2xUserFlows"
}
-->

``` http
GET https://graph.microsoft.com/v1.0/identity/b2xUserFlows/B2X_1_PartnerSignUp
```
# <a name="c"></a>[<span data-ttu-id="1a33e-138">C#</span><span class="sxs-lookup"><span data-stu-id="1a33e-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-b2xuserflows-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1a33e-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1a33e-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-b2xuserflows-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1a33e-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1a33e-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-b2xuserflows-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1a33e-141">Java</span><span class="sxs-lookup"><span data-stu-id="1a33e-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-b2xuserflows-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1a33e-142">响应</span><span class="sxs-lookup"><span data-stu-id="1a33e-142">Response</span></span>

<span data-ttu-id="1a33e-143">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="1a33e-143">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.b2xIdentityUserFlow"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "B2X_1_PartnerSignUp",
    "userFlowType": "signUpOrSignIn",
    "userFlowTypeVersion": 1
}
```

<!-- {
  "type": "#page.annotation",
  "description": "Get b2xUserFlow",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: get_b2xUserFlows/userFlowTypeVersion:\r\n      Expected type Single but actual was Int64. Property: userFlowTypeVersion, actual value: '1'"
  ]
}-->

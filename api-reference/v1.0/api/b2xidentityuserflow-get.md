---
title: 获取 b2xIdentityUserFlow
description: 检索 b2xIdentityUserFlow 对象的属性和关系。
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: identity-and-sign-in
ms.openlocfilehash: a498e4a6ab1d652dca3c90afc33649f0c0ada908
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882399"
---
# <a name="get-b2xidentityuserflow"></a><span data-ttu-id="a1cde-103">获取 b2xIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="a1cde-103">Get b2xIdentityUserFlow</span></span>

<span data-ttu-id="a1cde-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a1cde-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a1cde-105">检索 [b2xIdentityUserFlow 对象的属性和](../resources/b2xidentityuserflow.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="a1cde-105">Retrieve the properties and relationships of a [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a1cde-106">权限</span><span class="sxs-lookup"><span data-stu-id="a1cde-106">Permissions</span></span>

<span data-ttu-id="a1cde-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a1cde-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a1cde-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="a1cde-109">Permission type</span></span>      | <span data-ttu-id="a1cde-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a1cde-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a1cde-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a1cde-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a1cde-112">IdentityUserFlow.Read.All、IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1cde-112">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="a1cde-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a1cde-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="a1cde-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="a1cde-114">Not supported.</span></span>|
|<span data-ttu-id="a1cde-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="a1cde-115">Application</span></span>|<span data-ttu-id="a1cde-116">IdentityUserFlow.Read.All、IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1cde-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="a1cde-117">工作或学校帐户需要属于以下角色之一：</span><span class="sxs-lookup"><span data-stu-id="a1cde-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="a1cde-118">全局管理员</span><span class="sxs-lookup"><span data-stu-id="a1cde-118">Global administrator</span></span>
* <span data-ttu-id="a1cde-119">外部标识用户流管理员</span><span class="sxs-lookup"><span data-stu-id="a1cde-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="a1cde-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a1cde-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/b2xUserFlows/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a1cde-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="a1cde-121">Optional query parameters</span></span>

<span data-ttu-id="a1cde-122">可以使用 展开 `$expand` 默认不展开的特定用户流属性。</span><span class="sxs-lookup"><span data-stu-id="a1cde-122">You can use `$expand` to expand specific user flow properties that are not expanded by default.</span></span> <span data-ttu-id="a1cde-123">有关详细信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="a1cde-123">For more information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="a1cde-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="a1cde-124">Request headers</span></span>

|<span data-ttu-id="a1cde-125">名称</span><span class="sxs-lookup"><span data-stu-id="a1cde-125">Name</span></span>|<span data-ttu-id="a1cde-126">说明</span><span class="sxs-lookup"><span data-stu-id="a1cde-126">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="a1cde-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="a1cde-127">Authorization</span></span>|<span data-ttu-id="a1cde-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a1cde-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a1cde-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="a1cde-130">Request body</span></span>

<span data-ttu-id="a1cde-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a1cde-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a1cde-132">响应</span><span class="sxs-lookup"><span data-stu-id="a1cde-132">Response</span></span>

<span data-ttu-id="a1cde-133">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) 的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a1cde-133">If successful, this method returns a `200 OK` response code and a JSON representation of the [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a1cde-134">示例</span><span class="sxs-lookup"><span data-stu-id="a1cde-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="a1cde-135">请求</span><span class="sxs-lookup"><span data-stu-id="a1cde-135">Request</span></span>

<span data-ttu-id="a1cde-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a1cde-136">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_b2xUserFlows"
}
-->

``` http
GET https://graph.microsoft.com/v1.0/identity/b2xUserFlows/B2X_1_PartnerSignUp
```

### <a name="response"></a><span data-ttu-id="a1cde-137">响应</span><span class="sxs-lookup"><span data-stu-id="a1cde-137">Response</span></span>

<span data-ttu-id="a1cde-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="a1cde-138">The following is an example of the response.</span></span>

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

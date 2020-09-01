---
title: 获取 b2cUserFlows
description: 检索 b2cUserFlow 对象的属性和关系。
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: microsoft-identity-platform
ms.openlocfilehash: ea558ddd1f8146b33eb5b153dfc0fcb73b21d6b1
ms.sourcegitcommit: 2c6e16dd8381945de6adf1eea020c142969b7801
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/01/2020
ms.locfileid: "47319681"
---
# <a name="get-b2cuserflow"></a><span data-ttu-id="7b883-103">获取 b2cUserFlow</span><span class="sxs-lookup"><span data-stu-id="7b883-103">Get b2cUserFlow</span></span>

<span data-ttu-id="7b883-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7b883-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7b883-105">检索 [b2cUserFlow](../resources/b2cuserflows.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="7b883-105">Retrieve the properties and relationships of a [b2cUserFlow](../resources/b2cuserflows.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="7b883-106">权限</span><span class="sxs-lookup"><span data-stu-id="7b883-106">Permissions</span></span>

<span data-ttu-id="7b883-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7b883-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7b883-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="7b883-109">Permission type</span></span>      | <span data-ttu-id="7b883-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7b883-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7b883-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7b883-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7b883-112">IdentityUserFlow、IdentityUserFlow 和所有</span><span class="sxs-lookup"><span data-stu-id="7b883-112">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="7b883-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7b883-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="7b883-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="7b883-114">Not supported.</span></span>|
|<span data-ttu-id="7b883-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="7b883-115">Application</span></span>|<span data-ttu-id="7b883-116">IdentityUserFlow、IdentityUserFlow 和所有</span><span class="sxs-lookup"><span data-stu-id="7b883-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="7b883-117">工作或学校帐户需要属于下列角色之一：</span><span class="sxs-lookup"><span data-stu-id="7b883-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="7b883-118">全局管理员</span><span class="sxs-lookup"><span data-stu-id="7b883-118">Global administrator</span></span>
* <span data-ttu-id="7b883-119">外部标识用户流管理员</span><span class="sxs-lookup"><span data-stu-id="7b883-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="7b883-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7b883-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/b2cUserFlows/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7b883-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="7b883-121">Optional query parameters</span></span>

<span data-ttu-id="7b883-122">您可以使用 `$expand` 展开默认情况下不展开的特定用户流属性。</span><span class="sxs-lookup"><span data-stu-id="7b883-122">You can use `$expand` to expand specific user flow properties that are not expanded by default.</span></span>

<span data-ttu-id="7b883-123">有关详细信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="7b883-123">For more information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="7b883-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="7b883-124">Request headers</span></span>

|<span data-ttu-id="7b883-125">名称</span><span class="sxs-lookup"><span data-stu-id="7b883-125">Name</span></span>|<span data-ttu-id="7b883-126">说明</span><span class="sxs-lookup"><span data-stu-id="7b883-126">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="7b883-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="7b883-127">Authorization</span></span>|<span data-ttu-id="7b883-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7b883-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7b883-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="7b883-130">Request body</span></span>

<span data-ttu-id="7b883-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7b883-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7b883-132">响应</span><span class="sxs-lookup"><span data-stu-id="7b883-132">Response</span></span>

<span data-ttu-id="7b883-133">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [B2CUSERFLOW](../resources/b2cuserflows.md) 的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7b883-133">If successful, this method returns a `200 OK` response code and a JSON representation of the [b2cUserFlow](../resources/b2cuserflows.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7b883-134">示例</span><span class="sxs-lookup"><span data-stu-id="7b883-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="7b883-135">请求</span><span class="sxs-lookup"><span data-stu-id="7b883-135">Request</span></span>

<span data-ttu-id="7b883-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="7b883-136">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_b2cUserFlows"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2cUserFlows/{id}
```

### <a name="response"></a><span data-ttu-id="7b883-137">响应</span><span class="sxs-lookup"><span data-stu-id="7b883-137">Response</span></span>

<span data-ttu-id="7b883-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="7b883-138">The following is an example of the response.</span></span>

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

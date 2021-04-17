---
title: 列出 identityProvider
description: 列出 b2xIdentityUserFlow 中所有 identityProviders。
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: identity-and-sign-in
ms.openlocfilehash: 01e1e3092c31d3bc9cef921e817da991e9b804cb
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882991"
---
# <a name="list-identityproviders"></a><span data-ttu-id="7c57a-103">列出 identityProvider</span><span class="sxs-lookup"><span data-stu-id="7c57a-103">List identityProviders</span></span>

<span data-ttu-id="7c57a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7c57a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7c57a-105">获取 [b2xIdentityUserFlow 对象中的标识](../resources/b2xidentityuserflow.md) 提供程序。</span><span class="sxs-lookup"><span data-stu-id="7c57a-105">Get the identity providers in a [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="7c57a-106">权限</span><span class="sxs-lookup"><span data-stu-id="7c57a-106">Permissions</span></span>

<span data-ttu-id="7c57a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7c57a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7c57a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="7c57a-109">Permission type</span></span>      | <span data-ttu-id="7c57a-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7c57a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7c57a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7c57a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7c57a-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7c57a-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="7c57a-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7c57a-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="7c57a-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="7c57a-114">Not supported.</span></span>|
|<span data-ttu-id="7c57a-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="7c57a-115">Application</span></span>| <span data-ttu-id="7c57a-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7c57a-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="7c57a-117">工作或学校帐户需要属于以下角色之一：</span><span class="sxs-lookup"><span data-stu-id="7c57a-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="7c57a-118">全局管理员</span><span class="sxs-lookup"><span data-stu-id="7c57a-118">Global administrator</span></span>
* <span data-ttu-id="7c57a-119">外部标识用户流管理员</span><span class="sxs-lookup"><span data-stu-id="7c57a-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="7c57a-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7c57a-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/b2xUserFlows/{id}/identityProviders
```

## <a name="request-headers"></a><span data-ttu-id="7c57a-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="7c57a-121">Request headers</span></span>

|<span data-ttu-id="7c57a-122">名称</span><span class="sxs-lookup"><span data-stu-id="7c57a-122">Name</span></span>|<span data-ttu-id="7c57a-123">说明</span><span class="sxs-lookup"><span data-stu-id="7c57a-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="7c57a-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="7c57a-124">Authorization</span></span>|<span data-ttu-id="7c57a-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7c57a-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7c57a-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="7c57a-127">Request body</span></span>

<span data-ttu-id="7c57a-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7c57a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7c57a-129">响应</span><span class="sxs-lookup"><span data-stu-id="7c57a-129">Response</span></span>

<span data-ttu-id="7c57a-130">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [identityProviders](../resources/identityprovider.md) 的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7c57a-130">If successful, this method returns a `200 OK` response code and a JSON representation of the [identityProviders](../resources/identityprovider.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7c57a-131">示例</span><span class="sxs-lookup"><span data-stu-id="7c57a-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="7c57a-132">请求</span><span class="sxs-lookup"><span data-stu-id="7c57a-132">Request</span></span>

<span data-ttu-id="7c57a-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="7c57a-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_b2xUserFlow_list_identityProviders"
}
-->

``` http
GET https://graph.microsoft.com/v1.0/identity/b2xUserFlows/B2X_1_Partner/identityProviders
```

### <a name="response"></a><span data-ttu-id="7c57a-134">响应</span><span class="sxs-lookup"><span data-stu-id="7c57a-134">Response</span></span>

<span data-ttu-id="7c57a-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="7c57a-135">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityProvider",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "id": "Facebook-OAuth",
            "type": "Facebook",
            "name": "Facebook",
            "clientId": "clientIdFromFacebook",
            "clientSecret": "*****"
        },
        {
            "id": "Google-OAuth",
            "type": "Google",
            "name": "Google",
            "clientId": "clientIdFromGoogle",
            "clientSecret": "*****"
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
 "description": "get_b2xuserflow_list_identityproviders",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

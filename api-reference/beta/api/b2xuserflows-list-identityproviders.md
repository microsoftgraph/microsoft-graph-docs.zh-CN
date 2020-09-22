---
title: 列出 b2xUserFlow 中的所有 identityProviders
description: 列出 b2xUserFlow 中的所有 identityProviders。
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: microsoft-identity-platform
ms.openlocfilehash: f8d040d4d27646a663f430ae66e1e40f1abbe78d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47991388"
---
# <a name="list-all-identityproviders-in-a-b2xuserflow"></a><span data-ttu-id="1f5bb-103">列出 b2xUserFlow 中的所有 identityProviders</span><span class="sxs-lookup"><span data-stu-id="1f5bb-103">List all identityProviders in a b2xUserFlow</span></span>

<span data-ttu-id="1f5bb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1f5bb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1f5bb-105">获取 [b2xUserFlow](../resources/b2xuserflows.md) 对象中的标识提供程序。</span><span class="sxs-lookup"><span data-stu-id="1f5bb-105">Get the identity providers in a [b2xUserFlow](../resources/b2xuserflows.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="1f5bb-106">权限</span><span class="sxs-lookup"><span data-stu-id="1f5bb-106">Permissions</span></span>

<span data-ttu-id="1f5bb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1f5bb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1f5bb-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="1f5bb-109">Permission type</span></span>      | <span data-ttu-id="1f5bb-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1f5bb-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1f5bb-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1f5bb-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1f5bb-112">IdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="1f5bb-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="1f5bb-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1f5bb-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="1f5bb-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="1f5bb-114">Not supported.</span></span>|
|<span data-ttu-id="1f5bb-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="1f5bb-115">Application</span></span>| <span data-ttu-id="1f5bb-116">IdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="1f5bb-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="1f5bb-117">工作或学校帐户需要属于下列角色之一：</span><span class="sxs-lookup"><span data-stu-id="1f5bb-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="1f5bb-118">全局管理员</span><span class="sxs-lookup"><span data-stu-id="1f5bb-118">Global administrator</span></span>
* <span data-ttu-id="1f5bb-119">外部标识用户流管理员</span><span class="sxs-lookup"><span data-stu-id="1f5bb-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="1f5bb-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1f5bb-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /b2xUserFlows/{id}/identityProviders
```

## <a name="request-headers"></a><span data-ttu-id="1f5bb-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="1f5bb-121">Request headers</span></span>

|<span data-ttu-id="1f5bb-122">名称</span><span class="sxs-lookup"><span data-stu-id="1f5bb-122">Name</span></span>|<span data-ttu-id="1f5bb-123">说明</span><span class="sxs-lookup"><span data-stu-id="1f5bb-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="1f5bb-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="1f5bb-124">Authorization</span></span>|<span data-ttu-id="1f5bb-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1f5bb-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1f5bb-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="1f5bb-127">Request body</span></span>

<span data-ttu-id="1f5bb-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1f5bb-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1f5bb-129">响应</span><span class="sxs-lookup"><span data-stu-id="1f5bb-129">Response</span></span>

<span data-ttu-id="1f5bb-130">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [IDENTITYPROVIDERS](../resources/identityprovider.md) 的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1f5bb-130">If successful, this method returns a `200 OK` response code and a JSON representation of the [identityProviders](../resources/identityprovider.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1f5bb-131">示例</span><span class="sxs-lookup"><span data-stu-id="1f5bb-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="1f5bb-132">请求</span><span class="sxs-lookup"><span data-stu-id="1f5bb-132">Request</span></span>

<span data-ttu-id="1f5bb-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="1f5bb-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="1f5bb-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="1f5bb-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_b2xUserFlow_list_identityProviders"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2xUserFlows/{id}/identityProviders
```
# <a name="c"></a>[<span data-ttu-id="1f5bb-135">C#</span><span class="sxs-lookup"><span data-stu-id="1f5bb-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-b2xuserflow-list-identityproviders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1f5bb-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1f5bb-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-b2xuserflow-list-identityproviders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1f5bb-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1f5bb-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-b2xuserflow-list-identityproviders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1f5bb-138">响应</span><span class="sxs-lookup"><span data-stu-id="1f5bb-138">Response</span></span>

<span data-ttu-id="1f5bb-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="1f5bb-139">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityProvider"
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



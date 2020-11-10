---
title: 列出 b2cIdentityUserFlow 中的所有 identityProviders
description: 列出 b2cIdentityUserFlow 中的所有 identityProviders。
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 91025d9b81e34bbfca3931617b864ac214a9875a
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48961196"
---
# <a name="list-all-identityproviders-in-a-b2cidentityuserflow"></a><span data-ttu-id="77450-103">列出 b2cIdentityUserFlow 中的所有 identityProviders</span><span class="sxs-lookup"><span data-stu-id="77450-103">List all identityProviders in a b2cIdentityUserFlow</span></span>

<span data-ttu-id="77450-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="77450-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="77450-105">获取 [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) 对象中的标识提供程序。</span><span class="sxs-lookup"><span data-stu-id="77450-105">Get the identity providers in a [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="77450-106">权限</span><span class="sxs-lookup"><span data-stu-id="77450-106">Permissions</span></span>

<span data-ttu-id="77450-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="77450-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="77450-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="77450-109">Permission type</span></span>      | <span data-ttu-id="77450-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="77450-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="77450-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="77450-111">Delegated (work or school account)</span></span>|<span data-ttu-id="77450-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77450-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="77450-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="77450-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="77450-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="77450-114">Not supported.</span></span>|
|<span data-ttu-id="77450-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="77450-115">Application</span></span>| <span data-ttu-id="77450-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77450-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="77450-117">工作或学校帐户需要属于下列角色之一：</span><span class="sxs-lookup"><span data-stu-id="77450-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="77450-118">全局管理员</span><span class="sxs-lookup"><span data-stu-id="77450-118">Global administrator</span></span>
* <span data-ttu-id="77450-119">外部标识用户流管理员</span><span class="sxs-lookup"><span data-stu-id="77450-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="77450-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="77450-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /b2cUserFlows/{id}/identityProviders
```

## <a name="request-headers"></a><span data-ttu-id="77450-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="77450-121">Request headers</span></span>

|<span data-ttu-id="77450-122">名称</span><span class="sxs-lookup"><span data-stu-id="77450-122">Name</span></span>|<span data-ttu-id="77450-123">说明</span><span class="sxs-lookup"><span data-stu-id="77450-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="77450-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="77450-124">Authorization</span></span>|<span data-ttu-id="77450-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="77450-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="77450-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="77450-127">Request body</span></span>

<span data-ttu-id="77450-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="77450-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="77450-129">响应</span><span class="sxs-lookup"><span data-stu-id="77450-129">Response</span></span>

<span data-ttu-id="77450-130">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [IDENTITYPROVIDERS](../resources/identityprovider.md) 的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="77450-130">If successful, this method returns a `200 OK` response code and a JSON representation of the [identityProviders](../resources/identityprovider.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="77450-131">示例</span><span class="sxs-lookup"><span data-stu-id="77450-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="77450-132">请求</span><span class="sxs-lookup"><span data-stu-id="77450-132">Request</span></span>

<span data-ttu-id="77450-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="77450-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="77450-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="77450-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_b2cUserFlow_list_identityProviders"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2cUserFlows/{id}/identityProviders
```
# <a name="c"></a>[<span data-ttu-id="77450-135">C#</span><span class="sxs-lookup"><span data-stu-id="77450-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-b2cuserflow-list-identityproviders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="77450-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="77450-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-b2cuserflow-list-identityproviders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="77450-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="77450-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-b2cuserflow-list-identityproviders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="77450-138">Java</span><span class="sxs-lookup"><span data-stu-id="77450-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-b2cuserflow-list-identityproviders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="77450-139">响应</span><span class="sxs-lookup"><span data-stu-id="77450-139">Response</span></span>

<span data-ttu-id="77450-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="77450-140">The following is an example of the response.</span></span>

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



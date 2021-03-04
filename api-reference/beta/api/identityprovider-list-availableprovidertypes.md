---
title: 列出 availableProviderTypes
description: 检索目录中所有可用的标识提供程序类型。
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: identity-and-sign-in
ms.openlocfilehash: ef78aea89344c480e9a0bc9a89e19144b7726ea0
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50435467"
---
# <a name="list-availableprovidertypes"></a><span data-ttu-id="1877f-103">列出 availableProviderTypes</span><span class="sxs-lookup"><span data-stu-id="1877f-103">List availableProviderTypes</span></span>

<span data-ttu-id="1877f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1877f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1877f-105">检索目录中可用的所有标识提供程序类型。</span><span class="sxs-lookup"><span data-stu-id="1877f-105">Retrieves all identity provider types available in a directory.</span></span>

## <a name="permissions"></a><span data-ttu-id="1877f-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="1877f-106">Permissions</span></span>

<span data-ttu-id="1877f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1877f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1877f-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="1877f-109">Permission type</span></span>      | <span data-ttu-id="1877f-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1877f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1877f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1877f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1877f-112">IdentityProvider.Read.All、IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1877f-112">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="1877f-113">委派（Microsoft 个人帐户）</span><span class="sxs-lookup"><span data-stu-id="1877f-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="1877f-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="1877f-114">Not supported.</span></span>|
|<span data-ttu-id="1877f-115">Application</span><span class="sxs-lookup"><span data-stu-id="1877f-115">Application</span></span>|<span data-ttu-id="1877f-116">IdentityProvider.Read.All、IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1877f-116">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|

<span data-ttu-id="1877f-117">工作或学校帐户需要属于以下角色之一：</span><span class="sxs-lookup"><span data-stu-id="1877f-117">The work or school account needs to belong to one of the following roles:</span></span>
* <span data-ttu-id="1877f-118">全局管理员</span><span class="sxs-lookup"><span data-stu-id="1877f-118">Global administrator</span></span>
* <span data-ttu-id="1877f-119">外部标识提供程序管理员</span><span class="sxs-lookup"><span data-stu-id="1877f-119">External Identity Provider administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="1877f-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1877f-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityProviders/availableProviderTypes
```

## <a name="request-headers"></a><span data-ttu-id="1877f-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="1877f-121">Request headers</span></span>

|<span data-ttu-id="1877f-122">名称</span><span class="sxs-lookup"><span data-stu-id="1877f-122">Name</span></span>|<span data-ttu-id="1877f-123">说明</span><span class="sxs-lookup"><span data-stu-id="1877f-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="1877f-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="1877f-124">Authorization</span></span>|<span data-ttu-id="1877f-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1877f-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1877f-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="1877f-127">Request body</span></span>
<span data-ttu-id="1877f-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1877f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1877f-129">响应</span><span class="sxs-lookup"><span data-stu-id="1877f-129">Response</span></span>

<span data-ttu-id="1877f-130">如果成功，此函数会在响应正文中返回 `200 OK` 响应代码和一个 String 集合。</span><span class="sxs-lookup"><span data-stu-id="1877f-130">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1877f-131">示例</span><span class="sxs-lookup"><span data-stu-id="1877f-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="1877f-132">请求</span><span class="sxs-lookup"><span data-stu-id="1877f-132">Request</span></span>
<span data-ttu-id="1877f-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="1877f-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="1877f-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="1877f-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "identityprovider_availableprovidertypes"
}
-->

``` http
GET https://graph.microsoft.com/beta/identityProviders/availableProviderTypes
```
# <a name="c"></a>[<span data-ttu-id="1877f-135">C#</span><span class="sxs-lookup"><span data-stu-id="1877f-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/identityprovider-availableprovidertypes-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1877f-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1877f-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/identityprovider-availableprovidertypes-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1877f-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1877f-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/identityprovider-availableprovidertypes-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1877f-138">Java</span><span class="sxs-lookup"><span data-stu-id="1877f-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/identityprovider-availableprovidertypes-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1877f-139">响应</span><span class="sxs-lookup"><span data-stu-id="1877f-139">Response</span></span>

<span data-ttu-id="1877f-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="1877f-140">The following is an example of the response.</span></span>

<span data-ttu-id="1877f-141">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="1877f-141">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(Edm.String)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
      "Amazon",
      "OpenIDConnect",
      "Facebook",
      "GitHub",
      "Google",
      "LinkedIn",
      "Microsoft",
      "QQ",
      "Twitter",
      "WeChat",
      "Weibo"
  ]
}
```



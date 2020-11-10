---
title: 列出 availableProviderTypes
description: 检索目录中所有可用的标识提供程序类型。
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 1f0297edc48e413865fc03ffe6d8f7bd5642f7b8
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48953417"
---
# <a name="list-availableprovidertypes"></a><span data-ttu-id="14b70-103">列出 availableProviderTypes</span><span class="sxs-lookup"><span data-stu-id="14b70-103">List availableProviderTypes</span></span>

<span data-ttu-id="14b70-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="14b70-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="14b70-105">检索目录中可用的所有标识提供程序类型。</span><span class="sxs-lookup"><span data-stu-id="14b70-105">Retrieves all identity provider types available in a directory.</span></span>

## <a name="permissions"></a><span data-ttu-id="14b70-106">权限</span><span class="sxs-lookup"><span data-stu-id="14b70-106">Permissions</span></span>

<span data-ttu-id="14b70-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="14b70-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="14b70-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="14b70-109">Permission type</span></span>      | <span data-ttu-id="14b70-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="14b70-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="14b70-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="14b70-111">Delegated (work or school account)</span></span>|<span data-ttu-id="14b70-112">IdentityProvider.Read.All、IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14b70-112">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="14b70-113">委派（Microsoft 个人帐户）</span><span class="sxs-lookup"><span data-stu-id="14b70-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="14b70-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="14b70-114">Not supported.</span></span>|
|<span data-ttu-id="14b70-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="14b70-115">Application</span></span>|<span data-ttu-id="14b70-116">IdentityProvider.Read.All、IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14b70-116">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|

<span data-ttu-id="14b70-117">工作或学校帐户需要属于下列角色之一：</span><span class="sxs-lookup"><span data-stu-id="14b70-117">The work or school account needs to belong to one of the following roles:</span></span>
* <span data-ttu-id="14b70-118">全局管理员</span><span class="sxs-lookup"><span data-stu-id="14b70-118">Global administrator</span></span>
* <span data-ttu-id="14b70-119">外部标识提供程序管理员</span><span class="sxs-lookup"><span data-stu-id="14b70-119">External Identity Provider administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="14b70-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="14b70-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityProviders/availableProviderTypes
```

## <a name="request-headers"></a><span data-ttu-id="14b70-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="14b70-121">Request headers</span></span>

|<span data-ttu-id="14b70-122">名称</span><span class="sxs-lookup"><span data-stu-id="14b70-122">Name</span></span>|<span data-ttu-id="14b70-123">说明</span><span class="sxs-lookup"><span data-stu-id="14b70-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="14b70-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="14b70-124">Authorization</span></span>|<span data-ttu-id="14b70-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="14b70-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="14b70-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="14b70-127">Request body</span></span>
<span data-ttu-id="14b70-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="14b70-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="14b70-129">响应</span><span class="sxs-lookup"><span data-stu-id="14b70-129">Response</span></span>

<span data-ttu-id="14b70-130">如果成功，此函数会在响应正文中返回 `200 OK` 响应代码和一个 String 集合。</span><span class="sxs-lookup"><span data-stu-id="14b70-130">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="14b70-131">示例</span><span class="sxs-lookup"><span data-stu-id="14b70-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="14b70-132">请求</span><span class="sxs-lookup"><span data-stu-id="14b70-132">Request</span></span>
<span data-ttu-id="14b70-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="14b70-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="14b70-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="14b70-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "identityprovider_availableprovidertypes"
}
-->

``` http
GET https://graph.microsoft.com/beta/identityProviders/availableProviderTypes
```
# <a name="c"></a>[<span data-ttu-id="14b70-135">C#</span><span class="sxs-lookup"><span data-stu-id="14b70-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/identityprovider-availableprovidertypes-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="14b70-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="14b70-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/identityprovider-availableprovidertypes-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="14b70-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="14b70-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/identityprovider-availableprovidertypes-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="14b70-138">Java</span><span class="sxs-lookup"><span data-stu-id="14b70-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/identityprovider-availableprovidertypes-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="14b70-139">响应</span><span class="sxs-lookup"><span data-stu-id="14b70-139">Response</span></span>

<span data-ttu-id="14b70-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="14b70-140">The following is an example of the response.</span></span>

<span data-ttu-id="14b70-141">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="14b70-141">**Note:** The response object shown here might be shortened for readability.</span></span>

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



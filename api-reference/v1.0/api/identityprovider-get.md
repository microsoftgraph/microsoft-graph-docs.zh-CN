---
title: 获取 identityProvider
description: 检索现有 identityProvider 中的属性
localization_priority: Priority
author: valnav
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 90c9cec4d7a3a0dff47de37b461e087103ed7081
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35277131"
---
# <a name="get-identityprovider"></a><span data-ttu-id="f03b5-103">获取 identityProvider</span><span class="sxs-lookup"><span data-stu-id="f03b5-103">Get identityProvider</span></span>

<span data-ttu-id="f03b5-104">检索现有 [identityProvider](../resources/identityprovider.md) 中的属性。</span><span class="sxs-lookup"><span data-stu-id="f03b5-104">Retrieve the properties of an existing [identityProvider](../resources/identityprovider.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f03b5-105">权限</span><span class="sxs-lookup"><span data-stu-id="f03b5-105">Permissions</span></span>

<span data-ttu-id="f03b5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f03b5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f03b5-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="f03b5-108">Permission type</span></span>      | <span data-ttu-id="f03b5-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f03b5-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f03b5-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f03b5-110">Delegated (work or school account)</span></span>|<span data-ttu-id="f03b5-111">IdentityProvider.Read.All、IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f03b5-111">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="f03b5-112">委派（Microsoft 个人帐户）</span><span class="sxs-lookup"><span data-stu-id="f03b5-112">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="f03b5-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="f03b5-113">Not supported.</span></span>|
|<span data-ttu-id="f03b5-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="f03b5-114">Application</span></span>|<span data-ttu-id="f03b5-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="f03b5-115">Not supported.</span></span>|

<span data-ttu-id="f03b5-116">工作或学校帐户必须是租户的全局管理员。</span><span class="sxs-lookup"><span data-stu-id="f03b5-116">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="f03b5-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f03b5-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /identityProviders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="f03b5-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="f03b5-118">Request headers</span></span>

|<span data-ttu-id="f03b5-119">名称</span><span class="sxs-lookup"><span data-stu-id="f03b5-119">Name</span></span>|<span data-ttu-id="f03b5-120">说明</span><span class="sxs-lookup"><span data-stu-id="f03b5-120">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="f03b5-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f03b5-121">Authorization</span></span>|<span data-ttu-id="f03b5-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f03b5-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f03b5-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="f03b5-124">Request body</span></span>

<span data-ttu-id="f03b5-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f03b5-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f03b5-126">响应</span><span class="sxs-lookup"><span data-stu-id="f03b5-126">Response</span></span>

<span data-ttu-id="f03b5-127">如果成功，则此方法将在响应正文中返回 `200 OK` 响应代码和 [identityProviders](../resources/identityprovider.md) 的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f03b5-127">If successful, this method returns `200 OK` response code and a JSON representation of the [identityProvider](../resources/identityprovider.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f03b5-128">示例</span><span class="sxs-lookup"><span data-stu-id="f03b5-128">Example</span></span>

<span data-ttu-id="f03b5-129">以下示例会检索特定的 **identityProvider**。</span><span class="sxs-lookup"><span data-stu-id="f03b5-129">The following example retrieves a specific **identityProvider**.</span></span>

##### <a name="request"></a><span data-ttu-id="f03b5-130">请求</span><span class="sxs-lookup"><span data-stu-id="f03b5-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get-identityprovider"
}-->
```http
GET https://graph.microsoft.com/v1.0/identityProviders/Amazon-OAuth
```

##### <a name="response"></a><span data-ttu-id="f03b5-131">响应</span><span class="sxs-lookup"><span data-stu-id="f03b5-131">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.IdentityProvider"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "Amazon-OAUTH",
    "type": "Amazon",
    "name": "Login with Amazon",
    "clientId": "56433757-cadd-4135-8431-2c9e3fd68ae8",
    "clientSecret": "*****"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="f03b5-132">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="f03b5-132">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="f03b5-133">C#</span><span class="sxs-lookup"><span data-stu-id="f03b5-133">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-identityprovider-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f03b5-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="f03b5-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-identityprovider-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="f03b5-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f03b5-135">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get-identityprovider-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get identityProvider",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/identityprovider-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/identityprovider-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/identityprovider-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->

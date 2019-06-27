---
title: 列出 identityProvider
description: 检索目录中的所有 identityProvider。
localization_priority: Normal
ms.openlocfilehash: c7ddabf8aef2a4d50f6ea133ecf696c8bdda922b
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35262662"
---
# <a name="list-identityproviders"></a><span data-ttu-id="1d890-103">列出 identityProvider</span><span class="sxs-lookup"><span data-stu-id="1d890-103">List identityProviders</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1d890-104">检索目录中的所有 [identityProvider](../resources/identityprovider.md)。</span><span class="sxs-lookup"><span data-stu-id="1d890-104">Retrieve all [identityProviders](../resources/identityprovider.md) in the directory.</span></span>

## <a name="permissions"></a><span data-ttu-id="1d890-105">权限</span><span class="sxs-lookup"><span data-stu-id="1d890-105">Permissions</span></span>

<span data-ttu-id="1d890-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1d890-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1d890-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="1d890-108">Permission type</span></span>      | <span data-ttu-id="1d890-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1d890-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1d890-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1d890-110">Delegated (work or school account)</span></span>|<span data-ttu-id="1d890-111">IdentityProvider.Read.All、IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1d890-111">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="1d890-112">委派（Microsoft 个人帐户）</span><span class="sxs-lookup"><span data-stu-id="1d890-112">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="1d890-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="1d890-113">Not supported.</span></span>|
|<span data-ttu-id="1d890-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="1d890-114">Application</span></span>|<span data-ttu-id="1d890-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="1d890-115">Not supported.</span></span>|

<span data-ttu-id="1d890-116">工作或学校帐户必须是租户的全局管理员。</span><span class="sxs-lookup"><span data-stu-id="1d890-116">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="1d890-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1d890-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /identityProviders
```

## <a name="request-headers"></a><span data-ttu-id="1d890-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="1d890-118">Request headers</span></span>

|<span data-ttu-id="1d890-119">名称</span><span class="sxs-lookup"><span data-stu-id="1d890-119">Name</span></span>|<span data-ttu-id="1d890-120">说明</span><span class="sxs-lookup"><span data-stu-id="1d890-120">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="1d890-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="1d890-121">Authorization</span></span>|<span data-ttu-id="1d890-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1d890-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1d890-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="1d890-124">Request body</span></span>

<span data-ttu-id="1d890-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1d890-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1d890-126">响应</span><span class="sxs-lookup"><span data-stu-id="1d890-126">Response</span></span>

<span data-ttu-id="1d890-127">如果成功，则此方法将在响应正文中返回 `200 OK` 响应代码和 JSON 表示形式的 [identityProviders](../resources/identityprovider.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="1d890-127">If successful, this method returns `200 OK` response code and a collection of [identityProviders](../resources/identityprovider.md) in JSON representation in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1d890-128">示例</span><span class="sxs-lookup"><span data-stu-id="1d890-128">Example</span></span>

<span data-ttu-id="1d890-129">以下示例会检索所有 **identityProvider**。</span><span class="sxs-lookup"><span data-stu-id="1d890-129">The following example retrieves all **identityProvider**.</span></span>

##### <a name="request"></a><span data-ttu-id="1d890-130">请求</span><span class="sxs-lookup"><span data-stu-id="1d890-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_identityproviders"
}-->
```http
GET https://graph.microsoft.com/beta/identityProviders
```

##### <a name="response"></a><span data-ttu-id="1d890-131">响应</span><span class="sxs-lookup"><span data-stu-id="1d890-131">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.IdentityProvider",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
      {
        "id": "Amazon-OAUTH",
        "name": "Login with Amazon",
        "type": "Amazon",
        "clientId": "56433757-cadd-4135-8431-2c9e3fd68ae8",
        "clientSecret": "*****"
      }
    ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="1d890-132">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="1d890-132">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="1d890-133">C#</span><span class="sxs-lookup"><span data-stu-id="1d890-133">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_identityproviders-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1d890-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="1d890-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_identityproviders-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="1d890-135">目标-C</span><span class="sxs-lookup"><span data-stu-id="1d890-135">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_identityproviders-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List identityProviders",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/identityprovider-list.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/identityprovider-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/identityprovider-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->

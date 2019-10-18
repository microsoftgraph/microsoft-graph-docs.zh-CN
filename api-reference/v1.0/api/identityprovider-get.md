---
title: 获取 identityProvider
description: 检索现有 identityProvider 中的属性
localization_priority: Priority
author: valnav
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 3c58fb35c929659c5b35134f080a92051b8b059d
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36726751"
---
# <a name="get-identityprovider"></a><span data-ttu-id="259cf-103">获取 identityProvider</span><span class="sxs-lookup"><span data-stu-id="259cf-103">Get identityProvider</span></span>

<span data-ttu-id="259cf-104">检索现有 [identityProvider](../resources/identityprovider.md) 中的属性。</span><span class="sxs-lookup"><span data-stu-id="259cf-104">Retrieve the properties of an existing [identityProvider](../resources/identityprovider.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="259cf-105">权限</span><span class="sxs-lookup"><span data-stu-id="259cf-105">Permissions</span></span>

<span data-ttu-id="259cf-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="259cf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="259cf-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="259cf-108">Permission type</span></span>      | <span data-ttu-id="259cf-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="259cf-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="259cf-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="259cf-110">Delegated (work or school account)</span></span>|<span data-ttu-id="259cf-111">IdentityProvider.Read.All、IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="259cf-111">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="259cf-112">委派（Microsoft 个人帐户）</span><span class="sxs-lookup"><span data-stu-id="259cf-112">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="259cf-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="259cf-113">Not supported.</span></span>|
|<span data-ttu-id="259cf-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="259cf-114">Application</span></span>|<span data-ttu-id="259cf-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="259cf-115">Not supported.</span></span>|

<span data-ttu-id="259cf-116">工作或学校帐户必须是租户的全局管理员。</span><span class="sxs-lookup"><span data-stu-id="259cf-116">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="259cf-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="259cf-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /identityProviders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="259cf-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="259cf-118">Request headers</span></span>

|<span data-ttu-id="259cf-119">名称</span><span class="sxs-lookup"><span data-stu-id="259cf-119">Name</span></span>|<span data-ttu-id="259cf-120">说明</span><span class="sxs-lookup"><span data-stu-id="259cf-120">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="259cf-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="259cf-121">Authorization</span></span>|<span data-ttu-id="259cf-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="259cf-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="259cf-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="259cf-124">Request body</span></span>

<span data-ttu-id="259cf-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="259cf-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="259cf-126">响应</span><span class="sxs-lookup"><span data-stu-id="259cf-126">Response</span></span>

<span data-ttu-id="259cf-127">如果成功，则此方法将在响应正文中返回 `200 OK` 响应代码和 [identityProviders](../resources/identityprovider.md) 的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="259cf-127">If successful, this method returns `200 OK` response code and a JSON representation of the [identityProvider](../resources/identityprovider.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="259cf-128">示例</span><span class="sxs-lookup"><span data-stu-id="259cf-128">Example</span></span>

<span data-ttu-id="259cf-129">以下示例会检索特定的 **identityProvider**。</span><span class="sxs-lookup"><span data-stu-id="259cf-129">The following example retrieves a specific **identityProvider**.</span></span>

##### <a name="request"></a><span data-ttu-id="259cf-130">请求</span><span class="sxs-lookup"><span data-stu-id="259cf-130">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="259cf-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="259cf-131">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-identityprovider"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/identityProviders/Amazon-OAuth
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="259cf-132">C#</span><span class="sxs-lookup"><span data-stu-id="259cf-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-identityprovider-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="259cf-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="259cf-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-identityprovider-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="259cf-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="259cf-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-identityprovider-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="259cf-135">Java</span><span class="sxs-lookup"><span data-stu-id="259cf-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-identityprovider-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="259cf-136">响应</span><span class="sxs-lookup"><span data-stu-id="259cf-136">Response</span></span>

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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get identityProvider",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

---
title: 获取 identityProvider
description: 检索现有 Identityprovider.read.all 的属性。
localization_priority: Normal
ms.openlocfilehash: c6f9468e800319e18368f5d6d6d8ed8b26240491
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35857632"
---
# <a name="get-identityprovider"></a><span data-ttu-id="b5a1d-103">获取 identityProvider</span><span class="sxs-lookup"><span data-stu-id="b5a1d-103">Get identityProvider</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b5a1d-104">检索现有 [identityProvider](../resources/identityprovider.md) 中的属性。</span><span class="sxs-lookup"><span data-stu-id="b5a1d-104">Retrieve the properties of an existing [identityProvider](../resources/identityprovider.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b5a1d-105">权限</span><span class="sxs-lookup"><span data-stu-id="b5a1d-105">Permissions</span></span>

<span data-ttu-id="b5a1d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b5a1d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b5a1d-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="b5a1d-108">Permission type</span></span>      | <span data-ttu-id="b5a1d-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b5a1d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b5a1d-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b5a1d-110">Delegated (work or school account)</span></span>|<span data-ttu-id="b5a1d-111">IdentityProvider.Read.All、IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5a1d-111">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="b5a1d-112">委派（Microsoft 个人帐户）</span><span class="sxs-lookup"><span data-stu-id="b5a1d-112">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="b5a1d-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="b5a1d-113">Not supported.</span></span>|
|<span data-ttu-id="b5a1d-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="b5a1d-114">Application</span></span>|<span data-ttu-id="b5a1d-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="b5a1d-115">Not supported.</span></span>|

<span data-ttu-id="b5a1d-116">工作或学校帐户必须是租户的全局管理员。</span><span class="sxs-lookup"><span data-stu-id="b5a1d-116">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="b5a1d-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b5a1d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /identityProviders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="b5a1d-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="b5a1d-118">Request headers</span></span>

|<span data-ttu-id="b5a1d-119">名称</span><span class="sxs-lookup"><span data-stu-id="b5a1d-119">Name</span></span>|<span data-ttu-id="b5a1d-120">说明</span><span class="sxs-lookup"><span data-stu-id="b5a1d-120">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="b5a1d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b5a1d-121">Authorization</span></span>|<span data-ttu-id="b5a1d-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b5a1d-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b5a1d-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="b5a1d-124">Request body</span></span>

<span data-ttu-id="b5a1d-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b5a1d-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b5a1d-126">响应</span><span class="sxs-lookup"><span data-stu-id="b5a1d-126">Response</span></span>

<span data-ttu-id="b5a1d-127">如果成功，则此方法将在响应正文中返回 `200 OK` 响应代码和 [identityProviders](../resources/identityprovider.md) 的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b5a1d-127">If successful, this method returns `200 OK` response code and a JSON representation of the [identityProvider](../resources/identityprovider.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b5a1d-128">示例</span><span class="sxs-lookup"><span data-stu-id="b5a1d-128">Example</span></span>

<span data-ttu-id="b5a1d-129">以下示例会检索特定的 **identityProvider**。</span><span class="sxs-lookup"><span data-stu-id="b5a1d-129">The following example retrieves a specific **identityProvider**.</span></span>

##### <a name="request"></a><span data-ttu-id="b5a1d-130">请求</span><span class="sxs-lookup"><span data-stu-id="b5a1d-130">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="b5a1d-131">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="b5a1d-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_identityprovider"
}-->
```http
GET https://graph.microsoft.com/beta/identityProviders/Amazon-OAuth
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b5a1d-132">C#</span><span class="sxs-lookup"><span data-stu-id="b5a1d-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-identityprovider-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b5a1d-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="b5a1d-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-identityprovider-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b5a1d-134">目标-C</span><span class="sxs-lookup"><span data-stu-id="b5a1d-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-identityprovider-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="b5a1d-135">Java</span><span class="sxs-lookup"><span data-stu-id="b5a1d-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-identityprovider-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="b5a1d-136">响应</span><span class="sxs-lookup"><span data-stu-id="b5a1d-136">Response</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "Get identityProvider",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

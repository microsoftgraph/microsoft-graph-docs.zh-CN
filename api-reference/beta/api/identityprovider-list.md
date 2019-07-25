---
title: 列出 identityProvider
description: 检索目录中的所有 identityProvider。
localization_priority: Normal
ms.openlocfilehash: ed70262efd04878d054852d5fa0f692afe6238e2
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35857604"
---
# <a name="list-identityproviders"></a><span data-ttu-id="6ac2e-103">列出 identityProvider</span><span class="sxs-lookup"><span data-stu-id="6ac2e-103">List identityProviders</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6ac2e-104">检索目录中的所有 [identityProvider](../resources/identityprovider.md)。</span><span class="sxs-lookup"><span data-stu-id="6ac2e-104">Retrieve all [identityProviders](../resources/identityprovider.md) in the directory.</span></span>

## <a name="permissions"></a><span data-ttu-id="6ac2e-105">权限</span><span class="sxs-lookup"><span data-stu-id="6ac2e-105">Permissions</span></span>

<span data-ttu-id="6ac2e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6ac2e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6ac2e-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="6ac2e-108">Permission type</span></span>      | <span data-ttu-id="6ac2e-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6ac2e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6ac2e-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6ac2e-110">Delegated (work or school account)</span></span>|<span data-ttu-id="6ac2e-111">IdentityProvider.Read.All、IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6ac2e-111">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="6ac2e-112">委派（Microsoft 个人帐户）</span><span class="sxs-lookup"><span data-stu-id="6ac2e-112">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="6ac2e-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="6ac2e-113">Not supported.</span></span>|
|<span data-ttu-id="6ac2e-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="6ac2e-114">Application</span></span>|<span data-ttu-id="6ac2e-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="6ac2e-115">Not supported.</span></span>|

<span data-ttu-id="6ac2e-116">工作或学校帐户必须是租户的全局管理员。</span><span class="sxs-lookup"><span data-stu-id="6ac2e-116">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="6ac2e-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6ac2e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /identityProviders
```

## <a name="request-headers"></a><span data-ttu-id="6ac2e-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="6ac2e-118">Request headers</span></span>

|<span data-ttu-id="6ac2e-119">名称</span><span class="sxs-lookup"><span data-stu-id="6ac2e-119">Name</span></span>|<span data-ttu-id="6ac2e-120">说明</span><span class="sxs-lookup"><span data-stu-id="6ac2e-120">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="6ac2e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="6ac2e-121">Authorization</span></span>|<span data-ttu-id="6ac2e-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6ac2e-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6ac2e-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="6ac2e-124">Request body</span></span>

<span data-ttu-id="6ac2e-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6ac2e-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6ac2e-126">响应</span><span class="sxs-lookup"><span data-stu-id="6ac2e-126">Response</span></span>

<span data-ttu-id="6ac2e-127">如果成功，则此方法将在响应正文中返回 `200 OK` 响应代码和 JSON 表示形式的 [identityProviders](../resources/identityprovider.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="6ac2e-127">If successful, this method returns `200 OK` response code and a collection of [identityProviders](../resources/identityprovider.md) in JSON representation in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6ac2e-128">示例</span><span class="sxs-lookup"><span data-stu-id="6ac2e-128">Example</span></span>

<span data-ttu-id="6ac2e-129">以下示例会检索所有 **identityProvider**。</span><span class="sxs-lookup"><span data-stu-id="6ac2e-129">The following example retrieves all **identityProvider**.</span></span>

##### <a name="request"></a><span data-ttu-id="6ac2e-130">请求</span><span class="sxs-lookup"><span data-stu-id="6ac2e-130">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="6ac2e-131">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="6ac2e-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_identityproviders"
}-->
```http
GET https://graph.microsoft.com/beta/identityProviders
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="6ac2e-132">C#</span><span class="sxs-lookup"><span data-stu-id="6ac2e-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-identityproviders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6ac2e-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="6ac2e-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-identityproviders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6ac2e-134">目标-C</span><span class="sxs-lookup"><span data-stu-id="6ac2e-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-identityproviders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="6ac2e-135">Java</span><span class="sxs-lookup"><span data-stu-id="6ac2e-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-identityproviders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="6ac2e-136">响应</span><span class="sxs-lookup"><span data-stu-id="6ac2e-136">Response</span></span>

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
  ]
}
-->

---
title: 列出 identityProvider
description: 检索目录中的所有 identityProvider。
localization_priority: Normal
doc_type: apiPageType
author: valnav
ms.prod: microsoft-identity-platform
ms.openlocfilehash: cc4974de221c0b05992012d90215a0e721656dfe
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42446486"
---
# <a name="list-identityproviders"></a><span data-ttu-id="75290-103">列出 identityProvider</span><span class="sxs-lookup"><span data-stu-id="75290-103">List identityProviders</span></span>

<span data-ttu-id="75290-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="75290-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="75290-105">检索目录中的所有 [identityProvider](../resources/identityprovider.md)。</span><span class="sxs-lookup"><span data-stu-id="75290-105">Retrieve all [identityProviders](../resources/identityprovider.md) in the directory.</span></span>

## <a name="permissions"></a><span data-ttu-id="75290-106">权限</span><span class="sxs-lookup"><span data-stu-id="75290-106">Permissions</span></span>

<span data-ttu-id="75290-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="75290-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="75290-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="75290-109">Permission type</span></span>      | <span data-ttu-id="75290-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="75290-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="75290-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="75290-111">Delegated (work or school account)</span></span>|<span data-ttu-id="75290-112">IdentityProvider.Read.All、IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75290-112">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="75290-113">委派（Microsoft 个人帐户）</span><span class="sxs-lookup"><span data-stu-id="75290-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="75290-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="75290-114">Not supported.</span></span>|
|<span data-ttu-id="75290-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="75290-115">Application</span></span>|<span data-ttu-id="75290-116">IdentityProvider.Read.All、IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75290-116">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|

<span data-ttu-id="75290-117">工作或学校帐户必须是租户的全局管理员。</span><span class="sxs-lookup"><span data-stu-id="75290-117">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="75290-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="75290-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /identityProviders
```

## <a name="request-headers"></a><span data-ttu-id="75290-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="75290-119">Request headers</span></span>

|<span data-ttu-id="75290-120">名称</span><span class="sxs-lookup"><span data-stu-id="75290-120">Name</span></span>|<span data-ttu-id="75290-121">说明</span><span class="sxs-lookup"><span data-stu-id="75290-121">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="75290-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="75290-122">Authorization</span></span>|<span data-ttu-id="75290-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="75290-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="75290-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="75290-125">Request body</span></span>

<span data-ttu-id="75290-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="75290-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="75290-127">响应</span><span class="sxs-lookup"><span data-stu-id="75290-127">Response</span></span>

<span data-ttu-id="75290-128">如果成功，则此方法将在响应正文中返回 `200 OK` 响应代码和 JSON 表示形式的 [identityProviders](../resources/identityprovider.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="75290-128">If successful, this method returns `200 OK` response code and a collection of [identityProviders](../resources/identityprovider.md) in JSON representation in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="75290-129">示例</span><span class="sxs-lookup"><span data-stu-id="75290-129">Example</span></span>

<span data-ttu-id="75290-130">以下示例会检索所有 **identityProvider**。</span><span class="sxs-lookup"><span data-stu-id="75290-130">The following example retrieves all **identityProvider**.</span></span>

##### <a name="request"></a><span data-ttu-id="75290-131">请求</span><span class="sxs-lookup"><span data-stu-id="75290-131">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="75290-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="75290-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_identityproviders"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/identityProviders
```
# <a name="c"></a>[<span data-ttu-id="75290-133">C#</span><span class="sxs-lookup"><span data-stu-id="75290-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-identityproviders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="75290-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="75290-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-identityproviders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="75290-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="75290-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-identityproviders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="75290-136">响应</span><span class="sxs-lookup"><span data-stu-id="75290-136">Response</span></span>

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

---
title: 获取 identityProvider
description: 检索现有 Identityprovider.read.all 的属性。
localization_priority: Normal
doc_type: apiPageType
author: Nickgmicrosoft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 670c745966f3fecfbbe837e0d8c176d67a436a45
ms.sourcegitcommit: ee41ba9ec6001716f1a9d575741bbeef577e2473
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/09/2020
ms.locfileid: "43199605"
---
# <a name="get-identityprovider"></a><span data-ttu-id="5758b-103">获取 identityProvider</span><span class="sxs-lookup"><span data-stu-id="5758b-103">Get identityProvider</span></span>

<span data-ttu-id="5758b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5758b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5758b-105">检索现有 [identityProvider](../resources/identityprovider.md) 中的属性。</span><span class="sxs-lookup"><span data-stu-id="5758b-105">Retrieve the properties of an existing [identityProvider](../resources/identityprovider.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="5758b-106">权限</span><span class="sxs-lookup"><span data-stu-id="5758b-106">Permissions</span></span>

<span data-ttu-id="5758b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5758b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5758b-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="5758b-109">Permission type</span></span>      | <span data-ttu-id="5758b-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5758b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5758b-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5758b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5758b-112">IdentityProvider.Read.All、IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5758b-112">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="5758b-113">委派（Microsoft 个人帐户）</span><span class="sxs-lookup"><span data-stu-id="5758b-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="5758b-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="5758b-114">Not supported.</span></span>|
|<span data-ttu-id="5758b-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="5758b-115">Application</span></span>|<span data-ttu-id="5758b-116">IdentityProvider.Read.All、IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5758b-116">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|

<span data-ttu-id="5758b-117">工作或学校帐户必须是租户的全局管理员。</span><span class="sxs-lookup"><span data-stu-id="5758b-117">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="5758b-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5758b-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /identityProviders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="5758b-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="5758b-119">Request headers</span></span>

|<span data-ttu-id="5758b-120">名称</span><span class="sxs-lookup"><span data-stu-id="5758b-120">Name</span></span>|<span data-ttu-id="5758b-121">说明</span><span class="sxs-lookup"><span data-stu-id="5758b-121">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="5758b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5758b-122">Authorization</span></span>|<span data-ttu-id="5758b-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5758b-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5758b-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="5758b-125">Request body</span></span>

<span data-ttu-id="5758b-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5758b-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5758b-127">响应</span><span class="sxs-lookup"><span data-stu-id="5758b-127">Response</span></span>

<span data-ttu-id="5758b-128">如果成功，则此方法将在响应正文中返回 `200 OK` 响应代码和 [identityProviders](../resources/identityprovider.md) 的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5758b-128">If successful, this method returns `200 OK` response code and a JSON representation of the [identityProvider](../resources/identityprovider.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5758b-129">示例</span><span class="sxs-lookup"><span data-stu-id="5758b-129">Example</span></span>

<span data-ttu-id="5758b-130">以下示例会检索特定的 **identityProvider**。</span><span class="sxs-lookup"><span data-stu-id="5758b-130">The following example retrieves a specific **identityProvider**.</span></span>

##### <a name="request"></a><span data-ttu-id="5758b-131">请求</span><span class="sxs-lookup"><span data-stu-id="5758b-131">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="5758b-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="5758b-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_identityprovider"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/identityProviders/Amazon-OAuth
```
# <a name="c"></a>[<span data-ttu-id="5758b-133">C#</span><span class="sxs-lookup"><span data-stu-id="5758b-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-identityprovider-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5758b-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5758b-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-identityprovider-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5758b-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5758b-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-identityprovider-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="5758b-136">响应</span><span class="sxs-lookup"><span data-stu-id="5758b-136">Response</span></span>

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

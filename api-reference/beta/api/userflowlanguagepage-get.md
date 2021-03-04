---
title: 获取 userFlowLanguagePage
description: 读取用户流中某一语言的 userFlowLanguagePage 对象中的值。
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 0848078f889b5d959cadb2ec5c403d1d1edf3cb9
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50433458"
---
# <a name="get-userflowlanguagepage"></a><span data-ttu-id="effaf-103">获取 userFlowLanguagePage</span><span class="sxs-lookup"><span data-stu-id="effaf-103">Get userFlowLanguagePage</span></span>

<span data-ttu-id="effaf-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="effaf-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="effaf-105">读取用户流中某一语言的 [userFlowLanguagePage](../resources/userflowlanguagepage.md) 对象中的值。</span><span class="sxs-lookup"><span data-stu-id="effaf-105">Read the values in a [userFlowLanguagePage](../resources/userflowlanguagepage.md) object for a language in a user flow.</span></span> <span data-ttu-id="effaf-106">这些值在用户流定义的用户旅程中向用户显示。</span><span class="sxs-lookup"><span data-stu-id="effaf-106">These values are shown to a user during a user journey defined by a user flow.</span></span>

## <a name="permissions"></a><span data-ttu-id="effaf-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="effaf-107">Permissions</span></span>

<span data-ttu-id="effaf-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="effaf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="effaf-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="effaf-110">Permission type</span></span>      | <span data-ttu-id="effaf-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="effaf-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="effaf-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="effaf-112">Delegated (work or school account)</span></span>|<span data-ttu-id="effaf-113">IdentityUserFlow.Read.All、IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="effaf-113">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="effaf-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="effaf-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="effaf-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="effaf-115">Not supported.</span></span>|
|<span data-ttu-id="effaf-116">Application</span><span class="sxs-lookup"><span data-stu-id="effaf-116">Application</span></span>|<span data-ttu-id="effaf-117">IdentityUserFlow.Read.All、IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="effaf-117">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="effaf-118">工作或学校帐户需要属于以下角色之一：</span><span class="sxs-lookup"><span data-stu-id="effaf-118">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="effaf-119">全局管理员</span><span class="sxs-lookup"><span data-stu-id="effaf-119">Global administrator</span></span>
* <span data-ttu-id="effaf-120">外部标识用户流管理员</span><span class="sxs-lookup"><span data-stu-id="effaf-120">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="effaf-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="effaf-121">HTTP request</span></span>

<span data-ttu-id="effaf-122">若要引用对象中的内容，必须使用 `$value` 。</span><span class="sxs-lookup"><span data-stu-id="effaf-122">To reference the content within the object, you must use `$value`.</span></span> <span data-ttu-id="effaf-123">这将返回对象中的内容，并允许你直接引用它。</span><span class="sxs-lookup"><span data-stu-id="effaf-123">This returns the content within the object and allows you to reference it directly.</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /identity/b2cUserFlows/{id}/languages/{id}/defaultPages/{id}/$value
GET /identity/b2cUserFlows/{id}/languages/{id}/overridesPages/{id}/$value
GET /identity/b2xUserFlows/{id}/languages/{id}/defaultPages/{id}/$value
GET /identity/b2xUserFlows/{id}/languages/{id}/overridesPages/{id}/$value
```

## <a name="request-headers"></a><span data-ttu-id="effaf-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="effaf-124">Request headers</span></span>

|<span data-ttu-id="effaf-125">名称</span><span class="sxs-lookup"><span data-stu-id="effaf-125">Name</span></span>|<span data-ttu-id="effaf-126">说明</span><span class="sxs-lookup"><span data-stu-id="effaf-126">Description</span></span>|
|:---|:---|
|<span data-ttu-id="effaf-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="effaf-127">Authorization</span></span>|<span data-ttu-id="effaf-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="effaf-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="effaf-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="effaf-130">Request body</span></span>

<span data-ttu-id="effaf-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="effaf-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="effaf-132">响应</span><span class="sxs-lookup"><span data-stu-id="effaf-132">Response</span></span>

<span data-ttu-id="effaf-133">如果成功，此方法在响应正文中返回响应代码和 `200 OK` [userFlowLanguagePage](../resources/userflowlanguagepage.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="effaf-133">If successful, this method returns a `200 OK` response code and a [userFlowLanguagePage](../resources/userflowlanguagepage.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="effaf-134">示例</span><span class="sxs-lookup"><span data-stu-id="effaf-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="effaf-135">请求</span><span class="sxs-lookup"><span data-stu-id="effaf-135">Request</span></span>

<span data-ttu-id="effaf-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="effaf-136">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="effaf-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="effaf-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_userflowlanguagepage"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2cUserFlows/B2C_1_Customer/languages/en/defaultPages/idpselections/$value
```
# <a name="c"></a>[<span data-ttu-id="effaf-138">C#</span><span class="sxs-lookup"><span data-stu-id="effaf-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-userflowlanguagepage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="effaf-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="effaf-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-userflowlanguagepage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="effaf-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="effaf-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-userflowlanguagepage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="effaf-141">Java</span><span class="sxs-lookup"><span data-stu-id="effaf-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-userflowlanguagepage-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="effaf-142">响应</span><span class="sxs-lookup"><span data-stu-id="effaf-142">Response</span></span>

<span data-ttu-id="effaf-143">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="effaf-143">The following is an example of the response.</span></span>

<span data-ttu-id="effaf-144">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="effaf-144">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.userFlowLanguagePage"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "LocalizedStrings": [
      {
        "ElementType": "ClaimsProvider",
        "ElementId": null,
        "StringId": "AmazonExchange",
        "Override": false,
        "Value": "Amazon"
      },
      {
        "ElementType": "ClaimsProvider",
        "ElementId": null,
        "StringId": "FacebookExchange",
        "Override": false,
        "Value": "Facebook"
      }
   ]
}
```

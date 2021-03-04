---
title: 列表语言
description: 检索 B2C 用户流中支持自定义的语言列表。
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: e3b04b25796b7864d6dda74eaa7b2edc14b30c93
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50438293"
---
# <a name="list-languages"></a><span data-ttu-id="4b522-103">列表语言</span><span class="sxs-lookup"><span data-stu-id="4b522-103">List languages</span></span>

<span data-ttu-id="4b522-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4b522-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4b522-105">检索 Azure AD B2C 用户流中支持自定义的语言列表。</span><span class="sxs-lookup"><span data-stu-id="4b522-105">Retrieve a list of languages supported for customization in an Azure AD B2C user flow.</span></span>

<span data-ttu-id="4b522-106">**注意：** 若要检索支持自定义的语言列表，必须先对 Azure AD B2C 用户流启用语言自定义。</span><span class="sxs-lookup"><span data-stu-id="4b522-106">**Note:** To retrieve a list of languages supported for customization, you must first enable language customization on your Azure AD B2C user flow.</span></span> <span data-ttu-id="4b522-107">有关详细信息，请参阅 [Update b2cIdentityUserFlow](../api/b2cidentityuserflow-update.md)。</span><span class="sxs-lookup"><span data-stu-id="4b522-107">For more information, see [Update b2cIdentityUserFlow](../api/b2cidentityuserflow-update.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="4b522-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="4b522-108">Permissions</span></span>

<span data-ttu-id="4b522-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4b522-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4b522-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="4b522-111">Permission type</span></span>      | <span data-ttu-id="4b522-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4b522-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4b522-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4b522-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4b522-114">IdentityUserFlow.Read.All、IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b522-114">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="4b522-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4b522-115">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="4b522-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="4b522-116">Not supported.</span></span>|
|<span data-ttu-id="4b522-117">Application</span><span class="sxs-lookup"><span data-stu-id="4b522-117">Application</span></span>|<span data-ttu-id="4b522-118">IdentityUserFlow.Read.All、IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b522-118">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="4b522-119">工作或学校帐户需要属于以下角色之一：</span><span class="sxs-lookup"><span data-stu-id="4b522-119">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="4b522-120">全局管理员</span><span class="sxs-lookup"><span data-stu-id="4b522-120">Global administrator</span></span>
* <span data-ttu-id="4b522-121">外部标识用户流管理员</span><span class="sxs-lookup"><span data-stu-id="4b522-121">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="4b522-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4b522-122">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /identity/b2cUserFlows/{id}/languages
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4b522-123">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="4b522-123">Optional query parameters</span></span>

<span data-ttu-id="4b522-124">此方法支持 `$filter` 查询参数只显示已启用的语言。</span><span class="sxs-lookup"><span data-stu-id="4b522-124">This method supports the `$filter` query parameter to show only the enabled languages.</span></span> <span data-ttu-id="4b522-125">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="4b522-125">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="4b522-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="4b522-126">Request headers</span></span>

|<span data-ttu-id="4b522-127">名称</span><span class="sxs-lookup"><span data-stu-id="4b522-127">Name</span></span>|<span data-ttu-id="4b522-128">说明</span><span class="sxs-lookup"><span data-stu-id="4b522-128">Description</span></span>|
|:---|:---|
|<span data-ttu-id="4b522-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="4b522-129">Authorization</span></span>|<span data-ttu-id="4b522-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4b522-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4b522-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="4b522-132">Request body</span></span>

<span data-ttu-id="4b522-133">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4b522-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4b522-134">响应</span><span class="sxs-lookup"><span data-stu-id="4b522-134">Response</span></span>

<span data-ttu-id="4b522-135">如果成功，此方法在响应正文中返回响应代码和 `200 OK` [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="4b522-135">If successful, this method returns a `200 OK` response code and a collection of [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4b522-136">示例</span><span class="sxs-lookup"><span data-stu-id="4b522-136">Examples</span></span>

### <a name="example-1-retrieve-a-list-of-all-languages"></a><span data-ttu-id="4b522-137">示例 1：检索所有语言的列表</span><span class="sxs-lookup"><span data-stu-id="4b522-137">Example 1: Retrieve a list of all languages</span></span>

#### <a name="request"></a><span data-ttu-id="4b522-138">请求</span><span class="sxs-lookup"><span data-stu-id="4b522-138">Request</span></span>

<span data-ttu-id="4b522-139">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="4b522-139">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="4b522-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="4b522-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_userflowlanguageconfiguration"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2cUserFlows/B2C_1_CustomerSignUp/languages
```
# <a name="c"></a>[<span data-ttu-id="4b522-141">C#</span><span class="sxs-lookup"><span data-stu-id="4b522-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-userflowlanguageconfiguration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4b522-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4b522-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-userflowlanguageconfiguration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4b522-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4b522-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-userflowlanguageconfiguration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4b522-144">Java</span><span class="sxs-lookup"><span data-stu-id="4b522-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-userflowlanguageconfiguration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="4b522-145">响应</span><span class="sxs-lookup"><span data-stu-id="4b522-145">Response</span></span>

<span data-ttu-id="4b522-146">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="4b522-146">The following is an example of the response.</span></span>

<span data-ttu-id="4b522-147">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="4b522-147">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.userFlowLanguageConfiguration)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "odata.context": "https://graph.microsoft.com/beta/$metadata#identity/b2cUserFlows('B2C_1_CustomerSignUp')/languages",
  "value": [
    {
      "id": "en",
      "isEnabled": true,
      "displayName": "English"
    },
    {
      "id": "de",
      "isEnabled": false,
      "displayName": "Deutsch"
    }
  ]
}
```

### <a name="example-2-retrieve-a-list-of-only-enabled-languages"></a><span data-ttu-id="4b522-148">示例 2：检索仅启用语言的列表</span><span class="sxs-lookup"><span data-stu-id="4b522-148">Example 2: Retrieve a list of only enabled languages</span></span>

#### <a name="request"></a><span data-ttu-id="4b522-149">请求</span><span class="sxs-lookup"><span data-stu-id="4b522-149">Request</span></span>

<span data-ttu-id="4b522-150">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="4b522-150">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="4b522-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="4b522-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_userflowlanguageconfiguration_filter"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2cUserFlows/B2C_1_CustomerSignUp/languages?$filter=isEnabled eq true
```
# <a name="c"></a>[<span data-ttu-id="4b522-152">C#</span><span class="sxs-lookup"><span data-stu-id="4b522-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-userflowlanguageconfiguration-filter-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4b522-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4b522-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-userflowlanguageconfiguration-filter-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4b522-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4b522-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-userflowlanguageconfiguration-filter-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4b522-155">Java</span><span class="sxs-lookup"><span data-stu-id="4b522-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-userflowlanguageconfiguration-filter-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="4b522-156">响应</span><span class="sxs-lookup"><span data-stu-id="4b522-156">Response</span></span>

<span data-ttu-id="4b522-157">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="4b522-157">The following is an example of the response.</span></span>

<span data-ttu-id="4b522-158">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="4b522-158">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.userFlowLanguageConfiguration)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "odata.context": "https://graph.microsoft.com/beta/$metadata#identity/b2cUserFlows('B2C_1_CustomerSignUp')/languages",
  "value": [
    {
      "id": "en",
      "isEnabled": true,
      "displayName": "English"
    }
  ]
}
```

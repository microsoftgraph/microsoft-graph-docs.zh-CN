---
title: 获取 homeRealmDiscoveryPolicy
description: 检索 homeRealmDiscoveryPolicy 对象的属性和关系。
localization_priority: Normal
author: hpsin
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: bdd96dbd20429e0175f2d075f5e0abf6a95b764c
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52039592"
---
# <a name="get-homerealmdiscoverypolicy"></a><span data-ttu-id="aa54c-103">获取 homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="aa54c-103">Get homeRealmDiscoveryPolicy</span></span>

<span data-ttu-id="aa54c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aa54c-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="aa54c-105">检索 [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="aa54c-105">Retrieve the properties and relationships of a [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="aa54c-106">权限</span><span class="sxs-lookup"><span data-stu-id="aa54c-106">Permissions</span></span>

<span data-ttu-id="aa54c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="aa54c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="aa54c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="aa54c-109">Permission type</span></span>                        | <span data-ttu-id="aa54c-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="aa54c-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="aa54c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="aa54c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="aa54c-112">Policy.Read.All、Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="aa54c-112">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="aa54c-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="aa54c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aa54c-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="aa54c-114">Not supported.</span></span> |
| <span data-ttu-id="aa54c-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="aa54c-115">Application</span></span>                            | <span data-ttu-id="aa54c-116">Policy.Read.All、Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="aa54c-116">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="aa54c-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="aa54c-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/homeRealmDiscoveryPolicies/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="aa54c-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="aa54c-118">Optional query parameters</span></span>

<span data-ttu-id="aa54c-119">此方法支持 `$expand` 和 `$select` OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="aa54c-119">This method supports the `$expand` and `$select` OData query parameters to help customize the response.</span></span> <span data-ttu-id="aa54c-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="aa54c-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span> <span data-ttu-id="aa54c-121">使用 `$expand` 时，请确保你的应用请求读取扩展对象的权限。</span><span class="sxs-lookup"><span data-stu-id="aa54c-121">When using `$expand`, make sure that your app requests permissions to read the expanded objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="aa54c-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="aa54c-122">Request headers</span></span>

| <span data-ttu-id="aa54c-123">名称</span><span class="sxs-lookup"><span data-stu-id="aa54c-123">Name</span></span>      |<span data-ttu-id="aa54c-124">说明</span><span class="sxs-lookup"><span data-stu-id="aa54c-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="aa54c-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="aa54c-125">Authorization</span></span> | <span data-ttu-id="aa54c-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="aa54c-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="aa54c-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="aa54c-128">Request body</span></span>

<span data-ttu-id="aa54c-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="aa54c-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="aa54c-130">响应</span><span class="sxs-lookup"><span data-stu-id="aa54c-130">Response</span></span>

<span data-ttu-id="aa54c-131">如果成功，此方法在响应正文中返回 响应代码和请求的 `200 OK` [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="aa54c-131">If successful, this method returns a `200 OK` response code and the requested [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="aa54c-132">示例</span><span class="sxs-lookup"><span data-stu-id="aa54c-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="aa54c-133">请求</span><span class="sxs-lookup"><span data-stu-id="aa54c-133">Request</span></span>

<span data-ttu-id="aa54c-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="aa54c-134">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="aa54c-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="aa54c-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_homerealmdiscoverypolicy"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/policies/homeRealmDiscoveryPolicies/{id}
```
# <a name="c"></a>[<span data-ttu-id="aa54c-136">C#</span><span class="sxs-lookup"><span data-stu-id="aa54c-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-homerealmdiscoverypolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="aa54c-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="aa54c-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-homerealmdiscoverypolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="aa54c-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="aa54c-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-homerealmdiscoverypolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="aa54c-139">Java</span><span class="sxs-lookup"><span data-stu-id="aa54c-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-homerealmdiscoverypolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="aa54c-140">响应</span><span class="sxs-lookup"><span data-stu-id="aa54c-140">Response</span></span>

<span data-ttu-id="aa54c-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="aa54c-141">The following is an example of the response.</span></span>

> <span data-ttu-id="aa54c-142">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="aa54c-142">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.homeRealmDiscoveryPolicy"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "definition": [
    "definition-value"
  ],
  "displayName": "displayName-value",
  "isOrganizationDefault": true,
  "id": "id-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get homeRealmDiscoveryPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


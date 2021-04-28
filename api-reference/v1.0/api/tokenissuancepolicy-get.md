---
title: 获取 tokenIssuancePolicy
description: 检索 tokenIssuancePolicy 对象的属性和关系。
localization_priority: Normal
author: luleonpla
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 34a0c2cfd6c4847e9a6b50b49be87325fd05f323
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52054355"
---
# <a name="get-tokenissuancepolicy"></a><span data-ttu-id="a8407-103">获取 tokenIssuancePolicy</span><span class="sxs-lookup"><span data-stu-id="a8407-103">Get tokenIssuancePolicy</span></span>

<span data-ttu-id="a8407-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a8407-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="a8407-105">检索 [tokenIssuancePolicy](../resources/tokenIssuancePolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a8407-105">Retrieve the properties and relationships of a [tokenIssuancePolicy](../resources/tokenIssuancePolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a8407-106">权限</span><span class="sxs-lookup"><span data-stu-id="a8407-106">Permissions</span></span>

<span data-ttu-id="a8407-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a8407-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a8407-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="a8407-109">Permission type</span></span>                        | <span data-ttu-id="a8407-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a8407-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="a8407-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a8407-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="a8407-112">Policy.Read.All、Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="a8407-112">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="a8407-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a8407-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a8407-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="a8407-114">Not supported.</span></span> |
| <span data-ttu-id="a8407-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="a8407-115">Application</span></span>                            | <span data-ttu-id="a8407-116">Policy.Read.All、Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="a8407-116">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="a8407-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a8407-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/tokenIssuancePolicies/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a8407-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="a8407-118">Optional query parameters</span></span>

<span data-ttu-id="a8407-119">此方法支持 `$expand` 和 `$select` OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="a8407-119">This method supports the `$expand` and `$select` OData query parameters to help customize the response.</span></span> <span data-ttu-id="a8407-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="a8407-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span> <span data-ttu-id="a8407-121">使用 `$expand` 时，请确保应用请求读取扩展对象的权限。</span><span class="sxs-lookup"><span data-stu-id="a8407-121">When using `$expand`, make sure your app requests permissions to read the expanded objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a8407-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="a8407-122">Request headers</span></span>

| <span data-ttu-id="a8407-123">名称</span><span class="sxs-lookup"><span data-stu-id="a8407-123">Name</span></span>      |<span data-ttu-id="a8407-124">说明</span><span class="sxs-lookup"><span data-stu-id="a8407-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a8407-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="a8407-125">Authorization</span></span> | <span data-ttu-id="a8407-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a8407-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a8407-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="a8407-128">Request body</span></span>

<span data-ttu-id="a8407-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a8407-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a8407-130">响应</span><span class="sxs-lookup"><span data-stu-id="a8407-130">Response</span></span>

<span data-ttu-id="a8407-131">如果成功，此方法在响应正文中返回 响应代码和请求的 `200 OK` [tokenIssuancePolicy](../resources/tokenIssuancePolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a8407-131">If successful, this method returns a `200 OK` response code and the requested [tokenIssuancePolicy](../resources/tokenIssuancePolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a8407-132">示例</span><span class="sxs-lookup"><span data-stu-id="a8407-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a8407-133">请求</span><span class="sxs-lookup"><span data-stu-id="a8407-133">Request</span></span>

<span data-ttu-id="a8407-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a8407-134">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="a8407-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="a8407-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_tokenIssuancePolicy"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/policies/tokenIssuancepolicies/{id}
```
# <a name="c"></a>[<span data-ttu-id="a8407-136">C#</span><span class="sxs-lookup"><span data-stu-id="a8407-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-tokenissuancepolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a8407-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a8407-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-tokenissuancepolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a8407-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a8407-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-tokenissuancepolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a8407-139">Java</span><span class="sxs-lookup"><span data-stu-id="a8407-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-tokenissuancepolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a8407-140">响应</span><span class="sxs-lookup"><span data-stu-id="a8407-140">Response</span></span>

<span data-ttu-id="a8407-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="a8407-141">The following is an example of the response.</span></span>

> <span data-ttu-id="a8407-142">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="a8407-142">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tokenIssuancePolicy"
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
  "description": "Get tokenIssuancePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


---
title: 列出 tokenIssuancePolicy
description: 获取 tokenIssuancePolicy 对象的列表。
localization_priority: Normal
author: luleonpla
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 693579c25c7e96ccbdfceecee44791ba23ffeefa
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52054341"
---
# <a name="list-tokenissuancepolicy"></a><span data-ttu-id="ba8b3-103">列出 tokenIssuancePolicy</span><span class="sxs-lookup"><span data-stu-id="ba8b3-103">List tokenIssuancePolicy</span></span>

<span data-ttu-id="ba8b3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ba8b3-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="ba8b3-105">获取 [tokenIssuancePolicy 对象](../resources/tokenIssuancePolicy.md) 的列表。</span><span class="sxs-lookup"><span data-stu-id="ba8b3-105">Get a list of [tokenIssuancePolicy](../resources/tokenIssuancePolicy.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="ba8b3-106">权限</span><span class="sxs-lookup"><span data-stu-id="ba8b3-106">Permissions</span></span>

<span data-ttu-id="ba8b3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ba8b3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ba8b3-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="ba8b3-109">Permission type</span></span>                        | <span data-ttu-id="ba8b3-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ba8b3-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ba8b3-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ba8b3-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ba8b3-112">Policy.Read.All、Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="ba8b3-112">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="ba8b3-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ba8b3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ba8b3-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="ba8b3-114">Not supported.</span></span> |
| <span data-ttu-id="ba8b3-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="ba8b3-115">Application</span></span>                            | <span data-ttu-id="ba8b3-116">Policy.Read.All、Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="ba8b3-116">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="ba8b3-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ba8b3-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET policies/tokenIssuancePolicies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ba8b3-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="ba8b3-118">Optional query parameters</span></span>

<span data-ttu-id="ba8b3-119">此方法支持 `$expand` 、 `$filter` 、 和 `$select` `$top` OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="ba8b3-119">This method supports the `$expand`, `$filter`, `$select`, and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="ba8b3-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="ba8b3-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span> <span data-ttu-id="ba8b3-121">使用 `$expand` 时，请确保应用请求读取扩展对象的权限。</span><span class="sxs-lookup"><span data-stu-id="ba8b3-121">When using `$expand`, make sure your app requests permissions to read the expanded objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ba8b3-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="ba8b3-122">Request headers</span></span>

| <span data-ttu-id="ba8b3-123">名称</span><span class="sxs-lookup"><span data-stu-id="ba8b3-123">Name</span></span>      |<span data-ttu-id="ba8b3-124">说明</span><span class="sxs-lookup"><span data-stu-id="ba8b3-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ba8b3-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="ba8b3-125">Authorization</span></span> | <span data-ttu-id="ba8b3-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ba8b3-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ba8b3-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="ba8b3-128">Request body</span></span>

<span data-ttu-id="ba8b3-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ba8b3-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ba8b3-130">响应</span><span class="sxs-lookup"><span data-stu-id="ba8b3-130">Response</span></span>

<span data-ttu-id="ba8b3-131">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [tokenIssuancePolicy](../resources/tokenIssuancePolicy.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="ba8b3-131">If successful, this method returns a `200 OK` response code and a collection of [tokenIssuancePolicy](../resources/tokenIssuancePolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ba8b3-132">示例</span><span class="sxs-lookup"><span data-stu-id="ba8b3-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ba8b3-133">请求</span><span class="sxs-lookup"><span data-stu-id="ba8b3-133">Request</span></span>

<span data-ttu-id="ba8b3-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ba8b3-134">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="ba8b3-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="ba8b3-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "tokenIssuancePolicies"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/policies/tokenIssuancePolicies
```
# <a name="c"></a>[<span data-ttu-id="ba8b3-136">C#</span><span class="sxs-lookup"><span data-stu-id="ba8b3-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tokenissuancepolicies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ba8b3-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ba8b3-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tokenissuancepolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ba8b3-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ba8b3-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tokenissuancepolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ba8b3-139">Java</span><span class="sxs-lookup"><span data-stu-id="ba8b3-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/tokenissuancepolicies-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ba8b3-140">响应</span><span class="sxs-lookup"><span data-stu-id="ba8b3-140">Response</span></span>

<span data-ttu-id="ba8b3-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ba8b3-141">The following is an example of the response.</span></span>

> <span data-ttu-id="ba8b3-142">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="ba8b3-142">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tokenIssuancePolicy",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "definition": [
        "definition-value"
      ],
      "displayName": "displayName-value",
      "isOrganizationDefault": true,
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List tokenIssuancePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


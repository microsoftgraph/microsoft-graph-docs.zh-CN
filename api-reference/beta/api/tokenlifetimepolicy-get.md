---
title: 获取 tokenLifetimePolicy
description: 检索 tokenLifetimePolicy 对象的属性和关系。
localization_priority: Normal
author: lujiangfeng666
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 651b1c5c107ecabbdae95e58d3652acc14504f69
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48980228"
---
# <a name="get-tokenlifetimepolicy"></a><span data-ttu-id="edaa2-103">获取 tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="edaa2-103">Get tokenLifetimePolicy</span></span>

<span data-ttu-id="edaa2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="edaa2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="edaa2-105">检索 [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="edaa2-105">Retrieve the properties and relationships of a [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="edaa2-106">权限</span><span class="sxs-lookup"><span data-stu-id="edaa2-106">Permissions</span></span>

<span data-ttu-id="edaa2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="edaa2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="edaa2-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="edaa2-109">Permission type</span></span>                        | <span data-ttu-id="edaa2-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="edaa2-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="edaa2-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="edaa2-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="edaa2-112">Policy： Read. All，ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="edaa2-112">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="edaa2-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="edaa2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="edaa2-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="edaa2-114">Not supported.</span></span> |
| <span data-ttu-id="edaa2-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="edaa2-115">Application</span></span>                            | <span data-ttu-id="edaa2-116">Policy： Read. All，ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="edaa2-116">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="edaa2-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="edaa2-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/tokenLifetimePolicies/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="edaa2-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="edaa2-118">Optional query parameters</span></span>

<span data-ttu-id="edaa2-119">此方法支持 `$expand` 和 `$select` OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="edaa2-119">This method supports the `$expand` and `$select` OData query parameters to help customize the response.</span></span> <span data-ttu-id="edaa2-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="edaa2-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span> <span data-ttu-id="edaa2-121">使用时 `$expand` ，请确保您的应用程序请求读取扩展的对象的权限。</span><span class="sxs-lookup"><span data-stu-id="edaa2-121">When using `$expand` make sure your app requests permissions to read the expanded objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="edaa2-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="edaa2-122">Request headers</span></span>

| <span data-ttu-id="edaa2-123">名称</span><span class="sxs-lookup"><span data-stu-id="edaa2-123">Name</span></span>      |<span data-ttu-id="edaa2-124">说明</span><span class="sxs-lookup"><span data-stu-id="edaa2-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="edaa2-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="edaa2-125">Authorization</span></span> | <span data-ttu-id="edaa2-126">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="edaa2-126">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="edaa2-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="edaa2-127">Request body</span></span>

<span data-ttu-id="edaa2-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="edaa2-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="edaa2-129">响应</span><span class="sxs-lookup"><span data-stu-id="edaa2-129">Response</span></span>

<span data-ttu-id="edaa2-130">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和请求的 [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="edaa2-130">If successful, this method returns a `200 OK` response code and the requested [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="edaa2-131">示例</span><span class="sxs-lookup"><span data-stu-id="edaa2-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="edaa2-132">请求</span><span class="sxs-lookup"><span data-stu-id="edaa2-132">Request</span></span>

<span data-ttu-id="edaa2-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="edaa2-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="edaa2-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="edaa2-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_tokenlifetimepolicy"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/policies/tokenLifetimePolicies/{id}
```
# <a name="c"></a>[<span data-ttu-id="edaa2-135">C#</span><span class="sxs-lookup"><span data-stu-id="edaa2-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-tokenlifetimepolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="edaa2-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="edaa2-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-tokenlifetimepolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="edaa2-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="edaa2-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-tokenlifetimepolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="edaa2-138">Java</span><span class="sxs-lookup"><span data-stu-id="edaa2-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-tokenlifetimepolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="edaa2-139">响应</span><span class="sxs-lookup"><span data-stu-id="edaa2-139">Response</span></span>

<span data-ttu-id="edaa2-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="edaa2-140">The following is an example of the response.</span></span>

> <span data-ttu-id="edaa2-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="edaa2-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tokenLifetimePolicy"
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
  "description": "Get tokenLifetimePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->



---
title: 列出 tokenLifetimePolicies
description: 获取 tokenLifetimePolicy 对象的列表。
localization_priority: Normal
author: lujiangfeng666
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 7dd63e12ee5673d109a0d0f413cd76ebae7c48d4
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48980214"
---
# <a name="list-tokenlifetimepolicies"></a><span data-ttu-id="00935-103">列出 tokenLifetimePolicies</span><span class="sxs-lookup"><span data-stu-id="00935-103">List tokenLifetimePolicies</span></span>

<span data-ttu-id="00935-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="00935-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="00935-105">获取 [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="00935-105">Get a list of [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="00935-106">权限</span><span class="sxs-lookup"><span data-stu-id="00935-106">Permissions</span></span>

<span data-ttu-id="00935-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="00935-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="00935-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="00935-109">Permission type</span></span>                        | <span data-ttu-id="00935-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="00935-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="00935-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="00935-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="00935-112">Policy： Read. All，ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="00935-112">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="00935-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="00935-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="00935-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="00935-114">Not supported.</span></span> |
| <span data-ttu-id="00935-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="00935-115">Application</span></span>                            | <span data-ttu-id="00935-116">Policy： Read. All，ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="00935-116">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="00935-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="00935-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET policies/tokenLifetimePolicies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="00935-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="00935-118">Optional query parameters</span></span>

<span data-ttu-id="00935-119">此方法支持 `$expand` 、 `$filter` `$select` 和 `$top` OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="00935-119">This method supports the `$expand`, `$filter`, `$select` and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="00935-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="00935-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span> <span data-ttu-id="00935-121">使用时 `$expand` ，请确保您的应用程序请求读取扩展的对象的权限。</span><span class="sxs-lookup"><span data-stu-id="00935-121">When using `$expand` make sure your app requests permissions to read the expanded objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="00935-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="00935-122">Request headers</span></span>

| <span data-ttu-id="00935-123">名称</span><span class="sxs-lookup"><span data-stu-id="00935-123">Name</span></span>      |<span data-ttu-id="00935-124">说明</span><span class="sxs-lookup"><span data-stu-id="00935-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="00935-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="00935-125">Authorization</span></span> | <span data-ttu-id="00935-126">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="00935-126">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="00935-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="00935-127">Request body</span></span>

<span data-ttu-id="00935-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="00935-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="00935-129">响应</span><span class="sxs-lookup"><span data-stu-id="00935-129">Response</span></span>

<span data-ttu-id="00935-130">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="00935-130">If successful, this method returns a `200 OK` response code and a collection of [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="00935-131">示例</span><span class="sxs-lookup"><span data-stu-id="00935-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="00935-132">请求</span><span class="sxs-lookup"><span data-stu-id="00935-132">Request</span></span>

<span data-ttu-id="00935-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="00935-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="00935-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="00935-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_tokenlifetimepolicies"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/policies/tokenLifetimePolicies
```
# <a name="c"></a>[<span data-ttu-id="00935-135">C#</span><span class="sxs-lookup"><span data-stu-id="00935-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-tokenlifetimepolicies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="00935-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="00935-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-tokenlifetimepolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="00935-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="00935-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-tokenlifetimepolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="00935-138">Java</span><span class="sxs-lookup"><span data-stu-id="00935-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-tokenlifetimepolicies-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="00935-139">响应</span><span class="sxs-lookup"><span data-stu-id="00935-139">Response</span></span>

<span data-ttu-id="00935-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="00935-140">The following is an example of the response.</span></span>

> <span data-ttu-id="00935-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="00935-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tokenLifetimePolicy",
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
  "description": "List tokenLifetimePolicies",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->



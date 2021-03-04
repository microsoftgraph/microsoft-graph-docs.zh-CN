---
title: 列出 activityBasedTimeoutPolicies
description: 获取 activityBasedTimeoutPolicy 对象的列表。
localization_priority: Normal
author: lujiangfeng666
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: d763b085f0ec32dbaf282aa0ef07f3ceffc8c144
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50438993"
---
# <a name="list-activitybasedtimeoutpolicies"></a><span data-ttu-id="85b38-103">列出 activityBasedTimeoutPolicies</span><span class="sxs-lookup"><span data-stu-id="85b38-103">List activityBasedTimeoutPolicies</span></span>

<span data-ttu-id="85b38-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="85b38-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="85b38-105">获取 [activityBasedTimeoutPolicy 对象](../resources/activitybasedtimeoutpolicy.md) 的列表。</span><span class="sxs-lookup"><span data-stu-id="85b38-105">Get a list of [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="85b38-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="85b38-106">Permissions</span></span>

<span data-ttu-id="85b38-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="85b38-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="85b38-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="85b38-109">Permission type</span></span>                        | <span data-ttu-id="85b38-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="85b38-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="85b38-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="85b38-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="85b38-112">Policy.Read.All、Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="85b38-112">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="85b38-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="85b38-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="85b38-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="85b38-114">Not supported.</span></span> |
| <span data-ttu-id="85b38-115">Application</span><span class="sxs-lookup"><span data-stu-id="85b38-115">Application</span></span>                            | <span data-ttu-id="85b38-116">Policy.Read.All、Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="85b38-116">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="85b38-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="85b38-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET policies/activityBasedTimeoutPolicies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="85b38-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="85b38-118">Optional query parameters</span></span>

<span data-ttu-id="85b38-119">此方法支持和 `$filter` `$select` `$top` OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="85b38-119">This method supports the `$filter`, `$select` and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="85b38-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="85b38-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="85b38-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="85b38-121">Request headers</span></span>

| <span data-ttu-id="85b38-122">名称</span><span class="sxs-lookup"><span data-stu-id="85b38-122">Name</span></span>      |<span data-ttu-id="85b38-123">说明</span><span class="sxs-lookup"><span data-stu-id="85b38-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="85b38-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="85b38-124">Authorization</span></span> | <span data-ttu-id="85b38-125">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="85b38-125">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="85b38-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="85b38-126">Request body</span></span>

<span data-ttu-id="85b38-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="85b38-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="85b38-128">响应</span><span class="sxs-lookup"><span data-stu-id="85b38-128">Response</span></span>

<span data-ttu-id="85b38-129">如果成功，此方法在响应正文中返回响应 `200 OK` [代码和 activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="85b38-129">If successful, this method returns a `200 OK` response code and a collection of [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="85b38-130">示例</span><span class="sxs-lookup"><span data-stu-id="85b38-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="85b38-131">请求</span><span class="sxs-lookup"><span data-stu-id="85b38-131">Request</span></span>

<span data-ttu-id="85b38-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="85b38-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="85b38-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="85b38-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_activitybasedtimeoutpolicies"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/policies/activityBasedTimeoutPolicies
```
# <a name="c"></a>[<span data-ttu-id="85b38-134">C#</span><span class="sxs-lookup"><span data-stu-id="85b38-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-activitybasedtimeoutpolicies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="85b38-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="85b38-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-activitybasedtimeoutpolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="85b38-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="85b38-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-activitybasedtimeoutpolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="85b38-137">Java</span><span class="sxs-lookup"><span data-stu-id="85b38-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-activitybasedtimeoutpolicies-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="85b38-138">响应</span><span class="sxs-lookup"><span data-stu-id="85b38-138">Response</span></span>

<span data-ttu-id="85b38-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="85b38-139">The following is an example of the response.</span></span>

> <span data-ttu-id="85b38-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="85b38-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.activityBasedTimeoutPolicy",
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
  "description": "List activityBasedTimeoutPolicies",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->



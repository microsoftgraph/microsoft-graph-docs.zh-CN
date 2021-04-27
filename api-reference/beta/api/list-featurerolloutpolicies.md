---
title: 列出 featureRolloutPolicies
description: 检索 featureRolloutPolicy 对象的列表。
localization_priority: Normal
author: madhavpatel6
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: fe8a3a4b5d5318661856cc2f26f05a78283a43bf
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049308"
---
# <a name="list-featurerolloutpolicies"></a><span data-ttu-id="ab235-103">列出 featureRolloutPolicies</span><span class="sxs-lookup"><span data-stu-id="ab235-103">List featureRolloutPolicies</span></span>

<span data-ttu-id="ab235-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ab235-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [feature-rolloutpolicy-deprecate](../../includes/directory-featurerolloutpolicies-deprecate.md)]

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ab235-105">检索 [featureRolloutPolicy 对象](../resources/featurerolloutpolicy.md) 的列表。</span><span class="sxs-lookup"><span data-stu-id="ab235-105">Retrieve a list of [featureRolloutPolicy](../resources/featurerolloutpolicy.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="ab235-106">权限</span><span class="sxs-lookup"><span data-stu-id="ab235-106">Permissions</span></span>

<span data-ttu-id="ab235-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ab235-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ab235-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="ab235-109">Permission type</span></span>                        | <span data-ttu-id="ab235-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ab235-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ab235-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ab235-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ab235-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab235-112">Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="ab235-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ab235-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ab235-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="ab235-114">Not supported.</span></span> |
| <span data-ttu-id="ab235-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="ab235-115">Application</span></span>                            | <span data-ttu-id="ab235-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ab235-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ab235-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ab235-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/featureRolloutPolicies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ab235-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="ab235-118">Optional query parameters</span></span>

<span data-ttu-id="ab235-119">此方法支持以下 OData 查询参数来帮助自定义响应 `$count` `$expand` `$filter` `$orderby` `$select` `$skip` ：、、、。 `$top`</span><span class="sxs-lookup"><span data-stu-id="ab235-119">This method supports the following OData query parameters to help customize the response: `$count`, `$expand`, `$filter`, `$orderby`, `$select`, `$skip`, `$top`.</span></span> <span data-ttu-id="ab235-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="ab235-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="ab235-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="ab235-121">Request headers</span></span>

| <span data-ttu-id="ab235-122">名称</span><span class="sxs-lookup"><span data-stu-id="ab235-122">Name</span></span>      |<span data-ttu-id="ab235-123">说明</span><span class="sxs-lookup"><span data-stu-id="ab235-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ab235-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="ab235-124">Authorization</span></span> | <span data-ttu-id="ab235-125">Bearer {token}。</span><span class="sxs-lookup"><span data-stu-id="ab235-125">Bearer {token}.</span></span> <span data-ttu-id="ab235-126">必需</span><span class="sxs-lookup"><span data-stu-id="ab235-126">Required</span></span> |

## <a name="request-body"></a><span data-ttu-id="ab235-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="ab235-127">Request body</span></span>

<span data-ttu-id="ab235-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ab235-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ab235-129">响应</span><span class="sxs-lookup"><span data-stu-id="ab235-129">Response</span></span>

<span data-ttu-id="ab235-130">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [featureRolloutPolicy](../resources/featurerolloutpolicy.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="ab235-130">If successful, this method returns a `200 OK` response code and a collection of [featureRolloutPolicy](../resources/featurerolloutpolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ab235-131">示例</span><span class="sxs-lookup"><span data-stu-id="ab235-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ab235-132">请求</span><span class="sxs-lookup"><span data-stu-id="ab235-132">Request</span></span>

<span data-ttu-id="ab235-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ab235-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="ab235-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="ab235-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_featurerolloutpolicies_policies"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/policies/featureRolloutPolicies
```
# <a name="c"></a>[<span data-ttu-id="ab235-135">C#</span><span class="sxs-lookup"><span data-stu-id="ab235-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-featurerolloutpolicies-policies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ab235-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ab235-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-featurerolloutpolicies-policies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ab235-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ab235-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-featurerolloutpolicies-policies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ab235-138">Java</span><span class="sxs-lookup"><span data-stu-id="ab235-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-featurerolloutpolicies-policies-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ab235-139">响应</span><span class="sxs-lookup"><span data-stu-id="ab235-139">Response</span></span>

<span data-ttu-id="ab235-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ab235-140">The following is an example of the response.</span></span>

> <span data-ttu-id="ab235-141">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="ab235-141">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.featureRolloutPolicy",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "e3c2f23a-edd2-43a8-849f-154e70794ac5",
      "displayName": "PassthroughAuthentication rollout policy",
      "description": "PassthroughAuthentication rollout policy",
      "feature": "passthroughAuthentication",
      "isEnabled": true,
      "isAppliedToOrganization": false
    },
    {
      "id": "df85e4d9-e8c4-4033-a41c-73419a95c29c",
      "displayName": "SeamlessSso rollout policy",
      "description": "SeamlessSso rollout policy",
      "feature": "seamlessSso",
      "isEnabled": true,
      "isAppliedToOrganization": false
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List featureRolloutPolicies",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->



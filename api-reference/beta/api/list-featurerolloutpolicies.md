---
title: 列出 featureRolloutPolicies
description: 检索 featureRolloutPolicy 对象的列表。
localization_priority: Normal
author: madhavpatel6
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 0b6d28265d3f64a278e624d7fe17ded39072e772
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50952225"
---
# <a name="list-featurerolloutpolicies"></a><span data-ttu-id="11b87-103">列出 featureRolloutPolicies</span><span class="sxs-lookup"><span data-stu-id="11b87-103">List featureRolloutPolicies</span></span>

<span data-ttu-id="11b87-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="11b87-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [feature-rolloutpolicy-deprecate](../../includes/directory-featurerolloutpolicies-deprecate.md)]

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="11b87-105">检索 [featureRolloutPolicy 对象](../resources/featurerolloutpolicy.md) 的列表。</span><span class="sxs-lookup"><span data-stu-id="11b87-105">Retrieve a list of [featureRolloutPolicy](../resources/featurerolloutpolicy.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="11b87-106">权限</span><span class="sxs-lookup"><span data-stu-id="11b87-106">Permissions</span></span>

<span data-ttu-id="11b87-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="11b87-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="11b87-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="11b87-109">Permission type</span></span>                        | <span data-ttu-id="11b87-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="11b87-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="11b87-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="11b87-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="11b87-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="11b87-112">Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="11b87-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="11b87-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="11b87-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="11b87-114">Not supported.</span></span> |
| <span data-ttu-id="11b87-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="11b87-115">Application</span></span>                            | <span data-ttu-id="11b87-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="11b87-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="11b87-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="11b87-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/featureRolloutPolicies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="11b87-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="11b87-118">Optional query parameters</span></span>

<span data-ttu-id="11b87-119">此方法支持以下 OData 查询参数来帮助自定义响应 `$count` `$expand` `$filter` `$orderby` `$select` `$skip` ：、、、。 `$top`</span><span class="sxs-lookup"><span data-stu-id="11b87-119">This method supports the following OData query parameters to help customize the response: `$count`, `$expand`, `$filter`, `$orderby`, `$select`, `$skip`, `$top`.</span></span> <span data-ttu-id="11b87-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="11b87-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="11b87-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="11b87-121">Request headers</span></span>

| <span data-ttu-id="11b87-122">名称</span><span class="sxs-lookup"><span data-stu-id="11b87-122">Name</span></span>      |<span data-ttu-id="11b87-123">说明</span><span class="sxs-lookup"><span data-stu-id="11b87-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="11b87-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="11b87-124">Authorization</span></span> | <span data-ttu-id="11b87-125">Bearer {token}。</span><span class="sxs-lookup"><span data-stu-id="11b87-125">Bearer {token}.</span></span> <span data-ttu-id="11b87-126">必需</span><span class="sxs-lookup"><span data-stu-id="11b87-126">Required</span></span> |

## <a name="request-body"></a><span data-ttu-id="11b87-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="11b87-127">Request body</span></span>

<span data-ttu-id="11b87-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="11b87-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="11b87-129">响应</span><span class="sxs-lookup"><span data-stu-id="11b87-129">Response</span></span>

<span data-ttu-id="11b87-130">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [featureRolloutPolicy](../resources/featurerolloutpolicy.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="11b87-130">If successful, this method returns a `200 OK` response code and a collection of [featureRolloutPolicy](../resources/featurerolloutpolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="11b87-131">示例</span><span class="sxs-lookup"><span data-stu-id="11b87-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="11b87-132">请求</span><span class="sxs-lookup"><span data-stu-id="11b87-132">Request</span></span>

<span data-ttu-id="11b87-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="11b87-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_featurerolloutpolicies_policies"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/policies/featureRolloutPolicies
```

### <a name="response"></a><span data-ttu-id="11b87-134">响应</span><span class="sxs-lookup"><span data-stu-id="11b87-134">Response</span></span>

<span data-ttu-id="11b87-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="11b87-135">The following is an example of the response.</span></span>

> <span data-ttu-id="11b87-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="11b87-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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



---
title: 获取 claimsMappingPolicy
description: 检索 claimsMappingPolicy 对象的属性和关系。
localization_priority: Normal
author: paulgarn
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 10213a3112ab3b05f1e5b3dcfa4fe497dfadfc36
ms.sourcegitcommit: b083a570375252eff8054f9fe70e1e5e2becc06d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/23/2020
ms.locfileid: "44846234"
---
# <a name="get-claimsmappingpolicy"></a><span data-ttu-id="911c6-103">获取 claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="911c6-103">Get claimsMappingPolicy</span></span>

<span data-ttu-id="911c6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="911c6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="911c6-105">检索[claimsMappingPolicy](../resources/claimsmappingpolicy.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="911c6-105">Retrieve the properties and relationships of a [claimsMappingPolicy](../resources/claimsmappingpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="911c6-106">权限</span><span class="sxs-lookup"><span data-stu-id="911c6-106">Permissions</span></span>

<span data-ttu-id="911c6-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="911c6-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="911c6-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="911c6-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="911c6-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="911c6-109">Permission type</span></span>                        | <span data-ttu-id="911c6-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="911c6-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="911c6-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="911c6-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="911c6-112">Policy： Read. All，ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="911c6-112">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="911c6-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="911c6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="911c6-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="911c6-114">Not supported.</span></span> |
| <span data-ttu-id="911c6-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="911c6-115">Application</span></span>                            | <span data-ttu-id="911c6-116">Policy： Read. All，ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="911c6-116">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="911c6-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="911c6-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/claimsMappingPolicies/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="911c6-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="911c6-118">Optional query parameters</span></span>

<span data-ttu-id="911c6-119">此方法支持 `$expand` 和 `$select` OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="911c6-119">This method supports the `$expand` and `$select` OData query parameters to help customize the response.</span></span> <span data-ttu-id="911c6-120">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="911c6-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span> <span data-ttu-id="911c6-121">使用时 `$expand` ，请确保您的应用程序请求读取扩展的对象的权限。</span><span class="sxs-lookup"><span data-stu-id="911c6-121">When using `$expand` make sure your app requests permissions to read the expanded objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="911c6-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="911c6-122">Request headers</span></span>

| <span data-ttu-id="911c6-123">名称</span><span class="sxs-lookup"><span data-stu-id="911c6-123">Name</span></span>      |<span data-ttu-id="911c6-124">说明</span><span class="sxs-lookup"><span data-stu-id="911c6-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="911c6-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="911c6-125">Authorization</span></span> | <span data-ttu-id="911c6-126">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="911c6-126">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="911c6-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="911c6-127">Request body</span></span>

<span data-ttu-id="911c6-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="911c6-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="911c6-129">响应</span><span class="sxs-lookup"><span data-stu-id="911c6-129">Response</span></span>

<span data-ttu-id="911c6-130">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和请求的[claimsMappingPolicy](../resources/claimsmappingpolicy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="911c6-130">If successful, this method returns a `200 OK` response code and the requested [claimsMappingPolicy](../resources/claimsmappingpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="911c6-131">示例</span><span class="sxs-lookup"><span data-stu-id="911c6-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="911c6-132">请求</span><span class="sxs-lookup"><span data-stu-id="911c6-132">Request</span></span>

<span data-ttu-id="911c6-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="911c6-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="911c6-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="911c6-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_claimsmappingpolicy"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/policies/claimsMappingPolicies/{id}
```

### <a name="response"></a><span data-ttu-id="911c6-135">响应</span><span class="sxs-lookup"><span data-stu-id="911c6-135">Response</span></span>

<span data-ttu-id="911c6-136">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="911c6-136">The following is an example of the response.</span></span>

> <span data-ttu-id="911c6-137">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="911c6-137">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="911c6-138">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="911c6-138">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.claimsMappingPolicy"
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
  "description": "Get claimsMappingPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

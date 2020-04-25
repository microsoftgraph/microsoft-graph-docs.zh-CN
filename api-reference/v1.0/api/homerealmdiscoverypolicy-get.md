---
title: 获取 homeRealmDiscoveryPolicy
description: 检索 homeRealmDiscoveryPolicy 对象的属性和关系。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 57fa74e6561ad4010e9dbffa983257886c4316ad
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43805592"
---
# <a name="get-homerealmdiscoverypolicy"></a><span data-ttu-id="be82b-103">获取 homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="be82b-103">Get homeRealmDiscoveryPolicy</span></span>

<span data-ttu-id="be82b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="be82b-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="be82b-105">检索[homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="be82b-105">Retrieve the properties and relationships of a [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="be82b-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="be82b-106">Permissions</span></span>

<span data-ttu-id="be82b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="be82b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="be82b-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="be82b-109">Permission type</span></span>                        | <span data-ttu-id="be82b-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="be82b-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="be82b-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="be82b-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="be82b-112">Policy： Read. All，ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="be82b-112">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="be82b-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="be82b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="be82b-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="be82b-114">Not supported.</span></span> |
| <span data-ttu-id="be82b-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="be82b-115">Application</span></span>                            | <span data-ttu-id="be82b-116">Policy： Read. All，ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="be82b-116">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="be82b-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="be82b-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/homeRealmDiscoveryPolicies/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="be82b-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="be82b-118">Optional query parameters</span></span>

<span data-ttu-id="be82b-119">此方法支持`$expand`和`$select` OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="be82b-119">This method supports the `$expand` and `$select` OData query parameters to help customize the response.</span></span> <span data-ttu-id="be82b-120">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="be82b-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span> <span data-ttu-id="be82b-121">使用`$expand`时，请确保您的应用程序请求读取展开的对象的权限。</span><span class="sxs-lookup"><span data-stu-id="be82b-121">When using `$expand`, make sure that your app requests permissions to read the expanded objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="be82b-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="be82b-122">Request headers</span></span>

| <span data-ttu-id="be82b-123">名称</span><span class="sxs-lookup"><span data-stu-id="be82b-123">Name</span></span>      |<span data-ttu-id="be82b-124">说明</span><span class="sxs-lookup"><span data-stu-id="be82b-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="be82b-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="be82b-125">Authorization</span></span> | <span data-ttu-id="be82b-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="be82b-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="be82b-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="be82b-128">Request body</span></span>

<span data-ttu-id="be82b-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="be82b-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="be82b-130">响应</span><span class="sxs-lookup"><span data-stu-id="be82b-130">Response</span></span>

<span data-ttu-id="be82b-131">如果成功，此方法在响应`200 OK`正文中返回响应代码和请求的[homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="be82b-131">If successful, this method returns a `200 OK` response code and the requested [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="be82b-132">示例</span><span class="sxs-lookup"><span data-stu-id="be82b-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="be82b-133">请求</span><span class="sxs-lookup"><span data-stu-id="be82b-133">Request</span></span>

<span data-ttu-id="be82b-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="be82b-134">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="be82b-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="be82b-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_homerealmdiscoverypolicy"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/policies/homeRealmDiscoveryPolicies/{id}
```
# <a name="c"></a>[<span data-ttu-id="be82b-136">C#</span><span class="sxs-lookup"><span data-stu-id="be82b-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-homerealmdiscoverypolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="be82b-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="be82b-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-homerealmdiscoverypolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="be82b-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="be82b-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-homerealmdiscoverypolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="be82b-139">Java</span><span class="sxs-lookup"><span data-stu-id="be82b-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-homerealmdiscoverypolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="be82b-140">响应</span><span class="sxs-lookup"><span data-stu-id="be82b-140">Response</span></span>

<span data-ttu-id="be82b-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="be82b-141">The following is an example of the response.</span></span>

> <span data-ttu-id="be82b-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="be82b-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

---
title: 列出 tokenIssuancePolicy
description: 获取 tokenIssuancePolicy 对象的列表。
localization_priority: Normal
author: luleonpla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 108091747e7fd9e0b14db9161c05bd0a25b2ef4e
ms.sourcegitcommit: 79988a42d91cc25bdd1c531b5f3261901d720a9a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/28/2020
ms.locfileid: "43916337"
---
# <a name="list-tokenissuancepolicy"></a><span data-ttu-id="91631-103">列出 tokenIssuancePolicy</span><span class="sxs-lookup"><span data-stu-id="91631-103">List tokenIssuancePolicy</span></span>

<span data-ttu-id="91631-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="91631-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="91631-105">获取[tokenIssuancePolicy](../resources/tokenIssuancePolicy.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="91631-105">Get a list of [tokenIssuancePolicy](../resources/tokenIssuancePolicy.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="91631-106">权限</span><span class="sxs-lookup"><span data-stu-id="91631-106">Permissions</span></span>

<span data-ttu-id="91631-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="91631-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="91631-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="91631-109">Permission type</span></span>                        | <span data-ttu-id="91631-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="91631-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="91631-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="91631-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="91631-112">Policy： Read. All，ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="91631-112">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="91631-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="91631-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="91631-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="91631-114">Not supported.</span></span> |
| <span data-ttu-id="91631-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="91631-115">Application</span></span>                            | <span data-ttu-id="91631-116">Policy： Read. All，ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="91631-116">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="91631-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="91631-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET policies/tokenIssuancePolicies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="91631-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="91631-118">Optional query parameters</span></span>

<span data-ttu-id="91631-119">`$expand`此方法支持`$filter`、、 `$select`和`$top` OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="91631-119">This method supports the `$expand`, `$filter`, `$select`, and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="91631-120">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="91631-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span> <span data-ttu-id="91631-121">使用`$expand`时，请确保您的应用程序请求读取展开的对象的权限。</span><span class="sxs-lookup"><span data-stu-id="91631-121">When using `$expand`, make sure your app requests permissions to read the expanded objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="91631-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="91631-122">Request headers</span></span>

| <span data-ttu-id="91631-123">名称</span><span class="sxs-lookup"><span data-stu-id="91631-123">Name</span></span>      |<span data-ttu-id="91631-124">说明</span><span class="sxs-lookup"><span data-stu-id="91631-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="91631-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="91631-125">Authorization</span></span> | <span data-ttu-id="91631-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="91631-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="91631-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="91631-128">Request body</span></span>

<span data-ttu-id="91631-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="91631-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="91631-130">响应</span><span class="sxs-lookup"><span data-stu-id="91631-130">Response</span></span>

<span data-ttu-id="91631-131">如果成功，此方法在响应`200 OK`正文中返回响应代码和[tokenIssuancePolicy](../resources/tokenIssuancePolicy.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="91631-131">If successful, this method returns a `200 OK` response code and a collection of [tokenIssuancePolicy](../resources/tokenIssuancePolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="91631-132">示例</span><span class="sxs-lookup"><span data-stu-id="91631-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="91631-133">请求</span><span class="sxs-lookup"><span data-stu-id="91631-133">Request</span></span>

<span data-ttu-id="91631-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="91631-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="91631-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="91631-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "tokenIssuancePolicies"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/policies/tokenIssuancePolicies
```
# <a name="c"></a>[<span data-ttu-id="91631-136">C#</span><span class="sxs-lookup"><span data-stu-id="91631-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tokenissuancepolicies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="91631-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="91631-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tokenissuancepolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="91631-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="91631-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tokenissuancepolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


### <a name="response"></a><span data-ttu-id="91631-139">响应</span><span class="sxs-lookup"><span data-stu-id="91631-139">Response</span></span>

<span data-ttu-id="91631-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="91631-140">The following is an example of the response.</span></span>

> <span data-ttu-id="91631-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="91631-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

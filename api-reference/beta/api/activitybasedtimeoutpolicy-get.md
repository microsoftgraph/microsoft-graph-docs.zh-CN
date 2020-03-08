---
title: 获取 activityBasedTimeoutPolicy
description: 获取 activityBasedTimeoutPolicy 对象的属性。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 071d9d1cd69ceeedfe857a53b05ba7bf3495c75d
ms.sourcegitcommit: 435d80cfa71574c06d24780c591d4303a5cd9636
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2020
ms.locfileid: "42562372"
---
# <a name="get-activitybasedtimeoutpolicy"></a><span data-ttu-id="4f2a6-103">获取 activityBasedTimeoutPolicy</span><span class="sxs-lookup"><span data-stu-id="4f2a6-103">Get activityBasedTimeoutPolicy</span></span>

<span data-ttu-id="4f2a6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4f2a6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4f2a6-105">获取[activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="4f2a6-105">Get the properties of an [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="4f2a6-106">权限</span><span class="sxs-lookup"><span data-stu-id="4f2a6-106">Permissions</span></span>

<span data-ttu-id="4f2a6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4f2a6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4f2a6-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="4f2a6-109">Permission type</span></span>                        | <span data-ttu-id="4f2a6-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4f2a6-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="4f2a6-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4f2a6-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="4f2a6-112">Policy： Read. All，ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="4f2a6-112">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="4f2a6-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4f2a6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4f2a6-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="4f2a6-114">Not supported.</span></span> |
| <span data-ttu-id="4f2a6-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="4f2a6-115">Application</span></span>                            | <span data-ttu-id="4f2a6-116">Policy： Read. All，ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="4f2a6-116">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="4f2a6-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4f2a6-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/activityBasedTimeoutPolicies/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4f2a6-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="4f2a6-118">Optional query parameters</span></span>

<span data-ttu-id="4f2a6-119">此方法支持`$select` OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="4f2a6-119">This method supports the `$select` OData query parameters to help customize the response.</span></span> <span data-ttu-id="4f2a6-120">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="4f2a6-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="4f2a6-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="4f2a6-121">Request headers</span></span>

| <span data-ttu-id="4f2a6-122">名称</span><span class="sxs-lookup"><span data-stu-id="4f2a6-122">Name</span></span>      |<span data-ttu-id="4f2a6-123">说明</span><span class="sxs-lookup"><span data-stu-id="4f2a6-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="4f2a6-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="4f2a6-124">Authorization</span></span> | <span data-ttu-id="4f2a6-125">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="4f2a6-125">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="4f2a6-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="4f2a6-126">Request body</span></span>

<span data-ttu-id="4f2a6-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4f2a6-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4f2a6-128">响应</span><span class="sxs-lookup"><span data-stu-id="4f2a6-128">Response</span></span>

<span data-ttu-id="4f2a6-129">如果成功，此方法在响应`200 OK`正文中返回响应代码和请求的[activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="4f2a6-129">If successful, this method returns a `200 OK` response code and the requested [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4f2a6-130">示例</span><span class="sxs-lookup"><span data-stu-id="4f2a6-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4f2a6-131">请求</span><span class="sxs-lookup"><span data-stu-id="4f2a6-131">Request</span></span>

<span data-ttu-id="4f2a6-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="4f2a6-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4f2a6-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="4f2a6-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_activitybasedtimeoutpolicy"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/policies/activityBasedTimeoutPolicies/{id}
```
# <a name="c"></a>[<span data-ttu-id="4f2a6-134">C#</span><span class="sxs-lookup"><span data-stu-id="4f2a6-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-activitybasedtimeoutpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4f2a6-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4f2a6-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-activitybasedtimeoutpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4f2a6-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4f2a6-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-activitybasedtimeoutpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4f2a6-137">响应</span><span class="sxs-lookup"><span data-stu-id="4f2a6-137">Response</span></span>

<span data-ttu-id="4f2a6-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="4f2a6-138">The following is an example of the response.</span></span>

> <span data-ttu-id="4f2a6-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="4f2a6-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.activityBasedTimeoutPolicy"
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
  "description": "Get activityBasedTimeoutPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

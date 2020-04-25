---
title: 获取 activityBasedTimeoutPolicy
description: 获取 activityBasedTimeoutPolicy 对象的属性。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 90950f2f7134ed64c42e132c896619d0214d4381
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43806266"
---
# <a name="get-activitybasedtimeoutpolicy"></a><span data-ttu-id="6e38d-103">获取 activityBasedTimeoutPolicy</span><span class="sxs-lookup"><span data-stu-id="6e38d-103">Get activityBasedTimeoutPolicy</span></span>

<span data-ttu-id="6e38d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6e38d-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="6e38d-105">获取[activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="6e38d-105">Get the properties of an [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6e38d-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="6e38d-106">Permissions</span></span>

<span data-ttu-id="6e38d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6e38d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6e38d-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="6e38d-109">Permission type</span></span>                        | <span data-ttu-id="6e38d-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6e38d-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="6e38d-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6e38d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="6e38d-112">Policy： Read. All，ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="6e38d-112">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="6e38d-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6e38d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6e38d-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="6e38d-114">Not supported.</span></span> |
| <span data-ttu-id="6e38d-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="6e38d-115">Application</span></span>                            | <span data-ttu-id="6e38d-116">Policy： Read. All，ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="6e38d-116">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="6e38d-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6e38d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/activityBasedTimeoutPolicies/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6e38d-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="6e38d-118">Optional query parameters</span></span>

<span data-ttu-id="6e38d-119">此方法支持`$select` OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="6e38d-119">This method supports the `$select` OData query parameters to help customize the response.</span></span> <span data-ttu-id="6e38d-120">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="6e38d-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="6e38d-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="6e38d-121">Request headers</span></span>

| <span data-ttu-id="6e38d-122">名称</span><span class="sxs-lookup"><span data-stu-id="6e38d-122">Name</span></span>      |<span data-ttu-id="6e38d-123">说明</span><span class="sxs-lookup"><span data-stu-id="6e38d-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6e38d-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="6e38d-124">Authorization</span></span> | <span data-ttu-id="6e38d-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6e38d-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6e38d-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="6e38d-127">Request body</span></span>

<span data-ttu-id="6e38d-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6e38d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6e38d-129">响应</span><span class="sxs-lookup"><span data-stu-id="6e38d-129">Response</span></span>

<span data-ttu-id="6e38d-130">如果成功，此方法在响应`200 OK`正文中返回响应代码和请求的[activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="6e38d-130">If successful, this method returns a `200 OK` response code and the requested [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6e38d-131">示例</span><span class="sxs-lookup"><span data-stu-id="6e38d-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6e38d-132">请求</span><span class="sxs-lookup"><span data-stu-id="6e38d-132">Request</span></span>

<span data-ttu-id="6e38d-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="6e38d-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="6e38d-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="6e38d-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_activitybasedtimeoutpolicy"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/policies/activityBasedTimeoutPolicies/{id}
```
# <a name="c"></a>[<span data-ttu-id="6e38d-135">C#</span><span class="sxs-lookup"><span data-stu-id="6e38d-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-activitybasedtimeoutpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6e38d-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6e38d-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-activitybasedtimeoutpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6e38d-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6e38d-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-activitybasedtimeoutpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6e38d-138">Java</span><span class="sxs-lookup"><span data-stu-id="6e38d-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-activitybasedtimeoutpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="6e38d-139">响应</span><span class="sxs-lookup"><span data-stu-id="6e38d-139">Response</span></span>

<span data-ttu-id="6e38d-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="6e38d-140">The following is an example of the response.</span></span>

> <span data-ttu-id="6e38d-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="6e38d-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

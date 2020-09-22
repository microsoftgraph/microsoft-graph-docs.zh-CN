---
title: 获取 activityBasedTimeoutPolicy
description: 获取 activityBasedTimeoutPolicy 对象的属性。
localization_priority: Normal
author: lujiangfeng666
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 86dbe784c4a7a2c7069cfcfe6acf15336ccd98c1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47992942"
---
# <a name="get-activitybasedtimeoutpolicy"></a><span data-ttu-id="3cb54-103">获取 activityBasedTimeoutPolicy</span><span class="sxs-lookup"><span data-stu-id="3cb54-103">Get activityBasedTimeoutPolicy</span></span>

<span data-ttu-id="3cb54-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3cb54-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="3cb54-105">获取 [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="3cb54-105">Get the properties of an [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="3cb54-106">权限</span><span class="sxs-lookup"><span data-stu-id="3cb54-106">Permissions</span></span>

<span data-ttu-id="3cb54-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3cb54-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3cb54-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="3cb54-109">Permission type</span></span>                        | <span data-ttu-id="3cb54-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3cb54-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="3cb54-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3cb54-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="3cb54-112">Policy： Read. All，ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="3cb54-112">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="3cb54-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3cb54-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3cb54-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="3cb54-114">Not supported.</span></span> |
| <span data-ttu-id="3cb54-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="3cb54-115">Application</span></span>                            | <span data-ttu-id="3cb54-116">Policy： Read. All，ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="3cb54-116">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="3cb54-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3cb54-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/activityBasedTimeoutPolicies/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3cb54-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="3cb54-118">Optional query parameters</span></span>

<span data-ttu-id="3cb54-119">此方法支持 `$select` OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="3cb54-119">This method supports the `$select` OData query parameters to help customize the response.</span></span> <span data-ttu-id="3cb54-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="3cb54-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="3cb54-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="3cb54-121">Request headers</span></span>

| <span data-ttu-id="3cb54-122">名称</span><span class="sxs-lookup"><span data-stu-id="3cb54-122">Name</span></span>      |<span data-ttu-id="3cb54-123">说明</span><span class="sxs-lookup"><span data-stu-id="3cb54-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="3cb54-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="3cb54-124">Authorization</span></span> | <span data-ttu-id="3cb54-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3cb54-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3cb54-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="3cb54-127">Request body</span></span>

<span data-ttu-id="3cb54-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3cb54-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3cb54-129">响应</span><span class="sxs-lookup"><span data-stu-id="3cb54-129">Response</span></span>

<span data-ttu-id="3cb54-130">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和请求的 [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3cb54-130">If successful, this method returns a `200 OK` response code and the requested [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3cb54-131">示例</span><span class="sxs-lookup"><span data-stu-id="3cb54-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3cb54-132">请求</span><span class="sxs-lookup"><span data-stu-id="3cb54-132">Request</span></span>

<span data-ttu-id="3cb54-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="3cb54-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="3cb54-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="3cb54-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_activitybasedtimeoutpolicy"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/policies/activityBasedTimeoutPolicies/{id}
```
# <a name="c"></a>[<span data-ttu-id="3cb54-135">C#</span><span class="sxs-lookup"><span data-stu-id="3cb54-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-activitybasedtimeoutpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3cb54-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3cb54-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-activitybasedtimeoutpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3cb54-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3cb54-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-activitybasedtimeoutpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3cb54-138">Java</span><span class="sxs-lookup"><span data-stu-id="3cb54-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-activitybasedtimeoutpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="3cb54-139">响应</span><span class="sxs-lookup"><span data-stu-id="3cb54-139">Response</span></span>

<span data-ttu-id="3cb54-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="3cb54-140">The following is an example of the response.</span></span>

> <span data-ttu-id="3cb54-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="3cb54-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


---
title: 列出 activityBasedTimeoutPolicies
description: 获取 activityBasedTimeoutPolicy 对象的列表。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 69412f5f1add1da6d14adccc2012d60c4f7c8cf7
ms.sourcegitcommit: 0536ab327c8b8bf215b726e0d4c25e8f6e8996f9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/18/2020
ms.locfileid: "41234138"
---
# <a name="list-activitybasedtimeoutpolicies"></a><span data-ttu-id="c1e91-103">列出 activityBasedTimeoutPolicies</span><span class="sxs-lookup"><span data-stu-id="c1e91-103">List activityBasedTimeoutPolicies</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c1e91-104">获取[activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="c1e91-104">Get a list of [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="c1e91-105">Permissions</span><span class="sxs-lookup"><span data-stu-id="c1e91-105">Permissions</span></span>

<span data-ttu-id="c1e91-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c1e91-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c1e91-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="c1e91-108">Permission type</span></span>                        | <span data-ttu-id="c1e91-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c1e91-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="c1e91-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c1e91-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="c1e91-111">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="c1e91-111">Policy.Read.All</span></span> |
| <span data-ttu-id="c1e91-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c1e91-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c1e91-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="c1e91-113">Not supported.</span></span> |
| <span data-ttu-id="c1e91-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="c1e91-114">Application</span></span>                            | <span data-ttu-id="c1e91-115">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="c1e91-115">Policy.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c1e91-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c1e91-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET policies/activityBasedTimeoutPolicies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c1e91-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="c1e91-117">Optional query parameters</span></span>

<span data-ttu-id="c1e91-118">此方法支持`$filter` `$select`和`$top` OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="c1e91-118">This method supports the `$filter`, `$select` and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="c1e91-119">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="c1e91-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="c1e91-120">请求头</span><span class="sxs-lookup"><span data-stu-id="c1e91-120">Request headers</span></span>

| <span data-ttu-id="c1e91-121">名称</span><span class="sxs-lookup"><span data-stu-id="c1e91-121">Name</span></span>      |<span data-ttu-id="c1e91-122">说明</span><span class="sxs-lookup"><span data-stu-id="c1e91-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c1e91-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c1e91-123">Authorization</span></span> | <span data-ttu-id="c1e91-124">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="c1e91-124">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="c1e91-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="c1e91-125">Request body</span></span>

<span data-ttu-id="c1e91-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c1e91-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c1e91-127">响应</span><span class="sxs-lookup"><span data-stu-id="c1e91-127">Response</span></span>

<span data-ttu-id="c1e91-128">如果成功，此方法在响应`200 OK`正文中返回响应代码和[activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="c1e91-128">If successful, this method returns a `200 OK` response code and a collection of [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c1e91-129">示例</span><span class="sxs-lookup"><span data-stu-id="c1e91-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c1e91-130">请求</span><span class="sxs-lookup"><span data-stu-id="c1e91-130">Request</span></span>

<span data-ttu-id="c1e91-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c1e91-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_activitybasedtimeoutpolicies"
}-->

```http
GET https://graph.microsoft.com/beta/policies/activityBasedTimeoutPolicies
```

### <a name="response"></a><span data-ttu-id="c1e91-132">响应</span><span class="sxs-lookup"><span data-stu-id="c1e91-132">Response</span></span>

<span data-ttu-id="c1e91-133">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="c1e91-133">The following is an example of the response.</span></span>

> <span data-ttu-id="c1e91-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="c1e91-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
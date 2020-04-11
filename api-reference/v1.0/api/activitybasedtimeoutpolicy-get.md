---
title: 获取 activityBasedTimeoutPolicy
description: 获取 activityBasedTimeoutPolicy 对象的属性。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 59a51b16b04f1d5930d13074d4f372cffee2b8d9
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2020
ms.locfileid: "43227798"
---
# <a name="get-activitybasedtimeoutpolicy"></a><span data-ttu-id="64b75-103">获取 activityBasedTimeoutPolicy</span><span class="sxs-lookup"><span data-stu-id="64b75-103">Get activityBasedTimeoutPolicy</span></span>

<span data-ttu-id="64b75-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="64b75-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="64b75-105">获取[activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="64b75-105">Get the properties of an [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="64b75-106">权限</span><span class="sxs-lookup"><span data-stu-id="64b75-106">Permissions</span></span>

<span data-ttu-id="64b75-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="64b75-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="64b75-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="64b75-109">Permission type</span></span>                        | <span data-ttu-id="64b75-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="64b75-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="64b75-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="64b75-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="64b75-112">Policy： Read. All，ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="64b75-112">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="64b75-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="64b75-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="64b75-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="64b75-114">Not supported.</span></span> |
| <span data-ttu-id="64b75-115">Application</span><span class="sxs-lookup"><span data-stu-id="64b75-115">Application</span></span>                            | <span data-ttu-id="64b75-116">Policy： Read. All，ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="64b75-116">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="64b75-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="64b75-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/activityBasedTimeoutPolicies/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="64b75-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="64b75-118">Optional query parameters</span></span>

<span data-ttu-id="64b75-119">此方法支持`$select` OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="64b75-119">This method supports the `$select` OData query parameters to help customize the response.</span></span> <span data-ttu-id="64b75-120">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="64b75-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="64b75-121">请求头</span><span class="sxs-lookup"><span data-stu-id="64b75-121">Request headers</span></span>

| <span data-ttu-id="64b75-122">名称</span><span class="sxs-lookup"><span data-stu-id="64b75-122">Name</span></span>      |<span data-ttu-id="64b75-123">说明</span><span class="sxs-lookup"><span data-stu-id="64b75-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="64b75-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="64b75-124">Authorization</span></span> | <span data-ttu-id="64b75-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="64b75-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="64b75-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="64b75-127">Request body</span></span>

<span data-ttu-id="64b75-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="64b75-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="64b75-129">响应</span><span class="sxs-lookup"><span data-stu-id="64b75-129">Response</span></span>

<span data-ttu-id="64b75-130">如果成功，此方法在响应`200 OK`正文中返回响应代码和请求的[activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="64b75-130">If successful, this method returns a `200 OK` response code and the requested [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="64b75-131">示例</span><span class="sxs-lookup"><span data-stu-id="64b75-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="64b75-132">请求</span><span class="sxs-lookup"><span data-stu-id="64b75-132">Request</span></span>

<span data-ttu-id="64b75-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="64b75-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_activitybasedtimeoutpolicy"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/policies/activityBasedTimeoutPolicies/{id}
```

### <a name="response"></a><span data-ttu-id="64b75-134">响应</span><span class="sxs-lookup"><span data-stu-id="64b75-134">Response</span></span>

<span data-ttu-id="64b75-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="64b75-135">The following is an example of the response.</span></span>

> <span data-ttu-id="64b75-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="64b75-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

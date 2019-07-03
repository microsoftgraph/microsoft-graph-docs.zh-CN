---
title: 'reportRoot: getCredentialUsageSummary'
description: 报告贵组织中的用户数使用自助密码重置功能的当前状态。
localization_priority: Normal
author: davidmu1
ms.prod: reports
doc_type: apiPageType
ms.openlocfilehash: 6ec8afa24f83e50d2fcf354b37e1f5524eea2295
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35479041"
---
# <a name="reportroot-getcredentialusagesummary"></a><span data-ttu-id="74d33-103">reportRoot: getCredentialUsageSummary</span><span class="sxs-lookup"><span data-stu-id="74d33-103">reportRoot: getCredentialUsageSummary</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="74d33-104">报告您的组织中的用户数使用自助密码重置功能的当前状态。</span><span class="sxs-lookup"><span data-stu-id="74d33-104">Report the current state of how many users in your organization used the self-service password reset capabilities.</span></span>

## <a name="permissions"></a><span data-ttu-id="74d33-105">权限</span><span class="sxs-lookup"><span data-stu-id="74d33-105">Permissions</span></span>

<span data-ttu-id="74d33-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="74d33-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="74d33-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="74d33-108">Permission type</span></span>                        | <span data-ttu-id="74d33-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="74d33-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="74d33-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="74d33-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="74d33-111">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="74d33-111">Reports.Read.All</span></span> |
| <span data-ttu-id="74d33-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="74d33-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="74d33-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="74d33-113">Not supported.</span></span> |
| <span data-ttu-id="74d33-114">应用</span><span class="sxs-lookup"><span data-stu-id="74d33-114">Application</span></span>                            | <span data-ttu-id="74d33-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="74d33-115">Reports.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="74d33-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="74d33-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getCredentialUsageSummary
```

## <a name="function-parameters"></a><span data-ttu-id="74d33-117">函数参数</span><span class="sxs-lookup"><span data-stu-id="74d33-117">Function parameters</span></span>

<span data-ttu-id="74d33-118">您可以使用以下函数参数来调整响应。</span><span class="sxs-lookup"><span data-stu-id="74d33-118">You can use the following function parameter to adjust the response.</span></span>

| <span data-ttu-id="74d33-119">参数</span><span class="sxs-lookup"><span data-stu-id="74d33-119">Parameter</span></span> | <span data-ttu-id="74d33-120">类型</span><span class="sxs-lookup"><span data-stu-id="74d33-120">Type</span></span> | <span data-ttu-id="74d33-121">说明</span><span class="sxs-lookup"><span data-stu-id="74d33-121">Description</span></span> |
|:--------- |:---- |:----------- |
| <span data-ttu-id="74d33-122">period</span><span class="sxs-lookup"><span data-stu-id="74d33-122">period</span></span> | <span data-ttu-id="74d33-123">String</span><span class="sxs-lookup"><span data-stu-id="74d33-123">String</span></span> | <span data-ttu-id="74d33-124">指定需要使用情况数据的时间段。</span><span class="sxs-lookup"><span data-stu-id="74d33-124">Specifies the time period for which you need the usage data.</span></span> <span data-ttu-id="74d33-125">例如：`/reports/getCredentialUsageSummary(period='D30')`。</span><span class="sxs-lookup"><span data-stu-id="74d33-125">For example: `/reports/getCredentialUsageSummary(period='D30')`.</span></span> <span data-ttu-id="74d33-126">支持的期间`D1`: `D7`、和`D30`。</span><span class="sxs-lookup"><span data-stu-id="74d33-126">Supported periods: `D1`, `D7`, and `D30`.</span></span> <span data-ttu-id="74d33-127">Period 不区分大小写。</span><span class="sxs-lookup"><span data-stu-id="74d33-127">Period is case insensitive.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="74d33-128">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="74d33-128">Optional query parameters</span></span>

<span data-ttu-id="74d33-129">此函数支持可选的 OData 查询参数 **$filter**。</span><span class="sxs-lookup"><span data-stu-id="74d33-129">This function supports the optional OData query parameter **$filter**.</span></span> <span data-ttu-id="74d33-130">您可以对[credentialUsageSummary](../resources/credentialusagesummary.md)资源的以下一个或多个属性应用 **$filter** 。</span><span class="sxs-lookup"><span data-stu-id="74d33-130">You can apply **$filter** on one or more of the following properties of the [credentialUsageSummary](../resources/credentialusagesummary.md) resource.</span></span>

| <span data-ttu-id="74d33-131">属性</span><span class="sxs-lookup"><span data-stu-id="74d33-131">Properties</span></span> | <span data-ttu-id="74d33-132">说明和示例</span><span class="sxs-lookup"><span data-stu-id="74d33-132">Description and example</span></span> |
|:---- |:----------- |
| <span data-ttu-id="74d33-133">功能</span><span class="sxs-lookup"><span data-stu-id="74d33-133">feature</span></span> | <span data-ttu-id="74d33-134">指定所需的使用率数据的类型 (注册与重置)。</span><span class="sxs-lookup"><span data-stu-id="74d33-134">Specifies the type of usage data you want (registration vs. reset).</span></span> <span data-ttu-id="74d33-135">例如：`/reports/getCredentialUsageSummary(period='D30')?$filter=feature eq 'registration'`。</span><span class="sxs-lookup"><span data-stu-id="74d33-135">For example: `/reports/getCredentialUsageSummary(period='D30')?$filter=feature eq 'registration'`.</span></span> <span data-ttu-id="74d33-136">支持的筛选器`eq`运算符:。</span><span class="sxs-lookup"><span data-stu-id="74d33-136">Supported filter operators: `eq`.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="74d33-137">请求标头</span><span class="sxs-lookup"><span data-stu-id="74d33-137">Request headers</span></span>

| <span data-ttu-id="74d33-138">名称</span><span class="sxs-lookup"><span data-stu-id="74d33-138">Name</span></span>          | <span data-ttu-id="74d33-139">说明</span><span class="sxs-lookup"><span data-stu-id="74d33-139">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="74d33-140">Authorization</span><span class="sxs-lookup"><span data-stu-id="74d33-140">Authorization</span></span> | <span data-ttu-id="74d33-141">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="74d33-141">Bearer {token}</span></span> |
| <span data-ttu-id="74d33-142">Content-Type</span><span class="sxs-lookup"><span data-stu-id="74d33-142">Content-Type</span></span> | <span data-ttu-id="74d33-143">application/json</span><span class="sxs-lookup"><span data-stu-id="74d33-143">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="74d33-144">请求正文</span><span class="sxs-lookup"><span data-stu-id="74d33-144">Request body</span></span>

<span data-ttu-id="74d33-145">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="74d33-145">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="74d33-146">响应</span><span class="sxs-lookup"><span data-stu-id="74d33-146">Response</span></span>

<span data-ttu-id="74d33-147">如果成功, 此方法在响应`200 OK`正文中返回响应代码和新的[credentialUsageSummary](../resources/credentialusagesummary.md)集合对象。</span><span class="sxs-lookup"><span data-stu-id="74d33-147">If successful, this method returns a `200 OK` response code and a new [credentialUsageSummary](../resources/credentialusagesummary.md) collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="74d33-148">示例</span><span class="sxs-lookup"><span data-stu-id="74d33-148">Examples</span></span>

<span data-ttu-id="74d33-149">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="74d33-149">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="74d33-150">请求</span><span class="sxs-lookup"><span data-stu-id="74d33-150">Request</span></span>

<span data-ttu-id="74d33-151">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="74d33-151">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "reportroot_getcredentialusagesummary"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getCredentialUsageSummary(period='D30')?$filter=feature eq 'registration'
```

### <a name="response"></a><span data-ttu-id="74d33-152">响应</span><span class="sxs-lookup"><span data-stu-id="74d33-152">Response</span></span>

<span data-ttu-id="74d33-153">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="74d33-153">The following is an example of the response.</span></span>

> <span data-ttu-id="74d33-154">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="74d33-154">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="74d33-155">所有属性都是从实际调用返回的。</span><span class="sxs-lookup"><span data-stu-id="74d33-155">All the properties are returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.credentialUsageSummary",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/reports/$metadata#Collection(microsoft.graph.getCredentialUsageSummary)",
  "value":[
    {
      "id" : "id-value",
      "feature":"registration",
      "successfulActivityCount":12345,
      "failureActivityCount": 123,
      "authMethod": "email"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "reportRoot: getCredentialUsageSummary",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
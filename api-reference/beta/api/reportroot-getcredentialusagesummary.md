---
title: reportRoot： getCredentialUsageSummary
description: 报告贵组织中的用户数使用自助密码重置功能的当前状态。
localization_priority: Normal
author: khotz
ms.prod: reports
doc_type: apiPageType
ms.openlocfilehash: 79037b8c941989ddba273a34184d00607758fafb
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43473907"
---
# <a name="reportroot-getcredentialusagesummary"></a><span data-ttu-id="55f90-103">reportRoot： getCredentialUsageSummary</span><span class="sxs-lookup"><span data-stu-id="55f90-103">reportRoot: getCredentialUsageSummary</span></span>

<span data-ttu-id="55f90-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="55f90-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="55f90-105">报告您的组织中的用户数使用自助密码重置功能的当前状态。</span><span class="sxs-lookup"><span data-stu-id="55f90-105">Report the current state of how many users in your organization used the self-service password reset capabilities.</span></span>

## <a name="permissions"></a><span data-ttu-id="55f90-106">权限</span><span class="sxs-lookup"><span data-stu-id="55f90-106">Permissions</span></span>

<span data-ttu-id="55f90-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="55f90-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="55f90-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="55f90-109">Permission type</span></span>                        | <span data-ttu-id="55f90-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="55f90-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="55f90-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="55f90-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="55f90-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="55f90-112">Reports.Read.All</span></span> |
| <span data-ttu-id="55f90-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="55f90-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="55f90-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="55f90-114">Not supported.</span></span> |
| <span data-ttu-id="55f90-115">应用</span><span class="sxs-lookup"><span data-stu-id="55f90-115">Application</span></span>                            | <span data-ttu-id="55f90-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="55f90-116">Reports.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="55f90-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="55f90-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getCredentialUsageSummary
```

## <a name="function-parameters"></a><span data-ttu-id="55f90-118">函数参数</span><span class="sxs-lookup"><span data-stu-id="55f90-118">Function parameters</span></span>

<span data-ttu-id="55f90-119">您可以使用以下函数参数来调整响应。</span><span class="sxs-lookup"><span data-stu-id="55f90-119">You can use the following function parameter to adjust the response.</span></span>

| <span data-ttu-id="55f90-120">参数</span><span class="sxs-lookup"><span data-stu-id="55f90-120">Parameter</span></span> | <span data-ttu-id="55f90-121">类型</span><span class="sxs-lookup"><span data-stu-id="55f90-121">Type</span></span> | <span data-ttu-id="55f90-122">说明</span><span class="sxs-lookup"><span data-stu-id="55f90-122">Description</span></span> |
|:--------- |:---- |:----------- |
| <span data-ttu-id="55f90-123">period</span><span class="sxs-lookup"><span data-stu-id="55f90-123">period</span></span> | <span data-ttu-id="55f90-124">String</span><span class="sxs-lookup"><span data-stu-id="55f90-124">String</span></span> | <span data-ttu-id="55f90-125">指定需要使用情况数据的时间段。</span><span class="sxs-lookup"><span data-stu-id="55f90-125">Specifies the time period for which you need the usage data.</span></span> <span data-ttu-id="55f90-126">例如：`/reports/getCredentialUsageSummary(period='D30')`。</span><span class="sxs-lookup"><span data-stu-id="55f90-126">For example: `/reports/getCredentialUsageSummary(period='D30')`.</span></span> <span data-ttu-id="55f90-127">支持的期间`D1`： `D7`、和`D30`。</span><span class="sxs-lookup"><span data-stu-id="55f90-127">Supported periods: `D1`, `D7`, and `D30`.</span></span> <span data-ttu-id="55f90-128">Period 不区分大小写。</span><span class="sxs-lookup"><span data-stu-id="55f90-128">Period is case insensitive.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="55f90-129">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="55f90-129">Optional query parameters</span></span>

<span data-ttu-id="55f90-130">此函数支持可选的 OData 查询参数 **$filter**。</span><span class="sxs-lookup"><span data-stu-id="55f90-130">This function supports the optional OData query parameter **$filter**.</span></span> <span data-ttu-id="55f90-131">您可以对[credentialUsageSummary](../resources/credentialusagesummary.md)资源的以下一个或多个属性应用 **$filter** 。</span><span class="sxs-lookup"><span data-stu-id="55f90-131">You can apply **$filter** on one or more of the following properties of the [credentialUsageSummary](../resources/credentialusagesummary.md) resource.</span></span>

| <span data-ttu-id="55f90-132">属性</span><span class="sxs-lookup"><span data-stu-id="55f90-132">Properties</span></span> | <span data-ttu-id="55f90-133">说明和示例</span><span class="sxs-lookup"><span data-stu-id="55f90-133">Description and example</span></span> |
|:---- |:----------- |
| <span data-ttu-id="55f90-134">功能</span><span class="sxs-lookup"><span data-stu-id="55f90-134">feature</span></span> | <span data-ttu-id="55f90-135">指定所需的使用率数据的类型（注册与重置）。</span><span class="sxs-lookup"><span data-stu-id="55f90-135">Specifies the type of usage data you want (registration vs. reset).</span></span> <span data-ttu-id="55f90-136">例如：`/reports/getCredentialUsageSummary(period='D30')?$filter=feature eq 'registration'`。</span><span class="sxs-lookup"><span data-stu-id="55f90-136">For example: `/reports/getCredentialUsageSummary(period='D30')?$filter=feature eq 'registration'`.</span></span> <span data-ttu-id="55f90-137">支持的筛选器`eq`运算符：。</span><span class="sxs-lookup"><span data-stu-id="55f90-137">Supported filter operators: `eq`.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="55f90-138">请求标头</span><span class="sxs-lookup"><span data-stu-id="55f90-138">Request headers</span></span>

| <span data-ttu-id="55f90-139">名称</span><span class="sxs-lookup"><span data-stu-id="55f90-139">Name</span></span>          | <span data-ttu-id="55f90-140">说明</span><span class="sxs-lookup"><span data-stu-id="55f90-140">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="55f90-141">Authorization</span><span class="sxs-lookup"><span data-stu-id="55f90-141">Authorization</span></span> | <span data-ttu-id="55f90-142">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="55f90-142">Bearer {token}</span></span> |
| <span data-ttu-id="55f90-143">Content-Type</span><span class="sxs-lookup"><span data-stu-id="55f90-143">Content-Type</span></span> | <span data-ttu-id="55f90-144">application/json</span><span class="sxs-lookup"><span data-stu-id="55f90-144">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="55f90-145">请求正文</span><span class="sxs-lookup"><span data-stu-id="55f90-145">Request body</span></span>

<span data-ttu-id="55f90-146">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="55f90-146">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="55f90-147">响应</span><span class="sxs-lookup"><span data-stu-id="55f90-147">Response</span></span>

<span data-ttu-id="55f90-148">如果成功，此方法在响应`200 OK`正文中返回响应代码和新的[credentialUsageSummary](../resources/credentialusagesummary.md)集合对象。</span><span class="sxs-lookup"><span data-stu-id="55f90-148">If successful, this method returns a `200 OK` response code and a new [credentialUsageSummary](../resources/credentialusagesummary.md) collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="55f90-149">示例</span><span class="sxs-lookup"><span data-stu-id="55f90-149">Examples</span></span>

<span data-ttu-id="55f90-150">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="55f90-150">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="55f90-151">请求</span><span class="sxs-lookup"><span data-stu-id="55f90-151">Request</span></span>

<span data-ttu-id="55f90-152">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="55f90-152">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="55f90-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="55f90-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getcredentialusagesummary"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getCredentialUsageSummary(period='D30')?$filter=feature eq 'registration'
```
# <a name="c"></a>[<span data-ttu-id="55f90-154">C#</span><span class="sxs-lookup"><span data-stu-id="55f90-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getcredentialusagesummary-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="55f90-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="55f90-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getcredentialusagesummary-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="55f90-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="55f90-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getcredentialusagesummary-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="55f90-157">响应</span><span class="sxs-lookup"><span data-stu-id="55f90-157">Response</span></span>

<span data-ttu-id="55f90-158">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="55f90-158">The following is an example of the response.</span></span>

> <span data-ttu-id="55f90-159">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="55f90-159">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="55f90-160">所有属性都是从实际调用返回的。</span><span class="sxs-lookup"><span data-stu-id="55f90-160">All the properties are returned from an actual call.</span></span>

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

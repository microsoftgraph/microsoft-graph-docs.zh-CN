---
title: 列出 userCredentialUsageDetails
description: 获取给定租户的 userCredentialUsageDetails 对象的列表。
localization_priority: Normal
author: davidmu1
ms.prod: reports
doc_type: apiPageType
ms.openlocfilehash: 1ea46387a4d4f4c0920a94a2d082a20090fe0bb0
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35871201"
---
# <a name="list-usercredentialusagedetails"></a><span data-ttu-id="ce331-103">列出 userCredentialUsageDetails</span><span class="sxs-lookup"><span data-stu-id="ce331-103">List userCredentialUsageDetails</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ce331-104">获取给定租户的[userCredentialUsageDetails](../resources/usercredentialusagedetails.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="ce331-104">Get a list of [userCredentialUsageDetails](../resources/usercredentialusagedetails.md) objects for a given tenant.</span></span> <span data-ttu-id="ce331-105">详细信息包括用户信息、重置状态和失败原因。</span><span class="sxs-lookup"><span data-stu-id="ce331-105">Details include user information, status of the reset, and the reason for failure.</span></span>

## <a name="permissions"></a><span data-ttu-id="ce331-106">权限</span><span class="sxs-lookup"><span data-stu-id="ce331-106">Permissions</span></span>

<span data-ttu-id="ce331-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ce331-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ce331-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="ce331-109">Permission type</span></span>                        | <span data-ttu-id="ce331-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ce331-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ce331-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ce331-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ce331-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="ce331-112">Reports.Read.All</span></span> |
| <span data-ttu-id="ce331-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ce331-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ce331-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="ce331-114">Not supported.</span></span> |
| <span data-ttu-id="ce331-115">应用</span><span class="sxs-lookup"><span data-stu-id="ce331-115">Application</span></span>                            | <span data-ttu-id="ce331-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="ce331-116">Reports.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ce331-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ce331-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/userCredentialUsageDetails
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ce331-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="ce331-118">Optional query parameters</span></span>

<span data-ttu-id="ce331-119">此函数支持可选的 OData 查询参数 **$filter**。</span><span class="sxs-lookup"><span data-stu-id="ce331-119">This function supports the optional OData query parameter **$filter**.</span></span> <span data-ttu-id="ce331-120">您可以对[userCredentialUsageDetails](../resources/usercredentialusagedetails.md)资源的以下一个或多个属性应用 **$filter** 。</span><span class="sxs-lookup"><span data-stu-id="ce331-120">You can apply **$filter** on one or more of the following properties of the [userCredentialUsageDetails](../resources/usercredentialusagedetails.md) resource.</span></span>

| <span data-ttu-id="ce331-121">属性</span><span class="sxs-lookup"><span data-stu-id="ce331-121">Properties</span></span> | <span data-ttu-id="ce331-122">说明和示例</span><span class="sxs-lookup"><span data-stu-id="ce331-122">Description and example</span></span> |
|:--------- |:----------- |
| <span data-ttu-id="ce331-123">功能</span><span class="sxs-lookup"><span data-stu-id="ce331-123">feature</span></span> | <span data-ttu-id="ce331-124">按所需的使用情况数据类型进行筛选 (注册与重置)。</span><span class="sxs-lookup"><span data-stu-id="ce331-124">Filter by type of usage data that you want (registration vs reset).</span></span> <span data-ttu-id="ce331-125">例如：`/reports/userCredentialUsageDetails?$filter=feature eq 'registration'`。</span><span class="sxs-lookup"><span data-stu-id="ce331-125">For example: `/reports/userCredentialUsageDetails?$filter=feature eq 'registration'`.</span></span> <span data-ttu-id="ce331-126">支持的筛选器运算符:`eq`</span><span class="sxs-lookup"><span data-stu-id="ce331-126">Supported filter operators: `eq`</span></span> |
| <span data-ttu-id="ce331-127">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="ce331-127">userDisplayName</span></span> | <span data-ttu-id="ce331-128">按用户显示名称筛选。</span><span class="sxs-lookup"><span data-stu-id="ce331-128">Filter by user display name.</span></span> <span data-ttu-id="ce331-129">例如：`/reports/userCredentialUsageDetails?$filter=userDisplayName eq 'Contoso'`。</span><span class="sxs-lookup"><span data-stu-id="ce331-129">For example: `/reports/userCredentialUsageDetails?$filter=userDisplayName eq 'Contoso'`.</span></span> <span data-ttu-id="ce331-130">支持的筛选器`eq`运算符`startswith()`: 和。</span><span class="sxs-lookup"><span data-stu-id="ce331-130">Supported filter operators: `eq` and `startswith()`.</span></span> <span data-ttu-id="ce331-131">支持不区分大小写。</span><span class="sxs-lookup"><span data-stu-id="ce331-131">Supports case insensitive.</span></span> |
| <span data-ttu-id="ce331-132">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="ce331-132">userPrincipalName</span></span>  | <span data-ttu-id="ce331-133">按用户主体名称筛选。</span><span class="sxs-lookup"><span data-stu-id="ce331-133">Filter by user principal name.</span></span> <span data-ttu-id="ce331-134">例如：`/reports/userCredentialUsageDetails?$filter=userPrincipalName eq 'Contoso'`。</span><span class="sxs-lookup"><span data-stu-id="ce331-134">For example: `/reports/userCredentialUsageDetails?$filter=userPrincipalName eq 'Contoso'`.</span></span>    <span data-ttu-id="ce331-135">支持的筛选器`eq`运算符`startswith()`: 和。</span><span class="sxs-lookup"><span data-stu-id="ce331-135">Supported filter  operators: `eq` and `startswith()`.</span></span> <span data-ttu-id="ce331-136">支持不区分大小写。</span><span class="sxs-lookup"><span data-stu-id="ce331-136">Supports case insensitive.</span></span> |
| <span data-ttu-id="ce331-137">isSuccess</span><span class="sxs-lookup"><span data-stu-id="ce331-137">isSuccess</span></span> | <span data-ttu-id="ce331-138">按活动状态进行筛选。</span><span class="sxs-lookup"><span data-stu-id="ce331-138">Filter by status of the activity.</span></span> <span data-ttu-id="ce331-139">例如：`/reports/userCredentialUsageDetails?$filter=isSuccess eq true`。</span><span class="sxs-lookup"><span data-stu-id="ce331-139">For example: `/reports/userCredentialUsageDetails?$filter=isSuccess eq true`.</span></span> <span data-ttu-id="ce331-140">支持的筛选器`eq`运算符`orderby`: 和。</span><span class="sxs-lookup"><span data-stu-id="ce331-140">Supported filter operators: `eq` and `orderby`.</span></span> |
| <span data-ttu-id="ce331-141">authMethod</span><span class="sxs-lookup"><span data-stu-id="ce331-141">authMethod</span></span>  | <span data-ttu-id="ce331-142">在注册过程中使用身份验证方法进行筛选。</span><span class="sxs-lookup"><span data-stu-id="ce331-142">Filter by the authentication methods using during registration.</span></span> <span data-ttu-id="ce331-143">例如：`/reports/userCredentialUsageDetails?$filter=authMethod eq microsoft.graph.usageAuthMethod'email'`。</span><span class="sxs-lookup"><span data-stu-id="ce331-143">For example: `/reports/userCredentialUsageDetails?$filter=authMethod eq microsoft.graph.usageAuthMethod'email'`.</span></span> <span data-ttu-id="ce331-144">支持的筛选器`eq`运算符:。</span><span class="sxs-lookup"><span data-stu-id="ce331-144">Supported filter operators: `eq`.</span></span> |
| <span data-ttu-id="ce331-145">failureReason</span><span class="sxs-lookup"><span data-stu-id="ce331-145">failureReason</span></span> | <span data-ttu-id="ce331-146">按失败原因筛选 (如果活动已失败)。</span><span class="sxs-lookup"><span data-stu-id="ce331-146">Filter by failure reason (if the activity has failed).</span></span> <span data-ttu-id="ce331-147">例如：`/reports/userCredentialUsageDetails?$filter=failureReason eq 'Contoso'`。</span><span class="sxs-lookup"><span data-stu-id="ce331-147">For example: `/reports/userCredentialUsageDetails?$filter=failureReason eq 'Contoso'`.</span></span> <span data-ttu-id="ce331-148">支持的筛选器`eq`运算符`startswith()`: 和。</span><span class="sxs-lookup"><span data-stu-id="ce331-148">Supported filter operators: `eq` and `startswith()`.</span></span> <span data-ttu-id="ce331-149">支持不区分大小写。</span><span class="sxs-lookup"><span data-stu-id="ce331-149">Supports case insensitive.</span></span> |


## <a name="request-headers"></a><span data-ttu-id="ce331-150">请求标头</span><span class="sxs-lookup"><span data-stu-id="ce331-150">Request headers</span></span>

| <span data-ttu-id="ce331-151">名称</span><span class="sxs-lookup"><span data-stu-id="ce331-151">Name</span></span>      |<span data-ttu-id="ce331-152">说明</span><span class="sxs-lookup"><span data-stu-id="ce331-152">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ce331-153">Authorization</span><span class="sxs-lookup"><span data-stu-id="ce331-153">Authorization</span></span> | <span data-ttu-id="ce331-154">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="ce331-154">Bearer {token}</span></span> |
| <span data-ttu-id="ce331-155">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ce331-155">Content-Type</span></span> | <span data-ttu-id="ce331-156">application/json</span><span class="sxs-lookup"><span data-stu-id="ce331-156">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="ce331-157">请求正文</span><span class="sxs-lookup"><span data-stu-id="ce331-157">Request body</span></span>

<span data-ttu-id="ce331-158">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ce331-158">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ce331-159">响应</span><span class="sxs-lookup"><span data-stu-id="ce331-159">Response</span></span>

<span data-ttu-id="ce331-160">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[userCredentialUsageDetails](../resources/usercredentialusagedetails.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="ce331-160">If successful, this method returns a `200 OK` response code and a collection of [userCredentialUsageDetails](../resources/usercredentialusagedetails.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ce331-161">示例</span><span class="sxs-lookup"><span data-stu-id="ce331-161">Examples</span></span>

<span data-ttu-id="ce331-162">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="ce331-162">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="ce331-163">请求</span><span class="sxs-lookup"><span data-stu-id="ce331-163">Request</span></span>

<span data-ttu-id="ce331-164">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ce331-164">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="ce331-165">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="ce331-165">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_usercredentialusagedetails"
}-->

```http
GET https://graph.microsoft.com/beta/reports/userCredentialUsageDetails
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ce331-166">C#</span><span class="sxs-lookup"><span data-stu-id="ce331-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-usercredentialusagedetails-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ce331-167">Javascript</span><span class="sxs-lookup"><span data-stu-id="ce331-167">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-usercredentialusagedetails-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ce331-168">目标-C</span><span class="sxs-lookup"><span data-stu-id="ce331-168">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-usercredentialusagedetails-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="ce331-169">Java</span><span class="sxs-lookup"><span data-stu-id="ce331-169">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-usercredentialusagedetails-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ce331-170">响应</span><span class="sxs-lookup"><span data-stu-id="ce331-170">Response</span></span>

<span data-ttu-id="ce331-171">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="ce331-171">The following is an example of the response.</span></span>

> <span data-ttu-id="ce331-172">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="ce331-172">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="ce331-173">所有属性都是从实际调用返回的。</span><span class="sxs-lookup"><span data-stu-id="ce331-173">All the properties are returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.userCredentialUsageDetails",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 258

{
  "@odata.context":"https://graph.microsoft.com/beta/reports/$metadata#Collection(microsoft.graph.getUserCredentialUsageDetails)",
  "value":[
    {
      "id" : "id-value",
      "feature":"registration",
      "userPrincipalName":"userPrincipalName-value",
      "userDisplayName": "userDisplayName-value",
      "isSuccess" : true,
      "authMethod": "email",
      "failureReason": "User contacted an admin after trying the email verification option",
      "eventDateTime" : "2019-04-01T00:00:00Z"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List userCredentialUsageDetails",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

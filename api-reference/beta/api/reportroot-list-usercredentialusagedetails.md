---
title: 列出 userCredentialUsageDetails
description: 获取给定租户的 userCredentialUsageDetails 对象列表。
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
doc_type: apiPageType
ms.openlocfilehash: e64d98318bcf9b083005f79156bc425a3b0d0fbc
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50134482"
---
# <a name="list-usercredentialusagedetails"></a><span data-ttu-id="e1227-103">列出 userCredentialUsageDetails</span><span class="sxs-lookup"><span data-stu-id="e1227-103">List userCredentialUsageDetails</span></span>

<span data-ttu-id="e1227-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e1227-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e1227-105">获取给定 [租户的 userCredentialUsageDetails](../resources/usercredentialusagedetails.md) 对象列表。</span><span class="sxs-lookup"><span data-stu-id="e1227-105">Get a list of [userCredentialUsageDetails](../resources/usercredentialusagedetails.md) objects for a given tenant.</span></span> <span data-ttu-id="e1227-106">详细信息包括用户信息、重置状态和失败原因。</span><span class="sxs-lookup"><span data-stu-id="e1227-106">Details include user information, status of the reset, and the reason for failure.</span></span>

## <a name="permissions"></a><span data-ttu-id="e1227-107">权限</span><span class="sxs-lookup"><span data-stu-id="e1227-107">Permissions</span></span>

<span data-ttu-id="e1227-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e1227-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e1227-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="e1227-110">Permission type</span></span>                        | <span data-ttu-id="e1227-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e1227-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e1227-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e1227-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="e1227-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="e1227-113">Reports.Read.All</span></span> |
| <span data-ttu-id="e1227-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e1227-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e1227-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="e1227-115">Not supported.</span></span> |
| <span data-ttu-id="e1227-116">应用</span><span class="sxs-lookup"><span data-stu-id="e1227-116">Application</span></span>                            | <span data-ttu-id="e1227-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="e1227-117">Reports.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e1227-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e1227-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/userCredentialUsageDetails
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e1227-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="e1227-119">Optional query parameters</span></span>

<span data-ttu-id="e1227-120">此函数支持可选的 OData 查询 **参数**$filter。</span><span class="sxs-lookup"><span data-stu-id="e1227-120">This function supports the optional OData query parameter **$filter**.</span></span> <span data-ttu-id="e1227-121">你可以 **将$filter** [userCredentialUsageDetails](../resources/usercredentialusagedetails.md) 资源的以下一个或多个属性应用。</span><span class="sxs-lookup"><span data-stu-id="e1227-121">You can apply **$filter** on one or more of the following properties of the [userCredentialUsageDetails](../resources/usercredentialusagedetails.md) resource.</span></span>

| <span data-ttu-id="e1227-122">属性</span><span class="sxs-lookup"><span data-stu-id="e1227-122">Properties</span></span> | <span data-ttu-id="e1227-123">说明和示例</span><span class="sxs-lookup"><span data-stu-id="e1227-123">Description and example</span></span> |
|:--------- |:----------- |
| <span data-ttu-id="e1227-124">功能</span><span class="sxs-lookup"><span data-stu-id="e1227-124">feature</span></span> | <span data-ttu-id="e1227-125">按要注册和重置的使用情况 (类型) 。</span><span class="sxs-lookup"><span data-stu-id="e1227-125">Filter by type of usage data that you want (registration vs reset).</span></span> <span data-ttu-id="e1227-126">例如：`/reports/userCredentialUsageDetails?$filter=feature eq 'registration'`。</span><span class="sxs-lookup"><span data-stu-id="e1227-126">For example: `/reports/userCredentialUsageDetails?$filter=feature eq 'registration'`.</span></span> <span data-ttu-id="e1227-127">支持的筛选器运算符： `eq`</span><span class="sxs-lookup"><span data-stu-id="e1227-127">Supported filter operators: `eq`</span></span> |
| <span data-ttu-id="e1227-128">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="e1227-128">userDisplayName</span></span> | <span data-ttu-id="e1227-129">按用户筛选显示名称。</span><span class="sxs-lookup"><span data-stu-id="e1227-129">Filter by user display name.</span></span> <span data-ttu-id="e1227-130">例如：`/reports/userCredentialUsageDetails?$filter=userDisplayName eq 'Contoso'`。</span><span class="sxs-lookup"><span data-stu-id="e1227-130">For example: `/reports/userCredentialUsageDetails?$filter=userDisplayName eq 'Contoso'`.</span></span> <span data-ttu-id="e1227-131">支持的筛选器运算符： `eq` 和 `startswith()` 。</span><span class="sxs-lookup"><span data-stu-id="e1227-131">Supported filter operators: `eq` and `startswith()`.</span></span> <span data-ttu-id="e1227-132">支持不区分大小写。</span><span class="sxs-lookup"><span data-stu-id="e1227-132">Supports case insensitive.</span></span> |
| <span data-ttu-id="e1227-133">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="e1227-133">userPrincipalName</span></span>  | <span data-ttu-id="e1227-134">按用户主体名称进行筛选。</span><span class="sxs-lookup"><span data-stu-id="e1227-134">Filter by user principal name.</span></span> <span data-ttu-id="e1227-135">例如：`/reports/userCredentialUsageDetails?$filter=userPrincipalName eq 'Contoso'`。</span><span class="sxs-lookup"><span data-stu-id="e1227-135">For example: `/reports/userCredentialUsageDetails?$filter=userPrincipalName eq 'Contoso'`.</span></span>    <span data-ttu-id="e1227-136">支持的筛选器运算符： `eq` 和 `startswith()` 。</span><span class="sxs-lookup"><span data-stu-id="e1227-136">Supported filter  operators: `eq` and `startswith()`.</span></span> <span data-ttu-id="e1227-137">支持不区分大小写。</span><span class="sxs-lookup"><span data-stu-id="e1227-137">Supports case insensitive.</span></span> |
| <span data-ttu-id="e1227-138">isSuccess</span><span class="sxs-lookup"><span data-stu-id="e1227-138">isSuccess</span></span> | <span data-ttu-id="e1227-139">按活动状态进行筛选。</span><span class="sxs-lookup"><span data-stu-id="e1227-139">Filter by status of the activity.</span></span> <span data-ttu-id="e1227-140">例如：`/reports/userCredentialUsageDetails?$filter=isSuccess eq true`。</span><span class="sxs-lookup"><span data-stu-id="e1227-140">For example: `/reports/userCredentialUsageDetails?$filter=isSuccess eq true`.</span></span> <span data-ttu-id="e1227-141">支持的筛选器运算符： `eq` 和 `orderby` 。</span><span class="sxs-lookup"><span data-stu-id="e1227-141">Supported filter operators: `eq` and `orderby`.</span></span> |
| <span data-ttu-id="e1227-142">authMethod</span><span class="sxs-lookup"><span data-stu-id="e1227-142">authMethod</span></span>  | <span data-ttu-id="e1227-143">按注册期间使用的身份验证方法进行筛选。</span><span class="sxs-lookup"><span data-stu-id="e1227-143">Filter by the authentication methods using during registration.</span></span> <span data-ttu-id="e1227-144">例如：`/reports/userCredentialUsageDetails?$filter=authMethod eq microsoft.graph.usageAuthMethod'email'`。</span><span class="sxs-lookup"><span data-stu-id="e1227-144">For example: `/reports/userCredentialUsageDetails?$filter=authMethod eq microsoft.graph.usageAuthMethod'email'`.</span></span> <span data-ttu-id="e1227-145">支持的筛选器运算符： `eq` .</span><span class="sxs-lookup"><span data-stu-id="e1227-145">Supported filter operators: `eq`.</span></span> |
| <span data-ttu-id="e1227-146">failureReason</span><span class="sxs-lookup"><span data-stu-id="e1227-146">failureReason</span></span> | <span data-ttu-id="e1227-147">如果活动失败， (失败原因筛选) 。</span><span class="sxs-lookup"><span data-stu-id="e1227-147">Filter by failure reason (if the activity has failed).</span></span> <span data-ttu-id="e1227-148">例如：`/reports/userCredentialUsageDetails?$filter=failureReason eq 'Contoso'`。</span><span class="sxs-lookup"><span data-stu-id="e1227-148">For example: `/reports/userCredentialUsageDetails?$filter=failureReason eq 'Contoso'`.</span></span> <span data-ttu-id="e1227-149">支持的筛选器运算符： `eq` 和 `startswith()` 。</span><span class="sxs-lookup"><span data-stu-id="e1227-149">Supported filter operators: `eq` and `startswith()`.</span></span> <span data-ttu-id="e1227-150">支持不区分大小写。</span><span class="sxs-lookup"><span data-stu-id="e1227-150">Supports case insensitive.</span></span> |


## <a name="request-headers"></a><span data-ttu-id="e1227-151">请求标头</span><span class="sxs-lookup"><span data-stu-id="e1227-151">Request headers</span></span>

| <span data-ttu-id="e1227-152">名称</span><span class="sxs-lookup"><span data-stu-id="e1227-152">Name</span></span>      |<span data-ttu-id="e1227-153">说明</span><span class="sxs-lookup"><span data-stu-id="e1227-153">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e1227-154">Authorization</span><span class="sxs-lookup"><span data-stu-id="e1227-154">Authorization</span></span> | <span data-ttu-id="e1227-155">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="e1227-155">Bearer {token}</span></span> |
| <span data-ttu-id="e1227-156">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e1227-156">Content-Type</span></span> | <span data-ttu-id="e1227-157">application/json</span><span class="sxs-lookup"><span data-stu-id="e1227-157">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="e1227-158">请求正文</span><span class="sxs-lookup"><span data-stu-id="e1227-158">Request body</span></span>

<span data-ttu-id="e1227-159">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e1227-159">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e1227-160">响应</span><span class="sxs-lookup"><span data-stu-id="e1227-160">Response</span></span>

<span data-ttu-id="e1227-161">如果成功，此方法在响应正文中返回响应代码和 `200 OK` [userCredentialUsageDetails](../resources/usercredentialusagedetails.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="e1227-161">If successful, this method returns a `200 OK` response code and a collection of [userCredentialUsageDetails](../resources/usercredentialusagedetails.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e1227-162">示例</span><span class="sxs-lookup"><span data-stu-id="e1227-162">Examples</span></span>

<span data-ttu-id="e1227-163">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="e1227-163">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="e1227-164">请求</span><span class="sxs-lookup"><span data-stu-id="e1227-164">Request</span></span>

<span data-ttu-id="e1227-165">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e1227-165">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e1227-166">HTTP</span><span class="sxs-lookup"><span data-stu-id="e1227-166">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_usercredentialusagedetails"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/userCredentialUsageDetails
```
# <a name="c"></a>[<span data-ttu-id="e1227-167">C#</span><span class="sxs-lookup"><span data-stu-id="e1227-167">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-usercredentialusagedetails-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e1227-168">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e1227-168">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-usercredentialusagedetails-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e1227-169">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e1227-169">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-usercredentialusagedetails-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e1227-170">Java</span><span class="sxs-lookup"><span data-stu-id="e1227-170">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-usercredentialusagedetails-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e1227-171">响应</span><span class="sxs-lookup"><span data-stu-id="e1227-171">Response</span></span>

<span data-ttu-id="e1227-172">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="e1227-172">The following is an example of the response.</span></span>

> <span data-ttu-id="e1227-173">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="e1227-173">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="e1227-174">从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e1227-174">All the properties are returned from an actual call.</span></span>

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



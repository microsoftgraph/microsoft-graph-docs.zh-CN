---
title: 列出 credentialUserRegistrationDetails
description: 获取给定租户的 credentialUserRegistrationDetails 对象的列表。
localization_priority: Normal
author: davidmu1
ms.prod: reports
doc_type: apiPageType
ms.openlocfilehash: 040c90fb7b2158481379444bbf2699301681e448
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36722641"
---
# <a name="list-credentialuserregistrationdetails"></a><span data-ttu-id="5330f-103">列出 credentialUserRegistrationDetails</span><span class="sxs-lookup"><span data-stu-id="5330f-103">List credentialUserRegistrationDetails</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5330f-104">获取给定租户的[credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="5330f-104">Get a list of [credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md) objects for a given tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="5330f-105">权限</span><span class="sxs-lookup"><span data-stu-id="5330f-105">Permissions</span></span>

<span data-ttu-id="5330f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5330f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5330f-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="5330f-108">Permission type</span></span>                        | <span data-ttu-id="5330f-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5330f-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="5330f-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5330f-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="5330f-111">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="5330f-111">Reports.Read.All</span></span> |
| <span data-ttu-id="5330f-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5330f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5330f-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="5330f-113">Not supported.</span></span> |
| <span data-ttu-id="5330f-114">应用</span><span class="sxs-lookup"><span data-stu-id="5330f-114">Application</span></span>                            | <span data-ttu-id="5330f-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="5330f-115">Reports.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5330f-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5330f-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/credentialUserRegistrationDetails
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5330f-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="5330f-117">Optional query parameters</span></span>

<span data-ttu-id="5330f-118">此函数支持可选的 OData 查询参数 **$filter**。</span><span class="sxs-lookup"><span data-stu-id="5330f-118">This function supports the optional OData query parameter **$filter**.</span></span> <span data-ttu-id="5330f-119">您可以对[credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md)资源的以下一个或多个属性应用 **$filter** 。</span><span class="sxs-lookup"><span data-stu-id="5330f-119">You can apply **$filter** on one or more of the following properties of the [credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md) resource.</span></span>

| <span data-ttu-id="5330f-120">属性</span><span class="sxs-lookup"><span data-stu-id="5330f-120">Properties</span></span> | <span data-ttu-id="5330f-121">说明和示例</span><span class="sxs-lookup"><span data-stu-id="5330f-121">Description and example</span></span> |
| --------- | ----------------------- |
| <span data-ttu-id="5330f-122">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="5330f-122">userDisplayName</span></span> | <span data-ttu-id="5330f-123">按用户名称筛选。</span><span class="sxs-lookup"><span data-stu-id="5330f-123">Filter by user name.</span></span> <span data-ttu-id="5330f-124">例如：`/reports/userCredentialUsageDetails?$filter=userDisplayName eq 'Contoso'`。</span><span class="sxs-lookup"><span data-stu-id="5330f-124">For example: `/reports/userCredentialUsageDetails?$filter=userDisplayName eq 'Contoso'`.</span></span> <span data-ttu-id="5330f-125">支持的筛选器`eq`运算符: `startswith()`和。</span><span class="sxs-lookup"><span data-stu-id="5330f-125">Supported filter operators: `eq`, and `startswith()`.</span></span> <span data-ttu-id="5330f-126">支持不区分大小写。</span><span class="sxs-lookup"><span data-stu-id="5330f-126">Supports case insensitive.</span></span> |
| <span data-ttu-id="5330f-127">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="5330f-127">userPrincipalName</span></span> | <span data-ttu-id="5330f-128">按用户主体名称筛选。</span><span class="sxs-lookup"><span data-stu-id="5330f-128">Filter by user principal name.</span></span> <span data-ttu-id="5330f-129">例如：`/reports/userCredentialUsageDetails?$filter=userPrincipalName eq 'Contoso'`。</span><span class="sxs-lookup"><span data-stu-id="5330f-129">For example: `/reports/userCredentialUsageDetails?$filter=userPrincipalName eq 'Contoso'`.</span></span> <span data-ttu-id="5330f-130">支持的筛选器`eq`运算符`startswith()`: 和。</span><span class="sxs-lookup"><span data-stu-id="5330f-130">Supported filter operators: `eq` and `startswith()`.</span></span> <span data-ttu-id="5330f-131">支持不区分大小写。</span><span class="sxs-lookup"><span data-stu-id="5330f-131">Supports case insensitive.</span></span> |
| <span data-ttu-id="5330f-132">authMethods</span><span class="sxs-lookup"><span data-stu-id="5330f-132">authMethods</span></span> | <span data-ttu-id="5330f-133">按注册过程中使用的身份验证方法进行筛选。</span><span class="sxs-lookup"><span data-stu-id="5330f-133">Filter by the authentication methods used during registration.</span></span> <span data-ttu-id="5330f-134">例如：`/reports/userCredentialUsageDetails?$filter=authMethods/any(t:t eq microsoft.graph.registrationAuthMethod'email')`。</span><span class="sxs-lookup"><span data-stu-id="5330f-134">For example: `/reports/userCredentialUsageDetails?$filter=authMethods/any(t:t eq microsoft.graph.registrationAuthMethod'email')`.</span></span> <span data-ttu-id="5330f-135">支持的筛选器`eq`运算符:。</span><span class="sxs-lookup"><span data-stu-id="5330f-135">Supported filter operators: `eq`.</span></span> |
| <span data-ttu-id="5330f-136">isRegistered</span><span class="sxs-lookup"><span data-stu-id="5330f-136">isRegistered</span></span> | <span data-ttu-id="5330f-137">筛选已注册自助密码重置 (SSPR) 的用户。</span><span class="sxs-lookup"><span data-stu-id="5330f-137">Filter for users who have registered for self-service password reset (SSPR).</span></span> <span data-ttu-id="5330f-138">例如：`/reports/userCredentialUsageDetails?$filter=isRegistered eq true`。</span><span class="sxs-lookup"><span data-stu-id="5330f-138">For example: `/reports/userCredentialUsageDetails?$filter=isRegistered eq true`.</span></span> <span data-ttu-id="5330f-139">支持的筛选器`eq`运算符:。</span><span class="sxs-lookup"><span data-stu-id="5330f-139">Supported filter operators: `eq`.</span></span> |
| <span data-ttu-id="5330f-140">isEnabled</span><span class="sxs-lookup"><span data-stu-id="5330f-140">isEnabled</span></span> | <span data-ttu-id="5330f-141">筛选已启用 SSPR 的用户。</span><span class="sxs-lookup"><span data-stu-id="5330f-141">Filter for users who have been enabled for SSPR.</span></span> <span data-ttu-id="5330f-142">例如：`/reports/userCredentialUsageDetails?$filter=isEnabled eq true`。</span><span class="sxs-lookup"><span data-stu-id="5330f-142">For example: `/reports/userCredentialUsageDetails?$filter=isEnabled eq true`.</span></span> <span data-ttu-id="5330f-143">支持的 filtter 运算符`eq`:。</span><span class="sxs-lookup"><span data-stu-id="5330f-143">Supported filtter operators: `eq`.</span></span> |
| <span data-ttu-id="5330f-144">isCapable</span><span class="sxs-lookup"><span data-stu-id="5330f-144">isCapable</span></span> | <span data-ttu-id="5330f-145">筛选已准备好执行密码重置或多重身份验证 (MFA) 的用户。</span><span class="sxs-lookup"><span data-stu-id="5330f-145">Filter for users who are ready to perform password reset or multi-factor authentication (MFA).</span></span> <span data-ttu-id="5330f-146">例如：`/reports/userCredentialUsageDetails?$filter=isCapable eq true`。</span><span class="sxs-lookup"><span data-stu-id="5330f-146">For example: `/reports/userCredentialUsageDetails?$filter=isCapable eq true`.</span></span> <span data-ttu-id="5330f-147">支持的筛选器运算符:`eq`</span><span class="sxs-lookup"><span data-stu-id="5330f-147">Supported filter operators: `eq`</span></span> |
| <span data-ttu-id="5330f-148">isMfaRegistered</span><span class="sxs-lookup"><span data-stu-id="5330f-148">isMfaRegistered</span></span> | <span data-ttu-id="5330f-149">筛选已注册进行 MFA 的用户。</span><span class="sxs-lookup"><span data-stu-id="5330f-149">Filter for users who are registered for MFA.</span></span> <span data-ttu-id="5330f-150">例如：`/reports/userCredentialUsageDetails?$filter=isMfaRegistered eq true`。</span><span class="sxs-lookup"><span data-stu-id="5330f-150">For example: `/reports/userCredentialUsageDetails?$filter=isMfaRegistered eq true`.</span></span> <span data-ttu-id="5330f-151">支持的筛选器`eq`运算符:。</span><span class="sxs-lookup"><span data-stu-id="5330f-151">Supported filter operators: `eq`.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="5330f-152">请求标头</span><span class="sxs-lookup"><span data-stu-id="5330f-152">Request headers</span></span>

| <span data-ttu-id="5330f-153">名称</span><span class="sxs-lookup"><span data-stu-id="5330f-153">Name</span></span>      |<span data-ttu-id="5330f-154">说明</span><span class="sxs-lookup"><span data-stu-id="5330f-154">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5330f-155">Authorization</span><span class="sxs-lookup"><span data-stu-id="5330f-155">Authorization</span></span> | <span data-ttu-id="5330f-156">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="5330f-156">Bearer {token}</span></span> |
| <span data-ttu-id="5330f-157">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5330f-157">Content-Type</span></span> | <span data-ttu-id="5330f-158">application/json</span><span class="sxs-lookup"><span data-stu-id="5330f-158">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="5330f-159">请求正文</span><span class="sxs-lookup"><span data-stu-id="5330f-159">Request body</span></span>

<span data-ttu-id="5330f-160">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5330f-160">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5330f-161">响应</span><span class="sxs-lookup"><span data-stu-id="5330f-161">Response</span></span>

<span data-ttu-id="5330f-162">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="5330f-162">If successful, this method returns a `200 OK` response code and a collection of [credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5330f-163">示例</span><span class="sxs-lookup"><span data-stu-id="5330f-163">Examples</span></span>

<span data-ttu-id="5330f-164">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="5330f-164">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="5330f-165">请求</span><span class="sxs-lookup"><span data-stu-id="5330f-165">Request</span></span>

<span data-ttu-id="5330f-166">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="5330f-166">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="5330f-167">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="5330f-167">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_credentialuserregistrationdetails"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/credentialUserRegistrationDetails
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="5330f-168">C#</span><span class="sxs-lookup"><span data-stu-id="5330f-168">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-credentialuserregistrationdetails-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5330f-169">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5330f-169">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-credentialuserregistrationdetails-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="5330f-170">目标-C</span><span class="sxs-lookup"><span data-stu-id="5330f-170">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-credentialuserregistrationdetails-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="5330f-171">响应</span><span class="sxs-lookup"><span data-stu-id="5330f-171">Response</span></span>

<span data-ttu-id="5330f-172">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="5330f-172">The following is an example of the response.</span></span>

> <span data-ttu-id="5330f-173">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="5330f-173">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="5330f-174">所有属性都是从实际调用返回的。</span><span class="sxs-lookup"><span data-stu-id="5330f-174">All the properties are returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.credentialUserRegistrationDetails",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/reports/$metadata#Collection(microsoft.graph.credentialUserRegistrationDetails)",
  "value":[
    {
      "id" : "id-value",
      "userPrincipalName":"userPrincipalName",
      "userDisplayName": "userDisplayName-value",
      "authMethods": ["email", "mobileSMS"],
      "isRegistered" : false,
      "isEnabled" : true,
      "isCapable" : false,
      "isMfaRegistered" : true
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List credentialUserRegistrationDetails",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

---
title: 列出 credentialUserRegistrationDetails
description: 获取给定租户的 credentialUserRegistrationDetails 对象的列表。
localization_priority: Normal
author: khotz
ms.prod: reports
doc_type: apiPageType
ms.openlocfilehash: 6010d43b2e8a45f561db983c0cdb2573a667ebf1
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48973544"
---
# <a name="list-credentialuserregistrationdetails"></a><span data-ttu-id="4f853-103">列出 credentialUserRegistrationDetails</span><span class="sxs-lookup"><span data-stu-id="4f853-103">List credentialUserRegistrationDetails</span></span>

<span data-ttu-id="4f853-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4f853-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4f853-105">获取给定租户的 [credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md) 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="4f853-105">Get a list of [credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md) objects for a given tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="4f853-106">权限</span><span class="sxs-lookup"><span data-stu-id="4f853-106">Permissions</span></span>

<span data-ttu-id="4f853-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4f853-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4f853-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="4f853-109">Permission type</span></span>                        | <span data-ttu-id="4f853-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4f853-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="4f853-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4f853-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="4f853-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="4f853-112">Reports.Read.All</span></span> |
| <span data-ttu-id="4f853-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4f853-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4f853-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="4f853-114">Not supported.</span></span> |
| <span data-ttu-id="4f853-115">应用</span><span class="sxs-lookup"><span data-stu-id="4f853-115">Application</span></span>                            | <span data-ttu-id="4f853-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="4f853-116">Reports.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4f853-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4f853-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/credentialUserRegistrationDetails
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4f853-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="4f853-118">Optional query parameters</span></span>

<span data-ttu-id="4f853-119">此函数支持可选的 OData 查询参数 **$filter** 。</span><span class="sxs-lookup"><span data-stu-id="4f853-119">This function supports the optional OData query parameter **$filter**.</span></span> <span data-ttu-id="4f853-120">您可以对 [credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md)资源的以下一个或多个属性应用 **$filter** 。</span><span class="sxs-lookup"><span data-stu-id="4f853-120">You can apply **$filter** on one or more of the following properties of the [credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md) resource.</span></span>

| <span data-ttu-id="4f853-121">属性</span><span class="sxs-lookup"><span data-stu-id="4f853-121">Properties</span></span> | <span data-ttu-id="4f853-122">说明和示例</span><span class="sxs-lookup"><span data-stu-id="4f853-122">Description and example</span></span> |
| --------- | ----------------------- |
| <span data-ttu-id="4f853-123">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="4f853-123">userDisplayName</span></span> | <span data-ttu-id="4f853-124">按用户名称筛选。</span><span class="sxs-lookup"><span data-stu-id="4f853-124">Filter by user name.</span></span> <span data-ttu-id="4f853-125">例如：`/reports/credentialUserRegistrationDetails?$filter=userDisplayName eq 'Contoso'`。</span><span class="sxs-lookup"><span data-stu-id="4f853-125">For example: `/reports/credentialUserRegistrationDetails?$filter=userDisplayName eq 'Contoso'`.</span></span> <span data-ttu-id="4f853-126">支持的筛选器运算符： `eq` 和 `startswith()` 。</span><span class="sxs-lookup"><span data-stu-id="4f853-126">Supported filter operators: `eq`, and `startswith()`.</span></span> <span data-ttu-id="4f853-127">支持不区分大小写。</span><span class="sxs-lookup"><span data-stu-id="4f853-127">Supports case insensitive.</span></span> |
| <span data-ttu-id="4f853-128">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="4f853-128">userPrincipalName</span></span> | <span data-ttu-id="4f853-129">按用户主体名称筛选。</span><span class="sxs-lookup"><span data-stu-id="4f853-129">Filter by user principal name.</span></span> <span data-ttu-id="4f853-130">例如：`/reports/credentialUserRegistrationDetails?$filter=userPrincipalName eq 'Contoso'`。</span><span class="sxs-lookup"><span data-stu-id="4f853-130">For example: `/reports/credentialUserRegistrationDetails?$filter=userPrincipalName eq 'Contoso'`.</span></span> <span data-ttu-id="4f853-131">支持的筛选器运算符： `eq` 和 `startswith()` 。</span><span class="sxs-lookup"><span data-stu-id="4f853-131">Supported filter operators: `eq` and `startswith()`.</span></span> <span data-ttu-id="4f853-132">支持不区分大小写。</span><span class="sxs-lookup"><span data-stu-id="4f853-132">Supports case insensitive.</span></span> |
| <span data-ttu-id="4f853-133">authMethods</span><span class="sxs-lookup"><span data-stu-id="4f853-133">authMethods</span></span> | <span data-ttu-id="4f853-134">按注册过程中使用的身份验证方法进行筛选。</span><span class="sxs-lookup"><span data-stu-id="4f853-134">Filter by the authentication methods used during registration.</span></span> <span data-ttu-id="4f853-135">例如：`/reports/credentialUserRegistrationDetails?$filter=authMethods/any(t:t eq microsoft.graph.registrationAuthMethod'email')`。</span><span class="sxs-lookup"><span data-stu-id="4f853-135">For example: `/reports/credentialUserRegistrationDetails?$filter=authMethods/any(t:t eq microsoft.graph.registrationAuthMethod'email')`.</span></span> <span data-ttu-id="4f853-136">支持的筛选器运算符： `eq` 。</span><span class="sxs-lookup"><span data-stu-id="4f853-136">Supported filter operators: `eq`.</span></span> |
| <span data-ttu-id="4f853-137">isRegistered</span><span class="sxs-lookup"><span data-stu-id="4f853-137">isRegistered</span></span> | <span data-ttu-id="4f853-138">筛选已注册自助密码重置 (SSPR) 的用户。</span><span class="sxs-lookup"><span data-stu-id="4f853-138">Filter for users who have registered for self-service password reset (SSPR).</span></span> <span data-ttu-id="4f853-139">例如：`/reports/credentialUserRegistrationDetails?$filter=isRegistered eq true`。</span><span class="sxs-lookup"><span data-stu-id="4f853-139">For example: `/reports/credentialUserRegistrationDetails?$filter=isRegistered eq true`.</span></span> <span data-ttu-id="4f853-140">支持的筛选器运算符： `eq` 。</span><span class="sxs-lookup"><span data-stu-id="4f853-140">Supported filter operators: `eq`.</span></span> |
| <span data-ttu-id="4f853-141">isEnabled</span><span class="sxs-lookup"><span data-stu-id="4f853-141">isEnabled</span></span> | <span data-ttu-id="4f853-142">筛选已启用 SSPR 的用户。</span><span class="sxs-lookup"><span data-stu-id="4f853-142">Filter for users who have been enabled for SSPR.</span></span> <span data-ttu-id="4f853-143">例如：`/reports/credentialUserRegistrationDetails?$filter=isEnabled eq true`。</span><span class="sxs-lookup"><span data-stu-id="4f853-143">For example: `/reports/credentialUserRegistrationDetails?$filter=isEnabled eq true`.</span></span> <span data-ttu-id="4f853-144">支持的 filtter 运算符： `eq` 。</span><span class="sxs-lookup"><span data-stu-id="4f853-144">Supported filtter operators: `eq`.</span></span> |
| <span data-ttu-id="4f853-145">isCapable</span><span class="sxs-lookup"><span data-stu-id="4f853-145">isCapable</span></span> | <span data-ttu-id="4f853-146">筛选已准备好执行密码重置或多重身份验证 (MFA) 的用户。</span><span class="sxs-lookup"><span data-stu-id="4f853-146">Filter for users who are ready to perform password reset or multi-factor authentication (MFA).</span></span> <span data-ttu-id="4f853-147">例如：`/reports/credentialUserRegistrationDetails?$filter=isCapable eq true`。</span><span class="sxs-lookup"><span data-stu-id="4f853-147">For example: `/reports/credentialUserRegistrationDetails?$filter=isCapable eq true`.</span></span> <span data-ttu-id="4f853-148">支持的筛选器运算符： `eq`</span><span class="sxs-lookup"><span data-stu-id="4f853-148">Supported filter operators: `eq`</span></span> |
| <span data-ttu-id="4f853-149">isMfaRegistered</span><span class="sxs-lookup"><span data-stu-id="4f853-149">isMfaRegistered</span></span> | <span data-ttu-id="4f853-150">筛选已注册进行 MFA 的用户。</span><span class="sxs-lookup"><span data-stu-id="4f853-150">Filter for users who are registered for MFA.</span></span> <span data-ttu-id="4f853-151">例如：`/reports/credentialUserRegistrationDetails?$filter=isMfaRegistered eq true`。</span><span class="sxs-lookup"><span data-stu-id="4f853-151">For example: `/reports/credentialUserRegistrationDetails?$filter=isMfaRegistered eq true`.</span></span> <span data-ttu-id="4f853-152">支持的筛选器运算符： `eq` 。</span><span class="sxs-lookup"><span data-stu-id="4f853-152">Supported filter operators: `eq`.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="4f853-153">请求标头</span><span class="sxs-lookup"><span data-stu-id="4f853-153">Request headers</span></span>

| <span data-ttu-id="4f853-154">名称</span><span class="sxs-lookup"><span data-stu-id="4f853-154">Name</span></span>      |<span data-ttu-id="4f853-155">说明</span><span class="sxs-lookup"><span data-stu-id="4f853-155">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="4f853-156">Authorization</span><span class="sxs-lookup"><span data-stu-id="4f853-156">Authorization</span></span> | <span data-ttu-id="4f853-157">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="4f853-157">Bearer {token}</span></span> |
| <span data-ttu-id="4f853-158">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4f853-158">Content-Type</span></span> | <span data-ttu-id="4f853-159">application/json</span><span class="sxs-lookup"><span data-stu-id="4f853-159">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="4f853-160">请求正文</span><span class="sxs-lookup"><span data-stu-id="4f853-160">Request body</span></span>

<span data-ttu-id="4f853-161">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4f853-161">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4f853-162">响应</span><span class="sxs-lookup"><span data-stu-id="4f853-162">Response</span></span>

<span data-ttu-id="4f853-163">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="4f853-163">If successful, this method returns a `200 OK` response code and a collection of [credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4f853-164">示例</span><span class="sxs-lookup"><span data-stu-id="4f853-164">Examples</span></span>

<span data-ttu-id="4f853-165">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="4f853-165">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="4f853-166">请求</span><span class="sxs-lookup"><span data-stu-id="4f853-166">Request</span></span>

<span data-ttu-id="4f853-167">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="4f853-167">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4f853-168">HTTP</span><span class="sxs-lookup"><span data-stu-id="4f853-168">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_credentialuserregistrationdetails"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/credentialUserRegistrationDetails
```
# <a name="c"></a>[<span data-ttu-id="4f853-169">C#</span><span class="sxs-lookup"><span data-stu-id="4f853-169">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-credentialuserregistrationdetails-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4f853-170">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4f853-170">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-credentialuserregistrationdetails-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4f853-171">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4f853-171">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-credentialuserregistrationdetails-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4f853-172">Java</span><span class="sxs-lookup"><span data-stu-id="4f853-172">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-credentialuserregistrationdetails-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4f853-173">响应</span><span class="sxs-lookup"><span data-stu-id="4f853-173">Response</span></span>

<span data-ttu-id="4f853-174">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="4f853-174">The following is an example of the response.</span></span>

> <span data-ttu-id="4f853-175">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="4f853-175">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="4f853-176">所有属性都是从实际调用返回的。</span><span class="sxs-lookup"><span data-stu-id="4f853-176">All the properties are returned from an actual call.</span></span>

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



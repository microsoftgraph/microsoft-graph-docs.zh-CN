---
title: 列出 credentialUserRegistrationDetails
description: 获取给定租户的 credentialUserRegistrationDetails 对象列表。
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
doc_type: apiPageType
ms.openlocfilehash: bf6e99722c44ff0054869056be09314d6befac59
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50136666"
---
# <a name="list-credentialuserregistrationdetails"></a><span data-ttu-id="99506-103">列出 credentialUserRegistrationDetails</span><span class="sxs-lookup"><span data-stu-id="99506-103">List credentialUserRegistrationDetails</span></span>

<span data-ttu-id="99506-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="99506-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="99506-105">获取给定租户 [的 credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md) 对象列表。</span><span class="sxs-lookup"><span data-stu-id="99506-105">Get a list of [credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md) objects for a given tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="99506-106">权限</span><span class="sxs-lookup"><span data-stu-id="99506-106">Permissions</span></span>

<span data-ttu-id="99506-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="99506-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="99506-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="99506-109">Permission type</span></span>                        | <span data-ttu-id="99506-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="99506-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="99506-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="99506-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="99506-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="99506-112">Reports.Read.All</span></span> |
| <span data-ttu-id="99506-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="99506-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="99506-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="99506-114">Not supported.</span></span> |
| <span data-ttu-id="99506-115">应用</span><span class="sxs-lookup"><span data-stu-id="99506-115">Application</span></span>                            | <span data-ttu-id="99506-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="99506-116">Reports.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="99506-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="99506-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/credentialUserRegistrationDetails
```

## <a name="optional-query-parameters"></a><span data-ttu-id="99506-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="99506-118">Optional query parameters</span></span>

<span data-ttu-id="99506-119">此函数支持可选的 OData 查询 **参数**$filter。</span><span class="sxs-lookup"><span data-stu-id="99506-119">This function supports the optional OData query parameter **$filter**.</span></span> <span data-ttu-id="99506-120">可以将 **$filter凭据**[UserRegistrationDetails](../resources/credentialuserregistrationdetails.md)资源的以下一个或多个属性应用。</span><span class="sxs-lookup"><span data-stu-id="99506-120">You can apply **$filter** on one or more of the following properties of the [credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md) resource.</span></span>

| <span data-ttu-id="99506-121">属性</span><span class="sxs-lookup"><span data-stu-id="99506-121">Properties</span></span> | <span data-ttu-id="99506-122">说明和示例</span><span class="sxs-lookup"><span data-stu-id="99506-122">Description and example</span></span> |
| --------- | ----------------------- |
| <span data-ttu-id="99506-123">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="99506-123">userDisplayName</span></span> | <span data-ttu-id="99506-124">按用户名筛选。</span><span class="sxs-lookup"><span data-stu-id="99506-124">Filter by user name.</span></span> <span data-ttu-id="99506-125">例如：`/reports/credentialUserRegistrationDetails?$filter=userDisplayName eq 'Contoso'`。</span><span class="sxs-lookup"><span data-stu-id="99506-125">For example: `/reports/credentialUserRegistrationDetails?$filter=userDisplayName eq 'Contoso'`.</span></span> <span data-ttu-id="99506-126">支持的筛选器运算符： `eq` 和 `startswith()` 。</span><span class="sxs-lookup"><span data-stu-id="99506-126">Supported filter operators: `eq`, and `startswith()`.</span></span> <span data-ttu-id="99506-127">支持不区分大小写。</span><span class="sxs-lookup"><span data-stu-id="99506-127">Supports case insensitive.</span></span> |
| <span data-ttu-id="99506-128">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="99506-128">userPrincipalName</span></span> | <span data-ttu-id="99506-129">按用户主体名称进行筛选。</span><span class="sxs-lookup"><span data-stu-id="99506-129">Filter by user principal name.</span></span> <span data-ttu-id="99506-130">例如：`/reports/credentialUserRegistrationDetails?$filter=userPrincipalName eq 'Contoso'`。</span><span class="sxs-lookup"><span data-stu-id="99506-130">For example: `/reports/credentialUserRegistrationDetails?$filter=userPrincipalName eq 'Contoso'`.</span></span> <span data-ttu-id="99506-131">支持的筛选器运算符： `eq` 和 `startswith()` 。</span><span class="sxs-lookup"><span data-stu-id="99506-131">Supported filter operators: `eq` and `startswith()`.</span></span> <span data-ttu-id="99506-132">支持不区分大小写。</span><span class="sxs-lookup"><span data-stu-id="99506-132">Supports case insensitive.</span></span> |
| <span data-ttu-id="99506-133">authMethods</span><span class="sxs-lookup"><span data-stu-id="99506-133">authMethods</span></span> | <span data-ttu-id="99506-134">按注册期间使用的身份验证方法进行筛选。</span><span class="sxs-lookup"><span data-stu-id="99506-134">Filter by the authentication methods used during registration.</span></span> <span data-ttu-id="99506-135">例如：`/reports/credentialUserRegistrationDetails?$filter=authMethods/any(t:t eq microsoft.graph.registrationAuthMethod'email')`。</span><span class="sxs-lookup"><span data-stu-id="99506-135">For example: `/reports/credentialUserRegistrationDetails?$filter=authMethods/any(t:t eq microsoft.graph.registrationAuthMethod'email')`.</span></span> <span data-ttu-id="99506-136">支持的筛选器运算符： `eq` .</span><span class="sxs-lookup"><span data-stu-id="99506-136">Supported filter operators: `eq`.</span></span> |
| <span data-ttu-id="99506-137">isRegistered</span><span class="sxs-lookup"><span data-stu-id="99506-137">isRegistered</span></span> | <span data-ttu-id="99506-138">筛选已注册 SSPR 服务中的自助服务密码重置 (用户) 。</span><span class="sxs-lookup"><span data-stu-id="99506-138">Filter for users who have registered for self-service password reset (SSPR).</span></span> <span data-ttu-id="99506-139">例如：`/reports/credentialUserRegistrationDetails?$filter=isRegistered eq true`。</span><span class="sxs-lookup"><span data-stu-id="99506-139">For example: `/reports/credentialUserRegistrationDetails?$filter=isRegistered eq true`.</span></span> <span data-ttu-id="99506-140">支持的筛选器运算符： `eq` .</span><span class="sxs-lookup"><span data-stu-id="99506-140">Supported filter operators: `eq`.</span></span> |
| <span data-ttu-id="99506-141">isEnabled</span><span class="sxs-lookup"><span data-stu-id="99506-141">isEnabled</span></span> | <span data-ttu-id="99506-142">筛选已启用 SSPR 的用户。</span><span class="sxs-lookup"><span data-stu-id="99506-142">Filter for users who have been enabled for SSPR.</span></span> <span data-ttu-id="99506-143">例如：`/reports/credentialUserRegistrationDetails?$filter=isEnabled eq true`。</span><span class="sxs-lookup"><span data-stu-id="99506-143">For example: `/reports/credentialUserRegistrationDetails?$filter=isEnabled eq true`.</span></span> <span data-ttu-id="99506-144">支持的筛选运算符： `eq` .</span><span class="sxs-lookup"><span data-stu-id="99506-144">Supported filtter operators: `eq`.</span></span> |
| <span data-ttu-id="99506-145">isCapable</span><span class="sxs-lookup"><span data-stu-id="99506-145">isCapable</span></span> | <span data-ttu-id="99506-146">筛选准备在 MFA 服务中执行密码重置或多重 (的用户) 。</span><span class="sxs-lookup"><span data-stu-id="99506-146">Filter for users who are ready to perform password reset or multi-factor authentication (MFA).</span></span> <span data-ttu-id="99506-147">例如：`/reports/credentialUserRegistrationDetails?$filter=isCapable eq true`。</span><span class="sxs-lookup"><span data-stu-id="99506-147">For example: `/reports/credentialUserRegistrationDetails?$filter=isCapable eq true`.</span></span> <span data-ttu-id="99506-148">支持的筛选器运算符： `eq`</span><span class="sxs-lookup"><span data-stu-id="99506-148">Supported filter operators: `eq`</span></span> |
| <span data-ttu-id="99506-149">isMfaRegistered</span><span class="sxs-lookup"><span data-stu-id="99506-149">isMfaRegistered</span></span> | <span data-ttu-id="99506-150">筛选为 MFA 注册的用户。</span><span class="sxs-lookup"><span data-stu-id="99506-150">Filter for users who are registered for MFA.</span></span> <span data-ttu-id="99506-151">例如：`/reports/credentialUserRegistrationDetails?$filter=isMfaRegistered eq true`。</span><span class="sxs-lookup"><span data-stu-id="99506-151">For example: `/reports/credentialUserRegistrationDetails?$filter=isMfaRegistered eq true`.</span></span> <span data-ttu-id="99506-152">支持的筛选器运算符： `eq` .</span><span class="sxs-lookup"><span data-stu-id="99506-152">Supported filter operators: `eq`.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="99506-153">请求标头</span><span class="sxs-lookup"><span data-stu-id="99506-153">Request headers</span></span>

| <span data-ttu-id="99506-154">名称</span><span class="sxs-lookup"><span data-stu-id="99506-154">Name</span></span>      |<span data-ttu-id="99506-155">说明</span><span class="sxs-lookup"><span data-stu-id="99506-155">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="99506-156">Authorization</span><span class="sxs-lookup"><span data-stu-id="99506-156">Authorization</span></span> | <span data-ttu-id="99506-157">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="99506-157">Bearer {token}</span></span> |
| <span data-ttu-id="99506-158">Content-Type</span><span class="sxs-lookup"><span data-stu-id="99506-158">Content-Type</span></span> | <span data-ttu-id="99506-159">application/json</span><span class="sxs-lookup"><span data-stu-id="99506-159">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="99506-160">请求正文</span><span class="sxs-lookup"><span data-stu-id="99506-160">Request body</span></span>

<span data-ttu-id="99506-161">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="99506-161">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="99506-162">响应</span><span class="sxs-lookup"><span data-stu-id="99506-162">Response</span></span>

<span data-ttu-id="99506-163">如果成功，此方法在响应正文中返回响应代码 `200 OK` 和 [credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="99506-163">If successful, this method returns a `200 OK` response code and a collection of [credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="99506-164">示例</span><span class="sxs-lookup"><span data-stu-id="99506-164">Examples</span></span>

<span data-ttu-id="99506-165">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="99506-165">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="99506-166">请求</span><span class="sxs-lookup"><span data-stu-id="99506-166">Request</span></span>

<span data-ttu-id="99506-167">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="99506-167">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="99506-168">HTTP</span><span class="sxs-lookup"><span data-stu-id="99506-168">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_credentialuserregistrationdetails"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/credentialUserRegistrationDetails
```
# <a name="c"></a>[<span data-ttu-id="99506-169">C#</span><span class="sxs-lookup"><span data-stu-id="99506-169">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-credentialuserregistrationdetails-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="99506-170">JavaScript</span><span class="sxs-lookup"><span data-stu-id="99506-170">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-credentialuserregistrationdetails-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="99506-171">Objective-C</span><span class="sxs-lookup"><span data-stu-id="99506-171">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-credentialuserregistrationdetails-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="99506-172">Java</span><span class="sxs-lookup"><span data-stu-id="99506-172">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-credentialuserregistrationdetails-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="99506-173">响应</span><span class="sxs-lookup"><span data-stu-id="99506-173">Response</span></span>

<span data-ttu-id="99506-174">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="99506-174">The following is an example of the response.</span></span>

> <span data-ttu-id="99506-175">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="99506-175">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="99506-176">从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="99506-176">All the properties are returned from an actual call.</span></span>

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



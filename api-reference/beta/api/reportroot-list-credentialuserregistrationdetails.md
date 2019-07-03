---
title: 列出 credentialUserRegistrationDetails
description: 获取给定租户的 credentialUserRegistrationDetails 对象的列表。
localization_priority: Normal
author: davidmu1
ms.prod: reports
doc_type: apiPageType
ms.openlocfilehash: bf008013802f8dfe781bca998e38e03e3791317c
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35500649"
---
# <a name="list-credentialuserregistrationdetails"></a><span data-ttu-id="7b44e-103">列出 credentialUserRegistrationDetails</span><span class="sxs-lookup"><span data-stu-id="7b44e-103">List credentialUserRegistrationDetails</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7b44e-104">获取给定租户的[credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="7b44e-104">Get a list of [credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md) objects for a given tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="7b44e-105">权限</span><span class="sxs-lookup"><span data-stu-id="7b44e-105">Permissions</span></span>

<span data-ttu-id="7b44e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7b44e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7b44e-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="7b44e-108">Permission type</span></span>                        | <span data-ttu-id="7b44e-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7b44e-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="7b44e-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7b44e-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="7b44e-111">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="7b44e-111">Reports.Read.All</span></span> |
| <span data-ttu-id="7b44e-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7b44e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7b44e-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="7b44e-113">Not supported.</span></span> |
| <span data-ttu-id="7b44e-114">应用</span><span class="sxs-lookup"><span data-stu-id="7b44e-114">Application</span></span>                            | <span data-ttu-id="7b44e-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="7b44e-115">Reports.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7b44e-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7b44e-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/credentialUserRegistrationDetails
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7b44e-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="7b44e-117">Optional query parameters</span></span>

<span data-ttu-id="7b44e-118">此函数支持可选的 OData 查询参数 **$filter**。</span><span class="sxs-lookup"><span data-stu-id="7b44e-118">This function supports the optional OData query parameter **$filter**.</span></span> <span data-ttu-id="7b44e-119">您可以对[credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md)资源的以下一个或多个属性应用 **$filter** 。</span><span class="sxs-lookup"><span data-stu-id="7b44e-119">You can apply **$filter** on one or more of the following properties of the [credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md) resource.</span></span>

| <span data-ttu-id="7b44e-120">属性</span><span class="sxs-lookup"><span data-stu-id="7b44e-120">Properties</span></span> | <span data-ttu-id="7b44e-121">说明和示例</span><span class="sxs-lookup"><span data-stu-id="7b44e-121">Description and example</span></span> |
| --------- | ----------------------- |
| <span data-ttu-id="7b44e-122">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="7b44e-122">userDisplayName</span></span> | <span data-ttu-id="7b44e-123">按用户名称筛选。</span><span class="sxs-lookup"><span data-stu-id="7b44e-123">Filter by user name.</span></span> <span data-ttu-id="7b44e-124">例如：`/reports/userCredentialUsageDetails?$filter=userDisplayName eq 'Contoso'`。</span><span class="sxs-lookup"><span data-stu-id="7b44e-124">For example: `/reports/userCredentialUsageDetails?$filter=userDisplayName eq 'Contoso'`.</span></span> <span data-ttu-id="7b44e-125">支持的筛选器`eq`运算符: `startswith()`和。</span><span class="sxs-lookup"><span data-stu-id="7b44e-125">Supported filter operators: `eq`, and `startswith()`.</span></span> <span data-ttu-id="7b44e-126">支持不区分大小写。</span><span class="sxs-lookup"><span data-stu-id="7b44e-126">Supports case insensitive.</span></span> |
| <span data-ttu-id="7b44e-127">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="7b44e-127">userPrincipalName</span></span> | <span data-ttu-id="7b44e-128">按用户主体名称筛选。</span><span class="sxs-lookup"><span data-stu-id="7b44e-128">Filter by user principal name.</span></span> <span data-ttu-id="7b44e-129">例如：`/reports/userCredentialUsageDetails?$filter=userPrincipalName eq 'Contoso'`。</span><span class="sxs-lookup"><span data-stu-id="7b44e-129">For example: `/reports/userCredentialUsageDetails?$filter=userPrincipalName eq 'Contoso'`.</span></span> <span data-ttu-id="7b44e-130">支持的筛选器`eq`运算符`startswith()`: 和。</span><span class="sxs-lookup"><span data-stu-id="7b44e-130">Supported filter operators: `eq` and `startswith()`.</span></span> <span data-ttu-id="7b44e-131">支持不区分大小写。</span><span class="sxs-lookup"><span data-stu-id="7b44e-131">Supports case insensitive.</span></span> |
| <span data-ttu-id="7b44e-132">authMethods</span><span class="sxs-lookup"><span data-stu-id="7b44e-132">authMethods</span></span> | <span data-ttu-id="7b44e-133">按注册过程中使用的身份验证方法进行筛选。</span><span class="sxs-lookup"><span data-stu-id="7b44e-133">Filter by the authentication methods used during registration.</span></span> <span data-ttu-id="7b44e-134">例如：`/reports/userCredentialUsageDetails?$filter=authMethods/any(t:t eq microsoft.graph.registrationAuthMethod'email')`。</span><span class="sxs-lookup"><span data-stu-id="7b44e-134">For example: `/reports/userCredentialUsageDetails?$filter=authMethods/any(t:t eq microsoft.graph.registrationAuthMethod'email')`.</span></span> <span data-ttu-id="7b44e-135">支持的筛选器`eq`运算符:。</span><span class="sxs-lookup"><span data-stu-id="7b44e-135">Supported filter operators: `eq`.</span></span> |
| <span data-ttu-id="7b44e-136">isRegistered</span><span class="sxs-lookup"><span data-stu-id="7b44e-136">isRegistered</span></span> | <span data-ttu-id="7b44e-137">筛选已注册自助密码重置 (SSPR) 的用户。</span><span class="sxs-lookup"><span data-stu-id="7b44e-137">Filter for users who have registered for self-service password reset (SSPR).</span></span> <span data-ttu-id="7b44e-138">例如：`/reports/userCredentialUsageDetails?$filter=isRegistered eq true`。</span><span class="sxs-lookup"><span data-stu-id="7b44e-138">For example: `/reports/userCredentialUsageDetails?$filter=isRegistered eq true`.</span></span> <span data-ttu-id="7b44e-139">支持的筛选器`eq`运算符:。</span><span class="sxs-lookup"><span data-stu-id="7b44e-139">Supported filter operators: `eq`.</span></span> |
| <span data-ttu-id="7b44e-140">isEnabled</span><span class="sxs-lookup"><span data-stu-id="7b44e-140">isEnabled</span></span> | <span data-ttu-id="7b44e-141">筛选已启用 SSPR 的用户。</span><span class="sxs-lookup"><span data-stu-id="7b44e-141">Filter for users who have been enabled for SSPR.</span></span> <span data-ttu-id="7b44e-142">例如：`/reports/userCredentialUsageDetails?$filter=isEnabled eq true`。</span><span class="sxs-lookup"><span data-stu-id="7b44e-142">For example: `/reports/userCredentialUsageDetails?$filter=isEnabled eq true`.</span></span> <span data-ttu-id="7b44e-143">支持的 filtter 运算符`eq`:。</span><span class="sxs-lookup"><span data-stu-id="7b44e-143">Supported filtter operators: `eq`.</span></span> |
| <span data-ttu-id="7b44e-144">isCapable</span><span class="sxs-lookup"><span data-stu-id="7b44e-144">isCapable</span></span> | <span data-ttu-id="7b44e-145">筛选已准备好执行密码重置或多重身份验证 (MFA) 的用户。</span><span class="sxs-lookup"><span data-stu-id="7b44e-145">Filter for users who are ready to perform password reset or multi-factor authentication (MFA).</span></span> <span data-ttu-id="7b44e-146">例如：`/reports/userCredentialUsageDetails?$filter=isCapable eq true`。</span><span class="sxs-lookup"><span data-stu-id="7b44e-146">For example: `/reports/userCredentialUsageDetails?$filter=isCapable eq true`.</span></span> <span data-ttu-id="7b44e-147">支持的筛选器运算符:`eq`</span><span class="sxs-lookup"><span data-stu-id="7b44e-147">Supported filter operators: `eq`</span></span> |
| <span data-ttu-id="7b44e-148">isMfaRegistered</span><span class="sxs-lookup"><span data-stu-id="7b44e-148">isMfaRegistered</span></span> | <span data-ttu-id="7b44e-149">筛选已注册进行 MFA 的用户。</span><span class="sxs-lookup"><span data-stu-id="7b44e-149">Filter for users who are registered for MFA.</span></span> <span data-ttu-id="7b44e-150">例如：`/reports/userCredentialUsageDetails?$filter=isMfaRegistered eq true`。</span><span class="sxs-lookup"><span data-stu-id="7b44e-150">For example: `/reports/userCredentialUsageDetails?$filter=isMfaRegistered eq true`.</span></span> <span data-ttu-id="7b44e-151">支持的筛选器`eq`运算符:。</span><span class="sxs-lookup"><span data-stu-id="7b44e-151">Supported filter operators: `eq`.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="7b44e-152">请求标头</span><span class="sxs-lookup"><span data-stu-id="7b44e-152">Request headers</span></span>

| <span data-ttu-id="7b44e-153">名称</span><span class="sxs-lookup"><span data-stu-id="7b44e-153">Name</span></span>      |<span data-ttu-id="7b44e-154">说明</span><span class="sxs-lookup"><span data-stu-id="7b44e-154">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7b44e-155">Authorization</span><span class="sxs-lookup"><span data-stu-id="7b44e-155">Authorization</span></span> | <span data-ttu-id="7b44e-156">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="7b44e-156">Bearer {token}</span></span> |
| <span data-ttu-id="7b44e-157">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7b44e-157">Content-Type</span></span> | <span data-ttu-id="7b44e-158">application/json</span><span class="sxs-lookup"><span data-stu-id="7b44e-158">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="7b44e-159">请求正文</span><span class="sxs-lookup"><span data-stu-id="7b44e-159">Request body</span></span>

<span data-ttu-id="7b44e-160">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7b44e-160">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7b44e-161">响应</span><span class="sxs-lookup"><span data-stu-id="7b44e-161">Response</span></span>

<span data-ttu-id="7b44e-162">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="7b44e-162">If successful, this method returns a `200 OK` response code and a collection of [credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7b44e-163">示例</span><span class="sxs-lookup"><span data-stu-id="7b44e-163">Examples</span></span>

<span data-ttu-id="7b44e-164">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="7b44e-164">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="7b44e-165">请求</span><span class="sxs-lookup"><span data-stu-id="7b44e-165">Request</span></span>

<span data-ttu-id="7b44e-166">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="7b44e-166">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_credentialuserregistrationdetails"
}-->

```http
GET https://graph.microsoft.com/beta/reports/credentialUserRegistrationDetails
```

### <a name="response"></a><span data-ttu-id="7b44e-167">响应</span><span class="sxs-lookup"><span data-stu-id="7b44e-167">Response</span></span>

<span data-ttu-id="7b44e-168">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="7b44e-168">The following is an example of the response.</span></span>

> <span data-ttu-id="7b44e-169">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="7b44e-169">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="7b44e-170">所有属性都是从实际调用返回的。</span><span class="sxs-lookup"><span data-stu-id="7b44e-170">All the properties are returned from an actual call.</span></span>

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
---
title: 创建 identityProvider
description: 创建新的 Identityprovider.read.all 对象。
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: microsoft-identity-platform
ms.openlocfilehash: d5d6eb847179a062bda1c0013bafb73de38ab455
ms.sourcegitcommit: 9faca60f0cc4ee9d6dce33fd25c72e14b5487d34
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/29/2020
ms.locfileid: "46509705"
---
# <a name="create-identityprovider"></a><span data-ttu-id="ba1c2-103">创建 identityProvider</span><span class="sxs-lookup"><span data-stu-id="ba1c2-103">Create identityProvider</span></span>

<span data-ttu-id="ba1c2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ba1c2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ba1c2-105">创建新的[identityprovider.read.all](../resources/identityprovider.md)对象。</span><span class="sxs-lookup"><span data-stu-id="ba1c2-105">Create a new [identityProvider](../resources/identityprovider.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ba1c2-106">权限</span><span class="sxs-lookup"><span data-stu-id="ba1c2-106">Permissions</span></span>

<span data-ttu-id="ba1c2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ba1c2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ba1c2-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="ba1c2-109">Permission type</span></span>      | <span data-ttu-id="ba1c2-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ba1c2-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ba1c2-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ba1c2-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ba1c2-112">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba1c2-112">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="ba1c2-113">委派（Microsoft 个人帐户）</span><span class="sxs-lookup"><span data-stu-id="ba1c2-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="ba1c2-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="ba1c2-114">Not supported.</span></span>|
|<span data-ttu-id="ba1c2-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="ba1c2-115">Application</span></span>|<span data-ttu-id="ba1c2-116">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba1c2-116">IdentityProvider.ReadWrite.All</span></span>|

<span data-ttu-id="ba1c2-117">工作或学校帐户需要属于下列角色之一：</span><span class="sxs-lookup"><span data-stu-id="ba1c2-117">The work or school account needs to belong to one of the following roles:</span></span>
* <span data-ttu-id="ba1c2-118">全局管理员</span><span class="sxs-lookup"><span data-stu-id="ba1c2-118">Global administrator</span></span>
* <span data-ttu-id="ba1c2-119">外部标识提供程序管理员</span><span class="sxs-lookup"><span data-stu-id="ba1c2-119">External Identity Provider administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="ba1c2-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ba1c2-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identityProviders
```

## <a name="request-headers"></a><span data-ttu-id="ba1c2-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="ba1c2-121">Request headers</span></span>

|<span data-ttu-id="ba1c2-122">名称</span><span class="sxs-lookup"><span data-stu-id="ba1c2-122">Name</span></span>|<span data-ttu-id="ba1c2-123">说明</span><span class="sxs-lookup"><span data-stu-id="ba1c2-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="ba1c2-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="ba1c2-124">Authorization</span></span>|<span data-ttu-id="ba1c2-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ba1c2-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="ba1c2-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ba1c2-127">Content-Type</span></span>|<span data-ttu-id="ba1c2-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="ba1c2-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ba1c2-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="ba1c2-130">Request body</span></span>

<span data-ttu-id="ba1c2-131">在请求正文中，提供[identityprovider.read.all](../resources/identityprovider.md)或[openIdConnectProvider](../resources/openidconnectprovider.md) （仅适用于 Azure AD B2C）对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ba1c2-131">In the request body, provide a JSON representation of [identityProvider](../resources/identityprovider.md) or [openIdConnectProvider](../resources/openidconnectprovider.md) (only for Azure AD B2C) object.</span></span> <span data-ttu-id="ba1c2-132">下表中列出的所有属性均未必需属性。</span><span class="sxs-lookup"><span data-stu-id="ba1c2-132">All the properties listed in the following table are required.</span></span>

### <a name="identityprovider-object"></a><span data-ttu-id="ba1c2-133">Identityprovider.read.all 对象</span><span class="sxs-lookup"><span data-stu-id="ba1c2-133">identityProvider object</span></span>

|<span data-ttu-id="ba1c2-134">属性</span><span class="sxs-lookup"><span data-stu-id="ba1c2-134">Property</span></span>|<span data-ttu-id="ba1c2-135">类型</span><span class="sxs-lookup"><span data-stu-id="ba1c2-135">Type</span></span>|<span data-ttu-id="ba1c2-136">说明</span><span class="sxs-lookup"><span data-stu-id="ba1c2-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ba1c2-137">clientId</span><span class="sxs-lookup"><span data-stu-id="ba1c2-137">clientId</span></span>|<span data-ttu-id="ba1c2-138">字符串</span><span class="sxs-lookup"><span data-stu-id="ba1c2-138">String</span></span>|<span data-ttu-id="ba1c2-139">应用程序的客户端 ID。</span><span class="sxs-lookup"><span data-stu-id="ba1c2-139">The client ID for the application.</span></span> <span data-ttu-id="ba1c2-140">这是向标识提供程序注册应用程序时获取的客户端 ID。</span><span class="sxs-lookup"><span data-stu-id="ba1c2-140">This is the client ID obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="ba1c2-141">clientSecret</span><span class="sxs-lookup"><span data-stu-id="ba1c2-141">clientSecret</span></span>|<span data-ttu-id="ba1c2-142">字符串</span><span class="sxs-lookup"><span data-stu-id="ba1c2-142">String</span></span>|<span data-ttu-id="ba1c2-143">应用程序的客户端密码。</span><span class="sxs-lookup"><span data-stu-id="ba1c2-143">The client secret for the application.</span></span> <span data-ttu-id="ba1c2-144">这是向标识提供程序注册应用程序时获取的客户端密码。</span><span class="sxs-lookup"><span data-stu-id="ba1c2-144">This is the client secret obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="ba1c2-145">name</span><span class="sxs-lookup"><span data-stu-id="ba1c2-145">name</span></span>|<span data-ttu-id="ba1c2-146">字符串</span><span class="sxs-lookup"><span data-stu-id="ba1c2-146">String</span></span>|<span data-ttu-id="ba1c2-147">标识提供程序的显示名称。</span><span class="sxs-lookup"><span data-stu-id="ba1c2-147">The display name of the identity provider.</span></span>|
|<span data-ttu-id="ba1c2-148">type</span><span class="sxs-lookup"><span data-stu-id="ba1c2-148">type</span></span>|<span data-ttu-id="ba1c2-149">字符串</span><span class="sxs-lookup"><span data-stu-id="ba1c2-149">String</span></span>|<span data-ttu-id="ba1c2-150">标识提供程序类型。</span><span class="sxs-lookup"><span data-stu-id="ba1c2-150">The identity provider type.</span></span> <ul><span data-ttu-id="ba1c2-151">对于 B2B 方案：</span><span class="sxs-lookup"><span data-stu-id="ba1c2-151">For B2B scenario:</span></span><li/><span data-ttu-id="ba1c2-152">Google</span><span class="sxs-lookup"><span data-stu-id="ba1c2-152">Google</span></span><li/><span data-ttu-id="ba1c2-153">Facebook</span><span class="sxs-lookup"><span data-stu-id="ba1c2-153">Facebook</span></span></ul><ul><span data-ttu-id="ba1c2-154">对于 B2C 方案：</span><span class="sxs-lookup"><span data-stu-id="ba1c2-154">For B2C scenario:</span></span><li/><span data-ttu-id="ba1c2-155">Microsoft</span><span class="sxs-lookup"><span data-stu-id="ba1c2-155">Microsoft</span></span><li/><span data-ttu-id="ba1c2-156">Google</span><span class="sxs-lookup"><span data-stu-id="ba1c2-156">Google</span></span><li/><span data-ttu-id="ba1c2-157">Amazon</span><span class="sxs-lookup"><span data-stu-id="ba1c2-157">Amazon</span></span><li/><span data-ttu-id="ba1c2-158">领英</span><span class="sxs-lookup"><span data-stu-id="ba1c2-158">LinkedIn</span></span><li/><span data-ttu-id="ba1c2-159">Facebook</span><span class="sxs-lookup"><span data-stu-id="ba1c2-159">Facebook</span></span><li/><span data-ttu-id="ba1c2-160">GitHub</span><span class="sxs-lookup"><span data-stu-id="ba1c2-160">GitHub</span></span><li/><span data-ttu-id="ba1c2-161">Twitter</span><span class="sxs-lookup"><span data-stu-id="ba1c2-161">Twitter</span></span><li/><span data-ttu-id="ba1c2-162">微博</span><span class="sxs-lookup"><span data-stu-id="ba1c2-162">Weibo</span></span><li/><span data-ttu-id="ba1c2-163">QQ</span><span class="sxs-lookup"><span data-stu-id="ba1c2-163">QQ</span></span><li/><span data-ttu-id="ba1c2-164">微信</span><span class="sxs-lookup"><span data-stu-id="ba1c2-164">WeChat</span></span><li/><span data-ttu-id="ba1c2-165">OpenIDConnect</span><span class="sxs-lookup"><span data-stu-id="ba1c2-165">OpenIDConnect</span></span></ul>|

### <a name="openidconnectprovider-object"></a><span data-ttu-id="ba1c2-166">openIdConnectProvider 对象</span><span class="sxs-lookup"><span data-stu-id="ba1c2-166">openIdConnectProvider object</span></span>

|<span data-ttu-id="ba1c2-167">属性</span><span class="sxs-lookup"><span data-stu-id="ba1c2-167">Property</span></span>|<span data-ttu-id="ba1c2-168">类型</span><span class="sxs-lookup"><span data-stu-id="ba1c2-168">Type</span></span>|<span data-ttu-id="ba1c2-169">说明</span><span class="sxs-lookup"><span data-stu-id="ba1c2-169">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ba1c2-170">clientId</span><span class="sxs-lookup"><span data-stu-id="ba1c2-170">clientId</span></span>|<span data-ttu-id="ba1c2-171">字符串</span><span class="sxs-lookup"><span data-stu-id="ba1c2-171">String</span></span>|<span data-ttu-id="ba1c2-172">应用程序的客户端 ID。</span><span class="sxs-lookup"><span data-stu-id="ba1c2-172">The client ID for the application.</span></span> <span data-ttu-id="ba1c2-173">这是向标识提供程序注册应用程序时获取的客户端 ID。</span><span class="sxs-lookup"><span data-stu-id="ba1c2-173">This is the client ID obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="ba1c2-174">clientSecret</span><span class="sxs-lookup"><span data-stu-id="ba1c2-174">clientSecret</span></span>|<span data-ttu-id="ba1c2-175">字符串</span><span class="sxs-lookup"><span data-stu-id="ba1c2-175">String</span></span>|<span data-ttu-id="ba1c2-176">应用程序的客户端密码。</span><span class="sxs-lookup"><span data-stu-id="ba1c2-176">The client secret for the application.</span></span> <span data-ttu-id="ba1c2-177">这是向标识提供程序注册应用程序时获取的客户端密码。</span><span class="sxs-lookup"><span data-stu-id="ba1c2-177">This is the client secret obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="ba1c2-178">name</span><span class="sxs-lookup"><span data-stu-id="ba1c2-178">name</span></span>|<span data-ttu-id="ba1c2-179">字符串</span><span class="sxs-lookup"><span data-stu-id="ba1c2-179">String</span></span>|<span data-ttu-id="ba1c2-180">标识提供程序的显示名称。</span><span class="sxs-lookup"><span data-stu-id="ba1c2-180">The display name of the identity provider.</span></span>|
|<span data-ttu-id="ba1c2-181">type</span><span class="sxs-lookup"><span data-stu-id="ba1c2-181">type</span></span>|<span data-ttu-id="ba1c2-182">字符串</span><span class="sxs-lookup"><span data-stu-id="ba1c2-182">String</span></span>|<span data-ttu-id="ba1c2-183">标识提供程序类型。</span><span class="sxs-lookup"><span data-stu-id="ba1c2-183">The identity provider type.</span></span> <span data-ttu-id="ba1c2-184">值必须为 `OpenIdConnect` 。</span><span class="sxs-lookup"><span data-stu-id="ba1c2-184">The value must be `OpenIdConnect`.</span></span>|
|<span data-ttu-id="ba1c2-185">claimsMapping</span><span class="sxs-lookup"><span data-stu-id="ba1c2-185">claimsMapping</span></span>|[<span data-ttu-id="ba1c2-186">claimsMapping</span><span class="sxs-lookup"><span data-stu-id="ba1c2-186">claimsMapping</span></span>](../resources/claimsmapping.md)|<span data-ttu-id="ba1c2-187">在 `userId` `displayname` claimsMapping 对象中，和属性是必需的。</span><span class="sxs-lookup"><span data-stu-id="ba1c2-187">The `userId` and `displayname` properties are required in the claimsMapping object.</span></span>|
|<span data-ttu-id="ba1c2-188">metadataUrl</span><span class="sxs-lookup"><span data-stu-id="ba1c2-188">metadataUrl</span></span>|<span data-ttu-id="ba1c2-189">字符串</span><span class="sxs-lookup"><span data-stu-id="ba1c2-189">String</span></span>|<span data-ttu-id="ba1c2-190">开放 Id 的元数据文档的 URL 连接标识提供程序。</span><span class="sxs-lookup"><span data-stu-id="ba1c2-190">The URL for the metadata document of the Open Id Connect identity provider.</span></span>|
|<span data-ttu-id="ba1c2-191">responseMode</span><span class="sxs-lookup"><span data-stu-id="ba1c2-191">responseMode</span></span>|<span data-ttu-id="ba1c2-192">字符串</span><span class="sxs-lookup"><span data-stu-id="ba1c2-192">String</span></span>|<span data-ttu-id="ba1c2-193">定义应用于将数据从自定义标识提供程序发送回 Azure AD B2C 的方法。</span><span class="sxs-lookup"><span data-stu-id="ba1c2-193">Defines the method that should be used to send the data back from the custom identity provider to Azure AD B2C.</span></span> <span data-ttu-id="ba1c2-194">可以使用以下响应模式：</span><span class="sxs-lookup"><span data-stu-id="ba1c2-194">The following response modes can be used:</span></span> <ul><li/><span data-ttu-id="ba1c2-195">`form_post`：建议使用此响应模式以获得最佳安全性。</span><span class="sxs-lookup"><span data-stu-id="ba1c2-195">`form_post` : This response mode is recommended for best security.</span></span> <span data-ttu-id="ba1c2-196">响应通过 HTTP POST 方法传输，其中的代码或令牌使用应用程序/x www 格式 urlencoded 格式在正文中进行编码。</span><span class="sxs-lookup"><span data-stu-id="ba1c2-196">The response is transmitted via the HTTP POST method, with the code or token being encoded in the body using the application/x-www-form-urlencoded format.</span></span><li/><span data-ttu-id="ba1c2-197">`query`：代码或令牌作为查询参数返回。</span><span class="sxs-lookup"><span data-stu-id="ba1c2-197">`query` : The code or token is returned as a query parameter.</span></span></ul>|
|<span data-ttu-id="ba1c2-198">responseType</span><span class="sxs-lookup"><span data-stu-id="ba1c2-198">responseType</span></span>|<span data-ttu-id="ba1c2-199">字符串</span><span class="sxs-lookup"><span data-stu-id="ba1c2-199">String</span></span>|<span data-ttu-id="ba1c2-200">描述在对自定义标识提供程序的 authorization_endpoint 的初始调用中发送回的信息类型。</span><span class="sxs-lookup"><span data-stu-id="ba1c2-200">Describes what kind of information is sent back in the initial call to the authorization_endpoint of the custom identity provider.</span></span> <span data-ttu-id="ba1c2-201">可以使用以下响应类型：</span><span class="sxs-lookup"><span data-stu-id="ba1c2-201">The following response types can be used:</span></span><ul><li/> <span data-ttu-id="ba1c2-202">`code`：按照授权代码流，代码将返回到 Azure AD B2C。</span><span class="sxs-lookup"><span data-stu-id="ba1c2-202">`code` : As per the authorization code flow, a code will be returned back to Azure AD B2C.</span></span> <span data-ttu-id="ba1c2-203">Azure AD B2C 将继续调用 token_endpoint 以交换令牌的代码。</span><span class="sxs-lookup"><span data-stu-id="ba1c2-203">Azure AD B2C proceeds to call the token_endpoint to exchange the code for the token.</span></span><li/> <span data-ttu-id="ba1c2-204">`id_token`：从自定义标识提供程序向 Azure AD B2C 返回 ID 令牌。</span><span class="sxs-lookup"><span data-stu-id="ba1c2-204">`id_token` : An ID token is returned back to Azure AD B2C from the custom identity provider.</span></span> <li/><span data-ttu-id="ba1c2-205">`token`：从自定义标识提供程序向 Azure AD B2C 返回访问令牌。</span><span class="sxs-lookup"><span data-stu-id="ba1c2-205">`token` : An access token is returned back to Azure AD B2C from the custom identity provider.</span></span> <span data-ttu-id="ba1c2-206">（目前 Azure AD B2C 不支持此值）</span><span class="sxs-lookup"><span data-stu-id="ba1c2-206">(This value is not supported by Azure AD B2C at the moment)</span></span></ul>|
|<span data-ttu-id="ba1c2-207">scope</span><span class="sxs-lookup"><span data-stu-id="ba1c2-207">scope</span></span>|<span data-ttu-id="ba1c2-208">String</span><span class="sxs-lookup"><span data-stu-id="ba1c2-208">String</span></span>|<span data-ttu-id="ba1c2-209">作用域定义要从自定义标识提供程序中收集的信息和权限。</span><span class="sxs-lookup"><span data-stu-id="ba1c2-209">Scope defines the information and permissions you are looking to gather from your custom identity provider.</span></span>|

## <a name="response"></a><span data-ttu-id="ba1c2-210">响应</span><span class="sxs-lookup"><span data-stu-id="ba1c2-210">Response</span></span>

<span data-ttu-id="ba1c2-211">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和[Identityprovider.read.all](../resources/identityprovider.md)或[openIdConnectProvider](../resources/openidconnectprovider.md) （仅适用于 Azure AD B2C）对象。</span><span class="sxs-lookup"><span data-stu-id="ba1c2-211">If successful, this method returns a `201 Created` response code and [identityProvider](../resources/identityprovider.md) or [openIdConnectProvider](../resources/openidconnectprovider.md) (only for Azure AD B2C) object in the response body.</span></span> <span data-ttu-id="ba1c2-212">如果失败，将返回 `4xx` 错误并显示具体详细信息。</span><span class="sxs-lookup"><span data-stu-id="ba1c2-212">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="examples"></a><span data-ttu-id="ba1c2-213">示例</span><span class="sxs-lookup"><span data-stu-id="ba1c2-213">Examples</span></span>

### <a name="example-1-create-a-specific-identityprovider"></a><span data-ttu-id="ba1c2-214">示例1：创建特定的**identityprovider.read.all**</span><span class="sxs-lookup"><span data-stu-id="ba1c2-214">Example 1: Create a specific **identityProvider**</span></span>

#### <a name="request"></a><span data-ttu-id="ba1c2-215">请求</span><span class="sxs-lookup"><span data-stu-id="ba1c2-215">Request</span></span>

<span data-ttu-id="ba1c2-216">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ba1c2-216">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_identityprovider_from_identityproviders"
}
-->

``` http
POST https://graph.microsoft.com/beta/identityProviders
Content-type: application/json
Content-length: 154

{
  "@odata.type": "microsoft.graph.identityProvider",
  "name": "Login with Amazon",
  "type": "Amazon",
  "clientId": "56433757-cadd-4135-8431-2c9e3fd68ae8",
  "clientSecret": "000000000000"
}
```

#### <a name="response"></a><span data-ttu-id="ba1c2-217">响应</span><span class="sxs-lookup"><span data-stu-id="ba1c2-217">Response</span></span>

<span data-ttu-id="ba1c2-218">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ba1c2-218">The following is an example of the response.</span></span>

<span data-ttu-id="ba1c2-219">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="ba1c2-219">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.IdentityProvider"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
   "@odata.type": "microsoft.graph.identityProvider",
    "id": "Amazon-OAUTH",
    "name": "Login with Amazon",
    "type": "Amazon",
    "clientId": "56433757-cadd-4135-8431-2c9e3fd68ae8",
    "clientSecret": "*****"
}
```
### <a name="example-2-create-a-specific-openidconnectprovider-only-for-azure-ad-b2c"></a><span data-ttu-id="ba1c2-220">示例2：创建特定的**openIDConnectProvider** （仅适用于 AZURE AD B2C）</span><span class="sxs-lookup"><span data-stu-id="ba1c2-220">Example 2: Create a specific **openIDConnectProvider** (only for Azure AD B2C)</span></span>

#### <a name="request"></a><span data-ttu-id="ba1c2-221">请求</span><span class="sxs-lookup"><span data-stu-id="ba1c2-221">Request</span></span>

<span data-ttu-id="ba1c2-222">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ba1c2-222">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_openidconnectprovider_from_identityproviders"
}
-->

``` http
POST https://graph.microsoft.com/beta/identityProviders
Content-type: application/json

{
  "@odata.type": "microsoft.graph.openIdConnectProvider",
    "name": "Login with the Contoso identity provider",
    "type": "OpenIDConnect",
    "clientId": "56433757-cadd-4135-8431-2c9e3fd68ae8",
    "clientSecret": "12345",
    "claimsMapping": {
        "userId": "myUserId",
        "givenName": "myGivenName",
        "surname": "mySurname",
        "email": "myEmail",
        "displayName": "myDisplayName"
    },
    "domainHint": "mycustomoidc",
    "metadataUrl": "https://mycustomoidc.com/.well-known/openid-configuration",
    "responseMode": "form_post",
    "responseType": "code",
    "scope": "openid"
}

```

#### <a name="response"></a><span data-ttu-id="ba1c2-223">响应</span><span class="sxs-lookup"><span data-stu-id="ba1c2-223">Response</span></span>

<span data-ttu-id="ba1c2-224">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ba1c2-224">The following is an example of the response.</span></span>

<span data-ttu-id="ba1c2-225">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="ba1c2-225">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.openIdConnectProvider"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.type": "microsoft.graph.openIdConnectProvider",
  "id": "OIDC-V1-MyTest-085a8a0c-58cb-4b6d-8e07-1328ea404e1a",
  "name": "Login with the Contoso identity provider",
  "type": "OpenIDConnect",
  "clientId": "56433757-cadd-4135-8431-2c9e3fd68ae8",
  "clientSecret": "12345",
  "claimsMapping": {
      "userId": "myUserId",
      "givenName": "myGivenName",
      "surname": "mySurname",
      "email": "myEmail",
      "displayName": "myDisplayName"
  },
  "domainHint": "mycustomoidc",
  "metadataUrl": "https://mycustomoidc.com/.well-known/openid-configuration",
  "responseMode": "form_post",
  "responseType": "code",
  "scope": "openid"
}
```

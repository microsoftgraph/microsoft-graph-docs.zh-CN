---
title: 创建 b2cIdentityUserFlow
description: 创建新的 b2cIdentityUserFlow 对象。
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: identity-and-sign-in
ms.openlocfilehash: edb0a8eab1406c3bcdd3856c158b4fb936228eb5
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50435537"
---
# <a name="create-b2cidentityuserflow"></a><span data-ttu-id="1dd22-103">创建 b2cIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="1dd22-103">Create b2cIdentityUserFlow</span></span>

<span data-ttu-id="1dd22-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1dd22-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1dd22-105">创建新的 [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1dd22-105">Create a new [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="1dd22-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="1dd22-106">Permissions</span></span>

<span data-ttu-id="1dd22-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1dd22-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1dd22-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="1dd22-109">Permission type</span></span>      | <span data-ttu-id="1dd22-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1dd22-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1dd22-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1dd22-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1dd22-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1dd22-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="1dd22-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1dd22-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="1dd22-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="1dd22-114">Not supported.</span></span>|
|<span data-ttu-id="1dd22-115">Application</span><span class="sxs-lookup"><span data-stu-id="1dd22-115">Application</span></span>|<span data-ttu-id="1dd22-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1dd22-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="1dd22-117">工作或学校帐户需要属于以下角色之一：</span><span class="sxs-lookup"><span data-stu-id="1dd22-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="1dd22-118">全局管理员</span><span class="sxs-lookup"><span data-stu-id="1dd22-118">Global administrator</span></span>
* <span data-ttu-id="1dd22-119">外部标识用户流管理员</span><span class="sxs-lookup"><span data-stu-id="1dd22-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="1dd22-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1dd22-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identity/b2cUserFlows
```

## <a name="request-headers"></a><span data-ttu-id="1dd22-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="1dd22-121">Request headers</span></span>

|<span data-ttu-id="1dd22-122">名称</span><span class="sxs-lookup"><span data-stu-id="1dd22-122">Name</span></span>|<span data-ttu-id="1dd22-123">说明</span><span class="sxs-lookup"><span data-stu-id="1dd22-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="1dd22-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="1dd22-124">Authorization</span></span>|<span data-ttu-id="1dd22-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1dd22-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="1dd22-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1dd22-127">Content-Type</span></span>|<span data-ttu-id="1dd22-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="1dd22-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1dd22-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="1dd22-130">Request body</span></span>

<span data-ttu-id="1dd22-131">在请求正文中，提供 [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md)的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1dd22-131">In the request body, provide a JSON representation of a [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md).</span></span>

|<span data-ttu-id="1dd22-132">属性</span><span class="sxs-lookup"><span data-stu-id="1dd22-132">Property</span></span>|<span data-ttu-id="1dd22-133">类型</span><span class="sxs-lookup"><span data-stu-id="1dd22-133">Type</span></span>|<span data-ttu-id="1dd22-134">说明</span><span class="sxs-lookup"><span data-stu-id="1dd22-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1dd22-135">id</span><span class="sxs-lookup"><span data-stu-id="1dd22-135">id</span></span>|<span data-ttu-id="1dd22-136">String</span><span class="sxs-lookup"><span data-stu-id="1dd22-136">String</span></span>|<span data-ttu-id="1dd22-137">必需。</span><span class="sxs-lookup"><span data-stu-id="1dd22-137">Required.</span></span> <span data-ttu-id="1dd22-138">用户流名称。</span><span class="sxs-lookup"><span data-stu-id="1dd22-138">The name of the user flow.</span></span> <span data-ttu-id="1dd22-139">该名称将在创建后进行 `B2C_1` 预笔写。</span><span class="sxs-lookup"><span data-stu-id="1dd22-139">The name will be pre-pended with `B2C_1` after creation.</span></span>|
|<span data-ttu-id="1dd22-140">userFlowType</span><span class="sxs-lookup"><span data-stu-id="1dd22-140">userFlowType</span></span>|<span data-ttu-id="1dd22-141">String</span><span class="sxs-lookup"><span data-stu-id="1dd22-141">String</span></span>|<span data-ttu-id="1dd22-142">必需。</span><span class="sxs-lookup"><span data-stu-id="1dd22-142">Required.</span></span> <span data-ttu-id="1dd22-143">要创建的用户流的类型。</span><span class="sxs-lookup"><span data-stu-id="1dd22-143">The type of user flow you are creating.</span></span> <span data-ttu-id="1dd22-144">**userFlowType** 支持的值有：</span><span class="sxs-lookup"><span data-stu-id="1dd22-144">The supported values for **userFlowType** are:</span></span><br/><ul><li>`signUp`</li><li>`signIn`</li><li>`signUpOrSignIn`</li><li>`passwordReset`</li><li>`profileUpdate`</li><li>`resourceOwner`</li>|
|<span data-ttu-id="1dd22-145">userFlowTypeVersion</span><span class="sxs-lookup"><span data-stu-id="1dd22-145">userFlowTypeVersion</span></span>|<span data-ttu-id="1dd22-146">浮点</span><span class="sxs-lookup"><span data-stu-id="1dd22-146">Float</span></span>|<span data-ttu-id="1dd22-147">必需。</span><span class="sxs-lookup"><span data-stu-id="1dd22-147">Required.</span></span> <span data-ttu-id="1dd22-148">用户流版本。</span><span class="sxs-lookup"><span data-stu-id="1dd22-148">The version of the user flow.</span></span>|
|<span data-ttu-id="1dd22-149">isLanguageCustomizationEnabled</span><span class="sxs-lookup"><span data-stu-id="1dd22-149">isLanguageCustomizationEnabled</span></span>|<span data-ttu-id="1dd22-150">Boolean</span><span class="sxs-lookup"><span data-stu-id="1dd22-150">Boolean</span></span>|<span data-ttu-id="1dd22-151">可选。</span><span class="sxs-lookup"><span data-stu-id="1dd22-151">Optional.</span></span> <span data-ttu-id="1dd22-152">确定是否在 Azure AD B2C 用户流中启用语言自定义。</span><span class="sxs-lookup"><span data-stu-id="1dd22-152">Determines whether language customization is enabled within the Azure AD B2C user flow.</span></span> <span data-ttu-id="1dd22-153">默认情况下，不会为 Azure AD B2C 用户流启用语言自定义。</span><span class="sxs-lookup"><span data-stu-id="1dd22-153">Language customization is not enabled by default for Azure AD B2C user flows.</span></span>|
|<span data-ttu-id="1dd22-154">defaultLanguageTag</span><span class="sxs-lookup"><span data-stu-id="1dd22-154">defaultLanguageTag</span></span>|<span data-ttu-id="1dd22-155">String</span><span class="sxs-lookup"><span data-stu-id="1dd22-155">String</span></span>|<span data-ttu-id="1dd22-156">可选。</span><span class="sxs-lookup"><span data-stu-id="1dd22-156">Optional.</span></span>  <span data-ttu-id="1dd22-157">指定请求中未指定标记时所使用的 b2cIdentityUserFlow `ui_locale` 的默认语言。</span><span class="sxs-lookup"><span data-stu-id="1dd22-157">Specifies the default language of the b2cIdentityUserFlow that is used when no `ui_locale` tag is specified in the request.</span></span> <span data-ttu-id="1dd22-158">此字段符合 [RFC 5646](https://tools.ietf.org/html/rfc5646)。</span><span class="sxs-lookup"><span data-stu-id="1dd22-158">This field is [RFC 5646](https://tools.ietf.org/html/rfc5646) compliant.</span></span>|
|<span data-ttu-id="1dd22-159">identityProviders</span><span class="sxs-lookup"><span data-stu-id="1dd22-159">identityProviders</span></span>|<span data-ttu-id="1dd22-160">[identityProvider](../resources/identityprovider.md)集合 </span><span class="sxs-lookup"><span data-stu-id="1dd22-160">[identityProvider](../resources/identityprovider.md) collection</span></span>|<span data-ttu-id="1dd22-161">可选。</span><span class="sxs-lookup"><span data-stu-id="1dd22-161">Optional.</span></span> <span data-ttu-id="1dd22-162">要包括在用户流中的标识提供程序。</span><span class="sxs-lookup"><span data-stu-id="1dd22-162">The identity providers you want to include in the user flow.</span></span>|

## <a name="response"></a><span data-ttu-id="1dd22-163">响应</span><span class="sxs-lookup"><span data-stu-id="1dd22-163">Response</span></span>

<span data-ttu-id="1dd22-164">如果成功，此方法将响应代码和位置标头与 URI 返回到为此请求创建的 `201 Created` [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) 对象，并添加前缀 `B2C_1` 的名称。</span><span class="sxs-lookup"><span data-stu-id="1dd22-164">If successful, this method returns a `201 Created` response code and a Location header with a URI to the [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) object created for this request, with the `B2C_1` prefix added to the name.</span></span> <span data-ttu-id="1dd22-165">如果失败，将返回 `4xx` 错误并显示具体详细信息。</span><span class="sxs-lookup"><span data-stu-id="1dd22-165">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="examples"></a><span data-ttu-id="1dd22-166">示例</span><span class="sxs-lookup"><span data-stu-id="1dd22-166">Examples</span></span>

### <a name="example-1-create-a-user-flow-with-the-default-values"></a><span data-ttu-id="1dd22-167">示例 1：使用默认值创建用户流</span><span class="sxs-lookup"><span data-stu-id="1dd22-167">Example 1: Create a user flow with the default values</span></span>

#### <a name="request"></a><span data-ttu-id="1dd22-168">请求</span><span class="sxs-lookup"><span data-stu-id="1dd22-168">Request</span></span>

<span data-ttu-id="1dd22-169">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="1dd22-169">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1dd22-170">HTTP</span><span class="sxs-lookup"><span data-stu-id="1dd22-170">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_b2cuserflow_from_b2cuserflows"
}
-->

``` http
POST https://graph.microsoft.com/beta/identity/b2cUserFlows
Content-type: application/json
Content-length: 154

{
    "id": "Customer",
    "userFlowType": "signUpOrSignIn",
    "userFlowTypeVersion": 3
}
```

# <a name="c"></a>[<span data-ttu-id="1dd22-171">C#</span><span class="sxs-lookup"><span data-stu-id="1dd22-171">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-b2cuserflow-from-b2cuserflows-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1dd22-172">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1dd22-172">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-b2cuserflow-from-b2cuserflows-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1dd22-173">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1dd22-173">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-b2cuserflow-from-b2cuserflows-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1dd22-174">Java</span><span class="sxs-lookup"><span data-stu-id="1dd22-174">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-b2cuserflow-from-b2cuserflows-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="1dd22-175">响应</span><span class="sxs-lookup"><span data-stu-id="1dd22-175">Response</span></span>

<span data-ttu-id="1dd22-176">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="1dd22-176">The following is an example of the response.</span></span>

<span data-ttu-id="1dd22-177">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="1dd22-177">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.b2cIdentityUserFlow"
} -->

```http
HTTP/1.1 201 Created
Location: https://graph.microsoft.com/beta/identity/b2cUserFlows/B2C_1_Customer
Content-type: application/json

{
    "id": "B2C_1_Customer",
    "userFlowType": "signUpOrSignIn",
    "userFlowTypeVersion": 3,
    "isLanguageCustomizationEnabled": false,
    "defaultLanguageTag": "en"
}
```

### <a name="example-2-create-a-user-flow-with-the-default-values-and-an-identity-provider"></a><span data-ttu-id="1dd22-178">示例 2：使用默认值和标识提供程序创建用户流</span><span class="sxs-lookup"><span data-stu-id="1dd22-178">Example 2: Create a user flow with the default values and an identity provider</span></span>

#### <a name="request"></a><span data-ttu-id="1dd22-179">请求</span><span class="sxs-lookup"><span data-stu-id="1dd22-179">Request</span></span>

<span data-ttu-id="1dd22-180">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="1dd22-180">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1dd22-181">HTTP</span><span class="sxs-lookup"><span data-stu-id="1dd22-181">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_b2cuserflow_from_b2cuserflows_identityProvider"
}
-->

``` http
POST https://graph.microsoft.com/beta/identity/b2cUserFlows
Content-type: application/json
Content-length: 154

{
    "id": "Customer",
    "userFlowType": "signUpOrSignIn",
    "userFlowTypeVersion": 3,
    "identityProviders": [
        {
            "id": "Facebook-OAuth",
            "type": "Facebook",
            "Name": "Facebook"
        }
    ]
}
```
# <a name="c"></a>[<span data-ttu-id="1dd22-182">C#</span><span class="sxs-lookup"><span data-stu-id="1dd22-182">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-b2cuserflow-from-b2cuserflows-identityprovider-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1dd22-183">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1dd22-183">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-b2cuserflow-from-b2cuserflows-identityprovider-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1dd22-184">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1dd22-184">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-b2cuserflow-from-b2cuserflows-identityprovider-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1dd22-185">Java</span><span class="sxs-lookup"><span data-stu-id="1dd22-185">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-b2cuserflow-from-b2cuserflows-identityprovider-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="1dd22-186">响应</span><span class="sxs-lookup"><span data-stu-id="1dd22-186">Response</span></span>

<span data-ttu-id="1dd22-187">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="1dd22-187">The following is an example of the response.</span></span>

<span data-ttu-id="1dd22-188">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="1dd22-188">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.b2cIdentityUserFlow"
} -->

```http
HTTP/1.1 201 Created
Location: https://graph.microsoft.com/beta/identity/b2cUserFlows/B2C_1_Customer
Content-type: application/json

{
    "id": "B2C_1_Customer",
    "userFlowType": "signUpOrSignIn",
    "userFlowTypeVersion": 3,
    "isLanguageCustomizationEnabled": false,
    "defaultLanguageTag": "en"
}
```

<!-- {
  "type": "#page.annotation",
  "description": "Create b2CUserFlow",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: create_b2cUserFlow_from_b2cUserFlows/userFlowTypeVersion:\r\n      Expected type Single but actual was Int64. Property: userFlowTypeVersion, actual value: '3'",
    "Error: create_b2cUserFlow_from_b2cUserFlows_identityProvider/userFlowTypeVersion:\r\n    Expected type Single but actual was Int64. Property: userFlowTypeVersion, actual value: '3'"
  ]
}-->

### <a name="example-3-create-a-user-flow-with-the-default-values-and-configuration-for-api-connectors"></a><span data-ttu-id="1dd22-189">示例 3：使用 API 连接器的默认值和配置创建用户流</span><span class="sxs-lookup"><span data-stu-id="1dd22-189">Example 3: Create a user flow with the default values and configuration for API connectors</span></span>

#### <a name="request"></a><span data-ttu-id="1dd22-190">请求</span><span class="sxs-lookup"><span data-stu-id="1dd22-190">Request</span></span>

<span data-ttu-id="1dd22-191">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="1dd22-191">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="1dd22-192">HTTP</span><span class="sxs-lookup"><span data-stu-id="1dd22-192">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_b2cuserflow_from_b2cuserflows_apiconnectors"
}
-->

``` http
POST https://graph.microsoft.com/beta/identity/b2cUserFlows
Content-type: application/json
Content-length: 154

{
    "id": "UserFlowWithAPIConnector",
    "userFlowType": "signUpOrSignIn",
    "userFlowTypeVersion": 1,
    "apiConnectorConfiguration":{
        "postFederationSignup":{
            "@odata.id": "https://graph.microsoft.com/beta/identity/apiConnectors/{id}"
        },
        "postAttributeCollection":{
            "@odata.id": "https://graph.microsoft.com/beta/identity/apiConnectors/{id}"
        }
    }
}
```
# <a name="c"></a>[<span data-ttu-id="1dd22-193">C#</span><span class="sxs-lookup"><span data-stu-id="1dd22-193">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-b2cuserflow-from-b2cuserflows-apiconnectors-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1dd22-194">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1dd22-194">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-b2cuserflow-from-b2cuserflows-apiconnectors-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1dd22-195">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1dd22-195">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-b2cuserflow-from-b2cuserflows-apiconnectors-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1dd22-196">Java</span><span class="sxs-lookup"><span data-stu-id="1dd22-196">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-b2cuserflow-from-b2cuserflows-apiconnectors-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="1dd22-197">响应</span><span class="sxs-lookup"><span data-stu-id="1dd22-197">Response</span></span>

<span data-ttu-id="1dd22-198">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="1dd22-198">The following is an example of the response.</span></span>

<span data-ttu-id="1dd22-199">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="1dd22-199">**Note:** The response object shown here might be shortened for readability.</span></span>

<span data-ttu-id="1dd22-200">**注意：** 该属性 `apiConnectorConfiguration` 始终返回' {} 值。</span><span class="sxs-lookup"><span data-stu-id="1dd22-200">**Note:** The `apiConnectorConfiguration` property always returns a '{}' value.</span></span> <span data-ttu-id="1dd22-201">若要查看导航属性的完整值，请使用 [此](../api/b2cidentityuserflow-get-apiConnectorConfiguration.md) API。</span><span class="sxs-lookup"><span data-stu-id="1dd22-201">To see full value with the navigation properties, use [this](../api/b2cidentityuserflow-get-apiConnectorConfiguration.md) API.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.b2cIdentityUserFlow"
} -->

```http
HTTP/1.1 201 Created
Location: https://graph.microsoft.com/beta/identity/b2cUserFlows/B2C_1_Partner
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identity/b2cUserFlows/$entity",
    "id": "B2C_1_UserFlowWithAPIConnector",
    "userFlowType": "signUpOrSignIn",
    "userFlowTypeVersion": 1,
    "apiConnectorConfiguration": {}
}
```

<!-- {
  "type": "#page.annotation",
  "description": "Create b2cUserFlow",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: create_b2cUserFlow_from_b2cuserflows_apiconnectors/userFlowTypeVersion:\r\n      Expected type Single but actual was Int64. Property: userFlowTypeVersion, actual value: '1'"
  ]
}-->

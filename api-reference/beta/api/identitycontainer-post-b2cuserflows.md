---
title: 创建 b2cIdentityUserFlow
description: 创建新的 b2cIdentityUserFlow 对象。
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 88595851390bdfefb6db3e8246da92940084de92
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/18/2021
ms.locfileid: "50292012"
---
# <a name="create-b2cidentityuserflow"></a><span data-ttu-id="480af-103">创建 b2cIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="480af-103">Create b2cIdentityUserFlow</span></span>

<span data-ttu-id="480af-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="480af-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="480af-105">创建新的 [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="480af-105">Create a new [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="480af-106">权限</span><span class="sxs-lookup"><span data-stu-id="480af-106">Permissions</span></span>

<span data-ttu-id="480af-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="480af-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="480af-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="480af-109">Permission type</span></span>      | <span data-ttu-id="480af-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="480af-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="480af-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="480af-111">Delegated (work or school account)</span></span>|<span data-ttu-id="480af-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="480af-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="480af-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="480af-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="480af-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="480af-114">Not supported.</span></span>|
|<span data-ttu-id="480af-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="480af-115">Application</span></span>|<span data-ttu-id="480af-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="480af-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="480af-117">工作或学校帐户需要属于以下角色之一：</span><span class="sxs-lookup"><span data-stu-id="480af-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="480af-118">全局管理员</span><span class="sxs-lookup"><span data-stu-id="480af-118">Global administrator</span></span>
* <span data-ttu-id="480af-119">外部标识用户流管理员</span><span class="sxs-lookup"><span data-stu-id="480af-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="480af-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="480af-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identity/b2cUserFlows
```

## <a name="request-headers"></a><span data-ttu-id="480af-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="480af-121">Request headers</span></span>

|<span data-ttu-id="480af-122">名称</span><span class="sxs-lookup"><span data-stu-id="480af-122">Name</span></span>|<span data-ttu-id="480af-123">说明</span><span class="sxs-lookup"><span data-stu-id="480af-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="480af-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="480af-124">Authorization</span></span>|<span data-ttu-id="480af-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="480af-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="480af-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="480af-127">Content-Type</span></span>|<span data-ttu-id="480af-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="480af-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="480af-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="480af-130">Request body</span></span>

<span data-ttu-id="480af-131">在请求正文中，提供 [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md)的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="480af-131">In the request body, provide a JSON representation of a [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md).</span></span>

|<span data-ttu-id="480af-132">属性</span><span class="sxs-lookup"><span data-stu-id="480af-132">Property</span></span>|<span data-ttu-id="480af-133">类型</span><span class="sxs-lookup"><span data-stu-id="480af-133">Type</span></span>|<span data-ttu-id="480af-134">说明</span><span class="sxs-lookup"><span data-stu-id="480af-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="480af-135">id</span><span class="sxs-lookup"><span data-stu-id="480af-135">id</span></span>|<span data-ttu-id="480af-136">String</span><span class="sxs-lookup"><span data-stu-id="480af-136">String</span></span>|<span data-ttu-id="480af-137">必需。</span><span class="sxs-lookup"><span data-stu-id="480af-137">Required.</span></span> <span data-ttu-id="480af-138">用户流名称。</span><span class="sxs-lookup"><span data-stu-id="480af-138">The name of the user flow.</span></span> <span data-ttu-id="480af-139">该名称将在创建后进行 `B2C_1` 预笔写。</span><span class="sxs-lookup"><span data-stu-id="480af-139">The name will be pre-pended with `B2C_1` after creation.</span></span>|
|<span data-ttu-id="480af-140">userFlowType</span><span class="sxs-lookup"><span data-stu-id="480af-140">userFlowType</span></span>|<span data-ttu-id="480af-141">String</span><span class="sxs-lookup"><span data-stu-id="480af-141">String</span></span>|<span data-ttu-id="480af-142">必需。</span><span class="sxs-lookup"><span data-stu-id="480af-142">Required.</span></span> <span data-ttu-id="480af-143">要创建的用户流的类型。</span><span class="sxs-lookup"><span data-stu-id="480af-143">The type of user flow you are creating.</span></span> <span data-ttu-id="480af-144">**userFlowType** 支持的值有：</span><span class="sxs-lookup"><span data-stu-id="480af-144">The supported values for **userFlowType** are:</span></span><br/><ul><li>`signUp`</li><li>`signIn`</li><li>`signUpOrSignIn`</li><li>`passwordReset`</li><li>`profileUpdate`</li><li>`resourceOwner`</li>|
|<span data-ttu-id="480af-145">userFlowTypeVersion</span><span class="sxs-lookup"><span data-stu-id="480af-145">userFlowTypeVersion</span></span>|<span data-ttu-id="480af-146">浮点</span><span class="sxs-lookup"><span data-stu-id="480af-146">Float</span></span>|<span data-ttu-id="480af-147">必需。</span><span class="sxs-lookup"><span data-stu-id="480af-147">Required.</span></span> <span data-ttu-id="480af-148">用户流版本。</span><span class="sxs-lookup"><span data-stu-id="480af-148">The version of the user flow.</span></span>|
|<span data-ttu-id="480af-149">isLanguageCustomizationEnabled</span><span class="sxs-lookup"><span data-stu-id="480af-149">isLanguageCustomizationEnabled</span></span>|<span data-ttu-id="480af-150">Boolean</span><span class="sxs-lookup"><span data-stu-id="480af-150">Boolean</span></span>|<span data-ttu-id="480af-151">可选。</span><span class="sxs-lookup"><span data-stu-id="480af-151">Optional.</span></span> <span data-ttu-id="480af-152">确定是否在 Azure AD B2C 用户流中启用语言自定义。</span><span class="sxs-lookup"><span data-stu-id="480af-152">Determines whether language customization is enabled within the Azure AD B2C user flow.</span></span> <span data-ttu-id="480af-153">默认情况下，不会为 Azure AD B2C 用户流启用语言自定义。</span><span class="sxs-lookup"><span data-stu-id="480af-153">Language customization is not enabled by default for Azure AD B2C user flows.</span></span>|
|<span data-ttu-id="480af-154">defaultLanguageTag</span><span class="sxs-lookup"><span data-stu-id="480af-154">defaultLanguageTag</span></span>|<span data-ttu-id="480af-155">String</span><span class="sxs-lookup"><span data-stu-id="480af-155">String</span></span>|<span data-ttu-id="480af-156">可选。</span><span class="sxs-lookup"><span data-stu-id="480af-156">Optional.</span></span>  <span data-ttu-id="480af-157">指定请求中未指定标记时所使用的 b2cIdentityUserFlow `ui_locale` 的默认语言。</span><span class="sxs-lookup"><span data-stu-id="480af-157">Specifies the default language of the b2cIdentityUserFlow that is used when no `ui_locale` tag is specified in the request.</span></span> <span data-ttu-id="480af-158">此字段符合 [RFC 5646](https://tools.ietf.org/html/rfc5646)。</span><span class="sxs-lookup"><span data-stu-id="480af-158">This field is [RFC 5646](https://tools.ietf.org/html/rfc5646) compliant.</span></span>|
|<span data-ttu-id="480af-159">identityProviders</span><span class="sxs-lookup"><span data-stu-id="480af-159">identityProviders</span></span>|<span data-ttu-id="480af-160">[identityProvider](../resources/identityprovider.md)集合 </span><span class="sxs-lookup"><span data-stu-id="480af-160">[identityProvider](../resources/identityprovider.md) collection</span></span>|<span data-ttu-id="480af-161">可选。</span><span class="sxs-lookup"><span data-stu-id="480af-161">Optional.</span></span> <span data-ttu-id="480af-162">要包括在用户流中的标识提供程序。</span><span class="sxs-lookup"><span data-stu-id="480af-162">The identity providers you want to include in the user flow.</span></span>|

## <a name="response"></a><span data-ttu-id="480af-163">响应</span><span class="sxs-lookup"><span data-stu-id="480af-163">Response</span></span>

<span data-ttu-id="480af-164">如果成功，此方法将响应代码和位置标头与 URI 返回到为此请求创建的 `201 Created` [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) 对象，并添加前缀 `B2C_1` 的名称。</span><span class="sxs-lookup"><span data-stu-id="480af-164">If successful, this method returns a `201 Created` response code and a Location header with a URI to the [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) object created for this request, with the `B2C_1` prefix added to the name.</span></span> <span data-ttu-id="480af-165">如果失败，将返回 `4xx` 错误并显示具体详细信息。</span><span class="sxs-lookup"><span data-stu-id="480af-165">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="examples"></a><span data-ttu-id="480af-166">示例</span><span class="sxs-lookup"><span data-stu-id="480af-166">Examples</span></span>

### <a name="example-1-create-a-user-flow-with-the-default-values"></a><span data-ttu-id="480af-167">示例 1：使用默认值创建用户流</span><span class="sxs-lookup"><span data-stu-id="480af-167">Example 1: Create a user flow with the default values</span></span>

#### <a name="request"></a><span data-ttu-id="480af-168">请求</span><span class="sxs-lookup"><span data-stu-id="480af-168">Request</span></span>

<span data-ttu-id="480af-169">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="480af-169">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="480af-170">HTTP</span><span class="sxs-lookup"><span data-stu-id="480af-170">HTTP</span></span>](#tab/http)
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

# <a name="c"></a>[<span data-ttu-id="480af-171">C#</span><span class="sxs-lookup"><span data-stu-id="480af-171">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-b2cuserflow-from-b2cuserflows-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="480af-172">JavaScript</span><span class="sxs-lookup"><span data-stu-id="480af-172">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-b2cuserflow-from-b2cuserflows-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="480af-173">Objective-C</span><span class="sxs-lookup"><span data-stu-id="480af-173">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-b2cuserflow-from-b2cuserflows-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="480af-174">Java</span><span class="sxs-lookup"><span data-stu-id="480af-174">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-b2cuserflow-from-b2cuserflows-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="480af-175">响应</span><span class="sxs-lookup"><span data-stu-id="480af-175">Response</span></span>

<span data-ttu-id="480af-176">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="480af-176">The following is an example of the response.</span></span>

<span data-ttu-id="480af-177">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="480af-177">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-2-create-a-user-flow-with-the-default-values-and-an-identity-provider"></a><span data-ttu-id="480af-178">示例 2：使用默认值和标识提供程序创建用户流</span><span class="sxs-lookup"><span data-stu-id="480af-178">Example 2: Create a user flow with the default values and an identity provider</span></span>

#### <a name="request"></a><span data-ttu-id="480af-179">请求</span><span class="sxs-lookup"><span data-stu-id="480af-179">Request</span></span>

<span data-ttu-id="480af-180">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="480af-180">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="480af-181">HTTP</span><span class="sxs-lookup"><span data-stu-id="480af-181">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="480af-182">C#</span><span class="sxs-lookup"><span data-stu-id="480af-182">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-b2cuserflow-from-b2cuserflows-identityprovider-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="480af-183">JavaScript</span><span class="sxs-lookup"><span data-stu-id="480af-183">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-b2cuserflow-from-b2cuserflows-identityprovider-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="480af-184">Objective-C</span><span class="sxs-lookup"><span data-stu-id="480af-184">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-b2cuserflow-from-b2cuserflows-identityprovider-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="480af-185">Java</span><span class="sxs-lookup"><span data-stu-id="480af-185">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-b2cuserflow-from-b2cuserflows-identityprovider-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="480af-186">响应</span><span class="sxs-lookup"><span data-stu-id="480af-186">Response</span></span>

<span data-ttu-id="480af-187">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="480af-187">The following is an example of the response.</span></span>

<span data-ttu-id="480af-188">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="480af-188">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-3-create-a-user-flow-with-the-default-values-and-configuration-for-api-connectors"></a><span data-ttu-id="480af-189">示例 3：使用 API 连接器的默认值和配置创建用户流</span><span class="sxs-lookup"><span data-stu-id="480af-189">Example 3: Create a user flow with the default values and configuration for API connectors</span></span>

#### <a name="request"></a><span data-ttu-id="480af-190">请求</span><span class="sxs-lookup"><span data-stu-id="480af-190">Request</span></span>

<span data-ttu-id="480af-191">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="480af-191">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="480af-192">HTTP</span><span class="sxs-lookup"><span data-stu-id="480af-192">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="480af-193">C#</span><span class="sxs-lookup"><span data-stu-id="480af-193">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-b2cuserflow-from-b2cuserflows-apiconnectors-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="480af-194">JavaScript</span><span class="sxs-lookup"><span data-stu-id="480af-194">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-b2cuserflow-from-b2cuserflows-apiconnectors-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="480af-195">Objective-C</span><span class="sxs-lookup"><span data-stu-id="480af-195">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-b2cuserflow-from-b2cuserflows-apiconnectors-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="480af-196">Java</span><span class="sxs-lookup"><span data-stu-id="480af-196">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-b2cuserflow-from-b2cuserflows-apiconnectors-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="480af-197">响应</span><span class="sxs-lookup"><span data-stu-id="480af-197">Response</span></span>

<span data-ttu-id="480af-198">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="480af-198">The following is an example of the response.</span></span>

<span data-ttu-id="480af-199">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="480af-199">**Note:** The response object shown here might be shortened for readability.</span></span>

<span data-ttu-id="480af-200">**注意：** 该属性 `apiConnectorConfiguration` 始终返回' {} 值。</span><span class="sxs-lookup"><span data-stu-id="480af-200">**Note:** The `apiConnectorConfiguration` property always returns a '{}' value.</span></span> <span data-ttu-id="480af-201">若要查看导航属性的完整值，请使用 [此](../api/b2cidentityuserflow-get-apiConnectorConfiguration.md) API。</span><span class="sxs-lookup"><span data-stu-id="480af-201">To see full value with the navigation properties, use [this](../api/b2cidentityuserflow-get-apiConnectorConfiguration.md) API.</span></span>

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

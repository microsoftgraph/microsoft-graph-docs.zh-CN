---
title: 创建 b2xIdentityUserFlow
description: 创建新的 b2xIdentityUserFlow 对象。
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: identity-and-sign-in
ms.openlocfilehash: c6e65a9f3edaa5e3be984db518067def60a394ba
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50435516"
---
# <a name="create-b2xidentityuserflow"></a><span data-ttu-id="c631b-103">创建 b2xIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="c631b-103">Create b2xIdentityUserFlow</span></span>

<span data-ttu-id="c631b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c631b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c631b-105">创建新的 [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c631b-105">Create a new [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c631b-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="c631b-106">Permissions</span></span>

<span data-ttu-id="c631b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c631b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c631b-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="c631b-109">Permission type</span></span>      | <span data-ttu-id="c631b-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c631b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c631b-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c631b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c631b-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c631b-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="c631b-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c631b-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="c631b-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="c631b-114">Not supported.</span></span>|
|<span data-ttu-id="c631b-115">Application</span><span class="sxs-lookup"><span data-stu-id="c631b-115">Application</span></span>|<span data-ttu-id="c631b-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c631b-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="c631b-117">工作或学校帐户需要属于以下角色之一：</span><span class="sxs-lookup"><span data-stu-id="c631b-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="c631b-118">全局管理员</span><span class="sxs-lookup"><span data-stu-id="c631b-118">Global administrator</span></span>
* <span data-ttu-id="c631b-119">外部标识用户流管理员</span><span class="sxs-lookup"><span data-stu-id="c631b-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="c631b-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c631b-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identity/b2xUserFlow
```

## <a name="request-headers"></a><span data-ttu-id="c631b-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="c631b-121">Request headers</span></span>

|<span data-ttu-id="c631b-122">名称</span><span class="sxs-lookup"><span data-stu-id="c631b-122">Name</span></span>|<span data-ttu-id="c631b-123">说明</span><span class="sxs-lookup"><span data-stu-id="c631b-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="c631b-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="c631b-124">Authorization</span></span>|<span data-ttu-id="c631b-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c631b-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="c631b-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c631b-127">Content-Type</span></span>|<span data-ttu-id="c631b-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="c631b-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c631b-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="c631b-130">Request body</span></span>

<span data-ttu-id="c631b-131">在请求正文中，提供 [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md)的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c631b-131">In the request body, provide a JSON representation of a [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md).</span></span>

|<span data-ttu-id="c631b-132">属性</span><span class="sxs-lookup"><span data-stu-id="c631b-132">Property</span></span>|<span data-ttu-id="c631b-133">类型</span><span class="sxs-lookup"><span data-stu-id="c631b-133">Type</span></span>|<span data-ttu-id="c631b-134">说明</span><span class="sxs-lookup"><span data-stu-id="c631b-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c631b-135">id</span><span class="sxs-lookup"><span data-stu-id="c631b-135">id</span></span>|<span data-ttu-id="c631b-136">String</span><span class="sxs-lookup"><span data-stu-id="c631b-136">String</span></span>|<span data-ttu-id="c631b-137">必需。</span><span class="sxs-lookup"><span data-stu-id="c631b-137">Required.</span></span> <span data-ttu-id="c631b-138">用户流名称。</span><span class="sxs-lookup"><span data-stu-id="c631b-138">The name of the user flow.</span></span> <span data-ttu-id="c631b-139">该名称将在创建后进行 `B2X_1` 预笔写。</span><span class="sxs-lookup"><span data-stu-id="c631b-139">The name will be pre-pended with `B2X_1` after creation.</span></span>|
|<span data-ttu-id="c631b-140">userFlowType</span><span class="sxs-lookup"><span data-stu-id="c631b-140">userFlowType</span></span>|<span data-ttu-id="c631b-141">String</span><span class="sxs-lookup"><span data-stu-id="c631b-141">String</span></span>|<span data-ttu-id="c631b-142">必需。</span><span class="sxs-lookup"><span data-stu-id="c631b-142">Required.</span></span> <span data-ttu-id="c631b-143">要创建的用户流的类型。</span><span class="sxs-lookup"><span data-stu-id="c631b-143">The type of user flow you are creating.</span></span> <span data-ttu-id="c631b-144">此值将始终为 `signUpOrSignIn` 。</span><span class="sxs-lookup"><span data-stu-id="c631b-144">This value will always be `signUpOrSignIn`.</span></span>|
|<span data-ttu-id="c631b-145">userFlowTypeVersion</span><span class="sxs-lookup"><span data-stu-id="c631b-145">userFlowTypeVersion</span></span>|<span data-ttu-id="c631b-146">浮点</span><span class="sxs-lookup"><span data-stu-id="c631b-146">Float</span></span>|<span data-ttu-id="c631b-147">必需。</span><span class="sxs-lookup"><span data-stu-id="c631b-147">Required.</span></span> <span data-ttu-id="c631b-148">用户流版本。</span><span class="sxs-lookup"><span data-stu-id="c631b-148">The version of the user flow.</span></span> <span data-ttu-id="c631b-149">此值将始终为 1。</span><span class="sxs-lookup"><span data-stu-id="c631b-149">This value will always be 1.</span></span>|
|<span data-ttu-id="c631b-150">identityProviders</span><span class="sxs-lookup"><span data-stu-id="c631b-150">identityProviders</span></span>|<span data-ttu-id="c631b-151">[identityProvider](../resources/identityprovider.md)集合 </span><span class="sxs-lookup"><span data-stu-id="c631b-151">[identityProvider](../resources/identityprovider.md) collection</span></span>|<span data-ttu-id="c631b-152">可选。</span><span class="sxs-lookup"><span data-stu-id="c631b-152">Optional.</span></span> <span data-ttu-id="c631b-153">要包括在用户流中的标识提供程序。</span><span class="sxs-lookup"><span data-stu-id="c631b-153">The identity providers you want to include in the user flow.</span></span>|
|<span data-ttu-id="c631b-154">apiConnectorConfiguration</span><span class="sxs-lookup"><span data-stu-id="c631b-154">apiConnectorConfiguration</span></span>|[<span data-ttu-id="c631b-155">userFlowApiConnectorConfiguration</span><span class="sxs-lookup"><span data-stu-id="c631b-155">userFlowApiConnectorConfiguration</span></span>](../resources/userflowapiconnectorconfiguration.md)|<span data-ttu-id="c631b-156">可选。</span><span class="sxs-lookup"><span data-stu-id="c631b-156">Optional.</span></span> <span data-ttu-id="c631b-157">用于启用 API 连接器的配置，以便其可以成为用户流的一部分。</span><span class="sxs-lookup"><span data-stu-id="c631b-157">Configuration for enabling an API connector for use as part of the user flow.</span></span>|

## <a name="response"></a><span data-ttu-id="c631b-158">响应</span><span class="sxs-lookup"><span data-stu-id="c631b-158">Response</span></span>

<span data-ttu-id="c631b-159">如果成功，此方法将响应代码和位置标头与 URI 返回到为此请求创建的 `201 Created` [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) 对象，并添加前缀 `B2X_1` 的名称。</span><span class="sxs-lookup"><span data-stu-id="c631b-159">If successful, this method returns a `201 Created` response code and a Location header with a URI to the [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) object created for this request, with the `B2X_1` prefix added to the name.</span></span> <span data-ttu-id="c631b-160">如果失败，将返回 `4xx` 错误并显示具体详细信息。</span><span class="sxs-lookup"><span data-stu-id="c631b-160">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="examples"></a><span data-ttu-id="c631b-161">示例</span><span class="sxs-lookup"><span data-stu-id="c631b-161">Examples</span></span>

### <a name="example-1-create-a-user-flow-with-the-default-values"></a><span data-ttu-id="c631b-162">示例 1：使用默认值创建用户流</span><span class="sxs-lookup"><span data-stu-id="c631b-162">Example 1: Create a user flow with the default values</span></span>

#### <a name="request"></a><span data-ttu-id="c631b-163">请求</span><span class="sxs-lookup"><span data-stu-id="c631b-163">Request</span></span>

<span data-ttu-id="c631b-164">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c631b-164">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="c631b-165">HTTP</span><span class="sxs-lookup"><span data-stu-id="c631b-165">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_b2xuserflow_from_b2xuserflows"
}
-->

``` http
POST https://graph.microsoft.com/beta/identity/b2xUserFlows
Content-type: application/json
Content-length: 154

{
    "id": "Partner",
    "userFlowType": "signUpOrSignIn",
    "userFlowTypeVersion": 1
}
```
# <a name="c"></a>[<span data-ttu-id="c631b-166">C#</span><span class="sxs-lookup"><span data-stu-id="c631b-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-b2xuserflow-from-b2xuserflows-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c631b-167">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c631b-167">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-b2xuserflow-from-b2xuserflows-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c631b-168">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c631b-168">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-b2xuserflow-from-b2xuserflows-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c631b-169">Java</span><span class="sxs-lookup"><span data-stu-id="c631b-169">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-b2xuserflow-from-b2xuserflows-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c631b-170">响应</span><span class="sxs-lookup"><span data-stu-id="c631b-170">Response</span></span>

<span data-ttu-id="c631b-171">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="c631b-171">The following is an example of the response.</span></span>

<span data-ttu-id="c631b-172">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="c631b-172">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.b2xIdentityUserFlow"
} -->

```http
HTTP/1.1 201 Created
Location: https://graph.microsoft.com/beta/identity/b2xUserFlows/B2X_1_Partner
Content-type: application/json

{
    "id": "B2X_1_Partner",
    "userFlowType": "signUpOrSignIn",
    "userFlowTypeVersion": 1
}
```

### <a name="example-2-create-a-user-flow-with-the-default-values-and-an-identity-provider"></a><span data-ttu-id="c631b-173">示例 2：使用默认值和标识提供程序创建用户流</span><span class="sxs-lookup"><span data-stu-id="c631b-173">Example 2: Create a user flow with the default values and an identity provider</span></span>

#### <a name="request"></a><span data-ttu-id="c631b-174">请求</span><span class="sxs-lookup"><span data-stu-id="c631b-174">Request</span></span>

<span data-ttu-id="c631b-175">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c631b-175">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="c631b-176">HTTP</span><span class="sxs-lookup"><span data-stu-id="c631b-176">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_b2xuserflow_from_b2xuserflows_identityProviders"
}
-->

``` http
POST https://graph.microsoft.com/beta/identity/b2xUserFlows
Content-type: application/json
Content-length: 154

{
    "id": "Partner",
    "userFlowType": "signUpOrSignIn",
    "userFlowTypeVersion": 1,
    "identityProviders": [
        {
            "id": "Facebook-OAuth",
            "type": "Facebook",
            "name": "Facebook"
        }
    ]
}
```
# <a name="c"></a>[<span data-ttu-id="c631b-177">C#</span><span class="sxs-lookup"><span data-stu-id="c631b-177">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-b2xuserflow-from-b2xuserflows-identityproviders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c631b-178">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c631b-178">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-b2xuserflow-from-b2xuserflows-identityproviders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c631b-179">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c631b-179">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-b2xuserflow-from-b2xuserflows-identityproviders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c631b-180">Java</span><span class="sxs-lookup"><span data-stu-id="c631b-180">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-b2xuserflow-from-b2xuserflows-identityproviders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c631b-181">响应</span><span class="sxs-lookup"><span data-stu-id="c631b-181">Response</span></span>

<span data-ttu-id="c631b-182">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="c631b-182">The following is an example of the response.</span></span>

<span data-ttu-id="c631b-183">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="c631b-183">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.b2xIdentityUserFlow"
} -->

```http
HTTP/1.1 201 Created
Location: https://graph.microsoft.com/beta/identity/b2xUserFlows/B2X_1_Partner
Content-type: application/json

{
    "id": "B2X_1_Partner",
    "userFlowType": "signUpOrSignIn",
    "userFlowTypeVersion": 1
}
```

### <a name="example-3-create-a-user-flow-with-the-default-values-and-configuration-for-api-connectors"></a><span data-ttu-id="c631b-184">示例 3：使用 API 连接器的默认值和配置创建用户流</span><span class="sxs-lookup"><span data-stu-id="c631b-184">Example 3: Create a user flow with the default values and configuration for API connectors</span></span>

#### <a name="request"></a><span data-ttu-id="c631b-185">请求</span><span class="sxs-lookup"><span data-stu-id="c631b-185">Request</span></span>

<span data-ttu-id="c631b-186">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c631b-186">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="c631b-187">HTTP</span><span class="sxs-lookup"><span data-stu-id="c631b-187">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_b2xuserflow_from_b2xuserflows_apiconnectors"
}
-->

``` http
POST https://graph.microsoft.com/beta/identity/b2xUserFlows
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
# <a name="c"></a>[<span data-ttu-id="c631b-188">C#</span><span class="sxs-lookup"><span data-stu-id="c631b-188">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-b2xuserflow-from-b2xuserflows-apiconnectors-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c631b-189">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c631b-189">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-b2xuserflow-from-b2xuserflows-apiconnectors-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c631b-190">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c631b-190">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-b2xuserflow-from-b2xuserflows-apiconnectors-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c631b-191">Java</span><span class="sxs-lookup"><span data-stu-id="c631b-191">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-b2xuserflow-from-b2xuserflows-apiconnectors-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c631b-192">响应</span><span class="sxs-lookup"><span data-stu-id="c631b-192">Response</span></span>

<span data-ttu-id="c631b-193">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="c631b-193">The following is an example of the response.</span></span>

<span data-ttu-id="c631b-194">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="c631b-194">**Note:** The response object shown here might be shortened for readability.</span></span>

<span data-ttu-id="c631b-195">**注意：** 该属性 `apiConnectorConfiguration` 始终返回' {} 值。</span><span class="sxs-lookup"><span data-stu-id="c631b-195">**Note:** The `apiConnectorConfiguration` property always returns a '{}' value.</span></span> <span data-ttu-id="c631b-196">若要查看导航属性的完整值，请使用 [此](../api/b2xidentityuserflow-get-apiConnectorConfiguration.md) API。</span><span class="sxs-lookup"><span data-stu-id="c631b-196">To see full value with the navigation properties, use [this](../api/b2xidentityuserflow-get-apiConnectorConfiguration.md) API.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.b2xIdentityUserFlow"
} -->

```http
HTTP/1.1 201 Created
Location: https://graph.microsoft.com/beta/identity/b2xUserFlows/B2X_1_Partner
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identity/b2xUserFlows/$entity",
    "id": "B2X_1_UserFlowWithAPIConnector",
    "userFlowType": "signUpOrSignIn",
    "userFlowTypeVersion": 1,
    "apiConnectorConfiguration": {}
}
```

<!-- {
  "type": "#page.annotation",
  "description": "Create b2xUserFlow",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: create_b2xUserFlow_from_b2xUserFlows/userFlowTypeVersion:\r\n      Expected type Single but actual was Int64. Property: userFlowTypeVersion, actual value: '1'",
    "Error: create_b2xUserFlow_from_b2xUserFlows_identityProviders/userFlowTypeVersion:\r\n    Expected type Single but actual was Int64. Property: userFlowTypeVersion, actual value: '1'",
    "Error: create_b2xUserFlow_from_b2xuserflows_apiconnectors/userFlowTypeVersion:\r\n      Expected type Single but actual was Int64. Property: userFlowTypeVersion, actual value: '1'"
  ]
}-->

---
title: 创建 b2xIdentityUserFlow
description: 创建新的 b2xIdentityUserFlow 对象。
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: identity-and-sign-in
ms.openlocfilehash: 3711f7e607085096d28125cad94b86ea796b5044
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/21/2021
ms.locfileid: "51920280"
---
# <a name="create-b2xidentityuserflow"></a><span data-ttu-id="5a274-103">创建 b2xIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="5a274-103">Create b2xIdentityUserFlow</span></span>

<span data-ttu-id="5a274-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5a274-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5a274-105">创建新的 [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5a274-105">Create a new [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="5a274-106">权限</span><span class="sxs-lookup"><span data-stu-id="5a274-106">Permissions</span></span>

<span data-ttu-id="5a274-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5a274-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5a274-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="5a274-109">Permission type</span></span>      | <span data-ttu-id="5a274-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5a274-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5a274-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5a274-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5a274-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5a274-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="5a274-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5a274-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="5a274-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="5a274-114">Not supported.</span></span>|
|<span data-ttu-id="5a274-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="5a274-115">Application</span></span>|<span data-ttu-id="5a274-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5a274-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="5a274-117">工作或学校帐户需要属于以下角色之一：</span><span class="sxs-lookup"><span data-stu-id="5a274-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="5a274-118">全局管理员</span><span class="sxs-lookup"><span data-stu-id="5a274-118">Global administrator</span></span>
* <span data-ttu-id="5a274-119">外部标识用户流管理员</span><span class="sxs-lookup"><span data-stu-id="5a274-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="5a274-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5a274-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identity/b2xUserFlows
```

## <a name="request-headers"></a><span data-ttu-id="5a274-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="5a274-121">Request headers</span></span>

|<span data-ttu-id="5a274-122">名称</span><span class="sxs-lookup"><span data-stu-id="5a274-122">Name</span></span>|<span data-ttu-id="5a274-123">说明</span><span class="sxs-lookup"><span data-stu-id="5a274-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="5a274-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="5a274-124">Authorization</span></span>|<span data-ttu-id="5a274-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5a274-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="5a274-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5a274-127">Content-Type</span></span>|<span data-ttu-id="5a274-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="5a274-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5a274-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="5a274-130">Request body</span></span>

<span data-ttu-id="5a274-131">在请求正文中，提供 [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md)的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5a274-131">In the request body, provide a JSON representation of a [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md).</span></span>

|<span data-ttu-id="5a274-132">属性</span><span class="sxs-lookup"><span data-stu-id="5a274-132">Property</span></span>|<span data-ttu-id="5a274-133">类型</span><span class="sxs-lookup"><span data-stu-id="5a274-133">Type</span></span>|<span data-ttu-id="5a274-134">说明</span><span class="sxs-lookup"><span data-stu-id="5a274-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5a274-135">id</span><span class="sxs-lookup"><span data-stu-id="5a274-135">id</span></span>|<span data-ttu-id="5a274-136">String</span><span class="sxs-lookup"><span data-stu-id="5a274-136">String</span></span>|<span data-ttu-id="5a274-137">必填。</span><span class="sxs-lookup"><span data-stu-id="5a274-137">Required.</span></span> <span data-ttu-id="5a274-138">用户流名称。</span><span class="sxs-lookup"><span data-stu-id="5a274-138">The name of the user flow.</span></span> <span data-ttu-id="5a274-139">该名称将在创建后进行 `B2X_1` 预笔式处理。</span><span class="sxs-lookup"><span data-stu-id="5a274-139">The name will be pre-pended with `B2X_1` after creation.</span></span>|
|<span data-ttu-id="5a274-140">userFlowType</span><span class="sxs-lookup"><span data-stu-id="5a274-140">userFlowType</span></span>|<span data-ttu-id="5a274-141">String</span><span class="sxs-lookup"><span data-stu-id="5a274-141">String</span></span>|<span data-ttu-id="5a274-142">必填。</span><span class="sxs-lookup"><span data-stu-id="5a274-142">Required.</span></span> <span data-ttu-id="5a274-143">要创建的用户流的类型。</span><span class="sxs-lookup"><span data-stu-id="5a274-143">The type of user flow you are creating.</span></span> <span data-ttu-id="5a274-144">此值将始终为 `signUpOrSignIn` 。</span><span class="sxs-lookup"><span data-stu-id="5a274-144">This value will always be `signUpOrSignIn`.</span></span>|
|<span data-ttu-id="5a274-145">userFlowTypeVersion</span><span class="sxs-lookup"><span data-stu-id="5a274-145">userFlowTypeVersion</span></span>|<span data-ttu-id="5a274-146">浮点</span><span class="sxs-lookup"><span data-stu-id="5a274-146">Float</span></span>|<span data-ttu-id="5a274-147">必需。</span><span class="sxs-lookup"><span data-stu-id="5a274-147">Required.</span></span> <span data-ttu-id="5a274-148">用户流版本。</span><span class="sxs-lookup"><span data-stu-id="5a274-148">The version of the user flow.</span></span> <span data-ttu-id="5a274-149">此值将始终为 1。</span><span class="sxs-lookup"><span data-stu-id="5a274-149">This value will always be 1.</span></span>|
|<span data-ttu-id="5a274-150">apiConnectorConfiguration</span><span class="sxs-lookup"><span data-stu-id="5a274-150">apiConnectorConfiguration</span></span>|[<span data-ttu-id="5a274-151">userFlowApiConnectorConfiguration</span><span class="sxs-lookup"><span data-stu-id="5a274-151">userFlowApiConnectorConfiguration</span></span>](../resources/userflowapiconnectorconfiguration.md)|<span data-ttu-id="5a274-152">可选。</span><span class="sxs-lookup"><span data-stu-id="5a274-152">Optional.</span></span> <span data-ttu-id="5a274-153">用于启用 API 连接器的配置，以便其可以成为用户流的一部分。</span><span class="sxs-lookup"><span data-stu-id="5a274-153">Configuration for enabling an API connector for use as part of the user flow.</span></span>|

## <a name="response"></a><span data-ttu-id="5a274-154">响应</span><span class="sxs-lookup"><span data-stu-id="5a274-154">Response</span></span>

<span data-ttu-id="5a274-155">如果成功，此方法将返回响应代码和位置标头，其 URI 为为此请求创建的 `201 Created` [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) 对象，并添加前缀 `B2X_1` 到名称中。</span><span class="sxs-lookup"><span data-stu-id="5a274-155">If successful, this method returns a `201 Created` response code and a Location header with a URI to the [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) object created for this request, with the `B2X_1` prefix added to the name.</span></span> <span data-ttu-id="5a274-156">如果失败，将返回 `4xx` 错误并显示具体详细信息。</span><span class="sxs-lookup"><span data-stu-id="5a274-156">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="examples"></a><span data-ttu-id="5a274-157">示例</span><span class="sxs-lookup"><span data-stu-id="5a274-157">Examples</span></span>

### <a name="example-1-create-a-user-flow-with-the-default-values"></a><span data-ttu-id="5a274-158">示例 1：使用默认值创建用户流</span><span class="sxs-lookup"><span data-stu-id="5a274-158">Example 1: Create a user flow with the default values</span></span>

#### <a name="request"></a><span data-ttu-id="5a274-159">请求</span><span class="sxs-lookup"><span data-stu-id="5a274-159">Request</span></span>

<span data-ttu-id="5a274-160">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="5a274-160">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="5a274-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="5a274-161">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_b2xuserflow_from_b2xuserflows"
}
-->

``` http
POST https://graph.microsoft.com/v1.0/identity/b2xUserFlows
Content-type: application/json
Content-length: 154

{
    "id": "Partner",
    "userFlowType": "signUpOrSignIn",
    "userFlowTypeVersion": 1
}
```
# <a name="c"></a>[<span data-ttu-id="5a274-162">C#</span><span class="sxs-lookup"><span data-stu-id="5a274-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-b2xuserflow-from-b2xuserflows-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5a274-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5a274-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-b2xuserflow-from-b2xuserflows-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5a274-164">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5a274-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-b2xuserflow-from-b2xuserflows-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5a274-165">Java</span><span class="sxs-lookup"><span data-stu-id="5a274-165">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-b2xuserflow-from-b2xuserflows-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="5a274-166">响应</span><span class="sxs-lookup"><span data-stu-id="5a274-166">Response</span></span>

<span data-ttu-id="5a274-167">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="5a274-167">The following is an example of the response.</span></span>

<span data-ttu-id="5a274-168">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="5a274-168">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.b2xIdentityUserFlow"
} -->

```http
HTTP/1.1 201 Created
Location: https://graph.microsoft.com/v1.0/identity/b2xUserFlows/B2X_1_Partner
Content-type: application/json

{
    "id": "B2X_1_Partner",
    "userFlowType": "signUpOrSignIn",
    "userFlowTypeVersion": 1
}
```

### <a name="example-2-create-a-user-flow-with-the-default-values-and-an-identity-provider"></a><span data-ttu-id="5a274-169">示例 2：使用默认值和标识提供程序创建用户流</span><span class="sxs-lookup"><span data-stu-id="5a274-169">Example 2: Create a user flow with the default values and an identity provider</span></span>

#### <a name="request"></a><span data-ttu-id="5a274-170">请求</span><span class="sxs-lookup"><span data-stu-id="5a274-170">Request</span></span>

<span data-ttu-id="5a274-171">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="5a274-171">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="5a274-172">HTTP</span><span class="sxs-lookup"><span data-stu-id="5a274-172">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_b2xuserflow_from_b2xuserflows_identityProviders"
}
-->

``` http
POST https://graph.microsoft.com/v1.0/identity/b2xUserFlows
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
# <a name="c"></a>[<span data-ttu-id="5a274-173">C#</span><span class="sxs-lookup"><span data-stu-id="5a274-173">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-b2xuserflow-from-b2xuserflows-identityproviders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5a274-174">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5a274-174">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-b2xuserflow-from-b2xuserflows-identityproviders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5a274-175">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5a274-175">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-b2xuserflow-from-b2xuserflows-identityproviders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5a274-176">Java</span><span class="sxs-lookup"><span data-stu-id="5a274-176">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-b2xuserflow-from-b2xuserflows-identityproviders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="5a274-177">响应</span><span class="sxs-lookup"><span data-stu-id="5a274-177">Response</span></span>

<span data-ttu-id="5a274-178">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="5a274-178">The following is an example of the response.</span></span>

<span data-ttu-id="5a274-179">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="5a274-179">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.b2xIdentityUserFlow"
} -->

```http
HTTP/1.1 201 Created
Location: https://graph.microsoft.com/v1.0/identity/b2xUserFlows/B2X_1_Partner
Content-type: application/json

{
    "id": "B2X_1_Partner",
    "userFlowType": "signUpOrSignIn",
    "userFlowTypeVersion": 1
}
```

### <a name="example-3-create-a-user-flow-with-the-default-values-and-configuration-for-api-connectors"></a><span data-ttu-id="5a274-180">示例 3：使用 API 连接器的默认值和配置创建用户流</span><span class="sxs-lookup"><span data-stu-id="5a274-180">Example 3: Create a user flow with the default values and configuration for API connectors</span></span>

#### <a name="request"></a><span data-ttu-id="5a274-181">请求</span><span class="sxs-lookup"><span data-stu-id="5a274-181">Request</span></span>

<span data-ttu-id="5a274-182">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="5a274-182">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="5a274-183">HTTP</span><span class="sxs-lookup"><span data-stu-id="5a274-183">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_b2xuserflow_from_b2xuserflows_apiconnectors"
}
-->

``` http
POST https://graph.microsoft.com/v1.0/identity/b2xUserFlows
Content-type: application/json
Content-length: 154

{
    "id": "UserFlowWithAPIConnector",
    "userFlowType": "signUpOrSignIn",
    "userFlowTypeVersion": 1,
    "apiConnectorConfiguration":{
        "postFederationSignup":{
            "@odata.id": "https://graph.microsoft.com/v1/identity/apiConnectors/{id}"
        },
        "postAttributeCollection":{
            "@odata.id": "https://graph.microsoft.com/v1/identity/apiConnectors/{id}"
        }
    }
}
```
# <a name="c"></a>[<span data-ttu-id="5a274-184">C#</span><span class="sxs-lookup"><span data-stu-id="5a274-184">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-b2xuserflow-from-b2xuserflows-apiconnectors-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5a274-185">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5a274-185">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-b2xuserflow-from-b2xuserflows-apiconnectors-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5a274-186">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5a274-186">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-b2xuserflow-from-b2xuserflows-apiconnectors-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5a274-187">Java</span><span class="sxs-lookup"><span data-stu-id="5a274-187">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-b2xuserflow-from-b2xuserflows-apiconnectors-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="5a274-188">响应</span><span class="sxs-lookup"><span data-stu-id="5a274-188">Response</span></span>

<span data-ttu-id="5a274-189">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="5a274-189">The following is an example of the response.</span></span>

<span data-ttu-id="5a274-190">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="5a274-190">**Note:** The response object shown here might be shortened for readability.</span></span>

<span data-ttu-id="5a274-191">**注意：** 属性 `apiConnectorConfiguration` 始终返回 ' {} ' 值。</span><span class="sxs-lookup"><span data-stu-id="5a274-191">**Note:** The `apiConnectorConfiguration` property always returns a '{}' value.</span></span> <span data-ttu-id="5a274-192">若要使用导航属性查看完整值，请使用 [此](../api/b2xidentityuserflow-get-apiConnectorConfiguration.md) API。</span><span class="sxs-lookup"><span data-stu-id="5a274-192">To see full value with the navigation properties, use [this](../api/b2xidentityuserflow-get-apiConnectorConfiguration.md) API.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.b2xIdentityUserFlow"
} -->

```http
HTTP/1.1 201 Created
Location: https://graph.microsoft.com/v1.0/identity/b2xUserFlows/B2X_1_Partner
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identity/b2xUserFlows/$entity",
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

---
title: 创建 b2xIdentityUserFlow
description: 创建新的 b2xIdentityUserFlow 对象。
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: identity-and-sign-in
ms.openlocfilehash: b5f5d702a7707e942db6bbd6dd85eca02e26eb49
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882974"
---
# <a name="create-b2xidentityuserflow"></a><span data-ttu-id="8dac7-103">创建 b2xIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="8dac7-103">Create b2xIdentityUserFlow</span></span>

<span data-ttu-id="8dac7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8dac7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8dac7-105">创建新的 [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8dac7-105">Create a new [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="8dac7-106">权限</span><span class="sxs-lookup"><span data-stu-id="8dac7-106">Permissions</span></span>

<span data-ttu-id="8dac7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8dac7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8dac7-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="8dac7-109">Permission type</span></span>      | <span data-ttu-id="8dac7-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8dac7-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8dac7-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8dac7-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8dac7-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8dac7-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="8dac7-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8dac7-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="8dac7-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="8dac7-114">Not supported.</span></span>|
|<span data-ttu-id="8dac7-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="8dac7-115">Application</span></span>|<span data-ttu-id="8dac7-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8dac7-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="8dac7-117">工作或学校帐户需要属于以下角色之一：</span><span class="sxs-lookup"><span data-stu-id="8dac7-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="8dac7-118">全局管理员</span><span class="sxs-lookup"><span data-stu-id="8dac7-118">Global administrator</span></span>
* <span data-ttu-id="8dac7-119">外部标识用户流管理员</span><span class="sxs-lookup"><span data-stu-id="8dac7-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="8dac7-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8dac7-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identity/b2xUserFlows
```

## <a name="request-headers"></a><span data-ttu-id="8dac7-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="8dac7-121">Request headers</span></span>

|<span data-ttu-id="8dac7-122">名称</span><span class="sxs-lookup"><span data-stu-id="8dac7-122">Name</span></span>|<span data-ttu-id="8dac7-123">说明</span><span class="sxs-lookup"><span data-stu-id="8dac7-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="8dac7-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="8dac7-124">Authorization</span></span>|<span data-ttu-id="8dac7-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8dac7-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="8dac7-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8dac7-127">Content-Type</span></span>|<span data-ttu-id="8dac7-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="8dac7-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8dac7-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="8dac7-130">Request body</span></span>

<span data-ttu-id="8dac7-131">在请求正文中，提供 [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md)的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8dac7-131">In the request body, provide a JSON representation of a [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md).</span></span>

|<span data-ttu-id="8dac7-132">属性</span><span class="sxs-lookup"><span data-stu-id="8dac7-132">Property</span></span>|<span data-ttu-id="8dac7-133">类型</span><span class="sxs-lookup"><span data-stu-id="8dac7-133">Type</span></span>|<span data-ttu-id="8dac7-134">说明</span><span class="sxs-lookup"><span data-stu-id="8dac7-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8dac7-135">id</span><span class="sxs-lookup"><span data-stu-id="8dac7-135">id</span></span>|<span data-ttu-id="8dac7-136">String</span><span class="sxs-lookup"><span data-stu-id="8dac7-136">String</span></span>|<span data-ttu-id="8dac7-137">必填。</span><span class="sxs-lookup"><span data-stu-id="8dac7-137">Required.</span></span> <span data-ttu-id="8dac7-138">用户流名称。</span><span class="sxs-lookup"><span data-stu-id="8dac7-138">The name of the user flow.</span></span> <span data-ttu-id="8dac7-139">该名称将在创建后进行 `B2X_1` 预笔式处理。</span><span class="sxs-lookup"><span data-stu-id="8dac7-139">The name will be pre-pended with `B2X_1` after creation.</span></span>|
|<span data-ttu-id="8dac7-140">userFlowType</span><span class="sxs-lookup"><span data-stu-id="8dac7-140">userFlowType</span></span>|<span data-ttu-id="8dac7-141">String</span><span class="sxs-lookup"><span data-stu-id="8dac7-141">String</span></span>|<span data-ttu-id="8dac7-142">必填。</span><span class="sxs-lookup"><span data-stu-id="8dac7-142">Required.</span></span> <span data-ttu-id="8dac7-143">要创建的用户流的类型。</span><span class="sxs-lookup"><span data-stu-id="8dac7-143">The type of user flow you are creating.</span></span> <span data-ttu-id="8dac7-144">此值将始终为 `signUpOrSignIn` 。</span><span class="sxs-lookup"><span data-stu-id="8dac7-144">This value will always be `signUpOrSignIn`.</span></span>|
|<span data-ttu-id="8dac7-145">userFlowTypeVersion</span><span class="sxs-lookup"><span data-stu-id="8dac7-145">userFlowTypeVersion</span></span>|<span data-ttu-id="8dac7-146">浮点</span><span class="sxs-lookup"><span data-stu-id="8dac7-146">Float</span></span>|<span data-ttu-id="8dac7-147">必填。</span><span class="sxs-lookup"><span data-stu-id="8dac7-147">Required.</span></span> <span data-ttu-id="8dac7-148">用户流版本。</span><span class="sxs-lookup"><span data-stu-id="8dac7-148">The version of the user flow.</span></span> <span data-ttu-id="8dac7-149">此值将始终为 1。</span><span class="sxs-lookup"><span data-stu-id="8dac7-149">This value will always be 1.</span></span>|
|<span data-ttu-id="8dac7-150">apiConnectorConfiguration</span><span class="sxs-lookup"><span data-stu-id="8dac7-150">apiConnectorConfiguration</span></span>|[<span data-ttu-id="8dac7-151">userFlowApiConnectorConfiguration</span><span class="sxs-lookup"><span data-stu-id="8dac7-151">userFlowApiConnectorConfiguration</span></span>](../resources/userflowapiconnectorconfiguration.md)|<span data-ttu-id="8dac7-152">可选。</span><span class="sxs-lookup"><span data-stu-id="8dac7-152">Optional.</span></span> <span data-ttu-id="8dac7-153">用于启用 API 连接器的配置，以便其可以成为用户流的一部分。</span><span class="sxs-lookup"><span data-stu-id="8dac7-153">Configuration for enabling an API connector for use as part of the user flow.</span></span>|

## <a name="response"></a><span data-ttu-id="8dac7-154">响应</span><span class="sxs-lookup"><span data-stu-id="8dac7-154">Response</span></span>

<span data-ttu-id="8dac7-155">如果成功，此方法将返回响应代码和位置标头，其 URI 为为此请求创建的 `201 Created` [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) 对象，并添加前缀 `B2X_1` 到名称中。</span><span class="sxs-lookup"><span data-stu-id="8dac7-155">If successful, this method returns a `201 Created` response code and a Location header with a URI to the [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) object created for this request, with the `B2X_1` prefix added to the name.</span></span> <span data-ttu-id="8dac7-156">如果失败，将返回 `4xx` 错误并显示具体详细信息。</span><span class="sxs-lookup"><span data-stu-id="8dac7-156">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="examples"></a><span data-ttu-id="8dac7-157">示例</span><span class="sxs-lookup"><span data-stu-id="8dac7-157">Examples</span></span>

### <a name="example-1-create-a-user-flow-with-the-default-values"></a><span data-ttu-id="8dac7-158">示例 1：使用默认值创建用户流</span><span class="sxs-lookup"><span data-stu-id="8dac7-158">Example 1: Create a user flow with the default values</span></span>

#### <a name="request"></a><span data-ttu-id="8dac7-159">请求</span><span class="sxs-lookup"><span data-stu-id="8dac7-159">Request</span></span>

<span data-ttu-id="8dac7-160">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="8dac7-160">The following is an example of the request.</span></span>

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

#### <a name="response"></a><span data-ttu-id="8dac7-161">响应</span><span class="sxs-lookup"><span data-stu-id="8dac7-161">Response</span></span>

<span data-ttu-id="8dac7-162">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="8dac7-162">The following is an example of the response.</span></span>

<span data-ttu-id="8dac7-163">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="8dac7-163">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-2-create-a-user-flow-with-the-default-values-and-an-identity-provider"></a><span data-ttu-id="8dac7-164">示例 2：使用默认值和标识提供程序创建用户流</span><span class="sxs-lookup"><span data-stu-id="8dac7-164">Example 2: Create a user flow with the default values and an identity provider</span></span>

#### <a name="request"></a><span data-ttu-id="8dac7-165">请求</span><span class="sxs-lookup"><span data-stu-id="8dac7-165">Request</span></span>

<span data-ttu-id="8dac7-166">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="8dac7-166">The following is an example of the request.</span></span>

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

#### <a name="response"></a><span data-ttu-id="8dac7-167">响应</span><span class="sxs-lookup"><span data-stu-id="8dac7-167">Response</span></span>

<span data-ttu-id="8dac7-168">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="8dac7-168">The following is an example of the response.</span></span>

<span data-ttu-id="8dac7-169">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="8dac7-169">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-3-create-a-user-flow-with-the-default-values-and-configuration-for-api-connectors"></a><span data-ttu-id="8dac7-170">示例 3：使用 API 连接器的默认值和配置创建用户流</span><span class="sxs-lookup"><span data-stu-id="8dac7-170">Example 3: Create a user flow with the default values and configuration for API connectors</span></span>

#### <a name="request"></a><span data-ttu-id="8dac7-171">请求</span><span class="sxs-lookup"><span data-stu-id="8dac7-171">Request</span></span>

<span data-ttu-id="8dac7-172">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="8dac7-172">The following is an example of the request.</span></span>

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

#### <a name="response"></a><span data-ttu-id="8dac7-173">响应</span><span class="sxs-lookup"><span data-stu-id="8dac7-173">Response</span></span>

<span data-ttu-id="8dac7-174">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="8dac7-174">The following is an example of the response.</span></span>

<span data-ttu-id="8dac7-175">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="8dac7-175">**Note:** The response object shown here might be shortened for readability.</span></span>

<span data-ttu-id="8dac7-176">**注意：** 属性 `apiConnectorConfiguration` 始终返回 ' {} ' 值。</span><span class="sxs-lookup"><span data-stu-id="8dac7-176">**Note:** The `apiConnectorConfiguration` property always returns a '{}' value.</span></span> <span data-ttu-id="8dac7-177">若要使用导航属性查看完整值，请使用 [此](../api/b2xidentityuserflow-get-apiConnectorConfiguration.md) API。</span><span class="sxs-lookup"><span data-stu-id="8dac7-177">To see full value with the navigation properties, use [this](../api/b2xidentityuserflow-get-apiConnectorConfiguration.md) API.</span></span>

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

---
title: 创建 b2xIdentityUserFlow
description: 创建新的 b2xIdentityUserFlow 对象。
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: microsoft-identity-platform
ms.openlocfilehash: c178fef7450121574e15fb34245a8843fc120e97
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48953503"
---
# <a name="create-b2xidentityuserflow"></a><span data-ttu-id="9a1c9-103">创建 b2xIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="9a1c9-103">Create b2xIdentityUserFlow</span></span>

<span data-ttu-id="9a1c9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9a1c9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9a1c9-105">创建新的 [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9a1c9-105">Create a new [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="9a1c9-106">权限</span><span class="sxs-lookup"><span data-stu-id="9a1c9-106">Permissions</span></span>

<span data-ttu-id="9a1c9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9a1c9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9a1c9-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="9a1c9-109">Permission type</span></span>      | <span data-ttu-id="9a1c9-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9a1c9-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9a1c9-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9a1c9-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9a1c9-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a1c9-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="9a1c9-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9a1c9-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="9a1c9-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="9a1c9-114">Not supported.</span></span>|
|<span data-ttu-id="9a1c9-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="9a1c9-115">Application</span></span>|<span data-ttu-id="9a1c9-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a1c9-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="9a1c9-117">工作或学校帐户需要属于下列角色之一：</span><span class="sxs-lookup"><span data-stu-id="9a1c9-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="9a1c9-118">全局管理员</span><span class="sxs-lookup"><span data-stu-id="9a1c9-118">Global administrator</span></span>
* <span data-ttu-id="9a1c9-119">外部标识用户流管理员</span><span class="sxs-lookup"><span data-stu-id="9a1c9-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="9a1c9-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9a1c9-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identity/b2xUserFlow
```

## <a name="request-headers"></a><span data-ttu-id="9a1c9-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="9a1c9-121">Request headers</span></span>

|<span data-ttu-id="9a1c9-122">名称</span><span class="sxs-lookup"><span data-stu-id="9a1c9-122">Name</span></span>|<span data-ttu-id="9a1c9-123">说明</span><span class="sxs-lookup"><span data-stu-id="9a1c9-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="9a1c9-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="9a1c9-124">Authorization</span></span>|<span data-ttu-id="9a1c9-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9a1c9-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="9a1c9-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9a1c9-127">Content-Type</span></span>|<span data-ttu-id="9a1c9-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="9a1c9-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9a1c9-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="9a1c9-130">Request body</span></span>

<span data-ttu-id="9a1c9-131">在请求正文中，提供 [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md)的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9a1c9-131">In the request body, provide a JSON representation of a [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md).</span></span>

|<span data-ttu-id="9a1c9-132">属性</span><span class="sxs-lookup"><span data-stu-id="9a1c9-132">Property</span></span>|<span data-ttu-id="9a1c9-133">类型</span><span class="sxs-lookup"><span data-stu-id="9a1c9-133">Type</span></span>|<span data-ttu-id="9a1c9-134">说明</span><span class="sxs-lookup"><span data-stu-id="9a1c9-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9a1c9-135">id</span><span class="sxs-lookup"><span data-stu-id="9a1c9-135">id</span></span>|<span data-ttu-id="9a1c9-136">String</span><span class="sxs-lookup"><span data-stu-id="9a1c9-136">String</span></span>|<span data-ttu-id="9a1c9-137">必填。</span><span class="sxs-lookup"><span data-stu-id="9a1c9-137">Required.</span></span> <span data-ttu-id="9a1c9-138">用户流名称。</span><span class="sxs-lookup"><span data-stu-id="9a1c9-138">The name of the user flow.</span></span> <span data-ttu-id="9a1c9-139">创建后，名称将预先挂起 `B2X_1` 。</span><span class="sxs-lookup"><span data-stu-id="9a1c9-139">The name will be pre-pended with `B2X_1` after creation.</span></span>|
|<span data-ttu-id="9a1c9-140">userFlowType</span><span class="sxs-lookup"><span data-stu-id="9a1c9-140">userFlowType</span></span>|<span data-ttu-id="9a1c9-141">String</span><span class="sxs-lookup"><span data-stu-id="9a1c9-141">String</span></span>|<span data-ttu-id="9a1c9-142">必填。</span><span class="sxs-lookup"><span data-stu-id="9a1c9-142">Required.</span></span> <span data-ttu-id="9a1c9-143">您正在创建的用户流的类型。</span><span class="sxs-lookup"><span data-stu-id="9a1c9-143">The type of user flow you are creating.</span></span> <span data-ttu-id="9a1c9-144">此值将始终为 `signUpOrSignIn` 。</span><span class="sxs-lookup"><span data-stu-id="9a1c9-144">This value will always be `signUpOrSignIn`.</span></span>|
|<span data-ttu-id="9a1c9-145">userFlowTypeVersion</span><span class="sxs-lookup"><span data-stu-id="9a1c9-145">userFlowTypeVersion</span></span>|<span data-ttu-id="9a1c9-146">浮点</span><span class="sxs-lookup"><span data-stu-id="9a1c9-146">Float</span></span>|<span data-ttu-id="9a1c9-147">必填。</span><span class="sxs-lookup"><span data-stu-id="9a1c9-147">Required.</span></span> <span data-ttu-id="9a1c9-148">用户流版本。</span><span class="sxs-lookup"><span data-stu-id="9a1c9-148">The version of the user flow.</span></span> <span data-ttu-id="9a1c9-149">此值将始终为1。</span><span class="sxs-lookup"><span data-stu-id="9a1c9-149">This value will always be 1.</span></span>|
|<span data-ttu-id="9a1c9-150">identityProviders</span><span class="sxs-lookup"><span data-stu-id="9a1c9-150">identityProviders</span></span>|<span data-ttu-id="9a1c9-151">[identityProvider](../resources/identityprovider.md)集合 </span><span class="sxs-lookup"><span data-stu-id="9a1c9-151">[identityProvider](../resources/identityprovider.md) collection</span></span>|<span data-ttu-id="9a1c9-152">可选。</span><span class="sxs-lookup"><span data-stu-id="9a1c9-152">Optional.</span></span> <span data-ttu-id="9a1c9-153">要包括在用户流中的标识提供程序。</span><span class="sxs-lookup"><span data-stu-id="9a1c9-153">The identity providers you want to include in the user flow.</span></span>|

## <a name="response"></a><span data-ttu-id="9a1c9-154">响应</span><span class="sxs-lookup"><span data-stu-id="9a1c9-154">Response</span></span>

<span data-ttu-id="9a1c9-155">如果成功，此方法将向 `201 Created` 为此请求创建的 [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) 对象的 URI 返回响应代码和位置标头，并将 `B2X_1` 前缀添加到名称中。</span><span class="sxs-lookup"><span data-stu-id="9a1c9-155">If successful, this method returns a `201 Created` response code and a Location header with a URI to the [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) object created for this request, with the `B2X_1` prefix added to the name.</span></span> <span data-ttu-id="9a1c9-156">如果失败，将返回 `4xx` 错误并显示具体详细信息。</span><span class="sxs-lookup"><span data-stu-id="9a1c9-156">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="examples"></a><span data-ttu-id="9a1c9-157">示例</span><span class="sxs-lookup"><span data-stu-id="9a1c9-157">Examples</span></span>

### <a name="example-1-create-a-user-flow-with-the-default-values"></a><span data-ttu-id="9a1c9-158">示例1：创建具有默认值的用户流</span><span class="sxs-lookup"><span data-stu-id="9a1c9-158">Example 1: Create a user flow with the default values</span></span>

#### <a name="request"></a><span data-ttu-id="9a1c9-159">请求</span><span class="sxs-lookup"><span data-stu-id="9a1c9-159">Request</span></span>

<span data-ttu-id="9a1c9-160">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="9a1c9-160">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="9a1c9-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="9a1c9-161">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="9a1c9-162">C#</span><span class="sxs-lookup"><span data-stu-id="9a1c9-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-b2xuserflow-from-b2xuserflows-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9a1c9-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9a1c9-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-b2xuserflow-from-b2xuserflows-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9a1c9-164">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9a1c9-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-b2xuserflow-from-b2xuserflows-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9a1c9-165">Java</span><span class="sxs-lookup"><span data-stu-id="9a1c9-165">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-b2xuserflow-from-b2xuserflows-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9a1c9-166">响应</span><span class="sxs-lookup"><span data-stu-id="9a1c9-166">Response</span></span>

<span data-ttu-id="9a1c9-167">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="9a1c9-167">The following is an example of the response.</span></span>

<span data-ttu-id="9a1c9-168">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="9a1c9-168">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-2-create-a-user-flow-with-the-default-values-and-an-identity-provider"></a><span data-ttu-id="9a1c9-169">示例2：创建具有默认值和标识提供程序的用户流</span><span class="sxs-lookup"><span data-stu-id="9a1c9-169">Example 2: Create a user flow with the default values and an identity provider</span></span>

#### <a name="request"></a><span data-ttu-id="9a1c9-170">请求</span><span class="sxs-lookup"><span data-stu-id="9a1c9-170">Request</span></span>

<span data-ttu-id="9a1c9-171">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="9a1c9-171">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="9a1c9-172">HTTP</span><span class="sxs-lookup"><span data-stu-id="9a1c9-172">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="9a1c9-173">C#</span><span class="sxs-lookup"><span data-stu-id="9a1c9-173">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-b2xuserflow-from-b2xuserflows-identityproviders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9a1c9-174">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9a1c9-174">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-b2xuserflow-from-b2xuserflows-identityproviders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9a1c9-175">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9a1c9-175">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-b2xuserflow-from-b2xuserflows-identityproviders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9a1c9-176">Java</span><span class="sxs-lookup"><span data-stu-id="9a1c9-176">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-b2xuserflow-from-b2xuserflows-identityproviders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9a1c9-177">响应</span><span class="sxs-lookup"><span data-stu-id="9a1c9-177">Response</span></span>

<span data-ttu-id="9a1c9-178">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="9a1c9-178">The following is an example of the response.</span></span>

<span data-ttu-id="9a1c9-179">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="9a1c9-179">**Note:** The response object shown here might be shortened for readability.</span></span>

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

<!-- {
  "type": "#page.annotation",
  "description": "Create b2xUserFlow",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: create_b2xUserFlow_from_b2xUserFlows/userFlowTypeVersion:\r\n      Expected type Single but actual was Int64. Property: userFlowTypeVersion, actual value: '1'",
    "Error: create_b2xUserFlow_from_b2xUserFlows_identityProviders/userFlowTypeVersion:\r\n    Expected type Single but actual was Int64. Property: userFlowTypeVersion, actual value: '1'"
  ]
}-->



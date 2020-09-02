---
title: 创建 b2cUserFlow
description: 创建新的 b2cUserFlow 对象。
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 46a4c70329e021c89bf9107b877fcf9fae88b3ca
ms.sourcegitcommit: 726f20403323be7d267b67c2764ed7c244e02ee1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/02/2020
ms.locfileid: "47329971"
---
# <a name="create-b2cuserflow"></a><span data-ttu-id="62906-103">创建 b2cUserFlow</span><span class="sxs-lookup"><span data-stu-id="62906-103">Create b2cUserFlow</span></span>

<span data-ttu-id="62906-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="62906-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="62906-105">创建新的 [b2cUserFlow](../resources/b2cuserflows.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="62906-105">Create a new [b2cUserFlow](../resources/b2cuserflows.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="62906-106">权限</span><span class="sxs-lookup"><span data-stu-id="62906-106">Permissions</span></span>

<span data-ttu-id="62906-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="62906-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="62906-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="62906-109">Permission type</span></span>      | <span data-ttu-id="62906-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="62906-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="62906-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="62906-111">Delegated (work or school account)</span></span>|<span data-ttu-id="62906-112">IdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="62906-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="62906-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="62906-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="62906-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="62906-114">Not supported.</span></span>|
|<span data-ttu-id="62906-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="62906-115">Application</span></span>|<span data-ttu-id="62906-116">IdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="62906-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="62906-117">工作或学校帐户需要属于下列角色之一：</span><span class="sxs-lookup"><span data-stu-id="62906-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="62906-118">全局管理员</span><span class="sxs-lookup"><span data-stu-id="62906-118">Global administrator</span></span>
* <span data-ttu-id="62906-119">外部标识用户流管理员</span><span class="sxs-lookup"><span data-stu-id="62906-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="62906-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="62906-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identity/b2cUserFlows
```

## <a name="request-headers"></a><span data-ttu-id="62906-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="62906-121">Request headers</span></span>

|<span data-ttu-id="62906-122">名称</span><span class="sxs-lookup"><span data-stu-id="62906-122">Name</span></span>|<span data-ttu-id="62906-123">说明</span><span class="sxs-lookup"><span data-stu-id="62906-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="62906-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="62906-124">Authorization</span></span>|<span data-ttu-id="62906-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="62906-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="62906-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="62906-127">Content-Type</span></span>|<span data-ttu-id="62906-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="62906-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="62906-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="62906-130">Request body</span></span>

<span data-ttu-id="62906-131">在请求正文中，提供 [b2cUserFlow](../resources/b2cuserflows.md)的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="62906-131">In the request body, provide a JSON representation of a [b2cUserFlow](../resources/b2cuserflows.md).</span></span>

|<span data-ttu-id="62906-132">属性</span><span class="sxs-lookup"><span data-stu-id="62906-132">Property</span></span>|<span data-ttu-id="62906-133">类型</span><span class="sxs-lookup"><span data-stu-id="62906-133">Type</span></span>|<span data-ttu-id="62906-134">说明</span><span class="sxs-lookup"><span data-stu-id="62906-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="62906-135">id</span><span class="sxs-lookup"><span data-stu-id="62906-135">id</span></span>|<span data-ttu-id="62906-136">String</span><span class="sxs-lookup"><span data-stu-id="62906-136">String</span></span>|<span data-ttu-id="62906-137">必需。</span><span class="sxs-lookup"><span data-stu-id="62906-137">Required.</span></span> <span data-ttu-id="62906-138">用户流的名称。</span><span class="sxs-lookup"><span data-stu-id="62906-138">The name of the user flow.</span></span> <span data-ttu-id="62906-139">创建后，名称将预先挂起 `B2C_1` 。</span><span class="sxs-lookup"><span data-stu-id="62906-139">The name will be pre-pended with `B2C_1` after creation.</span></span>|
|<span data-ttu-id="62906-140">userFlowType</span><span class="sxs-lookup"><span data-stu-id="62906-140">userFlowType</span></span>|<span data-ttu-id="62906-141">String</span><span class="sxs-lookup"><span data-stu-id="62906-141">String</span></span>|<span data-ttu-id="62906-142">必需。</span><span class="sxs-lookup"><span data-stu-id="62906-142">Required.</span></span> <span data-ttu-id="62906-143">您正在创建的用户流的类型。</span><span class="sxs-lookup"><span data-stu-id="62906-143">The type of user flow you are creating.</span></span> <span data-ttu-id="62906-144">**UserFlowType**支持的值为：</span><span class="sxs-lookup"><span data-stu-id="62906-144">The supported values for **userFlowType** are:</span></span><br/><ul><li>`signUp`</li><li>`signIn`</li><li>`signUpOrSignIn`</li><li>`passwordReset`</li><li>`profileUpdate`</li><li>`resourceOwnerPasswordCredentialSignIn`</li>|
|<span data-ttu-id="62906-145">userFlowTypeVersion</span><span class="sxs-lookup"><span data-stu-id="62906-145">userFlowTypeVersion</span></span>|<span data-ttu-id="62906-146">浮点</span><span class="sxs-lookup"><span data-stu-id="62906-146">Float</span></span>|<span data-ttu-id="62906-147">必需。</span><span class="sxs-lookup"><span data-stu-id="62906-147">Required.</span></span> <span data-ttu-id="62906-148">用户流的版本。</span><span class="sxs-lookup"><span data-stu-id="62906-148">The version of the user flow.</span></span>|
|<span data-ttu-id="62906-149">identityProviders</span><span class="sxs-lookup"><span data-stu-id="62906-149">identityProviders</span></span>|<span data-ttu-id="62906-150">[identityprovider.read.all](../resources/identityprovider.md) 集合</span><span class="sxs-lookup"><span data-stu-id="62906-150">[identityProvider](../resources/identityprovider.md) collection</span></span>|<span data-ttu-id="62906-151">可选。</span><span class="sxs-lookup"><span data-stu-id="62906-151">Optional.</span></span> <span data-ttu-id="62906-152">要包括在用户流中的标识提供程序。</span><span class="sxs-lookup"><span data-stu-id="62906-152">The identity providers you want to include in the user flow.</span></span>|

## <a name="response"></a><span data-ttu-id="62906-153">响应</span><span class="sxs-lookup"><span data-stu-id="62906-153">Response</span></span>

<span data-ttu-id="62906-154">如果成功，此方法将向 `201 Created` 为此请求创建的 [b2cUserFlow](../resources/b2cuserflows.md) 对象的 URI 返回响应代码和位置标头，并将 `B2C_1` 前缀添加到名称中。</span><span class="sxs-lookup"><span data-stu-id="62906-154">If successful, this method returns a `201 Created` response code and a Location header with a URI to the [b2cUserFlow](../resources/b2cuserflows.md) object created for this request, with the `B2C_1` prefix added to the name.</span></span> <span data-ttu-id="62906-155">如果失败，将返回 `4xx` 错误并显示具体详细信息。</span><span class="sxs-lookup"><span data-stu-id="62906-155">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="examples"></a><span data-ttu-id="62906-156">示例</span><span class="sxs-lookup"><span data-stu-id="62906-156">Examples</span></span>

### <a name="example-1-create-a-user-flow-with-the-default-values"></a><span data-ttu-id="62906-157">示例1：创建具有默认值的用户流</span><span class="sxs-lookup"><span data-stu-id="62906-157">Example 1: Create a user flow with the default values</span></span>

#### <a name="request"></a><span data-ttu-id="62906-158">请求</span><span class="sxs-lookup"><span data-stu-id="62906-158">Request</span></span>

<span data-ttu-id="62906-159">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="62906-159">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="62906-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="62906-160">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="62906-161">C#</span><span class="sxs-lookup"><span data-stu-id="62906-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-b2cuserflow-from-b2cuserflows-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="62906-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="62906-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-b2cuserflow-from-b2cuserflows-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="62906-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="62906-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-b2cuserflow-from-b2cuserflows-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="62906-164">响应</span><span class="sxs-lookup"><span data-stu-id="62906-164">Response</span></span>

<span data-ttu-id="62906-165">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="62906-165">The following is an example of the response.</span></span>

<span data-ttu-id="62906-166">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="62906-166">**Note:** The response object shown here might be shortened for readability.</span></span>

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
    "userFlowTypeVersion": 3
}
```

### <a name="example-2-create-a-user-flow-with-the-default-values-and-an-identity-provider"></a><span data-ttu-id="62906-167">示例2：创建具有默认值和标识提供程序的用户流</span><span class="sxs-lookup"><span data-stu-id="62906-167">Example 2: Create a user flow with the default values and an identity provider</span></span>

#### <a name="request"></a><span data-ttu-id="62906-168">请求</span><span class="sxs-lookup"><span data-stu-id="62906-168">Request</span></span>

<span data-ttu-id="62906-169">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="62906-169">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="62906-170">HTTP</span><span class="sxs-lookup"><span data-stu-id="62906-170">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="62906-171">C#</span><span class="sxs-lookup"><span data-stu-id="62906-171">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-b2cuserflow-from-b2cuserflows-identityprovider-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="62906-172">JavaScript</span><span class="sxs-lookup"><span data-stu-id="62906-172">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-b2cuserflow-from-b2cuserflows-identityprovider-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="62906-173">Objective-C</span><span class="sxs-lookup"><span data-stu-id="62906-173">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-b2cuserflow-from-b2cuserflows-identityprovider-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="62906-174">响应</span><span class="sxs-lookup"><span data-stu-id="62906-174">Response</span></span>

<span data-ttu-id="62906-175">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="62906-175">The following is an example of the response.</span></span>

<span data-ttu-id="62906-176">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="62906-176">**Note:** The response object shown here might be shortened for readability.</span></span>

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
    "userFlowTypeVersion": 3
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

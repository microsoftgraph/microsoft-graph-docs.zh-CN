---
title: 创建 b2xIdentityUserFlow
description: 创建新的 b2xIdentityUserFlow 对象。
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 82fe1f9a825262deff595d636c5fbd899cc970b3
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/09/2020
ms.locfileid: "48406347"
---
# <a name="create-b2xidentityuserflow"></a><span data-ttu-id="0ee37-103">创建 b2xIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="0ee37-103">Create b2xIdentityUserFlow</span></span>

<span data-ttu-id="0ee37-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0ee37-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0ee37-105">创建新的 [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0ee37-105">Create a new [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="0ee37-106">权限</span><span class="sxs-lookup"><span data-stu-id="0ee37-106">Permissions</span></span>

<span data-ttu-id="0ee37-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0ee37-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0ee37-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="0ee37-109">Permission type</span></span>      | <span data-ttu-id="0ee37-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0ee37-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0ee37-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0ee37-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0ee37-112">IdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="0ee37-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="0ee37-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0ee37-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="0ee37-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="0ee37-114">Not supported.</span></span>|
|<span data-ttu-id="0ee37-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="0ee37-115">Application</span></span>|<span data-ttu-id="0ee37-116">IdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="0ee37-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="0ee37-117">工作或学校帐户需要属于下列角色之一：</span><span class="sxs-lookup"><span data-stu-id="0ee37-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="0ee37-118">全局管理员</span><span class="sxs-lookup"><span data-stu-id="0ee37-118">Global administrator</span></span>
* <span data-ttu-id="0ee37-119">外部标识用户流管理员</span><span class="sxs-lookup"><span data-stu-id="0ee37-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="0ee37-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0ee37-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identity/b2xUserFlow
```

## <a name="request-headers"></a><span data-ttu-id="0ee37-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="0ee37-121">Request headers</span></span>

|<span data-ttu-id="0ee37-122">名称</span><span class="sxs-lookup"><span data-stu-id="0ee37-122">Name</span></span>|<span data-ttu-id="0ee37-123">说明</span><span class="sxs-lookup"><span data-stu-id="0ee37-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="0ee37-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="0ee37-124">Authorization</span></span>|<span data-ttu-id="0ee37-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0ee37-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="0ee37-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0ee37-127">Content-Type</span></span>|<span data-ttu-id="0ee37-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="0ee37-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0ee37-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="0ee37-130">Request body</span></span>

<span data-ttu-id="0ee37-131">在请求正文中，提供 [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md)的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0ee37-131">In the request body, provide a JSON representation of a [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md).</span></span>

|<span data-ttu-id="0ee37-132">属性</span><span class="sxs-lookup"><span data-stu-id="0ee37-132">Property</span></span>|<span data-ttu-id="0ee37-133">类型</span><span class="sxs-lookup"><span data-stu-id="0ee37-133">Type</span></span>|<span data-ttu-id="0ee37-134">说明</span><span class="sxs-lookup"><span data-stu-id="0ee37-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0ee37-135">id</span><span class="sxs-lookup"><span data-stu-id="0ee37-135">id</span></span>|<span data-ttu-id="0ee37-136">String</span><span class="sxs-lookup"><span data-stu-id="0ee37-136">String</span></span>|<span data-ttu-id="0ee37-137">必需。</span><span class="sxs-lookup"><span data-stu-id="0ee37-137">Required.</span></span> <span data-ttu-id="0ee37-138">用户流名称。</span><span class="sxs-lookup"><span data-stu-id="0ee37-138">The name of the user flow.</span></span> <span data-ttu-id="0ee37-139">创建后，名称将预先挂起 `B2X_1` 。</span><span class="sxs-lookup"><span data-stu-id="0ee37-139">The name will be pre-pended with `B2X_1` after creation.</span></span>|
|<span data-ttu-id="0ee37-140">userFlowType</span><span class="sxs-lookup"><span data-stu-id="0ee37-140">userFlowType</span></span>|<span data-ttu-id="0ee37-141">字符串</span><span class="sxs-lookup"><span data-stu-id="0ee37-141">String</span></span>|<span data-ttu-id="0ee37-142">必需。</span><span class="sxs-lookup"><span data-stu-id="0ee37-142">Required.</span></span> <span data-ttu-id="0ee37-143">您正在创建的用户流的类型。</span><span class="sxs-lookup"><span data-stu-id="0ee37-143">The type of user flow you are creating.</span></span> <span data-ttu-id="0ee37-144">此值将始终为 `signUpOrSignIn` 。</span><span class="sxs-lookup"><span data-stu-id="0ee37-144">This value will always be `signUpOrSignIn`.</span></span>|
|<span data-ttu-id="0ee37-145">userFlowTypeVersion</span><span class="sxs-lookup"><span data-stu-id="0ee37-145">userFlowTypeVersion</span></span>|<span data-ttu-id="0ee37-146">浮点</span><span class="sxs-lookup"><span data-stu-id="0ee37-146">Float</span></span>|<span data-ttu-id="0ee37-147">必需。</span><span class="sxs-lookup"><span data-stu-id="0ee37-147">Required.</span></span> <span data-ttu-id="0ee37-148">用户流版本。</span><span class="sxs-lookup"><span data-stu-id="0ee37-148">The version of the user flow.</span></span> <span data-ttu-id="0ee37-149">此值将始终为1。</span><span class="sxs-lookup"><span data-stu-id="0ee37-149">This value will always be 1.</span></span>|
|<span data-ttu-id="0ee37-150">identityProviders</span><span class="sxs-lookup"><span data-stu-id="0ee37-150">identityProviders</span></span>|<span data-ttu-id="0ee37-151">[identityProvider](../resources/identityprovider.md)集合 </span><span class="sxs-lookup"><span data-stu-id="0ee37-151">[identityProvider](../resources/identityprovider.md) collection</span></span>|<span data-ttu-id="0ee37-152">可选。</span><span class="sxs-lookup"><span data-stu-id="0ee37-152">Optional.</span></span> <span data-ttu-id="0ee37-153">要包括在用户流中的标识提供程序。</span><span class="sxs-lookup"><span data-stu-id="0ee37-153">The identity providers you want to include in the user flow.</span></span>|

## <a name="response"></a><span data-ttu-id="0ee37-154">响应</span><span class="sxs-lookup"><span data-stu-id="0ee37-154">Response</span></span>

<span data-ttu-id="0ee37-155">如果成功，此方法将向 `201 Created` 为此请求创建的 [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) 对象的 URI 返回响应代码和位置标头，并将 `B2X_1` 前缀添加到名称中。</span><span class="sxs-lookup"><span data-stu-id="0ee37-155">If successful, this method returns a `201 Created` response code and a Location header with a URI to the [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) object created for this request, with the `B2X_1` prefix added to the name.</span></span> <span data-ttu-id="0ee37-156">如果失败，将返回 `4xx` 错误并显示具体详细信息。</span><span class="sxs-lookup"><span data-stu-id="0ee37-156">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="examples"></a><span data-ttu-id="0ee37-157">示例</span><span class="sxs-lookup"><span data-stu-id="0ee37-157">Examples</span></span>

### <a name="example-1-create-a-user-flow-with-the-default-values"></a><span data-ttu-id="0ee37-158">示例1：创建具有默认值的用户流</span><span class="sxs-lookup"><span data-stu-id="0ee37-158">Example 1: Create a user flow with the default values</span></span>

#### <a name="request"></a><span data-ttu-id="0ee37-159">请求</span><span class="sxs-lookup"><span data-stu-id="0ee37-159">Request</span></span>

<span data-ttu-id="0ee37-160">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="0ee37-160">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="0ee37-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="0ee37-161">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="0ee37-162">C#</span><span class="sxs-lookup"><span data-stu-id="0ee37-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-b2xuserflow-from-b2xuserflows-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0ee37-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0ee37-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-b2xuserflow-from-b2xuserflows-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0ee37-164">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0ee37-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-b2xuserflow-from-b2xuserflows-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="0ee37-165">响应</span><span class="sxs-lookup"><span data-stu-id="0ee37-165">Response</span></span>

<span data-ttu-id="0ee37-166">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="0ee37-166">The following is an example of the response.</span></span>

<span data-ttu-id="0ee37-167">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="0ee37-167">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-2-create-a-user-flow-with-the-default-values-and-an-identity-provider"></a><span data-ttu-id="0ee37-168">示例2：创建具有默认值和标识提供程序的用户流</span><span class="sxs-lookup"><span data-stu-id="0ee37-168">Example 2: Create a user flow with the default values and an identity provider</span></span>

#### <a name="request"></a><span data-ttu-id="0ee37-169">请求</span><span class="sxs-lookup"><span data-stu-id="0ee37-169">Request</span></span>

<span data-ttu-id="0ee37-170">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="0ee37-170">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="0ee37-171">HTTP</span><span class="sxs-lookup"><span data-stu-id="0ee37-171">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="0ee37-172">C#</span><span class="sxs-lookup"><span data-stu-id="0ee37-172">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-b2xuserflow-from-b2xuserflows-identityproviders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0ee37-173">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0ee37-173">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-b2xuserflow-from-b2xuserflows-identityproviders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0ee37-174">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0ee37-174">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-b2xuserflow-from-b2xuserflows-identityproviders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="0ee37-175">响应</span><span class="sxs-lookup"><span data-stu-id="0ee37-175">Response</span></span>

<span data-ttu-id="0ee37-176">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="0ee37-176">The following is an example of the response.</span></span>

<span data-ttu-id="0ee37-177">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="0ee37-177">**Note:** The response object shown here might be shortened for readability.</span></span>

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



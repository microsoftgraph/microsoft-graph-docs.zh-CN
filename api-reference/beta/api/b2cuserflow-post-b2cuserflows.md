---
title: 创建 b2cUserFlow
description: 创建新的 b2cUserFlow 对象。
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 4e001b0835e0ca902939d71b6425434cc4ee0446
ms.sourcegitcommit: 2c6e16dd8381945de6adf1eea020c142969b7801
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/01/2020
ms.locfileid: "47319684"
---
# <a name="create-b2cuserflow"></a><span data-ttu-id="6b39e-103">创建 b2cUserFlow</span><span class="sxs-lookup"><span data-stu-id="6b39e-103">Create b2cUserFlow</span></span>

<span data-ttu-id="6b39e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6b39e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6b39e-105">创建新的 [b2cUserFlow](../resources/b2cuserflows.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6b39e-105">Create a new [b2cUserFlow](../resources/b2cuserflows.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6b39e-106">权限</span><span class="sxs-lookup"><span data-stu-id="6b39e-106">Permissions</span></span>

<span data-ttu-id="6b39e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6b39e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6b39e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="6b39e-109">Permission type</span></span>      | <span data-ttu-id="6b39e-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6b39e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6b39e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6b39e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6b39e-112">IdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="6b39e-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="6b39e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6b39e-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="6b39e-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="6b39e-114">Not supported.</span></span>|
|<span data-ttu-id="6b39e-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="6b39e-115">Application</span></span>|<span data-ttu-id="6b39e-116">IdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="6b39e-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="6b39e-117">工作或学校帐户需要属于下列角色之一：</span><span class="sxs-lookup"><span data-stu-id="6b39e-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="6b39e-118">全局管理员</span><span class="sxs-lookup"><span data-stu-id="6b39e-118">Global administrator</span></span>
* <span data-ttu-id="6b39e-119">外部标识用户流管理员</span><span class="sxs-lookup"><span data-stu-id="6b39e-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="6b39e-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6b39e-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identity/b2cUserFlows
```

## <a name="request-headers"></a><span data-ttu-id="6b39e-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="6b39e-121">Request headers</span></span>

|<span data-ttu-id="6b39e-122">名称</span><span class="sxs-lookup"><span data-stu-id="6b39e-122">Name</span></span>|<span data-ttu-id="6b39e-123">说明</span><span class="sxs-lookup"><span data-stu-id="6b39e-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="6b39e-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="6b39e-124">Authorization</span></span>|<span data-ttu-id="6b39e-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6b39e-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="6b39e-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6b39e-127">Content-Type</span></span>|<span data-ttu-id="6b39e-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="6b39e-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6b39e-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="6b39e-130">Request body</span></span>

<span data-ttu-id="6b39e-131">在请求正文中，提供 [b2cUserFlow](../resources/b2cuserflows.md)的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6b39e-131">In the request body, provide a JSON representation of a [b2cUserFlow](../resources/b2cuserflows.md).</span></span>

|<span data-ttu-id="6b39e-132">属性</span><span class="sxs-lookup"><span data-stu-id="6b39e-132">Property</span></span>|<span data-ttu-id="6b39e-133">类型</span><span class="sxs-lookup"><span data-stu-id="6b39e-133">Type</span></span>|<span data-ttu-id="6b39e-134">说明</span><span class="sxs-lookup"><span data-stu-id="6b39e-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6b39e-135">id</span><span class="sxs-lookup"><span data-stu-id="6b39e-135">id</span></span>|<span data-ttu-id="6b39e-136">String</span><span class="sxs-lookup"><span data-stu-id="6b39e-136">String</span></span>|<span data-ttu-id="6b39e-137">必需。</span><span class="sxs-lookup"><span data-stu-id="6b39e-137">Required.</span></span> <span data-ttu-id="6b39e-138">用户流的名称。</span><span class="sxs-lookup"><span data-stu-id="6b39e-138">The name of the user flow.</span></span> <span data-ttu-id="6b39e-139">创建后，名称将预先挂起 `B2C_1` 。</span><span class="sxs-lookup"><span data-stu-id="6b39e-139">The name will be pre-pended with `B2C_1` after creation.</span></span>|
|<span data-ttu-id="6b39e-140">userFlowType</span><span class="sxs-lookup"><span data-stu-id="6b39e-140">userFlowType</span></span>|<span data-ttu-id="6b39e-141">String</span><span class="sxs-lookup"><span data-stu-id="6b39e-141">String</span></span>|<span data-ttu-id="6b39e-142">必需。</span><span class="sxs-lookup"><span data-stu-id="6b39e-142">Required.</span></span> <span data-ttu-id="6b39e-143">您正在创建的用户流的类型。</span><span class="sxs-lookup"><span data-stu-id="6b39e-143">The type of user flow you are creating.</span></span> <span data-ttu-id="6b39e-144">**UserFlowType**支持的值为：</span><span class="sxs-lookup"><span data-stu-id="6b39e-144">The supported values for **userFlowType** are:</span></span><br/><ul><li>`signUp`</li><li>`signIn`</li><li>`signUpOrSignIn`</li><li>`passwordReset`</li><li>`profileUpdate`</li><li>`resourceOwnerPasswordCredentialSignIn`</li>|
|<span data-ttu-id="6b39e-145">userFlowTypeVersion</span><span class="sxs-lookup"><span data-stu-id="6b39e-145">userFlowTypeVersion</span></span>|<span data-ttu-id="6b39e-146">浮点</span><span class="sxs-lookup"><span data-stu-id="6b39e-146">Float</span></span>|<span data-ttu-id="6b39e-147">必需。</span><span class="sxs-lookup"><span data-stu-id="6b39e-147">Required.</span></span> <span data-ttu-id="6b39e-148">用户流的版本。</span><span class="sxs-lookup"><span data-stu-id="6b39e-148">The version of the user flow.</span></span>|
|<span data-ttu-id="6b39e-149">identityProviders</span><span class="sxs-lookup"><span data-stu-id="6b39e-149">identityProviders</span></span>|<span data-ttu-id="6b39e-150">[identityprovider.read.all](../resources/identityprovider.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6b39e-150">[identityProvider](../resources/identityprovider.md) collection</span></span>|<span data-ttu-id="6b39e-151">可选。</span><span class="sxs-lookup"><span data-stu-id="6b39e-151">Optional.</span></span> <span data-ttu-id="6b39e-152">要包括在用户流中的标识提供程序。</span><span class="sxs-lookup"><span data-stu-id="6b39e-152">The identity providers you want to include in the user flow.</span></span>|

## <a name="response"></a><span data-ttu-id="6b39e-153">响应</span><span class="sxs-lookup"><span data-stu-id="6b39e-153">Response</span></span>

<span data-ttu-id="6b39e-154">如果成功，此方法将向 `201 Created` 为此请求创建的 [b2cUserFlow](../resources/b2cuserflows.md) 对象的 URI 返回响应代码和位置标头，并将 `B2C_1` 前缀添加到名称中。</span><span class="sxs-lookup"><span data-stu-id="6b39e-154">If successful, this method returns a `201 Created` response code and a Location header with a URI to the [b2cUserFlow](../resources/b2cuserflows.md) object created for this request, with the `B2C_1` prefix added to the name.</span></span> <span data-ttu-id="6b39e-155">如果失败，将返回 `4xx` 错误并显示具体详细信息。</span><span class="sxs-lookup"><span data-stu-id="6b39e-155">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="examples"></a><span data-ttu-id="6b39e-156">示例</span><span class="sxs-lookup"><span data-stu-id="6b39e-156">Examples</span></span>

### <a name="example-1-create-a-user-flow-with-the-default-values"></a><span data-ttu-id="6b39e-157">示例1：创建具有默认值的用户流</span><span class="sxs-lookup"><span data-stu-id="6b39e-157">Example 1: Create a user flow with the default values</span></span>

#### <a name="request"></a><span data-ttu-id="6b39e-158">请求</span><span class="sxs-lookup"><span data-stu-id="6b39e-158">Request</span></span>

<span data-ttu-id="6b39e-159">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="6b39e-159">The following is an example of the request.</span></span>

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

#### <a name="response"></a><span data-ttu-id="6b39e-160">响应</span><span class="sxs-lookup"><span data-stu-id="6b39e-160">Response</span></span>

<span data-ttu-id="6b39e-161">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="6b39e-161">The following is an example of the response.</span></span>

<span data-ttu-id="6b39e-162">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="6b39e-162">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-2-create-a-user-flow-with-the-default-values-and-an-identity-provider"></a><span data-ttu-id="6b39e-163">示例2：创建具有默认值和标识提供程序的用户流</span><span class="sxs-lookup"><span data-stu-id="6b39e-163">Example 2: Create a user flow with the default values and an identity provider</span></span>

#### <a name="request"></a><span data-ttu-id="6b39e-164">请求</span><span class="sxs-lookup"><span data-stu-id="6b39e-164">Request</span></span>

<span data-ttu-id="6b39e-165">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="6b39e-165">The following is an example of the request.</span></span>

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

#### <a name="response"></a><span data-ttu-id="6b39e-166">响应</span><span class="sxs-lookup"><span data-stu-id="6b39e-166">Response</span></span>

<span data-ttu-id="6b39e-167">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="6b39e-167">The following is an example of the response.</span></span>

<span data-ttu-id="6b39e-168">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="6b39e-168">**Note:** The response object shown here might be shortened for readability.</span></span>

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

---
title: 在用户流中配置 API 连接器
description: 通过更新 apiConnectorConfiguration 属性，为用户流中的特定步骤启用或禁用 API 连接器。
author: nickgmicrosoft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: cf5315c6100c55686001245f91a7a2847a2b5689
ms.sourcegitcommit: a9731e19589dcb5c0c6fe2e24b008c86573ef803
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/13/2021
ms.locfileid: "49844006"
---
# <a name="configure-userflowapiconnectorconfiguration"></a><span data-ttu-id="d1e46-103">配置 userFlowApiConnectorConfiguration</span><span class="sxs-lookup"><span data-stu-id="d1e46-103">Configure userFlowApiConnectorConfiguration</span></span>

<span data-ttu-id="d1e46-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d1e46-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d1e46-105">更新[b2cIdentityUserFlow](../resources/b2cidentityuserflow.md)中的[apiConnectorConfiguration](../resources/userflowapiconnectorconfiguration.md)属性，以在用户流中启用或禁用 API 连接器。</span><span class="sxs-lookup"><span data-stu-id="d1e46-105">Update the [apiConnectorConfiguration](../resources/userflowapiconnectorconfiguration.md) property in a [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) to enable or disable an API connector in a user flow.</span></span> <span data-ttu-id="d1e46-106">[apiConnectorConfiguration](../resources/userflowapiconnectorconfiguration.md)的每个关系对应于可配置为调用 API 连接器的用户流中的特定步骤。</span><span class="sxs-lookup"><span data-stu-id="d1e46-106">Each relationship of the [apiConnectorConfiguration](../resources/userflowapiconnectorconfiguration.md) corresponds to a specific step in the user flow that can be configured to call an API connector.</span></span> <span data-ttu-id="d1e46-107">一次为特定步骤 1 配置 API 连接器，如下所示。</span><span class="sxs-lookup"><span data-stu-id="d1e46-107">You configure an API connector for a particular step one at a time as shown below.</span></span>

## <a name="permissions"></a><span data-ttu-id="d1e46-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="d1e46-108">Permissions</span></span>

<span data-ttu-id="d1e46-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d1e46-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d1e46-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="d1e46-111">Permission type</span></span>|<span data-ttu-id="d1e46-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d1e46-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d1e46-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d1e46-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d1e46-114">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1e46-114">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="d1e46-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d1e46-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d1e46-116">不支持</span><span class="sxs-lookup"><span data-stu-id="d1e46-116">Not supported</span></span>|
|<span data-ttu-id="d1e46-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="d1e46-117">Application</span></span>|<span data-ttu-id="d1e46-118">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1e46-118">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="d1e46-119">工作或学校帐户需要属于以下角色之一：</span><span class="sxs-lookup"><span data-stu-id="d1e46-119">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="d1e46-120">全局管理员</span><span class="sxs-lookup"><span data-stu-id="d1e46-120">Global administrator</span></span>
* <span data-ttu-id="d1e46-121">外部标识用户流管理员</span><span class="sxs-lookup"><span data-stu-id="d1e46-121">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="d1e46-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d1e46-122">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
PUT /identity/b2cUserFlows/{b2cUserFlowId}/apiConnectorConfiguration/{step}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="d1e46-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="d1e46-123">Request headers</span></span>

|<span data-ttu-id="d1e46-124">名称</span><span class="sxs-lookup"><span data-stu-id="d1e46-124">Name</span></span>|<span data-ttu-id="d1e46-125">说明</span><span class="sxs-lookup"><span data-stu-id="d1e46-125">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d1e46-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="d1e46-126">Authorization</span></span>|<span data-ttu-id="d1e46-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d1e46-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="d1e46-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d1e46-129">Content-Type</span></span>|<span data-ttu-id="d1e46-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="d1e46-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d1e46-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="d1e46-132">Request body</span></span>

<span data-ttu-id="d1e46-133">在请求正文中，提供要使用特定步骤的 `id` [identityApiConnector](../resources/identityapiconnector.md) 的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d1e46-133">In the request body, provide a JSON representation of the `id` of the [identityApiConnector](../resources/identityapiconnector.md) you want to use the particular step.</span></span> <span data-ttu-id="d1e46-134">若要禁用 API 连接器，值可以是 {} 。</span><span class="sxs-lookup"><span data-stu-id="d1e46-134">To disable an API connector, the value can be {}.</span></span>

## <a name="response"></a><span data-ttu-id="d1e46-135">响应</span><span class="sxs-lookup"><span data-stu-id="d1e46-135">Response</span></span>

<span data-ttu-id="d1e46-136">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="d1e46-136">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="d1e46-137">示例</span><span class="sxs-lookup"><span data-stu-id="d1e46-137">Examples</span></span>

### <a name="example-1-enable-api-connector-for-post-idp-federation-on-sign-up"></a><span data-ttu-id="d1e46-138">示例 1：在注册时为 IDP 后联合身份验证启用 API 连接器</span><span class="sxs-lookup"><span data-stu-id="d1e46-138">Example 1: Enable API connector for Post IDP Federation on sign up</span></span>

#### <a name="request"></a><span data-ttu-id="d1e46-139">请求</span><span class="sxs-lookup"><span data-stu-id="d1e46-139">Request</span></span>

<span data-ttu-id="d1e46-140">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d1e46-140">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="d1e46-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="d1e46-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "put_b2cuserflows-apiconnectorconfiguration_postFederationSignup"
}
-->

``` http
PUT https://graph.microsoft.com/beta/identity/b2cUserFlows/B2C_1_testuserflow/apiConnectorConfiguration/postFederationSignup/$ref
Content-Type: application/json

{
    "@odata.id": "https://graph.microsoft.com/beta/identity/apiConnectors/{id}"   
}
```
# <a name="c"></a>[<span data-ttu-id="d1e46-142">C#</span><span class="sxs-lookup"><span data-stu-id="d1e46-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/put-b2cuserflows-apiconnectorconfiguration-postfederationsignup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d1e46-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d1e46-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/put-b2cuserflows-apiconnectorconfiguration-postfederationsignup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d1e46-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d1e46-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/put-b2cuserflows-apiconnectorconfiguration-postfederationsignup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d1e46-145">Java</span><span class="sxs-lookup"><span data-stu-id="d1e46-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/put-b2cuserflows-apiconnectorconfiguration-postfederationsignup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

#### <a name="response"></a><span data-ttu-id="d1e46-146">响应</span><span class="sxs-lookup"><span data-stu-id="d1e46-146">Response</span></span> 

<span data-ttu-id="d1e46-147">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="d1e46-147">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
}
-->

``` http
HTTP/1.1 204 No Content
```

### <a name="example-2-enable-api-connector-for-post-attribute-collection-on-sign-up"></a><span data-ttu-id="d1e46-148">示例 2：在注册时为 Post 属性集合启用 API 连接器</span><span class="sxs-lookup"><span data-stu-id="d1e46-148">Example 2: Enable API connector for Post Attribute Collection on sign up</span></span>

#### <a name="request"></a><span data-ttu-id="d1e46-149">请求</span><span class="sxs-lookup"><span data-stu-id="d1e46-149">Request</span></span> 

<span data-ttu-id="d1e46-150">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d1e46-150">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="d1e46-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="d1e46-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "put_b2cuserflows-apiconnectorconfiguration_postAttributeCollection"
}
-->

``` http
PUT https://graph.microsoft.com/beta/identity/b2cUserFlows/B2C_1_testuserflow/apiConnectorConfiguration/postAttributeCollection/$ref
Content-Type: application/json

{
    "@odata.id": "https://graph.microsoft.com/beta/identity/apiConnectors/{id}"   
}
```
# <a name="c"></a>[<span data-ttu-id="d1e46-152">C#</span><span class="sxs-lookup"><span data-stu-id="d1e46-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/put-b2cuserflows-apiconnectorconfiguration-postattributecollection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d1e46-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d1e46-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/put-b2cuserflows-apiconnectorconfiguration-postattributecollection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d1e46-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d1e46-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/put-b2cuserflows-apiconnectorconfiguration-postattributecollection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d1e46-155">Java</span><span class="sxs-lookup"><span data-stu-id="d1e46-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/put-b2cuserflows-apiconnectorconfiguration-postattributecollection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="d1e46-156">响应</span><span class="sxs-lookup"><span data-stu-id="d1e46-156">Response</span></span>

<span data-ttu-id="d1e46-157">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="d1e46-157">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
}
-->

``` http
HTTP/1.1 204 No Content
```

### <a name="example-3-disable-an-api-connector-for-post-attribute-collection-on-sign-up"></a><span data-ttu-id="d1e46-158">示例 3：在注册时禁用 Post 属性集合的 API 连接器</span><span class="sxs-lookup"><span data-stu-id="d1e46-158">Example 3: Disable an API connector for Post Attribute Collection on sign up</span></span>

#### <a name="request"></a><span data-ttu-id="d1e46-159">请求</span><span class="sxs-lookup"><span data-stu-id="d1e46-159">Request</span></span> 

<span data-ttu-id="d1e46-160">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d1e46-160">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="d1e46-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="d1e46-161">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "put_b2cuserflows-apiconnectorconfiguration_disable-postAttributeCollection"
}
-->

``` http
PUT https://graph.microsoft.com/beta/identity/b2cUserFlows/B2C_1_testuserflow/apiConnectorConfiguration/postAttributeCollection/$ref
Content-Type: application/json

{ }
```
# <a name="javascript"></a>[<span data-ttu-id="d1e46-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d1e46-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/put-b2cuserflows-apiconnectorconfiguration-disable-postattributecollection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d1e46-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d1e46-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/put-b2cuserflows-apiconnectorconfiguration-disable-postattributecollection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d1e46-164">Java</span><span class="sxs-lookup"><span data-stu-id="d1e46-164">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/put-b2cuserflows-apiconnectorconfiguration-disable-postattributecollection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="d1e46-165">响应</span><span class="sxs-lookup"><span data-stu-id="d1e46-165">Response</span></span>

<span data-ttu-id="d1e46-166">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="d1e46-166">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
}
-->

``` http
HTTP/1.1 204 No Content
```

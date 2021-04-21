---
title: 更新 identityApiConnector
description: 更新 identityApiConnector 对象的属性。
author: nickgmicrosoft
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 09733c849f99c2928ba7c2cc3b1702f411952cd7
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/21/2021
ms.locfileid: "51921611"
---
# <a name="update-identityapiconnector"></a><span data-ttu-id="4541a-103">更新 identityApiConnector</span><span class="sxs-lookup"><span data-stu-id="4541a-103">Update identityApiConnector</span></span>

<span data-ttu-id="4541a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4541a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4541a-105">更新 [identityApiConnector 对象](../resources/identityapiconnector.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="4541a-105">Update the properties of an [identityApiConnector](../resources/identityapiconnector.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="4541a-106">权限</span><span class="sxs-lookup"><span data-stu-id="4541a-106">Permissions</span></span>

<span data-ttu-id="4541a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4541a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4541a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="4541a-109">Permission type</span></span>                        | <span data-ttu-id="4541a-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4541a-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="4541a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4541a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="4541a-112">APIConnectors.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4541a-112">APIConnectors.ReadWrite.All</span></span> |
| <span data-ttu-id="4541a-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4541a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4541a-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="4541a-114">Not supported.</span></span>  |
| <span data-ttu-id="4541a-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="4541a-115">Application</span></span>                            | <span data-ttu-id="4541a-116">APIConnectors.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4541a-116">APIConnectors.ReadWrite.All</span></span> |

<span data-ttu-id="4541a-117">工作或学校帐户需要属于以下角色之一：</span><span class="sxs-lookup"><span data-stu-id="4541a-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="4541a-118">全局管理员</span><span class="sxs-lookup"><span data-stu-id="4541a-118">Global administrator</span></span>
* <span data-ttu-id="4541a-119">外部标识用户流管理员</span><span class="sxs-lookup"><span data-stu-id="4541a-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="4541a-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4541a-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
PATCH /identity/apiConnectors/{identityApiConnectorId}
```

## <a name="request-headers"></a><span data-ttu-id="4541a-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="4541a-121">Request headers</span></span>
|<span data-ttu-id="4541a-122">名称</span><span class="sxs-lookup"><span data-stu-id="4541a-122">Name</span></span>|<span data-ttu-id="4541a-123">说明</span><span class="sxs-lookup"><span data-stu-id="4541a-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="4541a-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="4541a-124">Authorization</span></span>|<span data-ttu-id="4541a-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4541a-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="4541a-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4541a-127">Content-Type</span></span>|<span data-ttu-id="4541a-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="4541a-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4541a-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="4541a-130">Request body</span></span>
<span data-ttu-id="4541a-131">在请求正文中，提供 [identityApiConnector](../resources/identityapiconnector.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4541a-131">In the request body, supply a JSON representation of the [identityApiConnector](../resources/identityapiconnector.md) object.</span></span>

<span data-ttu-id="4541a-132">下表显示了 [可更新的 identityApiConnector](../resources/identityapiconnector.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="4541a-132">The following table shows the properties of the [identityApiConnector](../resources/identityapiconnector.md) that can be updated.</span></span>


|<span data-ttu-id="4541a-133">属性</span><span class="sxs-lookup"><span data-stu-id="4541a-133">Property</span></span>|<span data-ttu-id="4541a-134">类型</span><span class="sxs-lookup"><span data-stu-id="4541a-134">Type</span></span>|<span data-ttu-id="4541a-135">说明</span><span class="sxs-lookup"><span data-stu-id="4541a-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4541a-136">displayName</span><span class="sxs-lookup"><span data-stu-id="4541a-136">displayName</span></span>|<span data-ttu-id="4541a-137">String</span><span class="sxs-lookup"><span data-stu-id="4541a-137">String</span></span>| <span data-ttu-id="4541a-138">API 连接器的名称。</span><span class="sxs-lookup"><span data-stu-id="4541a-138">The name of the API connector.</span></span> |
|<span data-ttu-id="4541a-139">targetUrl</span><span class="sxs-lookup"><span data-stu-id="4541a-139">targetUrl</span></span>|<span data-ttu-id="4541a-140">String</span><span class="sxs-lookup"><span data-stu-id="4541a-140">String</span></span>| <span data-ttu-id="4541a-141">要调用的 API 终结点的 URL。</span><span class="sxs-lookup"><span data-stu-id="4541a-141">The URL of the API endpoint to call.</span></span> |
|<span data-ttu-id="4541a-142">authenticationConfiguration</span><span class="sxs-lookup"><span data-stu-id="4541a-142">authenticationConfiguration</span></span>|[<span data-ttu-id="4541a-143">apiAuthenticationConfigurationBase</span><span class="sxs-lookup"><span data-stu-id="4541a-143">apiAuthenticationConfigurationBase</span></span>](../resources/apiauthenticationconfigurationbase.md)|<span data-ttu-id="4541a-144">描述用于调用 API 的身份验证配置详细信息的对象。</span><span class="sxs-lookup"><span data-stu-id="4541a-144">The object which describes the authentication configuration details for calling the API.</span></span> <span data-ttu-id="4541a-145">仅 [支持基本](../resources/basicauthentication.md) 身份验证 [和 PKCS 12 客户端](../resources/pkcs12certificate.md) 证书。</span><span class="sxs-lookup"><span data-stu-id="4541a-145">Only [Basic authentication](../resources/basicauthentication.md) and [PKCS 12 client certificate](../resources/pkcs12certificate.md) are supported.</span></span>|

## <a name="response"></a><span data-ttu-id="4541a-146">响应</span><span class="sxs-lookup"><span data-stu-id="4541a-146">Response</span></span>

<span data-ttu-id="4541a-147">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="4541a-147">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="4541a-148">示例</span><span class="sxs-lookup"><span data-stu-id="4541a-148">Examples</span></span>

### <a name="example-1-changing-display-name-targeturl-and-username--password-used-for-basic-authentication"></a><span data-ttu-id="4541a-149">示例 1：更改显示名称身份验证所使用的 &、targetUrl 和 username 密码</span><span class="sxs-lookup"><span data-stu-id="4541a-149">Example 1: Changing display name, targetUrl, and username & password used for basic authentication</span></span>

#### <a name="request"></a><span data-ttu-id="4541a-150">请求</span><span class="sxs-lookup"><span data-stu-id="4541a-150">Request</span></span>

<span data-ttu-id="4541a-151">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="4541a-151">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="4541a-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="4541a-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_identityapiconnector"
}
-->

``` http
PATCH https://graph.microsoft.com/v1.0/identity/apiConnectors/{identityApiConnectorId}
Content-Type: application/json

{
  "displayName": "New Test API",
  "targetUrl": "https://otherapi.com/api/endpoint",
  "authenticationConfiguration": {
    "@odata.type": "microsoft.graph.basicAuthentication",
    "username":"<NEW_USERNAME>", 
    "password":"<NEW_PASSWORD>"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="4541a-153">C#</span><span class="sxs-lookup"><span data-stu-id="4541a-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-identityapiconnector-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4541a-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4541a-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-identityapiconnector-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4541a-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4541a-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-identityapiconnector-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4541a-156">Java</span><span class="sxs-lookup"><span data-stu-id="4541a-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-identityapiconnector-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="4541a-157">响应</span><span class="sxs-lookup"><span data-stu-id="4541a-157">Response</span></span>

<span data-ttu-id="4541a-158">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="4541a-158">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
}
-->

``` http
HTTP/1.1 204 No Content
```

### <a name="example-2-changing-api-connector-to-use-client-certificate-authentication"></a><span data-ttu-id="4541a-159">示例 2：将 API 连接器更改为使用客户端证书身份验证</span><span class="sxs-lookup"><span data-stu-id="4541a-159">Example 2: Changing API connector to use client certificate authentication</span></span>

<span data-ttu-id="4541a-160">这将覆盖之前的任何 authenticationConfiguration 设置。</span><span class="sxs-lookup"><span data-stu-id="4541a-160">This will overwrite any previous authenticationConfiguration settings.</span></span> <span data-ttu-id="4541a-161">若要从基本身份验证更改为证书身份验证，请使用此模式。</span><span class="sxs-lookup"><span data-stu-id="4541a-161">To change from Basic authentication to certificate authentication, use this.</span></span> <span data-ttu-id="4541a-162">若要向证书列表中添加其他证书，请使用 [上载客户端证书](../api/identityapiconnector-uploadclientcertificate.md) 方法。</span><span class="sxs-lookup"><span data-stu-id="4541a-162">To add additional certificates to list of certificates, use the [Upload client certificate](../api/identityapiconnector-uploadclientcertificate.md) method.</span></span> <span data-ttu-id="4541a-163">使用此方法时，API 连接器的"Get"或"List"操作将为 `authenticationConfiguration` [microsoft.graph.clientCertificateAuthentication 类型](../resources/clientcertificateauthentication.md)。</span><span class="sxs-lookup"><span data-stu-id="4541a-163">When using this method, consequent "Get" or "List" operations of API connectors, `authenticationConfiguration` will be of type [microsoft.graph.clientCertificateAuthentication](../resources/clientcertificateauthentication.md).</span></span>

#### <a name="request"></a><span data-ttu-id="4541a-164">请求</span><span class="sxs-lookup"><span data-stu-id="4541a-164">Request</span></span>

<span data-ttu-id="4541a-165">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="4541a-165">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="4541a-166">HTTP</span><span class="sxs-lookup"><span data-stu-id="4541a-166">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_identityapiconnector"
}
-->

``` http
PATCH https://graph.microsoft.com/v1.0/identity/apiConnectors/be1f769b-9b13-437e-b540-79a905c4932c
Content-Type: application/json

{
  "authenticationConfiguration": {
    "@odata.type": "#microsoft.graph.pkcs12Certificate",
    "pkcs12Value": "eyJhbGciOiJSU0EtT0FFUCIsImVuYyI6IkEyNTZHQ00ifQ...kDJ04sJShkkgjL9Bm49plA",
    "password": "secret"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="4541a-167">C#</span><span class="sxs-lookup"><span data-stu-id="4541a-167">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-identityapiconnector-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4541a-168">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4541a-168">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-identityapiconnector-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4541a-169">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4541a-169">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-identityapiconnector-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4541a-170">Java</span><span class="sxs-lookup"><span data-stu-id="4541a-170">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-identityapiconnector-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="4541a-171">响应</span><span class="sxs-lookup"><span data-stu-id="4541a-171">Response</span></span>

<span data-ttu-id="4541a-172">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="4541a-172">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
}
-->

``` http
HTTP/1.1 204 No Content
```

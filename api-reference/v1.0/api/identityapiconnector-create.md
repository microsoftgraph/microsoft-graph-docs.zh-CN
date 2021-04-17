---
title: 创建 identityApiConnector
description: 创建新的 identityApiConnector 对象。
author: nickgmicrosoft
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: cb83cd4484ab20f88c9362d7b67a294a6359ff49
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882431"
---
# <a name="create-identityapiconnector"></a><span data-ttu-id="45908-103">创建 identityApiConnector</span><span class="sxs-lookup"><span data-stu-id="45908-103">Create identityApiConnector</span></span>

<span data-ttu-id="45908-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="45908-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="45908-105">创建新的 [identityApiConnector](../resources/identityapiconnector.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="45908-105">Create a new [identityApiConnector](../resources/identityapiconnector.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="45908-106">权限</span><span class="sxs-lookup"><span data-stu-id="45908-106">Permissions</span></span>

<span data-ttu-id="45908-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="45908-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="45908-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="45908-109">Permission type</span></span>                        | <span data-ttu-id="45908-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="45908-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="45908-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="45908-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="45908-112">APIConnectors.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45908-112">APIConnectors.ReadWrite.All</span></span> |
| <span data-ttu-id="45908-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="45908-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="45908-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="45908-114">Not supported.</span></span>  |
| <span data-ttu-id="45908-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="45908-115">Application</span></span>                            | <span data-ttu-id="45908-116">APIConnectors.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45908-116">APIConnectors.ReadWrite.All</span></span> |

<span data-ttu-id="45908-117">工作或学校帐户需要属于以下角色之一：</span><span class="sxs-lookup"><span data-stu-id="45908-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="45908-118">全局管理员</span><span class="sxs-lookup"><span data-stu-id="45908-118">Global administrator</span></span>
* <span data-ttu-id="45908-119">外部标识用户流管理员</span><span class="sxs-lookup"><span data-stu-id="45908-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="45908-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="45908-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

```http
POST /identity/apiConnectors
```

## <a name="request-headers"></a><span data-ttu-id="45908-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="45908-121">Request headers</span></span>

| <span data-ttu-id="45908-122">名称</span><span class="sxs-lookup"><span data-stu-id="45908-122">Name</span></span>          | <span data-ttu-id="45908-123">说明</span><span class="sxs-lookup"><span data-stu-id="45908-123">Description</span></span>                 |
| :------------ | :-------------------------- |
| <span data-ttu-id="45908-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="45908-124">Authorization</span></span> | <span data-ttu-id="45908-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="45908-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="45908-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="45908-127">Content-Type</span></span>  | <span data-ttu-id="45908-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="45908-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="45908-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="45908-130">Request body</span></span>

<span data-ttu-id="45908-131">在请求正文中，提供 [identityApiConnector](../resources/identityapiconnector.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="45908-131">In the request body, supply a JSON representation of the [identityApiConnector](../resources/identityapiconnector.md) object.</span></span>

<span data-ttu-id="45908-132">下表显示创建 [identityApiConnector](../resources/identityapiconnector.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="45908-132">The following table shows the properties that are required when you create the [identityApiConnector](../resources/identityapiconnector.md).</span></span>

|<span data-ttu-id="45908-133">属性</span><span class="sxs-lookup"><span data-stu-id="45908-133">Property</span></span>|<span data-ttu-id="45908-134">类型</span><span class="sxs-lookup"><span data-stu-id="45908-134">Type</span></span>|<span data-ttu-id="45908-135">说明</span><span class="sxs-lookup"><span data-stu-id="45908-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="45908-136">displayName</span><span class="sxs-lookup"><span data-stu-id="45908-136">displayName</span></span>|<span data-ttu-id="45908-137">String</span><span class="sxs-lookup"><span data-stu-id="45908-137">String</span></span>| <span data-ttu-id="45908-138">API 连接器的名称。</span><span class="sxs-lookup"><span data-stu-id="45908-138">The name of the API connector.</span></span> |
|<span data-ttu-id="45908-139">targetUrl</span><span class="sxs-lookup"><span data-stu-id="45908-139">targetUrl</span></span>|<span data-ttu-id="45908-140">String</span><span class="sxs-lookup"><span data-stu-id="45908-140">String</span></span>| <span data-ttu-id="45908-141">要调用的 API 终结点的 URL。</span><span class="sxs-lookup"><span data-stu-id="45908-141">The URL of the API endpoint to call.</span></span> |
|<span data-ttu-id="45908-142">authenticationConfiguration</span><span class="sxs-lookup"><span data-stu-id="45908-142">authenticationConfiguration</span></span>|[<span data-ttu-id="45908-143">apiAuthenticationConfigurationBase</span><span class="sxs-lookup"><span data-stu-id="45908-143">apiAuthenticationConfigurationBase</span></span>](../resources/apiauthenticationconfigurationbase.md)|<span data-ttu-id="45908-144">描述用于调用 API 的身份验证配置详细信息的对象。</span><span class="sxs-lookup"><span data-stu-id="45908-144">The object which describes the authentication configuration details for calling the API.</span></span> <span data-ttu-id="45908-145">[支持基本身份验证](../resources/basicauthentication.md)[和 PKCS 12 客户端](../resources/pkcs12certificate.md)证书。</span><span class="sxs-lookup"><span data-stu-id="45908-145">[Basic authentication](../resources/basicauthentication.md) and [PKCS 12 client certificate](../resources/pkcs12certificate.md) are supported.</span></span>|

## <a name="response"></a><span data-ttu-id="45908-146">响应</span><span class="sxs-lookup"><span data-stu-id="45908-146">Response</span></span>

<span data-ttu-id="45908-147">如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [identityApiConnector](../resources/identityapiconnector.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="45908-147">If successful, this method returns a `201 Created` response code and an [identityApiConnector](../resources/identityapiconnector.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="45908-148">示例</span><span class="sxs-lookup"><span data-stu-id="45908-148">Examples</span></span>

### <a name="example-1-create-an-api-connector-with-basic-authentication"></a><span data-ttu-id="45908-149">示例 1：使用基本身份验证创建 API 连接器</span><span class="sxs-lookup"><span data-stu-id="45908-149">Example 1: Create an API connector with basic authentication</span></span>

#### <a name="request"></a><span data-ttu-id="45908-150">请求</span><span class="sxs-lookup"><span data-stu-id="45908-150">Request</span></span>

<span data-ttu-id="45908-151">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="45908-151">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_identityapiconnector"
}
-->

```http
POST https://graph.microsoft.com/v1.0/identity/apiConnectors
Content-Type: application/json

{
    "displayName":"Test API",
    "targetUrl":"https://someapi.com/api",
    "authenticationConfiguration": {
      "@odata.type":"#microsoft.graph.basicAuthentication",
      "username": "MyUsername",
      "password": "MyPassword"
    }
}
```

#### <a name="response"></a><span data-ttu-id="45908-152">响应</span><span class="sxs-lookup"><span data-stu-id="45908-152">Response</span></span>

<span data-ttu-id="45908-153">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="45908-153">The following is an example of the response.</span></span>

><span data-ttu-id="45908-154">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="45908-154">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityApiConnector"
}
-->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identity/apiConnectors/$entity",
    "id":"guid",
    "displayName": "Test API",
    "targetUrl": "https://someapi.com/api",
    "authenticationConfiguration": {
        "@odata.type": "#microsoft.graph.basicAuthentication",
        "username": "MyUsername",
        "password": "******"
    }
}
```

### <a name="example-2-create-an-api-connector-with-client-certificate-authentication"></a><span data-ttu-id="45908-155">示例 2：使用客户端证书身份验证创建 API 连接器</span><span class="sxs-lookup"><span data-stu-id="45908-155">Example 2: Create an API connector with client certificate authentication</span></span>

#### <a name="request"></a><span data-ttu-id="45908-156">请求</span><span class="sxs-lookup"><span data-stu-id="45908-156">Request</span></span>

<span data-ttu-id="45908-157">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="45908-157">The following is an example of the request.</span></span>

> <span data-ttu-id="45908-158">**注意：** `authenticationConfiguration` 请求中的 类型为 [microsoft.graph.pkcs12certificate](../resources/pkcs12certificate.md)，表示上载或创建时所需的证书配置。</span><span class="sxs-lookup"><span data-stu-id="45908-158">**Note:** `authenticationConfiguration` in the request is of type [microsoft.graph.pkcs12certificate](../resources/pkcs12certificate.md), which represents the configuration of a certificate needed on upload or create.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_identityapiconnector"
}
-->

```http
POST https://graph.microsoft.com/v1.0/identity/apiConnectors
Content-Type: application/json

{
    "displayName":"Test API",
    "targetUrl":"https://someotherapi.com/api",
    "authenticationConfiguration": {
        "@odata.type":"#microsoft.graph.pkcs12Certificate",
        "pkcs12Value": "eyJhbGciOiJSU0EtT0FFUCIsImVuYyI6IkEyNTZHQ00ifQ...kDJ04sJShkkgjL9Bm49plA",
        "password": "CertificatePassword"
    }
}
```

#### <a name="response"></a><span data-ttu-id="45908-159">响应</span><span class="sxs-lookup"><span data-stu-id="45908-159">Response</span></span>

<span data-ttu-id="45908-160">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="45908-160">The following is an example of the response.</span></span>

> <span data-ttu-id="45908-161">**注意：** `authenticationConfiguration` 响应中的 类型为 [microsoft.graph.clientCertificateAuthentication，](../resources/clientcertificateauthentication.md) 因为这表示已上载证书的公共信息。</span><span class="sxs-lookup"><span data-stu-id="45908-161">**Note:** `authenticationConfiguration` in the response is of type [microsoft.graph.clientCertificateAuthentication](../resources/clientcertificateauthentication.md) because this represents the public information of uploaded certificates.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityApiConnector"
}
-->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identity/apiConnectors/$entity",
    "id":"guid",
    "displayName": "Test API",
    "targetUrl": "https://someotherapi.com/api",
    "authenticationConfiguration": {
        "@odata.type": "#microsoft.graph.clientCertificateAuthentication",
        "certificateList": [
            {
                "thumbprint": "0EB255CC895477798BA418B378255204304897AD",
                "notAfter": 1666350522,
                "notBefore": 1508670522,
                "isActive": true
            }
        ]
    }
}
```

---
title: identityApiConnector：uploadClientCertificate
description: 将 PKCS 12 格式密钥 (PFX) API 连接器身份验证配置。
localization_priority: Normal
author: nickgmicrosoft
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 779b4e6d7800ad9284c77295145ea1c5f27d82a3
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2021
ms.locfileid: "51509370"
---
# <a name="identityapiconnector-uploadclientcertificate"></a><span data-ttu-id="f6a0c-103">identityApiConnector：uploadClientCertificate</span><span class="sxs-lookup"><span data-stu-id="f6a0c-103">identityApiConnector: uploadClientCertificate</span></span>

<span data-ttu-id="f6a0c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f6a0c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f6a0c-105">将 PKCS 12 格式密钥 (.pfx) API 连接器的身份验证配置。</span><span class="sxs-lookup"><span data-stu-id="f6a0c-105">Upload a PKCS 12 format key (.pfx) to an API connector's authentication configuration.</span></span> <span data-ttu-id="f6a0c-106">输入是 PKCS 12 证书内容的 Base64 编码值。</span><span class="sxs-lookup"><span data-stu-id="f6a0c-106">The input is a base-64 encoded value of the PKCS 12 certificate contents.</span></span> <span data-ttu-id="f6a0c-107">此方法返回 [apiConnector](../resources/identityApiConnector.md)。</span><span class="sxs-lookup"><span data-stu-id="f6a0c-107">This method returns an [apiConnector](../resources/identityApiConnector.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f6a0c-108">权限</span><span class="sxs-lookup"><span data-stu-id="f6a0c-108">Permissions</span></span>

<span data-ttu-id="f6a0c-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f6a0c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f6a0c-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="f6a0c-111">Permission type</span></span>                        | <span data-ttu-id="f6a0c-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f6a0c-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="f6a0c-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f6a0c-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="f6a0c-114">APIConnectors.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6a0c-114">APIConnectors.ReadWrite.All</span></span> |
| <span data-ttu-id="f6a0c-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f6a0c-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f6a0c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f6a0c-116">Not supported.</span></span>  |
| <span data-ttu-id="f6a0c-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="f6a0c-117">Application</span></span>                            | <span data-ttu-id="f6a0c-118">APIConnectors.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6a0c-118">APIConnectors.ReadWrite.All</span></span> |

<span data-ttu-id="f6a0c-119">工作或学校帐户需要属于以下角色之一：</span><span class="sxs-lookup"><span data-stu-id="f6a0c-119">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="f6a0c-120">全局管理员</span><span class="sxs-lookup"><span data-stu-id="f6a0c-120">Global administrator</span></span>
* <span data-ttu-id="f6a0c-121">外部标识用户流管理员</span><span class="sxs-lookup"><span data-stu-id="f6a0c-121">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="f6a0c-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f6a0c-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identity/apiconnectors/{id}/uploadClientCertificate
```

## <a name="request-headers"></a><span data-ttu-id="f6a0c-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="f6a0c-123">Request headers</span></span>

| <span data-ttu-id="f6a0c-124">名称</span><span class="sxs-lookup"><span data-stu-id="f6a0c-124">Name</span></span>          | <span data-ttu-id="f6a0c-125">说明</span><span class="sxs-lookup"><span data-stu-id="f6a0c-125">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="f6a0c-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="f6a0c-126">Authorization</span></span> | <span data-ttu-id="f6a0c-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f6a0c-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f6a0c-129">Content-type</span><span class="sxs-lookup"><span data-stu-id="f6a0c-129">Content-type</span></span>  | <span data-ttu-id="f6a0c-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="f6a0c-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f6a0c-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="f6a0c-132">Request body</span></span>

<span data-ttu-id="f6a0c-133">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="f6a0c-133">In the request body, provide a JSON object with the following parameters.</span></span>

|<span data-ttu-id="f6a0c-134">属性</span><span class="sxs-lookup"><span data-stu-id="f6a0c-134">Property</span></span>|<span data-ttu-id="f6a0c-135">类型</span><span class="sxs-lookup"><span data-stu-id="f6a0c-135">Type</span></span>|<span data-ttu-id="f6a0c-136">说明</span><span class="sxs-lookup"><span data-stu-id="f6a0c-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f6a0c-137">pkcs12Value</span><span class="sxs-lookup"><span data-stu-id="f6a0c-137">pkcs12Value</span></span>|<span data-ttu-id="f6a0c-138">字符串</span><span class="sxs-lookup"><span data-stu-id="f6a0c-138">String</span></span>| <span data-ttu-id="f6a0c-139">这是用于发送 pfx 内容的字段。</span><span class="sxs-lookup"><span data-stu-id="f6a0c-139">This is the field for sending the pfx content.</span></span> <span data-ttu-id="f6a0c-140">该值应为实际证书内容的 Base64 编码版本。</span><span class="sxs-lookup"><span data-stu-id="f6a0c-140">The value should be a base-64 encoded version of the actual certificate content.</span></span> <span data-ttu-id="f6a0c-141">必填。</span><span class="sxs-lookup"><span data-stu-id="f6a0c-141">Required.</span></span>|
|<span data-ttu-id="f6a0c-142">密码</span><span class="sxs-lookup"><span data-stu-id="f6a0c-142">password</span></span>|<span data-ttu-id="f6a0c-143">String</span><span class="sxs-lookup"><span data-stu-id="f6a0c-143">String</span></span>| <span data-ttu-id="f6a0c-144">这是 pfx 文件的密码。</span><span class="sxs-lookup"><span data-stu-id="f6a0c-144">This is the password for the pfx file.</span></span> <span data-ttu-id="f6a0c-145">必填。</span><span class="sxs-lookup"><span data-stu-id="f6a0c-145">Required.</span></span> <span data-ttu-id="f6a0c-146">如果未使用密码，则仍必须提供 的值 `""` 。</span><span class="sxs-lookup"><span data-stu-id="f6a0c-146">If no password is used, must still provide a value of `""`.</span></span>|

## <a name="response"></a><span data-ttu-id="f6a0c-147">响应</span><span class="sxs-lookup"><span data-stu-id="f6a0c-147">Response</span></span>

<span data-ttu-id="f6a0c-148">如果成功，此方法将返回 `200 OK` 响应代码和 [apiConnector，](../resources/identityApiConnector.md) 其中包含客户端证书 `authenticationConfiguration` 的公共信息。</span><span class="sxs-lookup"><span data-stu-id="f6a0c-148">If successful, this method returns a `200 OK` response code and the [apiConnector](../resources/identityApiConnector.md) whose `authenticationConfiguration` contains the public information of the client certificate.</span></span>

## <a name="examples"></a><span data-ttu-id="f6a0c-149">示例</span><span class="sxs-lookup"><span data-stu-id="f6a0c-149">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f6a0c-150">请求</span><span class="sxs-lookup"><span data-stu-id="f6a0c-150">Request</span></span>

<span data-ttu-id="f6a0c-151">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f6a0c-151">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "identityapiconnector_uploadclientcertificate"
}-->

```http
POST https://graph.microsoft.com/beta/identity/apiconnectors/{id}/uploadClientCertificate
Content-type: application/json

{
    "pkcs12Value": "eyJhbGciOiJSU0EtT0FFUCIsImVuYyI6IkEyNTZHQ00ifQ...kDJ04sJShkkgjL9Bm49plA",
    "password": "<password>"
}
```

### <a name="response"></a><span data-ttu-id="f6a0c-152">响应</span><span class="sxs-lookup"><span data-stu-id="f6a0c-152">Response</span></span>

<span data-ttu-id="f6a0c-153">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="f6a0c-153">The following is an example of the response.</span></span>

> <span data-ttu-id="f6a0c-154">**注意：** `authenticationConfiguration` 响应中的 类型为 [microsoft.graph.clientCertificateAuthentication，](../resources/clientcertificateauthentication.md) 因为这表示已上载证书的公共信息。</span><span class="sxs-lookup"><span data-stu-id="f6a0c-154">**Note:** `authenticationConfiguration` in the response is of type [microsoft.graph.clientCertificateAuthentication](../resources/clientcertificateauthentication.md) because this represents the public information of uploaded certificates.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityApiConnector"
}
-->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identity/apiConnectors/$entity",
    "id": "guid",
    "displayName": "My API connector",
    "targetUrl": "https://api.contoso.com/endpoint",
    "authenticationConfiguration": {
        "@odata.type": "#microsoft.graph.clientCertificateAuthentication",
        "certificateList": [
            {
                "thumbprint": "0EB255CC895477798BA418B378255204304897AD",
                "notAfter": 1666350522,
                "notBefore": 1508670522,
                "isActive": true
            },
            {
                "thumbprint": "1AB255CC895477798BA418B378255204304897BC",
                "notAfter": 1766350522,
                "notBefore": 1608670522,
                "isActive": false
            }
        ]
    }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed982019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "identityApiConnector: uploadClientCertificate",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

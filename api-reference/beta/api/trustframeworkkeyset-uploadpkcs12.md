---
title: 'trustFrameworkKeySet: uploadPkcs12'
description: 将 PKCS 12 格式密钥（PFX）上传到键集。
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e0ca40056c2b7e5607afdb9ffb1ea2cb314c2bc8
ms.sourcegitcommit: 8bef2bc8b9e56d1a787ea2f0cda4ed94f05109ad
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/26/2019
ms.locfileid: "37734532"
---
# <a name="trustframeworkkeyset-uploadpkcs12"></a><span data-ttu-id="53ec3-103">trustFrameworkKeySet: uploadPkcs12</span><span class="sxs-lookup"><span data-stu-id="53ec3-103">trustFrameworkKeySet: uploadPkcs12</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="53ec3-104">将 PKCS12 格式密钥（PFX）上载到[trustFrameworkKeyset](../resources/trustframeworkkeyset.md)。</span><span class="sxs-lookup"><span data-stu-id="53ec3-104">Upload a PKCS12 format key (PFX) to a [trustFrameworkKeyset](../resources/trustframeworkkeyset.md).</span></span> <span data-ttu-id="53ec3-105">输入是 Pfx 证书内容的 base-64 编码值。</span><span class="sxs-lookup"><span data-stu-id="53ec3-105">The input is a base-64 encoded value of the Pfx certificate contents.</span></span> <span data-ttu-id="53ec3-106">此方法返回[trustFrameworkKey](../resources/trustframeworkkey.md)。</span><span class="sxs-lookup"><span data-stu-id="53ec3-106">This method returns [trustFrameworkKey](../resources/trustframeworkkey.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="53ec3-107">权限</span><span class="sxs-lookup"><span data-stu-id="53ec3-107">Permissions</span></span>

<span data-ttu-id="53ec3-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="53ec3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="53ec3-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="53ec3-110">Permission type</span></span>                        | <span data-ttu-id="53ec3-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="53ec3-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="53ec3-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="53ec3-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="53ec3-113">TrustFrameworkKeySet</span><span class="sxs-lookup"><span data-stu-id="53ec3-113">TrustFrameworkKeySet.ReadWrite.All</span></span> |
| <span data-ttu-id="53ec3-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="53ec3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="53ec3-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="53ec3-115">Not supported.</span></span> |
| <span data-ttu-id="53ec3-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="53ec3-116">Application</span></span>                            | <span data-ttu-id="53ec3-117">TrustFrameworkKeySet</span><span class="sxs-lookup"><span data-stu-id="53ec3-117">TrustFrameworkKeySet.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="53ec3-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="53ec3-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /trustFramework/keySets/{id}/uploadPkcs12
```

## <a name="request-headers"></a><span data-ttu-id="53ec3-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="53ec3-119">Request headers</span></span>

| <span data-ttu-id="53ec3-120">名称</span><span class="sxs-lookup"><span data-stu-id="53ec3-120">Name</span></span>          | <span data-ttu-id="53ec3-121">说明</span><span class="sxs-lookup"><span data-stu-id="53ec3-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="53ec3-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="53ec3-122">Authorization</span></span> | <span data-ttu-id="53ec3-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="53ec3-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="53ec3-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="53ec3-125">Content-type</span></span>  | <span data-ttu-id="53ec3-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="53ec3-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="53ec3-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="53ec3-128">Request body</span></span>

<span data-ttu-id="53ec3-129">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="53ec3-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="53ec3-130">参数</span><span class="sxs-lookup"><span data-stu-id="53ec3-130">Parameter</span></span>    | <span data-ttu-id="53ec3-131">类型</span><span class="sxs-lookup"><span data-stu-id="53ec3-131">Type</span></span>        | <span data-ttu-id="53ec3-132">说明</span><span class="sxs-lookup"><span data-stu-id="53ec3-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="53ec3-133">Key</span><span class="sxs-lookup"><span data-stu-id="53ec3-133">key</span></span>|<span data-ttu-id="53ec3-134">String</span><span class="sxs-lookup"><span data-stu-id="53ec3-134">String</span></span>|<span data-ttu-id="53ec3-135">这是用于发送 pfx 内容的字段。</span><span class="sxs-lookup"><span data-stu-id="53ec3-135">This is the field for sending pfx content.</span></span> <span data-ttu-id="53ec3-136">该值应为实际证书内容的以64编码的版本。</span><span class="sxs-lookup"><span data-stu-id="53ec3-136">The value should be a base-64 encoded version of the actual certificate content.</span></span>|
|<span data-ttu-id="53ec3-137">密码</span><span class="sxs-lookup"><span data-stu-id="53ec3-137">password</span></span>|<span data-ttu-id="53ec3-138">String</span><span class="sxs-lookup"><span data-stu-id="53ec3-138">String</span></span>|<span data-ttu-id="53ec3-139">这是将密码发送给 PFX 内容的字段。</span><span class="sxs-lookup"><span data-stu-id="53ec3-139">This is the field for sending the password to PFX content.</span></span>|

## <a name="response"></a><span data-ttu-id="53ec3-140">响应</span><span class="sxs-lookup"><span data-stu-id="53ec3-140">Response</span></span>

<span data-ttu-id="53ec3-141">如果成功，此方法在响应`200 OK`正文中返回响应代码和新的[trustFrameworkKey](../resources/trustframeworkkey.md)对象。</span><span class="sxs-lookup"><span data-stu-id="53ec3-141">If successful, this method returns a `200 OK` response code and a new [trustFrameworkKey](../resources/trustframeworkkey.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="53ec3-142">示例</span><span class="sxs-lookup"><span data-stu-id="53ec3-142">Examples</span></span>

### <a name="request"></a><span data-ttu-id="53ec3-143">请求</span><span class="sxs-lookup"><span data-stu-id="53ec3-143">Request</span></span>

<span data-ttu-id="53ec3-144">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="53ec3-144">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "trustframeworkkeyset_uploadpkcs12"
}-->

```http
POST https://graph.microsoft.com/beta/trustFramework/keySets/{id}/uploadPkcs12
Content-type: application/json

{
  "key": "Base64-encoded-pfx-content",
  "password": "password-value"
}
```

### <a name="response"></a><span data-ttu-id="53ec3-145">响应</span><span class="sxs-lookup"><span data-stu-id="53ec3-145">Response</span></span>

<span data-ttu-id="53ec3-146">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="53ec3-146">The following is an example of the response.</span></span>

> <span data-ttu-id="53ec3-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="53ec3-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.trustFrameworkKey"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "kid": "kid-value",
    "use": "sig",
    "kty": "OCT",
    "nbf": 1508969811,
    "exp": 1508973711
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "trustFrameworkKeySet: uploadPkcs12",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

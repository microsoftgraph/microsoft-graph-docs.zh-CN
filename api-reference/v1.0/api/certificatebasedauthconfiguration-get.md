---
title: 获取 certificateBasedAuthConfiguration
description: 获取 certificatebasedauthconfiguration 对象的属性。
localization_priority: Normal
author: adimitui
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 49d34e274d783750401479f76391ae7be09fe59b
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52051576"
---
# <a name="get-certificatebasedauthconfiguration"></a><span data-ttu-id="cb839-103">获取 certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="cb839-103">Get certificateBasedAuthConfiguration</span></span>

<span data-ttu-id="cb839-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cb839-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="cb839-105">获取 [certificateBasedAuthConfiguration 对象](../resources/certificateBasedAuthConfiguration.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="cb839-105">Get the properties of a [certificateBasedAuthConfiguration](../resources/certificateBasedAuthConfiguration.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="cb839-106">权限</span><span class="sxs-lookup"><span data-stu-id="cb839-106">Permissions</span></span>

<span data-ttu-id="cb839-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cb839-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cb839-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="cb839-109">Permission type</span></span>                        | <span data-ttu-id="cb839-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cb839-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="cb839-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cb839-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="cb839-112">Organization.Read.All、Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cb839-112">Organization.Read.All, Organization.ReadWrite.All</span></span> |
| <span data-ttu-id="cb839-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cb839-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cb839-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="cb839-114">Not supported.</span></span> |
| <span data-ttu-id="cb839-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="cb839-115">Application</span></span>    | <span data-ttu-id="cb839-116">Organization.Read.All、Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cb839-116">Organization.Read.All, Organization.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cb839-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cb839-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /organization/{id}/certificateBasedAuthConfiguration/{id}
```

## <a name="request-headers"></a><span data-ttu-id="cb839-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="cb839-118">Request headers</span></span>

| <span data-ttu-id="cb839-119">名称</span><span class="sxs-lookup"><span data-stu-id="cb839-119">Name</span></span>      |<span data-ttu-id="cb839-120">说明</span><span class="sxs-lookup"><span data-stu-id="cb839-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="cb839-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="cb839-121">Authorization</span></span> | <span data-ttu-id="cb839-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="cb839-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cb839-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="cb839-124">Request body</span></span>

<span data-ttu-id="cb839-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="cb839-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cb839-126">响应</span><span class="sxs-lookup"><span data-stu-id="cb839-126">Response</span></span>

<span data-ttu-id="cb839-127">如果成功，此方法在响应正文中返回 响应代码和请求的 `200 OK` [certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="cb839-127">If successful, this method returns a `200 OK` response code and the requested [certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cb839-128">示例</span><span class="sxs-lookup"><span data-stu-id="cb839-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="cb839-129">请求</span><span class="sxs-lookup"><span data-stu-id="cb839-129">Request</span></span>

<span data-ttu-id="cb839-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="cb839-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="cb839-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="cb839-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_certificatebasedauthconfiguration"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/organization/{id}/certificateBasedAuthConfiguration/{id}
```
# <a name="c"></a>[<span data-ttu-id="cb839-132">C#</span><span class="sxs-lookup"><span data-stu-id="cb839-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-certificatebasedauthconfiguration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cb839-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cb839-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-certificatebasedauthconfiguration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cb839-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cb839-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-certificatebasedauthconfiguration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cb839-135">Java</span><span class="sxs-lookup"><span data-stu-id="cb839-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-certificatebasedauthconfiguration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]


---


### <a name="response"></a><span data-ttu-id="cb839-136">响应</span><span class="sxs-lookup"><span data-stu-id="cb839-136">Response</span></span>

<span data-ttu-id="cb839-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="cb839-137">The following is an example of the response.</span></span>

> <span data-ttu-id="cb839-138">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="cb839-138">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.certificateBasedAuthConfiguration"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "id-value",
  "certificateAuthorities": [
    {
      "isRootAuthority": true,
      "certificateRevocationListUrl": "CRLUrl-value",
      "deltaCertificateRevocationListUrl": "deltaCRLUrl-value",
      "certificate": "Binary",
      "issuer": "issuer-value",
      "issuerSki": "issuerSki-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get certificateBasedAuthConfiguration",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


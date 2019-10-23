---
title: 获取 certificateBasedAuthConfiguration
description: 获取 certificatebasedauthconfiguration 对象的属性。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: d21f7e5824b1144234d2f3371eab53f2f835e4cc
ms.sourcegitcommit: c9b9ff2c862f8d96d282a7bdf641cdb9c53a4600
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2019
ms.locfileid: "37632567"
---
# <a name="get-certificatebasedauthconfiguration"></a><span data-ttu-id="26fda-103">获取 certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="26fda-103">Get certificateBasedAuthConfiguration</span></span>

<span data-ttu-id="26fda-104">获取[certificateBasedAuthConfiguration](../resources/certificateBasedAuthConfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="26fda-104">Get the properties of a [certificateBasedAuthConfiguration](../resources/certificateBasedAuthConfiguration.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="26fda-105">权限</span><span class="sxs-lookup"><span data-stu-id="26fda-105">Permissions</span></span>

<span data-ttu-id="26fda-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="26fda-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="26fda-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="26fda-108">Permission type</span></span>                        | <span data-ttu-id="26fda-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="26fda-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="26fda-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="26fda-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="26fda-111">全部，全部组织。</span><span class="sxs-lookup"><span data-stu-id="26fda-111">Organization.Read.All, Organization.ReadWrite.All</span></span> |
| <span data-ttu-id="26fda-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="26fda-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="26fda-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="26fda-113">Not supported.</span></span> |
| <span data-ttu-id="26fda-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="26fda-114">Application</span></span>    | <span data-ttu-id="26fda-115">全部，全部组织。</span><span class="sxs-lookup"><span data-stu-id="26fda-115">Organization.Read.All, Organization.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="26fda-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="26fda-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /organization/{id}/certificateBasedAuthConfiguration/{id}
```

## <a name="request-headers"></a><span data-ttu-id="26fda-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="26fda-117">Request headers</span></span>

| <span data-ttu-id="26fda-118">名称</span><span class="sxs-lookup"><span data-stu-id="26fda-118">Name</span></span>      |<span data-ttu-id="26fda-119">说明</span><span class="sxs-lookup"><span data-stu-id="26fda-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="26fda-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="26fda-120">Authorization</span></span> | <span data-ttu-id="26fda-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="26fda-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="26fda-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="26fda-123">Request body</span></span>

<span data-ttu-id="26fda-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="26fda-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="26fda-125">响应</span><span class="sxs-lookup"><span data-stu-id="26fda-125">Response</span></span>

<span data-ttu-id="26fda-126">如果成功，此方法在响应`200 OK`正文中返回响应代码和请求的[certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="26fda-126">If successful, this method returns a `200 OK` response code and the requested [certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="26fda-127">示例</span><span class="sxs-lookup"><span data-stu-id="26fda-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="26fda-128">请求</span><span class="sxs-lookup"><span data-stu-id="26fda-128">Request</span></span>

<span data-ttu-id="26fda-129">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="26fda-129">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="26fda-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="26fda-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_certificatebasedauthconfiguration"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/organization/{id}/certificateBasedAuthConfiguration/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="26fda-131">C#</span><span class="sxs-lookup"><span data-stu-id="26fda-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-certificatebasedauthconfiguration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="26fda-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="26fda-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-certificatebasedauthconfiguration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="26fda-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="26fda-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-certificatebasedauthconfiguration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="26fda-134">Java</span><span class="sxs-lookup"><span data-stu-id="26fda-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-certificatebasedauthconfiguration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]


---


### <a name="response"></a><span data-ttu-id="26fda-135">响应</span><span class="sxs-lookup"><span data-stu-id="26fda-135">Response</span></span>

<span data-ttu-id="26fda-136">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="26fda-136">The following is an example of the response.</span></span>

> <span data-ttu-id="26fda-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="26fda-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

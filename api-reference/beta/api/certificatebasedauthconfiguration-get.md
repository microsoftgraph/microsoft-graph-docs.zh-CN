---
title: 获取 certificateBasedAuthConfiguration
description: 获取 certificatebasedauthconfiguration 对象的属性。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: bc25b54bf9e0efaabd8d2771e63251522d482a71
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36720083"
---
# <a name="get-certificatebasedauthconfiguration"></a><span data-ttu-id="8390e-103">获取 certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="8390e-103">Get certificateBasedAuthConfiguration</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8390e-104">获取[certificateBasedAuthConfiguration](../resources/certificateBasedAuthConfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="8390e-104">Get the properties of a [certificateBasedAuthConfiguration](../resources/certificateBasedAuthConfiguration.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="8390e-105">权限</span><span class="sxs-lookup"><span data-stu-id="8390e-105">Permissions</span></span>

<span data-ttu-id="8390e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8390e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8390e-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="8390e-108">Permission type</span></span>                        | <span data-ttu-id="8390e-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8390e-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="8390e-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8390e-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="8390e-111">全部, 全部组织。</span><span class="sxs-lookup"><span data-stu-id="8390e-111">Organization.Read.All, Organization.ReadWrite.All</span></span> |
| <span data-ttu-id="8390e-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8390e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8390e-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="8390e-113">Not supported.</span></span> |
| <span data-ttu-id="8390e-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="8390e-114">Application</span></span>    | <span data-ttu-id="8390e-115">全部, 全部组织。</span><span class="sxs-lookup"><span data-stu-id="8390e-115">Organization.Read.All, Organization.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8390e-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8390e-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /organization/{id}/certificateBasedAuthConfiguration/{id}
```

## <a name="request-headers"></a><span data-ttu-id="8390e-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="8390e-117">Request headers</span></span>

| <span data-ttu-id="8390e-118">名称</span><span class="sxs-lookup"><span data-stu-id="8390e-118">Name</span></span>      |<span data-ttu-id="8390e-119">说明</span><span class="sxs-lookup"><span data-stu-id="8390e-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8390e-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="8390e-120">Authorization</span></span> | <span data-ttu-id="8390e-121">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="8390e-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="8390e-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="8390e-122">Request body</span></span>

<span data-ttu-id="8390e-123">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8390e-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8390e-124">响应</span><span class="sxs-lookup"><span data-stu-id="8390e-124">Response</span></span>

<span data-ttu-id="8390e-125">如果成功, 此方法在响应`200 OK`正文中返回响应代码和请求的[certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="8390e-125">If successful, this method returns a `200 OK` response code and the requested [certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8390e-126">示例</span><span class="sxs-lookup"><span data-stu-id="8390e-126">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8390e-127">请求</span><span class="sxs-lookup"><span data-stu-id="8390e-127">Request</span></span>

<span data-ttu-id="8390e-128">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="8390e-128">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="8390e-129">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="8390e-129">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_certificatebasedauthconfiguration"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/organization/{id}/certificateBasedAuthConfiguration/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="8390e-130">C#</span><span class="sxs-lookup"><span data-stu-id="8390e-130">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-certificatebasedauthconfiguration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8390e-131">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8390e-131">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-certificatebasedauthconfiguration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8390e-132">目标-C</span><span class="sxs-lookup"><span data-stu-id="8390e-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-certificatebasedauthconfiguration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8390e-133">响应</span><span class="sxs-lookup"><span data-stu-id="8390e-133">Response</span></span>

<span data-ttu-id="8390e-134">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="8390e-134">The following is an example of the response.</span></span>

> <span data-ttu-id="8390e-p102">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="8390e-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

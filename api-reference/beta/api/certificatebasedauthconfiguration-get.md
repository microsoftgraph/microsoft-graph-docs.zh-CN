---
title: 获取 certificateBasedAuthConfiguration
description: 获取 certificatebasedauthconfiguration 对象的属性。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 4e4f9c4d2a060c38d0aa74a8c7c66e1cd75587af
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42440526"
---
# <a name="get-certificatebasedauthconfiguration"></a><span data-ttu-id="512ba-103">获取 certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="512ba-103">Get certificateBasedAuthConfiguration</span></span>

<span data-ttu-id="512ba-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="512ba-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="512ba-105">获取[certificateBasedAuthConfiguration](../resources/certificateBasedAuthConfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="512ba-105">Get the properties of a [certificateBasedAuthConfiguration](../resources/certificateBasedAuthConfiguration.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="512ba-106">权限</span><span class="sxs-lookup"><span data-stu-id="512ba-106">Permissions</span></span>

<span data-ttu-id="512ba-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="512ba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="512ba-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="512ba-109">Permission type</span></span>                        | <span data-ttu-id="512ba-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="512ba-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="512ba-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="512ba-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="512ba-112">全部，全部组织。</span><span class="sxs-lookup"><span data-stu-id="512ba-112">Organization.Read.All, Organization.ReadWrite.All</span></span> |
| <span data-ttu-id="512ba-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="512ba-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="512ba-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="512ba-114">Not supported.</span></span> |
| <span data-ttu-id="512ba-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="512ba-115">Application</span></span>    | <span data-ttu-id="512ba-116">全部，全部组织。</span><span class="sxs-lookup"><span data-stu-id="512ba-116">Organization.Read.All, Organization.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="512ba-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="512ba-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /organization/{id}/certificateBasedAuthConfiguration/{id}
```

## <a name="request-headers"></a><span data-ttu-id="512ba-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="512ba-118">Request headers</span></span>

| <span data-ttu-id="512ba-119">名称</span><span class="sxs-lookup"><span data-stu-id="512ba-119">Name</span></span>      |<span data-ttu-id="512ba-120">说明</span><span class="sxs-lookup"><span data-stu-id="512ba-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="512ba-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="512ba-121">Authorization</span></span> | <span data-ttu-id="512ba-122">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="512ba-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="512ba-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="512ba-123">Request body</span></span>

<span data-ttu-id="512ba-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="512ba-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="512ba-125">响应</span><span class="sxs-lookup"><span data-stu-id="512ba-125">Response</span></span>

<span data-ttu-id="512ba-126">如果成功，此方法在响应`200 OK`正文中返回响应代码和请求的[certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="512ba-126">If successful, this method returns a `200 OK` response code and the requested [certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="512ba-127">示例</span><span class="sxs-lookup"><span data-stu-id="512ba-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="512ba-128">请求</span><span class="sxs-lookup"><span data-stu-id="512ba-128">Request</span></span>

<span data-ttu-id="512ba-129">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="512ba-129">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="512ba-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="512ba-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_certificatebasedauthconfiguration"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/organization/{id}/certificateBasedAuthConfiguration/{id}
```
# <a name="c"></a>[<span data-ttu-id="512ba-131">C#</span><span class="sxs-lookup"><span data-stu-id="512ba-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-certificatebasedauthconfiguration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="512ba-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="512ba-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-certificatebasedauthconfiguration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="512ba-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="512ba-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-certificatebasedauthconfiguration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="512ba-134">响应</span><span class="sxs-lookup"><span data-stu-id="512ba-134">Response</span></span>

<span data-ttu-id="512ba-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="512ba-135">The following is an example of the response.</span></span>

> <span data-ttu-id="512ba-p102">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="512ba-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

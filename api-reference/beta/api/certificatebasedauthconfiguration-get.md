---
title: 获取 certificateBasedAuthConfiguration
description: 获取 certificatebasedauthconfiguration 对象的属性。
localization_priority: Normal
author: adimitui
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a00e2638050c5a648e98e9e2edf297fa6662cc46
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48959409"
---
# <a name="get-certificatebasedauthconfiguration"></a><span data-ttu-id="74e04-103">获取 certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="74e04-103">Get certificateBasedAuthConfiguration</span></span>

<span data-ttu-id="74e04-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="74e04-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="74e04-105">获取 [certificateBasedAuthConfiguration](../resources/certificateBasedAuthConfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="74e04-105">Get the properties of a [certificateBasedAuthConfiguration](../resources/certificateBasedAuthConfiguration.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="74e04-106">权限</span><span class="sxs-lookup"><span data-stu-id="74e04-106">Permissions</span></span>

<span data-ttu-id="74e04-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="74e04-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="74e04-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="74e04-109">Permission type</span></span>                        | <span data-ttu-id="74e04-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="74e04-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="74e04-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="74e04-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="74e04-112">全部，全部组织。</span><span class="sxs-lookup"><span data-stu-id="74e04-112">Organization.Read.All, Organization.ReadWrite.All</span></span> |
| <span data-ttu-id="74e04-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="74e04-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="74e04-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="74e04-114">Not supported.</span></span> |
| <span data-ttu-id="74e04-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="74e04-115">Application</span></span>    | <span data-ttu-id="74e04-116">全部，全部组织。</span><span class="sxs-lookup"><span data-stu-id="74e04-116">Organization.Read.All, Organization.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="74e04-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="74e04-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /organization/{id}/certificateBasedAuthConfiguration/{id}
```

## <a name="request-headers"></a><span data-ttu-id="74e04-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="74e04-118">Request headers</span></span>

| <span data-ttu-id="74e04-119">名称</span><span class="sxs-lookup"><span data-stu-id="74e04-119">Name</span></span>      |<span data-ttu-id="74e04-120">说明</span><span class="sxs-lookup"><span data-stu-id="74e04-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="74e04-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="74e04-121">Authorization</span></span> | <span data-ttu-id="74e04-122">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="74e04-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="74e04-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="74e04-123">Request body</span></span>

<span data-ttu-id="74e04-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="74e04-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="74e04-125">响应</span><span class="sxs-lookup"><span data-stu-id="74e04-125">Response</span></span>

<span data-ttu-id="74e04-126">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和请求的 [certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="74e04-126">If successful, this method returns a `200 OK` response code and the requested [certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="74e04-127">示例</span><span class="sxs-lookup"><span data-stu-id="74e04-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="74e04-128">请求</span><span class="sxs-lookup"><span data-stu-id="74e04-128">Request</span></span>

<span data-ttu-id="74e04-129">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="74e04-129">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="74e04-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="74e04-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_certificatebasedauthconfiguration"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/organization/{id}/certificateBasedAuthConfiguration/{id}
```
# <a name="c"></a>[<span data-ttu-id="74e04-131">C#</span><span class="sxs-lookup"><span data-stu-id="74e04-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-certificatebasedauthconfiguration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="74e04-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="74e04-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-certificatebasedauthconfiguration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="74e04-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="74e04-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-certificatebasedauthconfiguration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="74e04-134">Java</span><span class="sxs-lookup"><span data-stu-id="74e04-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-certificatebasedauthconfiguration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="74e04-135">响应</span><span class="sxs-lookup"><span data-stu-id="74e04-135">Response</span></span>

<span data-ttu-id="74e04-136">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="74e04-136">The following is an example of the response.</span></span>

> <span data-ttu-id="74e04-p102">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="74e04-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


